# Exercise 5.1: Reviewing Security and Compliance in Copilot using Sensitivity Labels (Read Only)

In this exercise, you will explore how Microsoft Copilot integrates with Sensitivity Labels to enhance data security and compliance. Sensitivity Labels help classify and protect data based on its sensitivity level. You will learn about creating, applying, and publishing these labels using Microsoft Purview, understanding how they can be used to safeguard your organization’s sensitive information.

## Overview

**Microsoft Copilot** is designed with security and compliance in mind. It does not store or share any of the user's data. It only uses the data or information that the user explicitly provides as input or context. It also respects the user's privacy and preferences, and does not collect any personal or sensitive information by itself.

Given below are the capabilities from Microsoft Purview which strengthen your data security and compliance for **Microsoft Copilot for Microsoft 365**:

## Task 1: Implementing Sensitivity Labels with Purview 

Sensitivity labels are a way of categorizing and protecting your data based on its level of confidentiality and the impact to your business if it is leaked or misused. You can use sensitivity labels to apply metadata tags and encryption settings to your data sources, columns, tables, and files. Purview is a service that helps you manage and govern your data across your organization.

CoPilot is a system that aids in the management and control of data within an organization. It can work in conjunction with Sensitivity Labels to classify and protect sensitive information. Sensitivity Labels are attributes that can be applied to documents and emails to classify them based on the content sensitivity. These labels can trigger protective actions like encryption or visual markings. Once a sensitivity label is applied to content, it stays with the content regardless of where it's stored or with whom it's shared.

### Understanding Sensitivity labels

Sensitivity labels in Microsoft 365 allow organizations to classify and protect their sensitive content. Here's some information on what these labels represent in Contoso Ltd:

- **Confidential:**
The **Confidential** sensitivity label is used when information is meant to be restricted to a specific group of people within an organization. This label is typically used for data such as employee records, internal policies, or strategic plans. Unauthorized disclosure of this information can lead to potential damage to the organization, but not to the same extent as that classified as **Highly Confidential**.

- **Highly Confidential:**
The **Highly Confidential** sensitivity label is assigned to the most sensitive information that, if disclosed, could result in severe harm to the organization. This might include trade secrets, legal documents, or personally identifiable information (PII) such as social security numbers, credit card information, or health records. Extra security measures, like encryption, are often applied to these documents to prevent unauthorized access or sharing.

- **Internal:**
The **Internal** sensitivity label is used for information that is not intended for public view but doesn't necessarily contain sensitive data. This could include internal newsletters, meeting minutes, or project plans. This label serves as a reminder to employees that the information should not be shared outside the organization, though its disclosure wouldn't cause significant harm.

- **Public**
The **Public** sensitivity label is applied to information that can be freely shared both inside and outside the organization. This information poses no risk if disclosed and is often intended for public consumption. Examples could include press releases, marketing materials, or public-facing reports.

   >**Note:** Remember, sensitivity labels are a tool for managing and protecting data, but they are most effective when combined with user education about data handling and security best practices.

   >**Note:** Your access has been set to Global Reader, meaning you won't be able to make changes. These instructions are for viewing only, reflecting the read-only access granted in your environment.


### Task 1.1: How are sensitivity labels created in Microsoft Purview (Read Only)

In this task, you will learn how Purview is used to implement sensitivity labels for your data assets.

>**Note:** You are not expected to perform the following steps. This information is provided solely to give you an understanding of the process of creating and publishing Sensitivity Labels in the Purview portal.


- Navigate to the [Microsoft Purview] `https://compliance.microsoft.com/homepage` portal and from the left menu select **labels (1)** and in the yellow information box, indicate that Your organization has not turned on the ability to process content in Office online files that have encrypted sensitivity labels applied and are stored in OneDrive and SharePoint. Select **Turn on now (2)**. Once you do this, there can be a delay for the setting to propagate through the system.

   ![](./media/exercise3(2.1).png)

- On **Labels (1)** page, select **+ Create a label (2)**.

   ![](./media/exercise3(2.2).png)

- Provide a name and description for your label. Select **Next (4)** at the bottom of the page.

    | Setting | Action |
    | -- | -- |
    | **Name** | Enter **Confidential-Finance (1)** |
    | **Display name** | Enter **Confidential-Finance (2)** |
    | **Description for users** | Enter **Confidential-Finance Demo (3)** | 

   ![](./media/exercise3(2.3).png)

- Note the scope for this label. The scope is set to Items. Read the description but don’t change anything. Select **Next** at the bottom of the page.

   ![](./media/exercise3(2.4).png)

