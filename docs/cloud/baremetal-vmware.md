# VMWare on Bare Metal Classic

**VMware for IBM Cloud® Classic infrastructure** provides an industry-leading virtualization platform that abstracts processor, memory, storage, and networking resources to create multiple Virtual Servers on a single physical server. Multiple physical servers can be clustered together to create a private cloud.

IBM Cloud® provides the unique capability for customers to provision dedicated Bare Metal Servers where you can deploy your own VMware-based private cloud. 

!!! key "Key differentiator"

    vSphere workloads and catalogs can be provisioned onto VMware vSphere environments within IBM Cloud® data centers without modifying VMware VMs or guests. 
    These deployments are made possible by using a common vSphere hypervisor and management or orchestration platform.

## Use cases

The core objective of VMware and IBM Cloud is to assist vSphere administrators to deploy VMware vSphere environments within an IBM Cloud infrastructure. VMware administrators can use bare metal instances and network, storage, and backup and recovery constructs in a self-service manner. 

!!! use "Use cases"

    - Enable the creation of a hybrid cloud where on-premises VMware based servers, tooling, and processes can be extended into the public cloud.
    - vSphere workloads and catalogs can be provisioned onto VMware vSphere environments within IBM Cloud data centers without modification to VMware VMs or guests.
    - Use a common vSphere hypervisor and management or orchestration platform makes these deployments possible on premises and in IBM Cloud. 
    - vSphere implementations also enable the use of other components of the VMware vCloud Suite – vSphere, vRealize, vSAN, Site Recovery Manager (SRM), and NSX.

## VMWare on Classic offerings

IBM Cloud™ has a number of offerings for VMware deployments in Classic. These can be classified and described as:

- Automated vSphere Hypervisor Image deployment ([IBM Cloud Bare Metal Servers for Virtual Private Cloud with VMware vSphere](https://cloud.ibm.com/docs/vmware?topic=vmware-vmware-getting-started))
- Automated vSphere Hypervisor Image deployment, installation and configuration ([VMware Solutions Dedicated - VMware vSphere®](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vs_vsphereclusteroverview))
- Automated vCenter and vSphere clusters deployment, installation and configuration ([VMware Solutions Dedicated - vCenter Server](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vc_vcenterserveroverview))

See [VMware deployment offerings](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-getting-started#getting-started-depl-offerings)

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