# z/OS on IBM Cloud VPC

If you already use the **IBM Cloud** today, you may be familiar with both the process of provisioning a **Virtual Server Instance (VSI)** and the extensive catalog of services and products. With **IBM Wazi as-a-Service** in the IBM Cloud, the z/OS operating system is now an option when provisioning VSIs within the **Virtual Private Cloud (VPC)**. 

VPC provides a dedicated and isolated environment within the IBM Cloud to easily create VSIs, subnets, cloud object storage, security groups, and more, all within a protected space. The z/OS stock image benefits from the VPC features and comes with a pre-configured and customized software stack, but custom images can also be created with the **Wazi Image Builder**. 

!!! important

    With **Wazi as-a-Service** z/OS images in the IBM Cloud, you can provision your specific z/OS software stack for the area of z/OS under test, within minutes. You use the mainframe for the time required for the duration of the test, after which the test images can be deprovisioned.

In this article, learn the roadmap for how to create and configure IBM z/OS virtual server instances in IBM Cloud Virtual Private Cloud (VPC) from the cloud console.

## Use cases

!!! key "Use cases"

    - Performance testing
    - Regression testing
    - Scheduling and collaboration from many testers working hands-on
    - Training exercises or dry runs, especially to experiment with new tools or approaches
    - Projects of short duration requiring z/OS hardware

## Reference architecture

The following diagram shows best practices architecture for installing an isolated z/OS Wazi as a Service development environment on IBM Cloud.

![ibm architecture](./media/ibm-cloud-architecture.png)

This particular architecture shows z/OS Wazi as a Service development environment on IBM Cloud, with the option to deploy Wazi for Dev Spaces on any existing OpenShift cluster. It creates a virtual private cloud, creates a Wazi as a Service VSI in that VPC, creates and configures a VPN for accessing resources within that VPC, optionally creates a new OpenShift cluster and automatically deploys Wazi for Dev Spaces for you, and configures your environment with appropriate logging and monitoring services.

## Steps

You will need to create a VPC, SSH keys, a subnet and floating IP, security groups, and some storage volumes, and with those in place you provision a new VSI from the pre-installed z/OS stock image provided by IBM Wazi as-a-Service. After the VSI was fully provisioned and accessible,log in with SSH and TN3270 to perform setup and configuration tasks, such as copying over testcases and test resources. With that complete, you are ready to start running  test cases and performing our test scenarios.

### Steps to set up IBM Cloud account and the IBM Virtual Private Cloud (VPC)

1. To learn about setting up your IBM Cloud account, see [Setting up your IBM Cloud account](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-setting-up-your-cloud-account).
2. You first create a VPC then create your virtual server instance. To create these from the command line, see [Using the IBM Cloud console to create z/OS virtual server instances](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=czvicv-using-cloud-console-create-zos-virtual-server-instances) for the steps.
3. [Create a client-to-site VPN server for VPC](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-creating-client-site-vpn-server).
4. [Connect to z/OS virtual server instances](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-connecting-zos-virtual-server-instances).
5. [Install software products for z/OS virtual server instances](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-installing-software-products-zos-virtual-server-instances).

!!! tip

    Review and implement [Security best practices for z/OS virtual server instances](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-security-best-practices-zos-virtual-server-instances).

### Automated provisioning of the VSI using Ansible

