# Exercise 5.1: Reviewing Security and Compliance in Copilot using Sensitivity Labels

## Introduction

**Microsoft Copilot** is designed with security and compliance in mind. It does not store or share any of the user's data. It only uses the data or information that the user explicitly provides as input or context. It also respects the user's privacy and preferences, and it does not collect any personal or sensitive information by itself.

Given below are the capabilities from Microsoft Purview that strengthen your data security and compliance with **Microsoft Copilot for Microsoft 365**:

## Using Sensitivity Labels in Microsoft 365 Copilot

**Sensitivity labels** from Microsoft Purview Information Protection let you classify and protect your organization's data, while making sure that user productivity and their ability to collaborate aren't hindered.

Sensitivity labels offer the following capabilities:

1. **Customiable:** Specific to your organization and business needs, you can create categories for different levels of sensitive content in your organization. For example, Personal, Public, General, Confidential, and Highly Confidential.

1. **Clear Text:** Because a label is stored in clear text in the metadata for files and emails, third-party apps and services can read it and then apply their own protective actions, if required.

1. **Persistent**: Because the label is stored in metadata for files and emails, the label stays with the content, no matter where it's saved or stored. The label identification that's unique to your organization becomes the basis for applying and enforcing policies that you configure.

The sensitivity labels that you use to protect your organization's data are recognized and used by **Microsoft Copilot for Microsoft 365** to provide an extra layer of protection. For example, in Microsoft Copilot Graph-grounded chat conversations that can reference data from different types of items, the sensitivity label with the highest priority (typically, the most restrictive label) is visible to users. Similarly, when sensitivity label inheritance is supported by Copilot, the sensitivity label with the highest priority is selected.

If the labels applied encryption from Microsoft Purview Information Protection, Copilot checks the usage rights for the user. Only if the user is granted permission to copy (the **EXTRACT** usage right) from an item, is data from that item returned by Copilot.

In short, the user who uses **Microsoft Copilot**, cannot access labeled documents where he/she has not been added to the permissions for the label. When the user has been added to the permissions, with either Reviewer or Viewer permission, then the document can also not be accessed.

In summary, **Microsoft 365 Copilot** is more stringent when handling encrypted documents with a sensitivity label. As you will need either custom permissions or at least the co-author role, sensitive information is safeguarded. Provided, of course, that:

1. You have sensitivity labels employed within the enterprise.
1. You have set the right level of permissions for the labels.
1. You are protecting your most sensitive information using labels.

## Conclusion

In conclusion, the integration of **Sensitivity Labels in Microsoft Copilot** for **Microsoft 365** significantly enhances security and compliance measures. **Sensitivity Labels**, being customizable, allow organizations to tailor categories for different levels of sensitive content, ensuring alignment with specific business needs. The clear text storage of labels in metadata facilitates interoperability with third-party apps and services, enabling them to apply their protective actions if necessary.

In the context of **Microsoft Copilot**, Sensitivity Labels play a crucial role in providing an extra layer of protection. The visibility of the sensitivity label with the highest priority to users in Graph-grounded chat conversations ensures that the most restrictive label is appropriately acknowledged. To maximize the effectiveness of **Microsoft 365 Copilot** in safeguarding sensitive information, it is imperative for organizations to implement sensitivity labels, establish appropriate permissions, and protect their most sensitive data using these labels. This integrated approach ensures a robust security posture and compliance adherence within the **Microsoft 365** environment.
