# Exercise 5.3: Reviewing Security and Compliance in Copilot Using Data Classification (Read Only)

## Introduction

**Microsoft Copilot** is designed with security and compliance in mind. It does not store or share any of the user's data. It only uses the data or information that the user explicitly provides as input or context. It also respects the user's privacy and preferences, and does not collect any personal or sensitive information by itself.

Given below are the capabilities from Microsoft Purview whcih strengthen your data security and compliance for Microsoft Copilot for Microsoft 365:

## Using Data Classification in Microsoft 365 Copilot

**Data classification** plays a critical role in helping businesses organize and safeguard their data. Sorting information by its level of sensitivity — like personally identifiable information or confidential records — lets organizations put in place tailored security measures against unauthorized intrusion and data leaks. Additionally, data classification enables businesses to comply with industry regulations and legal requirements by helping ensure that sensitive information is handled appropriately.

**Data classification** forms the foundation needed for Copilot to function efficiently. By accurately categorizing data, Copilot can provide more precise recommendations, making the classification process faster and more reliable. **Copilot** uses AI and ML technologies to make the categorization of data automated and more efficient. By integrating with existing data management systems, such as SharePoint or OneDrive, Copilot analyses the content of documents and automatically assigns appropriate classification labels. This automation eliminates the need for manual classification, saving time and reducing the risk of human error.

One of the key benefits of Copilot is its ability to learn from user interactions. As users review and validate the classification suggestions Copilot provides, the system becomes more accurate over time, resulting in improved classification outcomes. This iterative learning process ensures that the system aligns with each organization's specific needs and requirements, making it an asset for data management.

### Preparing your data for Copilot

Before deploying Copilot, it is essential to prepare your data to maximize its effectiveness. Consider the following guidelines for effective preparation:

- **Data inventory and analysis:** Conduct a comprehensive inventory of your data and analyze its content to identify patterns and commonalities. This step will help in defining appropriate classification categories and labels.

- **Data cleansing and normalization:** Cleanse and normalize your data by removing duplicates, standardizing formats, removing old or legacy versions and ensuring consistency. This process will improve classification accuracy and optimize Copilot's performance by enabling it to surface accurate data.

- **Engage stakeholders:** Involve key stakeholders, such as legal, compliance and IT teams, in the data preparation process. Their input will ensure the classification process aligns with regulatory requirements and organizational policies.

- **Training and awareness:** Provide training and awareness sessions to users and administrators about the importance of data classification and how to effectively use Copilot. This approach will facilitate a smooth transition and increase user adoption. In addition, utilize organizational change management strategies to champion the process and educate the workforce on how data classification and sanitization can expedite Copilot’s ingestion of the data.

>**Note:** You are not expected to perform the following steps. This information is provided solely to give you an understanding of the process of Data Classification in the Purview portal. Your access has been set to Global Reader, meaning you won't be able to make changes. These instructions are for viewing only, reflecting the read-only access granted in your environment.

### Task 1: Using the Microsoft data classification dashboard

The **data classification page** provides visibility into that body of content, specifically:

- the number items that have been classified as a sensitive information type and what those classifications are

- the top applied sensitivity labels in both Microsoft 365 and Azure Information Protection

- the top applied retention labels

- a summary of activities that users are taking on your sensitive content

- the locations of your sensitive and retained data

Follow the given steps to access the **Microsoft data classification dashboard**:

1. Navigate to `https://compliance.microsoft.com/` and sign in using the **CloudLabs provided credentials**.

1. In the left navigation pane of the compliance portal, select **Data classification** and then, select **Overview**.

1. Data classification will scan your sensitive content and labeled content before you create any policies. This is called **zero change management**. This lets you see the impact that all the retention and sensitivity labels are having in your environment and empower you to start assessing your protection and governance policy needs.

1. The **Top sensitive information type** card shows the top sensitive information types that have been found and labeled across your organization.

1. To find out how many items are in any given classification category, hover over the bar for the category.

    >**Note:** If the card displays the message "**No data found with sensitive information**", it means that there are no items in your organization that have been classified as being a sensitive information type or no items that have been crawled.