- On the **Choose protection settings for labeled items** select **Apply or remove encryption (1)** and **Apply content marking (2)**, then select **Next (3)**.

   ![](./media/exercise3(2.5).png)   

- The Encryption window shows the configuration for the encryption settings. Review the information box under Configure encryption settings and review the configured settings. Notice how the user access to content is set to never expire. You can also assign permissions to specific users and groups By clicking on the **Assign permissions (1)**. On the Assign permissions blade, click on **+ Add users or groups (2)**.

   ![](./media/exercise3(2.6).png)

-  On the **Add users or groups** window, select the user name and click on **Add (2)**.

   ![](./media/exercise3(2.7).png)

- You will be redirected to the **Assign Permission** page. Verify that the user is selected and click on **Save (2)**.

   ![](./media/exercise3(2.8).png)

   >**Note:** Only selected users can interact with content that has this label applied. Under users and groups, the tenant is defined so all users in your tenant can view content that has this label.

- Click Next on Encryption window.

   ![](./media/exercise3(2.9).png)

- On the content markings page, take note of the information box at the top of the page. Turn on the **Content Making (1)** and select the check box for **Add a watermark (2)**, **Add a header (3)** and **Add a footer (4)**.

   ![](./media/exercise3(2.10).png)

- Under **Add a watermark**, click on **Customize text (1)**. Under Watermark text, type **Confidential watermark text (2)** and click on **Save (3)**.

   ![](./media/exercise3(2.11).png)

- Under **Add a header**, click on **Customize text (1)**. Under Header text, type **Confidential Document (2)** and click on **Save (3)**.

   ![](./media/exercise3(2.12).png)

- Under **Add a footer**, click on **Customize text (1)**. Under Footer text, type **Confidential Document (2)** and click on **Save (3)**.

   ![](./media/exercise3(2.13).png)

   >**Note**: Content markings will be applied to documents but only headers and footers will be applied to email messages. In other words, watermarks are not applied to emails.

- The content marking associated with this label is a watermark. Select Next at the bottom of the page.

   ![](./media/exercise3(2.14).png)

- You are now in the Auto-labeling for files and emails window. Turn on the **Auto-labeling for files and emails (1)** and Read the description of auto-labelling on the top of the page and the information box below it and under Detect content that matches these conditions click on **+ Add condition (2)** from the drop-down select **Content contains (3)** then under Group name select **Add (4)** drop-down, select Sensitive info type and in Sensitive info type (5) window search for **Credit (6)** and select the **Credit card number (7)**, select **Add (8)** from the button, select **Next (9)** on the bottom of the page.

   ![](./media/exercise3(2.15).png)
  
   ![](./media/exercise3(2.16).png)
  
   ![](./media/exercise3(2.17).png)
  
   ![](./media/exercise3(2.18).png)

- This next window defines protection settings for groups and sites that have this label applied. If this is not enabled, select Next at the bottom of the page.

   ![](./media/exercise3(2.19).png)

- Review the settings and click on Create label.

   ![](./media/exercise3(2.20).png)

### Task 1.3: Publish sensitivity label (Read Only)

The task aims to provide a streamlined method for publishing sensitivity labels to users. Users are guided through a series of steps within Microsoft Purview, specifically under Label policies. The objective is to make the selected labels, such as Confidential-Finance and Highly-Confidential, available to all users, ensuring consistent and standardized data protection measures.

- In the Microsoft Purview. portal, under Solutions, expand Information protection and in the drop-down select **Label policies (1)** and click on **Publish label (2)**.

   ![](./media/exercise3(2.21).png)

- Select **Choose sensitivity labels to publish (1)**. A window opens that provides information about the policy. Select **Confidential-Finance (2)** from the label and select **Add (3)**.

   ![](./media/exercise3(2.22).png)

- Back on **Choose sensitivity labels to publish** blade, click on **Next**.

   ![](./media/exercise3(2.23).png)

- Click on **Next** on the **Assign Admin Units** page.

   ![](./media/exercise3(2.24).png)

- Read the description under **Publish to users and groups**. Notice that this label is available to all users. Don’t change any settings. Select **Next** at the bottom of the page.

   ![](./media/exercise3(2.25).png)

- Under the policy settings, don’t change any settings. Select **Next** at the bottom of the page.

   ![](./media/exercise3(2.26).png)

- Under the **Apply a Default label to documents**, don’t change any settings. Select **Next** at the bottom of the page.

   ![](./media/exercise3(2.27).png)

- Under the **Apply a Default label to emails**, don’t change any settings. Select **Next** at the bottom of the page.

   ![](./media/exercise3(2.28).png)

