# Power Systems Virtual Server

**IBM® Power® Systems Virtual Server** is an IaaS offering that allows you to deploy your current **IBM i**, **AIX** and **Linux** workloads in a hybrid cloud environment, without refactoring. Some examples include **SAP**, **SAP HANA**, and **Oracle**, though other home-grown applications are supported too.

Power Systems Virtual Server are located in the IBM data centers, distinct from the IBM Cloud servers with separate networks and direct-attached storage. You can use the Power Systems Virtual Servers to deploy a virtual server, also known as a _logical partition (LPAR)_, in a matter of minutes. 

## Performance

Uncapped shared processors are shared among other clients, while capped shared processors do not expand resources beyond those that are requested, and are used mostly for licensing. Dedicated resources are allocated for a specific client, usually for for specific third-party considerations. Performance on PowerVS is the same as on-prem.

### Storage performance

For each Power Systems Virtual Server instance, you must select a storage tier - **Tier 1** or **Tier 3**. The storage tiers in Power Systems Virtual Server are based on I/O operations per second (IOPS). It means that the performance of your storage volumes is limited to the maximum number of IOPS based on volume size and storage tier. Although, the exact numbers might change over time, the Tier 3 storage is currently set to 3 IOPS/GB, and the Tier 1 storage is currently set to 10 IOPS/GB. See [Storage tiers](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-about-virtual-server#storage-tiers). 

### Networks

When you create a Power Systems Virtual Server, you can select a private or public network interface. See Public and private networks](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-about-virtual-server#public-private-networks),

### Connect to on-premises

Configure the on-prem environment as a virtual connection in IBM Transit Gateway. Or create a VPN connection if the workspace uses Cloud connections or DL.

## How to deploy

Bring your own customized **AIX** or **IBM i** operating system (OS) image to deploy within Power Systems Virtual Server. Simply store your image on Cloud Object Storage (COS), point the Power Systems Virtual Server console to the image, and deploy the Virtual Server instance.

See [Deploying a custom image within a Power Systems Virtual Server](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-deploy-custom-image).

### SAP NetWeaver, SAP HANA

If you are creating or configuring a Power Systems Virtual Server instance to support an SAP NetWeaver or SAP HANA workload, see [Planning your deployment](https://cloud.ibm.com/docs/sap?topic=sap-power-vs-planning-items) and [Deploying your infrastructure](https://cloud.ibm.com/docs/sap?topic=sap-power-vs-set-up-infrastructure).

### Red Hat OpenShift

If you are creating or configuring a **Red Hat OpenShift** Cluster on Power Systems Virtual Server, see [Deploying Red Hat OpenShift Container Platform 4.x on IBM Power Systems Virtual Servers](https://developer.ibm.com/series/deploy-ocp-cloud-paks-power-virtual-server/).

## Key use cases

IBM Power Systems clients who have typically relied upon on-premises-only infrastructure can now quickly and economically extend your Power IT resources off-premises. Avoid the large capital expense or added risk when migrating your essential workloads and get started with Power Systems Virtual Servers today

- **Business continuity planning**. Use Power Systems Virtual Server as a reliable HA/DR destination for on-premise environments, without doubling the cost of hardware ownership. See [case study](https://www.cidademarketing.com.br/marketing/2021/09/02/brf-conclui-plano-de-recuperacao-de-desastres-com-ibm-power-virtual-servers/).

- **Data center strategy optimization**. Provision on-demand to stay up to date with the latest software and streamlined licensing costs, without upskilling in new specialized technologies. See [case study](https://www.ibm.com/case-studies/iptor-sweden/).

- **Modernize**. Start the hybrid cloud journey with a quick, temporary sandbox environment for testing, without sacrificing mission critical uptime. See [case study](https://www.ibm.com/case-studies/fnz-uk/).

- **Operational excellence and cost optimization**. Reduce operational cost with the same Power infrastructure, performance, security and reliability; all without replatforming workloads. See [case study](https://www.ibm.com/blogs/systems/labeyrie-fine-foods-picks-ibm-power-systems-virtual-server/).

## Hardware specification

The following IBM Power Systems can host a Power Systems Virtual Server: 

- IBM Power System S922 (9009-22A)
- IBM Power System S922 (9009-22G)
- IBM Power System E980 (9080-M9S)
- IBM Power System E1080 (9080-HEX)
- IBM Power System S1022 (9105-22A)

See [Hardware specifications](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-about-virtual-server#hardware-specifications). See [Pricing](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-pricing-virtual-server#pricing-virtual-server).

## Get started with a dev test environment

1. **Create a workspace**. A workspace is a free working environment that acts as a folder for all your Power Systems Virtual Server resources at a specific geographic region, including compute, networking, and storage resources.

2. **Create a virtual server instance**. Deploy your first virtual server instance with the storage and network needed.

See [Everything you love about POWER with the benefits of Hybrid Cloud](https://cloud.ibm.com/power/overview).

## Getting started with a production environment

See [Everything you love about POWER with the benefits of Hybrid Cloud](https://cloud.ibm.com/power/overview); click the **Advanced for production** tab.

## See also

- TrustRadius [IBM Power Virtual Server](https://www.trustradius.com/products/ibm-power-system-virtual-server/reviews#overview)

## References

- [Everything you love about POWER with the benefits of Hybrid Cloud](https://cloud.ibm.com/power/overview)
- [Getting started with IBM Power Systems Virtual Servers](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-getting-started)
- [Deploying a custom image within a Power Systems Virtual Server](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-deploy-custom-image)