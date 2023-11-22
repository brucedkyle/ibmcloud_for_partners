# Red Hat OpenShift on IBM Z and LinuxONE

<img style="float: right; width: 15%; padding: 0px 0px 1% 1% "  alt="IBM Cloud" src="../media/redhat.jpg" />
Organizations face the challenge of delivering extraordinary customer experiences by developing new applications, while modernizing existing applications to speed up their cloud-native journey. 

**Red Hat® OpenShift® on IBM zSystems and LinuxONE** empowers organizations to accelerate transformation with greater flexibility and agility through integrated tooling and a security-focused and resilient foundation for cloud-native development.

## Cloud Native development

The Red Hat OpenShift Container Platform subscription includes several capabilities that are enabled for IBM zSystems and LinuxONE:

- [Red Hat OpenShift Service Mesh](https://www.redhat.com/en/topics/microservices/why-choose-openshift-service-mesh), built on Istio, provides a uniform way to connect, manage, and observe microservices-based applications as managing and security between services become more difficult. 
- [Red Hat OpenShift Pipelines](https://www.redhat.com/en/technologies/cloud-computing/openshift/ci-cd), a cloud-native, continuous integration and continuous delivery (CI/CD) solution based on Kubernetes resources.
- [Red Hat OpenShift Serverless](https://www.redhat.com/en/topics/microservices/why-choose-openshift-serverless), a serverless cloud computing model providing developers with a modern, cloud-native app dev stack for hybrid clouds. Serverless lets developers focus on their code without worrying about the infrastructure.
- [Red Hat OpenShift Do (odo)](https://developers.redhat.com/products/odo/overview?cm_mc_uid=52990874348515971042091&cm_mc_sid_50200000=46387671615500364956&_ga=2.189824299.1899383767.1615500365-834723249.1601921261) is a command-line interface tool for writing and deploying applications on OpenShift and Kubernetes, allowing developers to focus on what’s most important to them—code. 

For a deeper dive, see [Cloud Native Development](https://www.ibm.com/it-infrastructure/z/capabilities/cloud-native-development).

## Security

Red Hat OpenShift on IBM zSystems and LinuxONE allows businesses to integrate and modernize their applications with a firm foundation built for security, resiliency, and availability. 

IBM zSystems and LinuxONE prevent security threats and protect data across a hybrid cloud environment with certified multitenant workload isolation and a transparent, pervasive encryption with optimized performance. 

IBM zSystems and LiunxONE also protects the integrity and confidentiality of data with **Crypto Express adapters (HSM)** designed to meet strong security requirements of **FIPS 140-2 Level 4**, have quantum-safe cryptography embedded, and support compliance to regulatory guidelines efficiently and productively. 

For more information, see [LinuxONE Security](./linuxone.md#security) in this wiki.

## Co-located workloads

Cloud-native applications can be located close to existing workloads to improve throughput and reduce latency, empowering organizations to integrate and modernize without disrupting current services along their cloud-native journey.

See [LinuxONE Co-location pattern](./linuxone.md#co-location-pattern) article in this wiki for more information.

## Infrastructure and installation

Kernel-based Virtual Machine (KVM) is a fully supported virtualization option on IBM zSystems and LinuxONE for OpenShift users, alongside the traditional IBM z/VM hypervisor.

Running [user provisioned infrastructure (UPI)](https://docs.openshift.com/container-platform/4.12/installing/installing_ibm_z/installing-ibm-z.html#installing-ibm-z) installs of Red Hat OpenShift using KVM via libvirt on IBM zSystems and LinuxONE are supported. For environments provisioned using IBM Cloud Infrastructure Center, which provides the Infrastructure-as-a-Service (IaaS) layer on IBM zSystems and LinuxONE, the [platform-agnostic installer](https://access.redhat.com/articles/4207611) should be used.

## z/OS Cloud Broker

[IBM z/OS Cloud Broker](https://www.ibm.com/marketplace/zos-cloud-broker) enables OpenShift applications to easily interact with data and applications on IBM Z. 

## References

- [IBM and Red Hat bring OpenShift to IBM Z and LinuxONE](https://cloud.redhat.com/blog/ibm-and-red-hat-bring-openshift-to-ibm-z-and-linuxone)
- IDC white paper: [Transforming a Corporate Datacenter into a Modern Environment: Kubernetes as a Foundation for Hybrid Cloud](https://www.ibm.com/account/reg/signup?formid=urx-40088)
- Red Hat datasheet: [Red Hat OpenShift for IBM zSystems and IBM LinuxONE](https://www.redhat.com/en/resources/openshift-ibm-z-linuxone-datasheet)