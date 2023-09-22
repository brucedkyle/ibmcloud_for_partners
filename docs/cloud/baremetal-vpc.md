# IBM Cloud Bare Metal on VPC Infrastructure

You can provision dedicated, **Bare Metal Servers for VPC** on your own software-defined, private cloud and deploy to multizone regions. A bare metal server is ideal for expanding capacity of applications that benefit from elastic, quick provisioning, and deprovisioning. Accelerate deployment with preset server profiles for your high-performance workloads.

Choose a pre-set metal server profile and deploy to multiline regions in 10 minutes or less, across a software-defined network. Features the latest 2nd Generation Intel Xeon processor. Ideal for high-availability and maximum-elasticity demands.

You get the full suite of IBM Cloud VPC networking benefits, plus 4x faster networking throughput (up to 100 Gbps). Using a VPC for your dedicated, bare metal servers helps you isolate and provision network segments on the cloud, where you then can deploy and manage your compute, storage, and networking.

!!! key "Key user stories"

    - As an enterprise customer of IBM Cloud, I want to migrate my applications from Classic IaaS to VPC to eliminate networking challenges behind traditional gateways, VLANs, and assigned IPs.
    - As a bare metal user, I need scalability, elasticity, and performance. VSI VPC and VSI Classic do not meet my application performance requirements and do not want to make trade-offs.
    - As a VPC user I want to manage my own virtualization and use bare metal for its single tenancy and consistent higher performance.

## Benefits

In addition to natively landing within VPC for its advantages across compute, networking, and storage, bare metal VPC provides:

- Dedicated single tenancy
- Hardware level performance
- Larger core and memory profiles
- 4x faster network performance
- Customer managed virtualization

## Bare metal servers vs virtual server instances

In general, you choose bare metal servers over virtual server instances if you need access to the actual hardware to run a hypervisor such as VMware's ESXi, or run real-time workloads.

Bare Metal Servers for VPC offers improved security compared to a virtual server instance as customers fully manage the physical resources of a bare metal server until it is decommissioned. By contrast, virtual server instances can share resources such as CPU, memory, and processes, across an IBM managed hypervisor.

!!! Tip

    Keep the following lifecycle operations differences in mind:
    
    - For **bare metal servers**, you can restart, or power the server off and on. When you power off a server, the server is powered off physically, but the data on it is preserved, and you continue to be billed.
    - For **virtual server instances**, you can restart, stop, and start the instance. But these functions don't impact the physical server status. Billing is suspended for some types of instances when powered off. However, any persistent storage continues to be billed. For more information about suspend billing, see [Suspend billing for VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-suspend-billing).

!!! note "For VMware support by VPC" 

    Bare Metal Servers for VPC sets up a VMware virtualization environment in a VPC. 

## Use cases for bare metal VPC

General bare metal users can deploy:

| | Pain point | Solution |
|--|--|--|
| **End User Virtualization** | VPC doesn’t allow me a way to create and manage my own VMs | Bare metal VPC does not install a KVM hypervisor offering users the option to virtualize with a software/hypervisor of their choosing |
| **Network Intensive Applications** | Classic networking speeds create a bottleneck for my workload | 100Gbps network uplinks in VPC allow up to 8 customer managed vNICs per server eliminating throughput concerns |
| **Compute Sensitive Workloads** | VSIs do not offer the full server resource and consistent performance I need to run my application | 100% of bare metal compute resources are provided to the customer for dedicated physical core performance and maximum memory consumption |

## Support for VMware vSphere networking

**Bare Metal Servers for VPC** fully supports **VMware vSphere networking** functions. To set up networks in the vSphere environment, you need to first understand the mapping of the networking concepts between your bare metal server and vSphere. See [Mapping network concepts between bare metal servers and VMware vSphere](https://cloud.ibm.com/docs/vpc?topic=vpc-bare-metal-servers-network&interface=cli#mapping-network-concepts).

## Profiles

You can choose different bare metal server profiles to match your individual workload needs and help accelerate deployment of your compute resources. You get maximum performance without oversubscribing. IBM Cloud VPC Infrastructure for bare metal servers provides profiles with or without secondary NVMe drives. 

- Balanced profiles are ideal for common high-performance cloud workloads.
- Memory profiles are ideal for more memory intensive cloud workloads.

See [x86-64 bare metal server profiles](https://cloud.ibm.com/docs/vpc?topic=vpc-bare-metal-servers-profile)

### Advanced Intel® Xeon® CPUs

IBM Cloud Bare Metal Servers for VPC Infrastructure are deployed only with second Gen **Intel® Xeon® Platinum 8260** processors that are built for cloud-enterprise applications, HPC workloads, IoT workloads, enhanced networking, and security.

### SmartNIC technology

Get 4x faster network throughput up to 100 Gbps.

## Pricing

See [Pricing](https://www.ibm.com/cloud/vpc/pricing?_gl=1*4wqy4n*_ga*MTgzNjAxNTg1NC4xNjk0NTM4ODk0*_ga_FYECCCS21D*MTY5NDcyMzIyNi43LjEuMTY5NDcyOTQ5NC4wLjAuMA..#tab_2651670).

## Getting started

- [Creating Bare Metal Servers on VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-creating-bare-metal-servers&interface=ui) using the UI, CLI, and API

## References

- Product page: [IBM Cloud Bare Metal Servers](https://www.ibm.com/cloud/bare-metal-servers)
- Documentation [About Bare Metal Servers for VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-about-bare-metal-servers)