Michael Cohoon wrote an article, [Automated Provisioning of z/OS in the IBM Cloud](https://community.ibm.com/community/user/ibmz-and-linuxone/blogs/michael-cohoon1/2022/12/09/automated-provisioning-of-zos-in-the-ibm-cloud?CommunityKey=2a2f855c-5950-4a9d-8485-86645982646a), that provides code that his team used to automate the configuration of IBM Cloud resources and the provisioning of a z/OS VSI. In the article, he explains how to:

1. Construct a configuration file
2. Create IBM Cloud resources
3. Provision a z/OS Virtual Server Instance
4. Deprovision the z/OS VSI

The programmatic ways in which you can now manage z/OS test instances makes it easy to integrate automation to develop and test your  applications. **Ansible for IBM Cloud** and **Ansible for z/OS collections** are two of the tools that you can use to target the Wazi as-a-Service z/OS images for you test application development and test.

Also see [Red Hat Ansible Certified Content for IBM Z](https://www.ibm.com/support/z-content-solutions/ansible/).

### Use Wazi aaS to configure your z/OS instance

Use Wazi as a Service to configure either stock images or custom images.

### Configure of stock images

<img style="float: right; width: 20%; padding: 0px 0px 1% 1% "  alt="zos stock images" src="../media/zOS-stock-images.png" />
You can select the content you want from a stock image. The illustration to the right shows choices you can make in provisioning the stock images as of the time of this writing.

Select a set of components for each of the following:

- Base z/OS
- Middleware
- Programming Language
- Additional content

For a complete list of what you can select for the stock image, see [Configurations in z/OS stock images](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-configurations-in-zos-stock-images).

Next, use Wazi as a Service to further configure your settings. See [Configuring settings on the web server UI](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=builder-configuring-wazi-image),

### System Modification Program/Extended (SMP/E)

You can use the System Modification Program/Extended (SMP/E) database, which is also called _consolidated software inventory (CSI)_, to query preinstalled products and services in the z/OS stock images. See [Viewing products and services in z/OS stock images](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-viewing-products-services-in-zos-stock-images) for the commands.

### IBM Z Hypervisor as a Service (zHYPaaS)

The zHYPaaS host control program creates a virtual machine (VM) runtime environment for each guest operating system (OS) and can host many guests at the same time. For more information, see [IBM Z Hypervisor as a Service (zHYPaaS) overview](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=vpc-z-hypervisor-as-service-zhypaas-overview).

### Bring your own image

Use **IBM® Wazi Image Builder** to create and manage custom images from an existing Z platform. See [Bringing your own image with Wazi Image Builder](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=bringing-your-own-image-wazi-image-builder).

## Automation of IBM Cloud z/OS Development Reference Architecture

When using z/OS on IBM Cloud, you will want to automate provisioning and deprovisioning your instances.

!!! tip "Reasons for testing automation"

    Automation of end-to-end test execution, especially for regression testing, provides repeatable scenarios for testing, experimentation, and training.  With Wazi as-a-Service z/OS images and the IBM Cloud CLI, Ansible Collection, Terraform provider, and REST APIs, you can completely automate the lifecycle aspects of the z/OS images under test, such as:
    
    1. Provision z/OS instances and the software stack that will run in them
    2. Then taking certain actions
    3. Check for expected system behaviors
    4. Restart z/OS or its components when failures occur
    5. Deprovision the instances and their data when finished.

Best practices have been implemented and published to set up **IBM Wazi for Dev Spaces** onto an existing OpenShift cluster, or to provision IBM Z, Virtual Servers and/or OpenShift clusters.

The automation supports the provisioning of an IBM Cloud z/OS Development Environment using isolated VPC networks and OpenShift with a set of developer tools formulated an SDLC for native z/OS development with CICS and DB2.

Within this repository you will find a set of Terraform template bundles that embody best practices for provisioning and configuring cloud resources in an IBM Cloud cloud account. We recommend using this with an IBM Cloud Enterprise sub-account.

See the code [TechZone Automation - IBM Cloud z/OS Development Reference Architecture](https://github.com/IBM/automation-ibmcloud-infra-zos-dev) on GitHub.

## Next steps

For a deeper dive, see the product documentation [Creating z/OS VSIs in IBM Cloud VPC](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=creating-zos-vsis-in-cloud-vpc).

## References

- IBM Wazi as a Service documentation [Creating z/OS VSIs in IBM Cloud VPC](https://www.ibm.com/docs/en/wazi-aas/1.0.0?topic=creating-zos-vsis-in-cloud-vpc).
- [Provisioning z/OS in the IBM Cloud](https://community.ibm.com/community/user/ibmz-and-linuxone/blogs/michael-cohoon1/2022/11/01/provisioning-zos-in-the-ibm-cloud)
- [z/OS software configuration in a WAZI as a Service Environment](https://community.ibm.com/community/user/ibmz-and-linuxone/blogs/michael-grtzner1/2022/12/06/zos-software-configuration-in-an-wazi-as-a-service)
- GitHub [TechZone Automation - IBM Cloud z/OS Development Reference Architecture](https://github.com/IBM/automation-ibmcloud-infra-zos-dev)