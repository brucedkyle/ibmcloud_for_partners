# VMware on Bare Metal Classic

**VMware® for IBM Cloud® Classic infrastructure** provides an industry-leading virtualization platform that abstracts processor, memory, storage, and networking resources to create multiple Virtual Servers on a single physical server. Multiple physical servers can be clustered together to create a private cloud.

IBM Cloud® provides the unique capability for customers to provision dedicated Bare Metal Servers where you can deploy your own VMware-based private cloud. 

## vCenter Server

VMware vCenter Server® is a hosted private cloud that delivers the VMware vSphere® stack as a service. The VMware® environment is built in addition to a minimum of three IBM Cloud® bare metal servers, and it offers shared network-attached storage and dedicated software-defined storage options. It also includes the automatic deployment and configuration of an easy-to-manage logical edge firewall, which VMware NSX® powers.

After initial instance deployment, you can increase shared storage by ordering more Network File System (NFS) file shares from the IBM Cloud infrastructure customer portal. You can attach them manually to all VMware ESXi™ servers in a cluster. You can also take advantage of VMware vSAN™ as a storage option. To increase the vSAN-based storage capacity of a vSAN cluster, you can add more ESXi servers post-deployment.

For more information, see [vCenter Server overview](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vc_vcenterserveroverview#vc_vcenterserveroverview-specs).

### vCenter Server reference architecture

This illustration shows an architecture pattern demonstrates a Client VPN based connectivity to a vCenter Server instance provisioned in IBM Cloud classic infrastructure. This solution uses a bastion VPC with client-to-site VPNaaS and a connecting IBM Cloud Transit Gateway, or alternatively using a VPC provisioned with classic connectivity. IBM Cloud DNS Services are used in VPC with a custom resolver.

[![bastion vCenter architecture](./media/arch-pattern-bastion-vpc.svg)](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-arch-pattern-bastion-vpc)

For other reference architectures, see [Architecture patterns for the vCenter Server deployment default connectivity options](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-arch-pattern-nsx-t-topology-overview) along with the other dozen variations in the documentation.

## vSphere

VMware vSphere® is a streamlined and optimized ordering platform for VMware. With this platform, you can build your own IBM-hosted VMware environment by customizing and ordering the VMware-compatible hardware based on your selected VMware components.

!!! key "Key differentiator"

    vSphere workloads and catalogs can be provisioned onto VMware vSphere environments within IBM Cloud® data centers without modifying VMware VMs or guests. 
    
    These deployments are made possible by using a common vSphere hypervisor and management or orchestration platform.

The IBM Cloud for VMware Solutions console filters the hardware automatically, based on the VMware components that you select. 

!!! tip
    
    Use this offering to create a new instance of VMware ESXi™ servers or scale out an existing instance of ESXi servers in an IBM Cloud data center. Depending on the VMware components that you select, you can start with just one ESXi server and then scale the instance later as needed.

VMware vSphere does not automate the installation, configuration, and bring-up of the optional VMware components. The platform allows maximum of flexibility to design and build your hosted VMware environment while you incorporate VMware-compatible hardware.

For more information, see [VMware vSphere overview](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vs_vsphereoverview).

## Use cases

The core objective of VMware and IBM Cloud is to assist vSphere administrators to deploy VMware vSphere environments within an IBM Cloud infrastructure. VMware administrators can use bare metal instances and network, storage, and backup and recovery constructs in a self-service manner. 

!!! use "Use cases"

    - Enable the creation of a hybrid cloud where on-premises VMware based servers, tooling, and processes can be extended into the public cloud.
    - vSphere workloads and catalogs can be provisioned onto VMware vSphere environments within IBM Cloud data centers without modification to VMware VMs or guests.
    - Use a common vSphere hypervisor and management or orchestration platform makes these deployments possible on premises and in IBM Cloud. 
    - vSphere implementations also enable the use of other components of the VMware vCloud Suite – vSphere, vRealize, vSAN, Site Recovery Manager (SRM), and NSX.

## Design

The solutions design serves as a baseline architecture that provides the foundation for other internal or vendor-specific components to be added for specific use cases.

![vmware design](./media/vcsv4radiagrams-ra-variationsonatheme.svg)

!!! note

    VMware vSphere® is a streamlined and optimized ordering platform for VMware®. With this platform, you can build your own IBM®-hosted VMware environment by customizing and ordering the VMware-compatible hardware based on your selected VMware components.

    See [VMware vSphere overview](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vs_vsphereoverview).

## VMware on Classic offerings

IBM Cloud™ has a number of offerings for VMware deployments in Classic. These can be classified and described as:

- Automated vSphere Hypervisor Image deployment ([IBM Cloud Bare Metal Servers for Virtual Private Cloud with VMware vSphere](https://cloud.ibm.com/docs/vmware?topic=vmware-vmware-getting-started)).
- Automated vSphere Hypervisor Image deployment, installation and configuration ([VMware Solutions Dedicated - VMware vSphere®](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vs_vsphereclusteroverview)).
- Automated vCenter and vSphere clusters deployment, installation and configuration ([VMware Solutions Dedicated - vCenter Server](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vc_vcenterserveroverview)).

See [VMware deployment offerings](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-getting-started#getting-started-depl-offerings).

!!! important "Regulated workloads"

    If you need secure-by-default architecture for regulated workloads, see [VMware Regulated Workloads on IBM Cloud](./vmware-regulated.md).

## Licensing

When you deploy ESX through the IBM Cloud® catalog, VMware Service Provider Program licensing (VSPP) automatically enables. On deployment, a default user 'ibmvmadmin' is added to the ESX server for data collection. Do not delete this default user. VSPP charges for RAM that is reserved and used for all “powered on” virtual machines (not “per socket” like a standard host license).

See:

- [FAQs: VMware](https://cloud.ibm.com/docs/vmware?topic=vmware-vmware-faq).
- [Ordering VMware licenses](https://cloud.ibm.com/docs/vmware?topic=vmware-ordering-vmware-license)
- [Ordering NetApp licenses](https://cloud.ibm.com/docs/vmware?topic=vmware-order-netapp-licenses)
- [Applying IBM Cloud®-issued licenses for VMware vSphere](https://cloud.ibm.com/docs/vmware?topic=vmware-apply-vmware-vsphere-6-licenses)

## QuantaStor for VMware

See [QuantaStor for VMware Architecture Guide](https://cloud.ibm.com/docs/vmware?topic=vmware-quantastor-architecture-guide)

## Security

VMWare on IBM Cloud® is integrated with the **Security and Compliance Center** to help you manage security and compliance for your organization.

With the Security and Compliance Center, you can:

- Monitor for controls and goals that pertain to VMWare on IBM Cloud®
- Define rules for VMWare on IBM Cloud® that can help to standardize resource configuration

See [Managing security and compliance with VMWare on IBM Cloud](https://cloud.ibm.com/docs/vmware?topic=vmware-manage-security-compliance).

## Getting started

See:

- [VMware Solutions](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-getting-started)
- [Getting started with VMware vSphere](https://cloud.ibm.com/docs/vmware?topic=vmware-get-started-vsphere-6)
- [Getting Started with VMware vSphere NSX](https://cloud.ibm.com/docs/vmware?topic=vmware-getting-started-nsx)
- [Using cookbooks for VMware deployments](https://cloud.ibm.com/docs/vmware?topic=vmware-using-vmware-cookbooks)

## References

- VMware Classic: [Getting started with VMware and IBM Cloud](https://cloud.ibm.com/docs/vmware?topic=vmware-vmware-getting-started).