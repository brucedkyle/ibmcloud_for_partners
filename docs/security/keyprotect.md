# Key Protect

**IBM® Key Protect for IBM Cloud®** is a full-service encryption solution that allows data to be secured and stored in IBM Cloud using the latest envelope encryption techniques that leverage FIPS 140-2 Level 3 certified cloud-based _hardware security modules (HSM)_.

> The trick to securing your data is not just to encrypt information so that it cannot be decoded easily but to protect the ciphers used to encrypt and decrypt it (since having a cipher is as good as having the data).

!!! Tip

    **Key Protect** is a cloud-based key management system that provides the best of cost, security, and scale. <br/><br/> If you are looking for a dedicated key management solution that supports customer-controlled, cloud-based HSMs **IBM Cloud Hyper Protect Crypto Services** <ins>integrates with Key Protect</ins> to enable _Keep Your Own Keys (KYOK)_ for IBM Cloud, so your organization has more control and authority over its data. 

## Benefits

- **Fully managed key management system**. Create or import both root and standard keys. Manage your user roles, key states, and set a rotation schedule. Leverage the power of IBM master keys stored inside an HSM shared across IBM Cloud multi-zone regions for the best in cost, performance, and security. 
- **Integration with IBM products**. Key Protect integrates easily with a variety of IBM database, storage, container, and ingestion services. For more information, see [Integrating services](https://cloud.ibm.com/docs/key-protect?topic=key-protect-integrate-services). 
- **Security, compliance, and auditing**. In addition to the FIPS 140-2 Level 3 certified cloud-based hardware security modules (HSMs), Key Protect leverages IBM Cloud [Identity and Access Management (IAM) roles](https://cloud.ibm.com/docs/account?topic=account-userroles).
- **Monitoring**. Use the IBM Cloud Monitoring service and IBM Cloud Activity Tracker to measure how users and applications interact with Key Protect.
- **Low cost**. See [pricing](https://cloud.ibm.com/docs/key-protect?topic=key-protect-pricing-plan).

## How it works

Key Protect keeps data secure by encrypting the data encryption keys (DEKs) that encrypt your plaintext data with root keys managed by IBM via an impenetrable HSM. In this kind of a system, known as _envelope encryption_, the process of decrypting the data means first "unwrapping" the encrypted DEK (opening its envelope, in other words) and then using the DEK to decrypt the data.

The following architecture diagram shows how Key Protect components work to protect your sensitive data and keys.

![kp architecture](./media/kp-architecture.svg)

For more information about envelope encryption works, see [Protecting data with envelope encryption](https://cloud.ibm.com/docs/key-protect?topic=key-protect-envelope-encryption).

To comply with strict data governance and regulatory audit requirements, you want to integrate your apps with a key management service that offers fine-grained access control to encryption keys, audit trail capabilities, and flexible options for uploading encryption keys that you generate on-premises.

With Key Protect, you create encryption keys by using your internal key management system, and then upload those keys for use on the cloud.

You can choose from [different options](https://cloud.ibm.com/docs/key-protect?topic=key-protect-importing-keys#plan-ahead) for uploading keys based on your ongoing security needs. As you manage the lifecycle of encryption keys, you control access to resources by using Cloud Identity and Access Management, and you monitor API activity to the service with Activity Tracker.

## Envelope encryption

Key Protect uses _envelope encryption_ to assist in protecting your Key Protect data. Envelope encryption involves encrypting your data with a Data Encryption Key, then encrypting the Data Encryption Key with a root key. 

The following diagram shows a contextual view of envelope encryption.

![envelope encryption](./media/envelope-encryption.svg)

For more information about root keys and standard keys and the steps involved in using envelope encryption with Key Protect, see [Protecting data with envelope encryption](https://cloud.ibm.com/docs/key-protect?topic=key-protect-envelope-encryption).

## Pricing

See:

- [Pricing for Key Protect on IBM Cloud](https://cloud.ibm.com/docs/key-protect?topic=key-protect-pricing-plan&interface=ui).
- [Pricing for Key Protect on Satellite](https://cloud.ibm.com/docs/key-protect?topic=key-protect-pricing-plan-satellite&interface=ui)

## Reference

- [About Key Protect](https://cloud.ibm.com/docs/key-protect?topic=key-protect-about)
- [Protecting data with envelope encryption](https://cloud.ibm.com/docs/key-protect?topic=key-protect-envelope-encryption)