1. The **Top sensitivity labels applied to content** card shows the number of items (email or document) by sensitivity level.

    >**Note:** If you haven't created or published any sensitivity labels or no content has had a sensitivity label applied, this card will display the message **"No sensitivity labels detected"**.

1. The **Top retention labels applied to content** card shows you how many items have a given retention label. Retention labels are used to manage the retention and disposition of content in your organization. When applied, they can be used to control how long an item will be kept before deletion, whether it should be reviewed prior to deletion, when its retention period expires, and whether it should be marked as a record.

    >**Note:** If this card displays the message,**"No retention labels detected"**, it means you haven't created or published any retention labels or no content has had a retention label applied.

1. The **Top activities detected** card provides a quick summary of the most common actions that users are taking on the sensitivity labeled items.

    >**Note:** If this card displays the message, **"No activity detected"** it means that there's been no activity on the files or that user and admin auditing isn't turned on.

1. The **Sensitivity and retention labeled data by location** cards provide visibility into the number of items that have which label as well as their location.

    >**Note:** If this card displays the message, **"No locations detected"**, it means you haven't created or published any sensitivity labels or no content has had a retention label applied.

### Task 2: Using Content Explorer for Data Classification

**Content explorer** allows you to natively view the items that were summarized on the **Overview** page. It shows a current snapshot of the items that have a sensitivity label, a retention label or have been classified as a sensitive information type in your organization.

Follow the given steps to use the content explorer for data classification:

1. Navigate to `https://compliance.microsoft.com/` and sign in using the **CloudLabs provided credentials**.

1. In the left navigation pane of the compliance portal, select **Data classification** and then, select **Content explorer**.

1. If you know the name of the label, or the sensitive information type, you can type that into the filter box.

1. Alternately, you can browse for the item by expanding the label type and selecting the label from the list.

1. Select a location under **All locations** and drill down the folder structure to the item and double-click to open the item natively in content explorer.

1. To create a .csv file that contains a listing of whatever the focus of the pane is, select **export**.

>**Note:** It can take up to **seven days** for counts to be updated in content explorer.

### Task 3: Using Activity Explorer

**Activity explorer** allows you to monitor what's being done with your labeled content. It provides a historical view of activities on your labeled content. The activity information is collected from the Microsoft 365 unified audit logs, transformed, and then made available in the Activity explorer UI. Activity explorer reports on up to 30 days worth of data. There are more than 30 different filters available for use, like Data range, Activity type, Location, User, Sensitivity label, Retention label etc.

>**Note:** Make sure **Audit** is turned on before using this in your account. If it's not, select **Turn Audit ON** from the activity explorer page.

To go to the **Activity Explorer**, follow the given steps:

1. Navigate to `https://compliance.microsoft.com/` and sign in using the **CloudLabs provided credentials**.

1. In the left navigation pane of the compliance portal, select **Data classification** and then, select **Activity explorer**.

Activity explorer gathers information from the audit logs of multiple sources of activities. Some examples of the **Sensitivity label activities** and **Retention labeling activities** from applications native to Microsoft Office, the Azure Information Protection (AIP) unified labeling client and scanner, SharePoint, Exchange (sensitivity labels only), and OneDrive include:

- Labels applied
- Labels changed (upgraded, downgraded, or removed)
- Autolabeling simulation
- File read

In addition, using Endpoint data loss prevention (DLP), Activity explorer gathers DLP policy matches events from Exchange, SharePoint, OneDrive, Teams Chat and Channel, on-premises SharePoint folders and libraries and more.

## Conclusion

In conclusion, understanding and leveraging the capabilities of **Microsoft Copilot** within the Microsoft 365 ecosystem are crucial steps towards enhancing data security and compliance for organizations. The emphasis on **data classification** forms a cornerstone for efficient functioning of Copilot, enabling it to provide accurate recommendations and automate the categorization process.

By embracing the security and compliance features of **Microsoft Copilot**, organizations can not only streamline data management processes but also adhere to industry regulations and legal requirements. This, in turn, fosters a secure digital environment, safeguarding sensitive information and reinforcing trust in the organization's commitment to privacy and data protection.
