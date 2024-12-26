# Exercise 5.4: Reviewing Security and Compliance in Copilot Using Customer Keys (Read Only)

In this exercise, we will examine how Customer Keys bolster security and compliance in Microsoft 365 Copilot. Customer Keys allow organizations to control their own encryption keys, which enhances data protection and helps meet regulatory requirements. This feature complements existing encryption methods like BitLocker and SSE, ensuring that sensitive data remains secure.

## Overview

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

## Conclusion

In conclusion, the incorporation of **Customer Keys in Microsoft 365 Copilot** adds an extra layer of protection, fortifying data security and compliance measures. This exercise has elucidated the significance of Customer Keys in preventing unauthorized access to data, complementing existing security measures like BitLocker disk encryption and SSE in Microsoft data centers.

The interoperability of items encrypted with Microsoft Purview Customer Key with **Copilot for Microsoft 365** underscores the seamless integration of security features across Microsoft 365 services. Overall, the utilization of Customer Keys reinforces the robustness of security protocols, contributing to a resilient and compliant environment within the **Microsoft 365** ecosystem.

## Summary

In this exercise, we explored the role of Customer Keys in enhancing data security and compliance in Microsoft 365 Copilot. By managing their own encryption keys, organizations add an extra layer of protection to their data and meet compliance obligations more effectively. The use of Customer Keys ensures that Microsoft 365 services, including Copilot, maintain robust security and meet regulatory standards.
