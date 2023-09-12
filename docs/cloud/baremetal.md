# IBM Cloud Bare Metal Servers

**IBM Cloud Bare Metal Servers** are single-tenant, dedicated servers that can be deployed and managed as cloud services. They are part of IBM Cloud and are available in either [classic](https://www.ibm.com/products/bare-metal-servers/classic) or [VPC](https://www.ibm.com/products/bare-metal-servers/vpc) deployment models. 


!!! key "Key value"

    Servers can be provisioned and used in hourly and monthly billing increments.
    
    IBM also offers certified infrastructure for some of the most common and demanding enterprise workloads, such as:

    - Bare Metal Servers are available in hourly or monthly increments
    - You get the latest-generation [NVIDIA GPUs](https://www.ibm.com/cloud/gpu) and x86 microarchitecture from [Intel Xeon](https://www.ibm.com/cloud/intel) and [AMD EPYC](https://www.ibm.com/cloud/amd)
    - Multiple Bare Metal Servers can communicate on the IBM Cloud virtual private network as if stationed on the same rack

## Enterprise workloads

For many companies moving to cloud, charting a path forward for their existing applications and infratsructure is a significant part of the task. To support these organizations, IBM offers [SAP-certified](https://cloud.ibm.com/docs/sap?topic=sap-get-started&_gl=1*1n05tqp*_ga*MzUyMzc1NTEuMTY5MzM0MTgyMA..*_ga_FYECCCS21D*MTY5NDEwMDM1OC4xNC4xLjE2OTQxMDE4NTQuMC4wLjA.) and [VMware-certified](https://cloud.ibm.com/docs/vmware?topic=vmware-vmware-getting-started&_gl=1*1n05tqp*_ga*MzUyMzc1NTEuMTY5MzM0MTgyMA..*_ga_FYECCCS21D*MTY5NDEwMDM1OC4xNC4xLjE2OTQxMDE4NTQuMC4wLjA.) infrastructure. This infrastructure is designed to help companies accelerate their migration and modernization journeys. 

## Deployment Options

Customize and deploy IBM Cloud Bare Metal Servers for any workload, including VMware and SAP, on the IBM Cloud infrastructure of your choice. Both deployments are dedicated to your single-tenancy use, with built-in security benefits and computing control.

- [IBM Cloud Bare Metal Servers for Classic](./baremetal-classic.md).
- [IBM Cloud VPC Infrastructure](./baremetal-vpc.md)

!!! Important

    With Bare Metal Servers for VPC, you can enjoy the security and performance of the private cloud with the flexibility and scalability of the public cloud. Compared to the classic bare metal infrastructures, Bare Metal Servers for VPC provides better connectivity and networking throughput by using VPC concepts.

## IBM Cloud VPC Infrastructure

Choose a pre-set metal server profile and deploy to multiline regions in 10 minutes or less, across a software-defined network. 

Features the latest 2nd Generation Intel Xeon processor. 

!!! Tip

    Cloud VPC is ideal for high-availability and maximum-elasticity demands.

For more information see [VPC deployment](https://www.ibm.com/products/bare-metal-servers/vpc)

## Classic vs VPC

In general, you choose bare metal servers over virtual server instances if you need access to the actual hardware to run a hypervisor such as VMware's ESXi, or run real-time workloads.

Bare Metal Servers for VPC sets up a VMware virtualization environment in a VPC. Bare Metal Servers for VPC offers improved security compared to a virtual server instance as customers fully manage the physical resources of a bare metal server until it is decommissioned. By contrast, virtual server instances can share resources such as CPU, memory, and processes, across an IBM managed hypervisor.

Keep the following lifecycle operations differences in mind:

- For bare metal servers, you can restart, or power the server off and on. When you power off a server, the server is powered off physically, but the data on it is preserved, and you continue to be billed.
- For virtual server instances, you can restart, stop, and start the instance. But these functions do not impact the physical server status. Billing is suspended for some types of instances when powered off. However, any persistent storage continues to be billed. For more information about suspend billing, see [Suspend billing for VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-suspend-billing).

## TrustRadius reviews

[Product reviews](https://www.trustradius.com/products/ibm-cloud-bare-metal-servers/reviews) by IBM Cloud Bare Metal Servers customers.

## Next steps

See to the following topics to start planning and creating your bare metal servers on VPC:

- [Planning for Bare Metal Servers for VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-planning-for-bare-metal-servers)
- [Creating a bare metal server on VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-creating-bare-metal-servers)

## Reference

- Product page [IBM Cloud Bare Metal Servers](https://www.ibm.com/products/bare-metal-servers)
- Documentation [Bare Metal Servers for Classic](https://cloud.ibm.com/docs/bare-metal?topic=bare-metal-getting-started)
- Documentation [About Bare Metal Servers for VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-about-bare-metal-servers)