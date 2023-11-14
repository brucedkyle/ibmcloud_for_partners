# IBM Cloud Hyper Protect Virtual Servers with LinuxONE

**Hyper Protect Virtual Servers** are fully developer-friendly and able to use industry-standard, _Open Container Initiative (OCI)_ images with a standard user interface to provision, manage, maintain and monitor within the **Virtual Private Cloud (VPC)** infrastructure of **IBM Cloud**. By leveraging VPC, this next generation of Hyper Protect Virtual Servers is able to offer additional network security.

!!! Key

    Complete data privacy and protection over your containerized workloads that hold sensitive data.

## Confidential computing on LinuxONE

Confidential computing is enabled on **LinuxONE** (s390x processor architecture) by using [IBM Secure Execution for Linux](https://www.ibm.com/docs/en/linux-on-systems?topic=virtualization-introducing-secure-execution-linux). This technology is part of the hardware of IBM z15 (z15) and IBM LinuxONE III generation systems. With IBM Secure Execution for Linux, you can securely deploy workloads in the cloud. It ensures the integrity and confidentiality of boot images, and server authenticity. Applications are isolated from the operating system, thus providing more privacy and security for the workload.

By using IBM Secure Execution for Linux, you can create encrypted Linux images that can run on a public, private, or hybrid cloud with their in-use memory protected. The workload or data is protected from external and insider threats.

A new operating system that leverages the IBM Secure Execution for Linux technology is now available as **IBM Hyper Protect**. The associated image that's used to create the instance is called the [IBM Hyper Protect Container Runtime (HPCR) image](https://cloud.ibm.com/docs/vpc?topic=vpc-vsabout-images#hyper-protect-runtime). 

## Virtual server instance

A virtual server instance that's provisioned by using the HPCR image is called as an **IBM Cloud Hyper Protect Virtual Servers for VPC (Virtual Private Cloud)** instance.

For a technical deep dive into the IBM Hyper Protect Platform, see the white paper [The Second Generation of IBM Hyper Protect Platform](https://www.ibm.com/downloads/cas/GPVMWPM3).

## Benefits of Hyper Protect Virtual Servers for VPC

The Hyper Protect Virtual Servers for VPC takes advantage of the IBM Secure Execution for Linux to provide a boundary around each instance and provides the following benefits:

**Secure Execution boundary for protection from internal and external threats**. 
Hyper Protect Virtual Servers for VPC provides technical assurance that unauthorized users, including IBM Cloud admins, do not have access to the application. Workloads are locked down by individual, instance-level secure boundaries.

**Multiparty contract and attestation of deployment**. 
Apply Zero Trust principles from workload development through deployment. As multiple personas and legal entities collaborate, it’s essential to separate duty and access. Hyper Protect Virtual Servers for VPC is based on a newly introduced encrypted contract concept. It enables each persona to provide its contribution and be ensured through encryption that none of the other personas can access this data or intellectual property. The deployment can be validated by an auditor persona through an attestation record, which is signed and encrypted to ensure only the auditor has this level of insight.

**Malware protections**. 
Hyper Protect Virtual Servers for VPC leverages Secure Build to set up a verification process to ensure that only authorized code is running in an application. It deploys only container versions that are validated at deployment through explicit digest or are signed and may be pulled from a private container registry with authentication only.

**Bring your own OCI image and leverage managed Container Runtime service**
Use any open-container initiative (OCI) image and gain the benefits of a confidential computing solution for extra levels of protection. Ensure through a signed contract, that only a given combination of your workload and environment is deployed.

**Built on the Virtual Private Cloud (VPC) infrastructure for extra network security**
Choose from various profile sizes and grow as needed to protect containerized applications and pay-as-you-go on an hourly basis.
Leverage your existing or common network security groups and logging infrastructure.

## Tutorial

This tutorial walks you through the steps to deploy a sample application on Hyper Protect Virtual Server for VPC, which highlights how Confidential Computing can help protect Personally Identifiable Information (PII).

You can provision Hyper Protect Virtual Servers with the advantage of IBM Secure Execution for Linux on IBM Cloud Virtual Private Cloud (VPC) or On-Premises. In this tutorial, we use Hyper Protect Virtual Servers for VPC.

![pay now pattern](./media/paynow-code-pattern.svg)

See [Deploying a sample application on Hyper Protect Virtual Server for VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-financial-transaction-confidential-computing-on-hyper-protect-virtual-server-for-vpc&interface=ui) for the step-by-step tutorial.

## Next steps

Learn more at:

Follow the steps at [Confidential computing with LinuxONE](https://cloud.ibm.com/docs/vpc?topic=vpc-about-se&interface=ui) to get started, including:

- [Additional security responsibilities for IBM Cloud Hyper Protect Virtual Servers for VPC](https://cloud.ibm.com/docs/vpc?topic=vpc-hpvs-security-req&interface=ui)
- [Validating certificates](https://cloud.ibm.com/docs/vpc?topic=vpc-cert_validate&interface=ui)
- [Creating a contract](https://cloud.ibm.com/docs/vpc?topic=vpc-about-contract_se&interface=ui)
- [Attestation](https://cloud.ibm.com/docs/vpc?topic=vpc-about-attestation&interface=ui)
- [Logging](https://cloud.ibm.com/docs/vpc?topic=vpc-logging-for-hyper-protect-virtual-servers-for-vpc&interface=ui)
- [Securing data](https://cloud.ibm.com/docs/vpc?topic=vpc-hyper-protect-virtual-server-mng-data&interface=ui)
- [Verify disk encryption](https://cloud.ibm.com/docs/vpc?topic=vpc-hpvs-disks-encryption-validate&interface=ui)
- [Hyper Protect Secure Build](https://cloud.ibm.com/docs/vpc?topic=vpc-about-hpsb&interface=ui)
- [Using dynamic registry reference](https://cloud.ibm.com/docs/vpc?topic=vpc-hyper-protect-virtual-server-use-dynamic-registry-reference&interface=ui)

## Reference

- Product page [IBM Cloud Hyper Protect Virtual Servers](https://www.ibm.com/products/hyper-protect-virtual-servers/cloud)
- [Confidential computing with LinuxONE](https://cloud.ibm.com/docs/vpc?topic=vpc-about-se&interface=ui)