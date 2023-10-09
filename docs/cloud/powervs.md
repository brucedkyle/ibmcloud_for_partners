# Power Systems Virtual Server

<img style="float: right; width: 25%; padding: 0px 0px 1% 1% "  alt="cataloglogo" src="../media/powervs.png" />
**IBM® Power® Systems Virtual Server** is an IaaS offering that allows you to deploy your current **IBM i**, **AIX** and **Linux** workloads in a hybrid cloud environment, without refactoring. Some examples include **SAP**, **SAP HANA**, and **Oracle**, though other home-grown applications are supported too.

Power Systems Virtual Server are located in the IBM data centers, distinct from the IBM Cloud servers with separate networks and direct-attached storage. You can use the Power Systems Virtual Servers to deploy a virtual server, also known as a _logical partition (LPAR)_, in a matter of minutes. 

!!! key "Key value"

    IBM Power:

    - IBM Power is known for its scalability and performance with the most demanding workloads. 
    - IBM Power provides superior virtualization and management features for flexibility, and security with better isolation and integrated stack.

    IBM Power Virtual Servers:

    - The Power Systems Virtual Servers are located in the IBM data centers, distinct from the IBM Cloud servers with separate networks and direct-attached storage. 
    - Power Systems Virtual Server maintain key enterprise software certification and support as the Power Systems Virtual Server architecture is identical to certified on-premises infrastructure.
    - Run existing workloads, such as SAP, SAP HANA, Oracle, and applications on AIX, Linux, IBM i, OpenShift.
    - Straight-forward deployment/migration:
        1. Simply store your image on Cloud Object Storage (COS)
        2. Point the Power Systems Virtual Server console to the image
        3. Deploy the Virtual Server instance.</ol>

## Key use cases

IBM Power Systems clients who have typically relied upon on-premises-only infrastructure can now quickly and economically extend your Power IT resources off-premises. Avoid the large capital expense or added risk when migrating your essential workloads and get started with Power Systems Virtual Servers today.

