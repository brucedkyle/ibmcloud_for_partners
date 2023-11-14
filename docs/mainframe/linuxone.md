# LinuxONE

IBM LinuxONE is an enterprise-grade Linux® server that brings together IBM’s experience in building enterprie systems with the openness of the Linux operating system.

!!! key "Sustainability"

    LinuxONE is designed to help you meet your sustainability goals. Consolidating workloads from many x86 servers onto a single LinuxONE server can reduce energy costs, carbon footprint, and floor space.

    Learn how a single IBM LinuxONE Emperor 4 delivers scalability, doing the work of up to 2000 x86 cores.[^1]

    Consolidating Linux workloads on 5 IBM LinuxONE Emperor 4 systems instead of running them on compared x86 servers under similar conditions can reduce energy consumption by 75%, space by 50%, and the CO2e footprint by over 850 metric tons annually.[^2]

    See [Sustainability on IBM LinuxONE 4](https://www.ibm.com/products/linuxone-4/sustainability).

With a unique architecture designed to meet the needs of mission-critical workloads, LinuxONE provides a sustainable, secure and scalable system for companies of all sizes. 

IBM® LinuxONE is a platform for the Linux® operating system built on a secure, reliable, scalable and [sustainable](https://www.ibm.com/products/linuxone-4/sustainability) architecture. It is used in many different industries worldwide.

LinuxONE is available in single frame, multi frame and rack mount servers. LinuxONE 4 servers can have up to 200 cores running at 5.2 GHz and up to 40 TB of memory.

## LinuxONE 4

[IBM LinuxONE 4](https://www.ibm.com/products/linuxone-4) is the latest iteration of IBM LinuxONE enterprise servers with on-chip AI inferencing and industry-first quantum-safe technologies. 

IBM LinuxONE 4 helps organizations that care about achieving sustainability goals reduce energy costs and carbon footprint with a security-rich, high-performance server platform for data-intensive workloads.

!!! keys "Features"

    - [Simplified compliance](https://www.ibm.com/products/z-security-and-compliance-center).
    - [Confidential computing](https://www.ibm.com/downloads/cas/O158MBWG)
    - [Quantum-safe cryptography](https://research.ibm.com/blog/nist-quantum-safe-protocols)
    - [Open hubrid cloud](https://www.ibm.com/downloads/cas/A2LMYLGN)
    - [Secure critical workloads](https://www.ibm.com/products/hyper-protect-virtual-servers)
    - 99.999999% Availability
    - Engergy efficiency

## LinuxONE for VPC

LinuxONE for VPC are virtual servers based on the LinuxONE processor architecture that bring the advantages of the platform together with the advantages of VPC. For the first time, LinuxONE is available as a choice in the public cloud. This grants additional and unique options for companies and individuals looking to develop in the public cloud with the backing of an enterprise-grade Linux server. 

For those who have or are interested in similar deployments on-premises, this option allows development and testing of the application or workload in the public cloud. Spin up a few instances to experience the LinuxONE platform for just a few hours or stand up a permanent public cloud development environment before porting workloads to production on-premises. Besides the Virtual Private Cloud, these virtual servers come with a host of benefits, such as the following:

- Simplified logging and monitoring: Use a dashboard to view the health of virtual servers and their usage in a graphical interface.
- Backup and restore: Use in combination with [IBM Cloud Object Storage](https://www.ibm.com/cloud/object-storage) to ensure high availability.
- File share: Share data volumes between instances for faster communication.
- Snapshot: Take moment-in-time backups of instances and save in storage for quick recovery.
- Start/Stop/Restart: Invoke a restart without submitting a ticket and waiting for help.
- Terraform integration: Efficiently scale-up cloud infrastructure with an industry-standard tool
- Network features: Enable customers to build a secure private network for protected communication between all of their environments

## Get started on IBM Cloud

Provisioning, deployment and management all occur through the standard [IBM Cloud Virtual Servers for VPC catalog page](https://cloud.ibm.com/vpc-ext/provision/vs). Check out the [VPC documentation](https://cloud.ibm.com/docs/vpc?topic=vpc-getting-started) for additional help.

Try out LinuxONE:

[![openshift on linuxone](./media/openshift-on-linux-one.png)](https://linuxone.cloud.marist.edu/#/register?flag=OCP) 
[![LinuxONE VM](./media/linuxone-vm.png)](https://linuxone.cloud.marist.edu/#/register?flag=VM)

### Use containers on LinuxONE

See [Containers on LinuxONE](./containers.md)

## Next steps

See:

- [IBM Developer LinuxONE resources hub](https://developer.ibm.com/components/ibm-linuxone/) 
- [IBM LinuxONE Redbooks](https://www.redbooks.ibm.com/domains/linuxone)

[![fast start linuxone](./media/fast-start-linux-one.png)](https://www.ibm.com/community/z/linuxone-cc/faststart/?cm_sp=ibmdev-_-developer-articles-_-ibmcom)

Download [LinuxONE for Dummies](https://www.ibm.com/account/reg/us-en/signup?formid=urx-36404&cm_sp=ibmdev-_-developer-articles-_-ibmcom).

## References

- Product page [IBM LinuxONE](https://www.ibm.com/linuxone)
- [Journey to LinuxONE](https://www.ibm.com/support/z-content-solutions/journey-to-linuxone/)
- Blog post [Announcing IBM Cloud LinuxONE Virtual Servers for VPC](https://www.ibm.com/blog/announcement/announcing-ibm-linuxone-for-vpc/)
- Developer [Get started with IBM LinuxONE](https://developer.ibm.com/articles/get-started-with-ibm-linuxone/)
- [Sustainability on IBM LinuxONE 4]

[^1]:
    IBM internal tests show that when running WebSphere and DB2 workloads, IBM LinuxONE Emperor 4 requires 16 times fewer cores than the compared x86 servers. If you scale this up to a complete IT solution this means when running this workload, the IBM LinuxONE Emperor 4 Max 125 would be doing the work of about 2000 cores of the compared x86 servers.
[^2]:
    DISCLAIMER: Compared 5 IBM Machine Type 3931 Max 125 model consists of three CPC drawers containing 125 configurable cores (CPs, zIIPs, or IFLs) and two I/O drawers to support both network and external storage versus 192 x86 systems with a total of 10364 cores. IBM Machine Type 3931 power consumption was based on inputs to the IBM Machine Type 3931 IBM Power Estimation Tool for a memo configuration. x86 power consumption was based on March 2022 IDC QPI power values for 7 Cascade Lake and 5 Ice Lake server models, with 32 to 112 cores per server. All compared x86 servers were 2 or 4 socket servers. IBM Z and x86 are running 24x7x365 with production and non-production workloads. Savings assumes a Power Usage Effectiveness (PUE) ratio of 1.57 to calculate additional power for data center cooling. PUE is based on Uptime Institute 2021 Global Data Center Survey (https://uptimeinstitute.com/about-ui/press-releases/uptime-institute-11th-annual-global-data-center-survey). CO2e and other equivalencies that are based on the EPA GHG calculator (https://www.epa.gov/energy/greenhouse-gas-equivalencies-calculator) use U.S. National weighted averages. Results may vary based on client-specific usage and location.