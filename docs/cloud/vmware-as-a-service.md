# VMware as a Service

**IBM Cloud® for VMware as a Service** provides the **VMware Cloud Director™** platform as a managed service. IBM® performs the configuration, hosting, operations, and lifecycle management of the VMware® software so you can quickly deploy your VMware-based cloud computing environments.

!!! key "Keys"

    - Single-tenant VMware as a Service (VMwaaS) on vCloud Director
    - Rapid onboard to an existing, highly-available management plane hosted by IBM
    - Ideal for customers needing direct control over capacity and compute isolation 
    - Based on VMware Cloud Director on NSX-T
    - 7 Host Server Instances to build on
    - Discounts for 1yr and 3yr Committed Instances
    - vSAN or NFS Storage

Compute resources are available as dedicated hosts, by using IBM Cloud bare metal servers, with multiple host configurations available to address various workload requirements.

The following diagram shows VMware as a Service architecture.

![vmware as a service architecture](./media/vmware-aas-archi.svg)

## VMware as a Service features and functions

The VMware as a Service offering has the following features:

- VMware stack management up to the hypervisor level
    - IBM-managed infrastructure
    - IBM-managed VMware components and services
- Dedicated hosts and multiple host profiles for creating VMware vCenter clusters
- Multiple performance options for attached vSAN™ and Network File Storage (NFS v3)
- Optional data protection through the Veeam® Backup and Replication service
- Monthly billing
- Unique provider-managed encryption keys per instance with encrypted VMware storage profiles
- Single sign-on (SSO) with role-based authentication and authorization from IBM Cloud IAM (Identity and Access Management) to VMware Cloud Director
- Improved provisioning speed, availability, and resilience
- Regional-level High Availability through creating VMware Cloud Director provider virtual data centers (PVDCs) and vCenter clusters in multiple data centers in the same region.
- Full compatibility to run existing VMware workloads. Migration of existing IBM Cloud, on-premises or other workloads are fully supported.
- Each VMware as a Service instance contains the following VMware components:
    - Dedicated VMware ESXi™ hosts
    - Dedicated VMware vCenter
    - Dedicated VMware NSX-T™ with dedicated networking
    - Dedicated VMware Cloud Director
- Right-size and scale the VMware environment
    - Add and remove hosts per VMware vCenter cluster
    - Add and remove storage per VMware vCenter cluster
    - Add and remove VMware vCenter clusters
    - Add and remove VMware Cloud Director PVDCs
- Create and delete virtual data centers to deploy VMware workload vApps and virtual machines in VMware Cloud Director

## Next steps

See:

- [Understanding high availability for VMware as a Service](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-ha)
- [Understanding business continuity and disaster recovery for VMware as a Service](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-bc-dr)
- [Learning about VMware as a Service architecture and workload isolation](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-architecture-workload-isolation-learning)
- [Managing IAM access for VMware as a Service](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vmaas-iam&interface=ui)
- [Securing your data in VMware as a Service](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vmaas-data-security&interface=ui)

## Reference

See [VMware as a Service overview](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vmware-aas-overview).