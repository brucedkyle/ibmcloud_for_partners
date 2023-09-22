# VMware solutions on VPC

The **IBM Cloud® for VMware Solutions** offerings help you extend your existing VMware® virtualized data center into IBM Cloud. 


!!! important 

    The IBM Cloud bare metal server for IBM Cloud VPC provides you compute capacity to host VMware workloads in the IBM Cloud VPC.

With this solution, you have the flexibility to design a VMware deployment for your needs, which is integrated with IBM Cloud VPC. The following diagram shows an overview of the solution.

![vmware vpc](./media/vpc-ryo-diagrams-overview.svg)

The IBM Cloud bare metal server is integrated with the VPC network, and you can take advantage of the network, storage, and security capabilities provided by IBM Cloud VPC. 

## Advantages over bare metal


!!! key "Key Benefits"

    VMware Solutions in IBM Cloud VPC have the following key benefits over IBM Cloud classic deployments:

    - IBM Cloud VPC gives you the ability to easily and rapidly define and control a virtual network, which is logically isolated from all other tenants. The logical isolation is implemented by using virtual network functions and security that is built into the platform.
    - Provisioning the IBM Cloud bare metal server on IBM Cloud VPC takes minutes instead of hours when compared to the IBM Cloud bare metal server on IBM Cloud classic.
    - VMware workloads by running in IBM Cloud VPC can take advantage of all original functions for VPC networking capabilities and other IBM Cloud interconnectivity services.

## Roll-your-own VMware solution on VPC

**Roll-your-own VMware® solution** in VPC is not a managed service. You can use IBM Cloud® services to build your own VMware solution in IBM Cloud VPC.

You are responsible for the VPC deployment and related networking resources, IBM Cloud bare metal server in VPCs and for the deployment, configuration, security, management, and monitoring of all VMware software components.

Consider:

- [Sizing your VMware vSphere clusters](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-sizing)
- [VMware licensing](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-licensing)
- [Network design and connectivity](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-net-design)
- [Security planning and hardening](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-sec-planning)
- [Active Directory](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-ad)
- [Maintenance planning](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-maint-planning)
- [Monitoring](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-monitoring)
- [Business continuity and availability](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-business-cont)
- [Storage planning](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations#vpc-ryo-considerations-storage)

See [Overview of roll-your-own VMware solution on VPC](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-overview)

### IBM Cloud bare metal server for IBM Cloud VPC architecture

The following diagram provides architecture overview of the roll-your-own VMware® solution in IBM Cloud® Virtual Private Cloud. 

[![roll your own vmware in vpc](./media/vpc-ryo-diagrams-aod-non-nsx-based.svg)](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-arch-overview)

The architecture uses the new IBM Cloud bare metal server for IBM Cloud VPC. This fast provisioning IBM Cloud bare metal server provides you compute capacity to host VMware clusters in the IBM Cloud VPC. Through the integration with the VPC platform, you can take full advantage of the network, storage, and security capabilities provided by the VPC.

See:

- [VPC design for VMware deployment](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-vpc-vmw)

### VMware software-defined networking for your workloads and NSX-T™

You can also use VMware software-defined networking for your workloads and NSX-T™. If you use NSX-T with your solution, then you need extra subnets, such as TEP traffic and NSX-T uplinks. 

[![NSX-T solution]./media/vpc-ryo-diagrams-aod-nsx-t-based.svg)](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-arch-overview)

For more information, see:

- [VMware NSX-T design on VPC](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-nsx-t)
- [VMware NSX-T logical routers on VPC deployments](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-nsx-t-logical-routers)
- [VMware NSX-T logical routing on VPC](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-nsx-t-vpc-routing)

## References

- [Deployment considerations for the roll-your-own VMware solution on VPC](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-considerations)
- [Architecture overview of roll-your-own VMware solution on VPC](https://cloud.ibm.com/docs/vmwaresolutions?topic=vmwaresolutions-vpc-ryo-arch-overview)