- Under the **Apply a default label to meetings and calendar events**, don’t change any settings. Select **Next** at the bottom of the page.

   ![](./media/exercise3(2.29).png)

- Under the **Apply a default label to Fabric and Power BI content**, don’t change any settings. Select **Next** at the bottom of the page.

   ![](./media/exercise3(2.30).png)

- The last configuration option is to name your policy. Enter the policy name as **Confidential-Policy (1)**. Select **Next (2)** on the bottom of the page to exit the policy configuration and return to the **Information Protection** page.

   ![](./media/exercise3(2.31).png)

- Review the settings and click on **Submit** and then select **Done**.

   ![](./media/exercise3(2.32).png)
  
   ![](./media/exercise3(2.33).png)

- Back to **Label policies** blade and notice the newly published label.

   ![](./media/exercise3(2.34).png)



This task has provided a clear walkthrough for implementing sensitivity labels in Microsoft Purview, enabling users to categorize and safeguard data based on confidentiality. The guided steps cover label creation, encryption configuration, content marking, and automated labeling, fostering a strong understanding of data protection. Customization options for watermarks, headers, and footers enhance security measures. Demonstrating practical application, the task integrates sensitivity labels seamlessly into Word documents, emphasizing their importance in real-world scenarios. The subsequent label publishing and application steps ensure consistent and standardized data protection, contributing to a robust organizational data governance framework.


## Using Sensitivity Labels in Microsoft 365 Copilot

**Sensitivity labels** from Microsoft Purview Information Protection let you classify and protect your organization's data, while making sure that user productivity and their ability to collaborate isn't hindered.

Sensitivity labels offer the following capabilities:

1. **Customiable:** Specific to your organization and business needs, you can create categories for different levels of sensitive content in your organization. For example, Personal, Public, General, Confidential, and Highly Confidential.

1. **Clear Text:** Because a label is stored in clear text in the metadata for files and emails, third-party apps and services can read it and then apply their own protective actions, if required.

1. **Persistent**: Because the label is stored in metadata for files and emails, the label stays with the content, no matter where it's saved or stored. The label identification that's unique to your organization becomes the basis for applying and enforcing policies that you configure.

The sensitivity labels that you use to protect your organization's data are recognized and used by **Microsoft Copilot for Microsoft 365** to provide an extra layer of protection. For example, in Microsoft Copilot Graph-grounded chat conversations that can reference data from different types of items, the sensitivity label with the highest priority (typically, the most restrictive label) is visible to users. Similarly, when sensitivity label inheritance is supported by Copilot, the sensitivity label with the highest priority is selected.

If the labels applied encryption from Microsoft Purview Information Protection, Copilot checks the usage rights for the user. Only if the user is granted permissions to copy (the **EXTRACT** usage right) from an item, is data from that item returned by Copilot.

In short, the user that uses **Microsoft Copilot**, cannot access labeled documents where he/she has not been added to the permissions for the label. When the user has been added to the permissions, with either Reviewer or Viewer permission, then the document can also not be accessed.

In summary, **Microsoft 365 Copilot** is more stringent when handling encrypted documents with a sensitivity label. As you will need either custom permissions or at least the Co-author role, sensitive information is safeguarded. Provided, of course, that:

1. you have sensitivity labels employed within the enterprise;
1. you have set the right level of permissions to the labels;
1. you are protecting your most sensitive information using labels.

## Conclusion

In conclusion, the integration of **Sensitivity Labels in Microsoft Copilot** for **Microsoft 365** significantly enhances security and compliance measures. **Sensitivity Labels**, being customizable, allow organizations to tailor categories for different levels of sensitive content, ensuring alignment with specific business needs. The clear text storage of labels in metadata facilitates interoperability with third-party apps and services, enabling them to apply their protective actions if necessary.

In the context of **Microsoft Copilot**, Sensitivity Labels play a crucial role in providing an extra layer of protection. The visibility of the sensitivity label with the highest priority to users in Graph-grounded chat conversations ensures that the most restrictive label is appropriately acknowledged. To maximize the effectiveness of **Microsoft 365 Copilot** in safeguarding sensitive information, it is imperative for organizations to implement sensitivity labels, establish appropriate permissions, and protect their most sensitive data using these labels. This integrated approach ensures a robust security posture and compliance adherence within the **Microsoft 365** environment.

## Summary

In this exercise, you learned how to use Sensitivity Labels with Microsoft Copilot to secure data effectively. Sensitivity Labels help classify and protect sensitive information by applying protections like encryption. You saw how to create and publish these labels in Microsoft Purview, ensuring that sensitive data is only accessible to authorized users. This approach enhances security and compliance, maintaining robust data protection within your organization.
