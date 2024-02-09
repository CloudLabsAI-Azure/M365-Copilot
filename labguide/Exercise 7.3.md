# Exercise 7.3: Reviewing Security and Compliance in Copilot Using Customer Keys

## Introduction

**Microsoft Copilot** is designed with security and compliance in mind. It does not store or share any of the user's data. It only uses the data or information that the user explicitly provides as input or context. It also respects the user's privacy and preferences, and does not collect any personal or sensitive information by itself.

Given below are the capabilities from Microsoft Purview whcih strengthen your data security and compliance for Microsoft Copilot for Microsoft 365:

## Using Customer Keys in Microsoft 365 Copilot

A **Customer Key** provides extra protection against viewing of data by unauthorized systems or personnel, and complements BitLocker disk encryption and SSE in Microsoft data centers. It helps you meet regulatory or compliance obligations for controlling root keys. You explicitly authorize Microsoft 365 services to use your encryption keys to provide value added cloud services, such as eDiscovery, anti-malware, anti-spam, search indexing, and so on.

Customer Key is built on service encryption and lets you provide and control encryption keys. Microsoft 365 then uses these keys to encrypt your data at rest and helps you meet compliance obligations because you control the encryption keys that Microsoft 365 uses to encrypt and decrypt data.

When you revoke access to your keys as part of leaving the service, the availability key is deleted, resulting in cryptographic deletion of your data. Cryptographic deletion mitigates the risk of data remanence, which is important for meeting both security and compliance obligations.

As with other Microsoft 365 services, such as eDiscovery and search, items encrypted with Microsoft Purview Customer Key are supported and eligible to be returned by **Copilot for Microsoft 365**.

### Encryption Ciphers used by Customer Key

Customer Key uses various encryption ciphers to encrypt keys as shown in the following figure:

![](./media/customer-key-encryption.png)
