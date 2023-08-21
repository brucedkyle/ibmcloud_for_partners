# Key Protect

**IBM® Key Protect for IBM Cloud®** is a full-service encryption solution that allows data to be secured and stored in IBM Cloud using the latest envelope encryption techniques that leverage FIPS 140-2 Level 3 certified cloud-based _hardware security modules (HSM)_.

> The trick to securing your data is not just to encrypt information so that it cannot be decoded easily but to protect the ciphers used to encrypt and decrypt it (since having a cipher is as good as having the data).

Key Protect keeps data secure by encrypting the data encryption keys (DEKs) that encrypt your plaintext data with root keys managed by IBM via an impenetrable HSM. In this kind of a system, known as _envelope encryption_, the process of decrypting the data means first "unwrapping" the encrypted DEK (opening its envelope, in other words) and then using the DEK to decrypt the data.

!!! Tip

    **Key Protect** is a cloud-based key management system that provides the best of cost, security, and scale. If you are looking for a dedicated key management solution that supports customer-controlled, cloud-based HSMs **IBM Cloud Hyper Protect Crypto Services** <ins>integrates with Key Protect</ins> to enable _Keep Your Own Keys (KYOK)_ for IBM Cloud, so your organization has more control and authority over its data. 

For more information about envelope encryption works, check out [Protecting data with envelope encryption](https://cloud.ibm.com/docs/key-protect?topic=key-protect-envelope-encryption).


## Reference

- [About Key Protect](https://cloud.ibm.com/docs/key-protect?topic=key-protect-about)