# IBM Cloud Bare Metal Servers for Classic

Your IBM Cloud bare metal server is an hourly or monthly, single-tenant server that is dedicated to you. Your server isn't shared in any part, including server resources, with other customers. You manage your server, which is provisioned without a hypervisor, and deployed in one or more data centers. Multiple Bare Metal Servers can communicate on the IBM Cloud virtual private network as if stationed on the same rack.

For more information see [Classic deployment](https://www.ibm.com/cloud/bare-metal-servers/classic).

This article provides an overview of the options and how to get started using a bare metal server.

## Bare metal server options

Customize your bare metal server with over 11 million different configuration combinations and get 20 TB of cost-free bandwidth. Choose the latest Intel Xeon or AMD EPYC CPUs. Ideal for large, steady state, predictable operations.

## Server options

- **Fast provisioning**. Compute options (number of cores, speed, RAM, and number of drives) are preset. Preset servers are ready to configure 30 - 40 minutes after provisioning.
- **Custom**. If one of the fast provisioning options does not meet your needs, you can customize your servers. Customized servers are generally provisioned in 2 - 4 hours. The provisioning time depends on complexity, quantity, and testing options.
- **SAP-certified bare metal servers**. Certified to support your SAP HANA and SAP NetWeaver workloads. For more information, see [SAP-certified infrastructure](https://www.ibm.com/cloud/sap/certified-infrastructure?_gl=1*agl8p8*_ga*MzUyMzc1NTEuMTY5MzM0MTgyMA..*_ga_FYECCCS21D*MTY5NDEwMDM1OC4xNC4xLjE2OTQxMDI0MzkuMC4wLjA.).
- **VMWare-certified servers**. Deploy your own VMware®-based private cloud. For more information, see [Getting started with VMware](https://cloud.ibm.com/docs/vmware?topic=vmware-vmware-getting-started).

## Hardware options

- [Intel Sapphire Rapids CPUs](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-sapphire-rapids-support)
- [AMD CPUs](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-amd-procs). AMD EPYC® "Rome" generation CPUs are now an option.
- [Intel Cascade Lake CPUs](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-cascade-lake-support)
- [NVIDIA GPUs](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-gpu-support). Make sure that you install the appropriate drivers. See [NVIDIA drivers](https://www.nvidia.com/Download/index.aspx?lang=en-us)

## Server enhancement options

When you provision a bare metal server, you have the following enhancement options to help make managing your server easier. 

- [Dynamic inventory](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-dynamic-inv). For more information about provisioning a bare metal server, see [Selecting from fast provisioning servers](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-bm-select-popular-servers).
- [Network redundancy](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-network-redundancy). Port redundancy provides networking failover by maintaining a primary and secondary network port. If the primary port fails, the secondary (redundant) port enables.
- [Block and file storage add-on](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-block-and-file-add-on). You can now order block and file storage (20 - 12,000 GB) when you provision a bare metal server. For more information, see [Getting started with Block Storage](https://cloud.ibm.com/docs/BlockStorage?topic=BlockStorage-getting-started) and [Getting started with File Storage](https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-getting-started).

## Bare metal server add-ons

See [Bare metal server add-ons](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm#bm-add-ons) for details about the following add-ons:

- Power Supply
- IBM Cloud Backup
- Server security
- Business continuity insurance
- Firewall
- Monitor - host ping
- Notification
- Public secondary IP addresses
- IPv6 IP addresses

### Intel Software Guard Extension

[Intel® Software Guard Extension (SGX)](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-bm-intel-sgx) is an architecture extension that is designed to increase security by using protected areas in memory that runs your sensitive code and data. For more information, see [Intel® Software Guard Extensions](https://software.intel.com/en-us/sgx).

To provision a bare metal server with Intel SGX, see [Provisioning a bare metal server with Intel SGX](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-bm-server-provision-sgx#bm-server-provision-sgx).

### Intel Optane SSD

[Intel® Optane™ SSD](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-ordering-ssd) DC P4800X is a solid-state drive that combines the attributes of storage and memory to create a new storage tier. The drives are available for a selection of IBM Cloud® Bare Metal Servers.

For more information, see [Product Brief: Intel® Optane™ SSD DC P4800X Series](https://www.intel.com/content/www/us/en/solid-state-drives/optane-ssd-dc-p4800x-brief.html) and [Experience next level compute performance](https://www.ibm.com/cloud/bare-metal-servers/intel?_gl=1*1mlk2fy*_ga*MzUyMzc1NTEuMTY5MzM0MTgyMA..*_ga_FYECCCS21D*MTY5NDEwMDM1OC4xNC4xLjE2OTQxMDQxMzkuMC4wLjA.).

For information on ordering and considerations with GPUs, see [Ordering Optane drives and GPUs](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-ordering-ssd#ssd_gpu).

### NVMe solid-state drives (SSD)

See [Considerations for NVMe SSDs](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-ordering-nvme-ssd#NVMe_considerations) and [Order an NVMe SSD](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-ordering-nvme-ssd#order-NVMe-ssd).

### RAID

See [About RAID](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-bm-raid-levels) for RAID levels offered.

### Software options

IBM Cloud has strategic relationships with vendors to provide month-to-month licenses on 32-bit and 64-bit compatible software.

#### Anti-virus, security

IBM offers Trellix solutions for anti-virus, Adaptive Threat Protection (ATP), ENS Firewall, ENS Threat Prevention, ENS Web Control on Windows® devices. You can get protection for Windows for a monthly fee.

#### Operating systems

See [Supported operating systems for IBM Cloud® server software](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-software#supported-operating-systems-for-ibm-cloud-servers).

### Network options

The following [network options](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options) are avaiable:

- [Interface](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-interfaces). Choose whether you want your server to have public internet access, or only a private interface.
- [Port redundancy](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-port-redundancy). Choose from:

    - **Automatic** is the default and recommended setting. Automatic port redundancy provides two physical network ports that are configured with LACP bonding on both the network and the operating system at time of provisioning. 
    - **User managed** is available for advanced configurations. It provides two physical network ports, but the ports are configured independently on both the network and the operating system. 
    - **None** provides a single physical port to each network.

- [Port speed](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-port-speed). Select either 100 Mbps, 1 Gbps, 10 Gbps, or 25 Gbps as the maximum operating speed of all network interfaces.
- [Public egress bandwidth](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-bandwidth-public)
- [Provision VLAN selection](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-vlan-selection). This selection is optional, and shows only existing VLANs located that are within the selected data center. The selector is for a private VLAN, and when you choose a private VLAN, a public VLAN selector is presented. It shows public VLANs that are available in the same pod as the selected private VLAN (if a public interface is applicable). 
- [Provision subnet selection](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-subnet-selection)
- [Primary IP addresses](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-ip-address-primary) and [Secondary IP addresses](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-network-options#network-ip-address-secondary)

## VMware

IBM Cloud® provides the unique capability for you to provision dedicated Bare Metal Servers upon which you can deploy your own VMware based private cloud. For example, you can enable the creation of a hybrid cloud where on-premises VMware based servers, tooling, and processes can be extended into the public cloud. 

For more information, see [Getting started with VMware and IBM Cloud](https://cloud.ibm.com/docs/vmware?topic=vmware-vmware-getting-started).


## SAP-certified infrastructure

The IBM Cloud® SAP-Certified Infrastructure gives you the flexibility to run your SAP workloads in the IBM Cloud when you need them, where you need them with over 60 IBM data centers worldwide. For more information, see [Getting started with SAP](https://cloud.ibm.com/docs/sap).

## Landing zone for Virtual Server Instances

A best practice landing zone architecture shows how to build virtual server instances (VSI) across multiple subnets with any number of block storage volumes that are connected by any number of load balancers, as shown in the following diagram.

![vsi-lb](./media/vsi-lb.png)

For more information and for the Terraform code to implement, see [IBM Secure Landing Zone VSI Module](https://github.com/terraform-ibm-modules/terraform-ibm-landing-zone-vsi).

## Next steps

Learn how to:

- [Provision](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-bm-select-popular-servers)
- [Connect to your servers](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-navigating-devices)
- [Configure a server](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-navigating-devices) including how to assign IP addresses, mount an ISO on bare metal
- [Manage a server](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-bm-manage-servers)
- [Monitor](https://cloud.ibm.com/docs/cloud-infrastructure?topic=cloud-infrastructure-monitoring-iaas)
- [Migration](https://cloud.ibm.com/docs/cloud-infrastructure?topic=cloud-infrastructure-about-migration-infra)

## References

- Product documentation [Bare Metal Servers for Classic](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-about-bm)
- [IBM Secure Landing Zone VSI Module](https://github.com/terraform-ibm-modules/terraform-ibm-landing-zone-vsi)