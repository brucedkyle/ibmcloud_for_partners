# PowerVS on IBM Cloud VPC Landing Zone

<img style="float: right; width: 10%; padding: 0px 0px 1% 1%"  alt="cataloglogo" src="../media/catalog-logo-infrastructure.svg" />
**Power Systems Virtual Servers** integrates your **AIX**, **IBM i**, or **Linux®** capabilities in an off-premises environment distinct from the IBM Cloud. You get fast, self-service provisioning, flexible management both on-premises and off-premises, and similar to on-premises it can be connected to access a stack of enterprise services from IBM – all with pay-as-you-use billing that lets you easily scale up and out. 

You can quickly deploy a Power Systems Virtual Server to meet your specific business needs and easily control workload demands. This article points you to the steps on building out a landing zone for your PowerVS deployment.

!!! tip

    If you are creating or configuring a Power Systems Virtual Server instance to support an SAP NetWeaver or SAP HANA workload, see [Planning your deployment](https://cloud.ibm.com/docs/sap?topic=sap-power-vs-planning-items) and [Deploying IBM Cloud VPC infrastructure for Power Systems Virtual Server SAP workloads](https://cloud.ibm.com/docs/sap?topic=sap-power-vs-set-up-vpc-infrastructure). 

## Terminology

Before you create a virtual server, you must understand the difference in terminology between a Power Systems Virtual Server _workspace_ and a Power Systems Virtual Server _instance_. 

You can think of the Power Systems Virtual Server _workspace_ as a container for all Power Systems Virtual Server _instances_ at a specific geographic region. 

The workspace can contain multiple Power Systems Virtual Server instances. 

## Use the IBM Cloud catalog to deploy PowerVS

To get started, you can follow the step-by-step instructions for deploying an offering in the IBM Cloud catalog at:

- [Getting started with IBM Power Systems Virtual Servers](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-getting-started)
- [Creating a Power Systems Virtual Server](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-creating-power-virtual-server#creating-power-virtual-server)

The instructions provide a convient way to deploy PowerVS in a VPC landing zone. 

<img alt="power vs on vpc catalog" width="70%" src="../media/powervs-on-vpc-catalog.png">

The catalog provides options for:

- **Quick start** that deploys VPC services and a Power Virtual Server workspace and interconnects them. It also creates one Power virtual server instance of chosen t-shirt size or custom configuration. This is for dev/test environments and to get started.
- **PowerVS workspace** also described as **full-stack variation** that deploys the workspace, but does not deploy the PowerVS instances. Use this to set up your production environment.

## Quick start architecture

The **quick start** architecture provides an excellent dev/test environment for your PowerVS deployment.

The following diagram illustrates the Quick start architecture. 

![quick start architecture](./media/deploy-arch-ibm-pvs-inf-quickstart.svg)

The following table summarizes the solution.

| Variation  | Available on IBM Catalog  |  Requires Schematics Workspace ID | Creates VPC Landing Zone | Performs VPC VSI OS Config | Creates PowerVS Infrastructure | Creates PowerVS Instance | Performs PowerVS OS Config |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| [Quickstart](./)    | :heavy_check_mark:  |   N/A  | :heavy_check_mark:| :heavy_check_mark: | :heavy_check_mark:  | :heavy_check_mark: | N/A |


This example sets up the following infrastructure:

- A VPC Infrastructure with the following features:

    - One VSI for management(jump/bastion).
    - Installation and configuration of Squid Proxy, DNS Forwarder, NTP forwarder and NFS on the bastion host, and sets the host as the server for the NTP, NFS, and DNS services by using Ansible roles.

- A PowerVS workspace with the following network topology:

    - Creates two private networks: a management network and a backup network.
    - Creates one or two IBM Cloud connections.
    - Attaches the IBM Cloud connections to a transit gateway.
    - Attaches the private networks to the IBM Cloud connections.
    - Creates an SSH key for power workspace

- A PowerVS Instance with following options:

    - t-shirt profile (Aix/IBMi/SAP Image)
    - Custom profile (cores, memory storage and image)
    - 1 volume

The following illustration provides a "heat map" of the features provided offered in the Quick Start architecture.

![quick start heat map](./media/heat-map-deploy-arch-ibm-pvs-inf-quickstart.svg)

For more information and the Terraform code used to set up the Quick Start, see [IBM Cloud catalog example for Power Virtual Server with VPC landing zone Quickstart Variation](https://github.com/terraform-ibm-modules/terraform-ibm-powervs-infrastructure/tree/main/solutions/quickstart) on GitHub.

## Full stack architecture

The **PowerVS workspace** option aka _full stack architecture_ that is shown as an option in the catalog deploys the infrastructure you need, but does not include the PowerVS instances. The architecture is based on best practices.

The following diagram shows the full-stack architecture.

![full stack architecture](./media/deploy-arch-ibm-pvs-inf-full-stack.svg)

The following table summaries the deployment.

| Variation  | Available on IBM Catalog  |  Requires Schematics Workspace ID | Creates VPC Landing Zone | Performs VPC VSI OS Config | Creates PowerVS Infrastructure | Creates PowerVS Instance | Performs PowerVS OS Config |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| [Full-Stack](./)  | :heavy_check_mark:  | N/A  | :heavy_check_mark:  | :heavy_check_mark:  |  :heavy_check_mark: | N/A | N/A |

This example sets up the following infrastructure:

- A VPC Infrastructure with the following components:

    - Provisions three VPCs with one VSI in each VPC (one management(jump/bastion) VSI, one inet-svs VSI configured as squid proxy server, one private-svs VSI configured as NFS, NTP, DNS server).
    - Installs and configures the Squid Proxy, DNS Forwarder, NTP forwarder and NFS on hosts, and sets the host as the server for the NTP, NFS, and DNS services by using Ansible roles.

- A PowerVS workspace instance with the following network topology:

- Creates two private networks: a management network and a backup network.
- Creates one or two IBM Cloud connections.
- Attaches the IBM Cloud connections to a transit gateway.
- Attaches the private networks to the IBM Cloud connections.
- Creates an SSH key.

The following illustration provides a "heat map" of the features provided offered in the Full Stack architecture.

![full stack heat map](./media/heat-map-deploy-arch-ibm-pvs-inf-full-stack.svg)

For more information and the Terraform code used to set up the Full Stack, see [IBM Cloud catalog example for Power Virtual Server with VPC landing zone Full-Stack Variation](https://github.com/terraform-ibm-modules/terraform-ibm-powervs-infrastructure/tree/main/solutions/full-stack) on GitHub.

## Extension architecture

An additional architecture is provided, called  extends an existing PowerVS infrastructure for deployable architectures deployed as full-stack with an additional PowerVS workspace. It provisions the following infrastructure on top of deployed Full Stack solution :

- A PowerVS workspace instance with the following network topology:

    - Creates two private networks: a management network and a backup network
    - Creates one or two IBM Cloud connections
    - Attaches the IBM Cloud connections to a transit gateway
    - Attaches the private networks to the IBM Cloud connections
    - Creates an SSH key

For more information and the Terraform code use to set up the Extension, see [IBM Cloud catalog example for Power Virtual Server with VPC landing zone Extension Variation](https://github.com/terraform-ibm-modules/terraform-ibm-powervs-infrastructure/tree/main/solutions/extension).

## Next step

See [Deploying a custom image within a Power Systems Virtual Server](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-deploy-custom-image).

## Reference

- [Getting started with IBM Power Systems Virtual Servers](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-getting-started)
- [IBM Power Virtual Server with VPC landing zone module](https://github.com/terraform-ibm-modules/terraform-ibm-powervs-infrastructure#ibm-power-virtual-server-with-vpc-landing-zone-module)