# Unified Key Orchestrator

Managing keys in silos on-premises and across multiple clouds brings up challenges around demonstrating compliance, ensuring the right security posture with key usage and maintaining data governance and sovereignty. A [Gartner report](https://www.gartner.com/en/documents/3991120/develop-an-enterprisewide-encryption-key-management-stra) suggests that security and risk management leaders must develop an enterprise-wide encryption key management strategy or lose the data.

Built on the _Keep Your Own Key_ technology, **Unified Key Orchestrator** helps enterprises manage their data encryption keys across multiple key stores across multiple clouds environments, including keys managed on-premises, on IBM Cloud, AWS and Microsoft Azure.

## Getting started

This section points you to tutorials on how to use Unified Key Orchestrator for:

- AWS 
- Azure and Microsoft 365 workloads
- Cloud Satellite

### With AWS

See [Securely manage AWS S3 encryption keys with IBM Cloud Hyper Protect Crypto Services with Unified Key Orchestrator](https://developer.ibm.com/tutorials/securely-manage-aws-s3-encryption-keys-with-ibm-cloud-hyper-protect-crypto-services-with-unified-key-orchestrator/?_gl=1*1rrqi9j*_ga*MzIxMDU5Njc3LjE2OTIxOTgwODI.*_ga_FYECCCS21D*MTY5MjM4NTg5NC4xMC4xLjE2OTIzOTgwNzkuMC4wLjA.)

The following diagram illustrates the architecture.

![aws](./media/architecture-aws.jpg)

### Microsoft 365

This tutorial focuses on using IBM Cloud Hyper Protect Crypto Services with Unified Key Orchestrator to manage the regulatory compliance requirements of company data in a Microsoft 365 environment on Azure with Azure Key Vault and Azure Active Directory.

See [Manage regulatory compliance of company data in Microsoft 365 with Hyper Protect Unified Key Orchestrator](https://developer.ibm.com/tutorials/manage-regulatory-compliance-of-company-data-in-microsoft-office-365-in-azure/?_gl=1*1dmhv82*_ga*MzIxMDU5Njc3LjE2OTIxOTgwODI.*_ga_FYECCCS21D*MTY5MjM4NTg5NC4xMC4xLjE2OTIzOTgyMzUuMC4wLjA.)

The following diagram illustrates the use case.

![banking use case](./media/banking.png)

### IBM Cloud Satellite

[IBM Cloud Satellite](https://cloud.ibm.com/docs/satellite?topic=satellite-getting-started) provides you with flexibility and scalability to bring your own infrastructures to IBM Cloud. You can run IBM Cloud services anywhere including on your on-prem data centers and other cloud providers. With IBM Cloud Satellite, you can connect your multiple environments to implement distributed cloud solutions to help your enterprise hybrid cloud transformation. 

Key Protect on Satellite allows you to fully control your encryption keys by using your on-prem hardware security module (HSM). Hyper Protect Crypto Services with Unified Key Orchestrator enables you to manage keys in various key management systems, including Key Protect on Satellite, from a single pane of glass.

See [Using Hyper Protect Crypto Services with Unified Key Orchestrator to manage keys in Key Protect on Satellite](https://cloud.ibm.com/docs/hs-crypto?topic=hs-crypto-tutorial-uko-satellite).

The following diagram illustrates the use case:

![cloud satellite](./media/uko-kp-satellite.svg)



## References

- [Announcing Multicloud Key Management with IBM Cloud Hyper Protect Crypto Services](https://www.ibm.com/blog/announcement/announcing-multicloud-key-management-with-ibm-cloud-hyper-protect-crypto-services/)