!!! usecase "Use cases"

    - **Business continuity planning**. Use Power Systems Virtual Server as a reliable HA/DR destination for on-premise environments, without doubling the cost of hardware ownership. See [case study](https://www.cidademarketing.com.br/marketing/2021/09/02/brf-conclui-plano-de-recuperacao-de-desastres-com-ibm-power-virtual-servers/).
    - **Data center strategy optimization**. Provision on-demand to stay up to date with the latest software and streamlined licensing costs, without upskilling in new specialized technologies. See [case study](https://www.ibm.com/case-studies/iptor-sweden/).
    - **Modernize**. Start the hybrid cloud journey with a quick, temporary sandbox environment for testing, without sacrificing mission critical uptime. See [case study](https://www.ibm.com/case-studies/fnz-uk/).
    - **Operational excellence and cost optimization**. Reduce operational cost with the same Power infrastructure, performance, security and reliability; all without replatforming workloads. See [case study](https://www.ibm.com/blogs/systems/labeyrie-fine-foods-picks-ibm-power-systems-virtual-server/).

## Business value

- **Maximize availability** of business-critical workloads to get efficient scaling and consistent pay-for-use consumption across public and private clouds.
- **Respond faster to business demands** with quick provisioning on IBM Cloud.
- **Reliability** with built-in advanced recovery and self-healing for infrastructure redundancy and 
disaster recovery in IBM Cloud.
- **Supports business-critical workloads**:
    - Certified SAP IaaS
    - SAP NetWeaver and S4/HANA
    - Oracle Supported
    - IBM i workloads
    - Epic - Healthcare (training case)
    - Red Hat OpenShift
    - IBM Cloud Paks
    - OS: AIX, IBM i, Linux

- **Comprehensive Compliance**
    - GDPR
    - SOC 1 Type I and II
    - PCI DSS Certification
    - ISO 27K

## Performance

Uncapped shared processors are shared among other clients, while capped shared processors do not expand resources beyond those that are requested, and are used mostly for licensing. Dedicated resources are allocated for a specific client, usually for for specific third-party considerations. Performance on PowerVS is the same as on-prem.

### Storage performance

For each Power Systems Virtual Server instance, you must select a storage tier - **Tier 1** or **Tier 3**. The storage tiers in Power Systems Virtual Server are based on I/O operations per second (IOPS). It means that the performance of your storage volumes is limited to the maximum number of IOPS based on volume size and storage tier. Although, the exact numbers might change over time, the Tier 3 storage is currently set to 3 IOPS/GB, and the Tier 1 storage is currently set to 10 IOPS/GB. See [Storage tiers](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-about-virtual-server#storage-tiers). 

### Networks

When you create a Power Systems Virtual Server, you can select a private or public network interface. See [Public and private networks](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-about-virtual-server#public-private-networks).

### Connect to on-premises

Configure the on-prem environment as a virtual connection in **IBM Transit Gateway**. Or create a VPN connection if the workspace uses Cloud connections or DL.

### Cost effective

For Power applications moving to cloud, Power Virtual Server yields about 47% savings over Azure and AWS 
(x86) Public Clouds.

On-premises Power legacy to Power Virtual Server yields on average 35% savings.

## How to deploy

Bring your own customized **AIX** or **IBM i** operating system (OS) image to deploy within Power Systems Virtual Server. Simply store your image on Cloud Object Storage (COS), point the Power Systems Virtual Server console to the image, and deploy the Virtual Server instance.

See [Deploying a custom image within a Power Systems Virtual Server](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-deploy-custom-image).

### SAP NetWeaver, SAP HANA

If you are creating or configuring a Power Systems Virtual Server instance to support an SAP NetWeaver or SAP HANA workload, see [Planning your deployment](https://cloud.ibm.com/docs/sap?topic=sap-power-vs-planning-items) and [Deploying your infrastructure](https://cloud.ibm.com/docs/sap?topic=sap-power-vs-set-up-infrastructure).

[Forrester Total Economic Impact study](https://www.ibm.com/downloads/cas/4RLB8QVG) describes 212% ROI for SAP on IBM Cloud over 3 years. 

### Red Hat OpenShift

If you are creating or configuring a **Red Hat OpenShift** Cluster on Power Systems Virtual Server, see [Deploying Red Hat OpenShift Container Platform 4.x on IBM Power Systems Virtual Servers](https://developer.ibm.com/series/deploy-ocp-cloud-paks-power-virtual-server/).

## Hardware specification

The following IBM Power Systems can host a Power Systems Virtual Server: 

- IBM Power System S922 (9009-22A)
- IBM Power System S922 (9009-22G)
- IBM Power System E980 (9080-M9S)
- IBM Power System E1080 (9080-HEX)
- IBM Power System S1022 (9105-22A)

See [Hardware specifications](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-about-virtual-server#hardware-specifications). See [Pricing](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-pricing-virtual-server#pricing-virtual-server).

## Step-by-step tutorial

See [IBM Power Systems Virtual Server Level 3 Demonstration Guide](https://ibm.github.io/SalesEnablement-PowerVS-L3/). You will learn the knowledge and tools to perform hands-on demonstrations of IBM Power Systems Virtual Server (PowerVS). 

The tutorial is part of the [IBM Power Systems Virtual Server for Sales Level 3](https://yourlearning.ibm.com/activity/PLAN-570C104B7C0E) badge for IBMers and partners that provides hands-on practice with a live environment.

## Get started with a dev test environment

1. **Create a workspace**. A workspace is a free working environment that acts as a folder for all your Power Systems Virtual Server resources at a specific geographic region, including compute, networking, and storage resources.

2. **Create a virtual server instance**. Deploy your first virtual server instance with the storage and network needed.

See [Everything you love about POWER with the benefits of Hybrid Cloud](https://cloud.ibm.com/power/overview).

## Getting started with a production environment

See [Everything you love about POWER with the benefits of Hybrid Cloud](https://cloud.ibm.com/power/overview); click the **Advanced for production** tab.

## Reference architectures

See [IBM Power Systems architecture](https://www.ibm.com/cloud/architecture/architectures/power/overview/).

## See also

- TrustRadius [IBM Power Virtual Server](https://www.trustradius.com/products/ibm-power-system-virtual-server/reviews#overview).
- White paper [Navigating your hybrid multicloud vision with IBM Power](https://www.ibm.com/downloads/cas/G4DO3DJE)

## References

- [Everything you love about POWER with the benefits of Hybrid Cloud](https://cloud.ibm.com/power/overview)
- [Getting started with IBM Power Systems Virtual Servers](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-getting-started)
- [Deploying a custom image within a Power Systems Virtual Server](https://cloud.ibm.com/docs/power-iaas?topic=power-iaas-deploy-custom-image)
- [IBM Power Systems Virtual Server Sales Foundation](https://learn.ibm.com/course/view.php?id=11419) badge for IBMers and partners.

## For Business Partners

- [Client Presentation - IBM Power Systems Virtual Server (PowerVS)](https://ibm.seismic.com/Link/Content/DCmqdd962PMDH8QP3hpTdHdgVhg3)