# Microsoft Copilot for 365

### Expected Duration : 8 hours

## Overview

**Contoso Ltd.**, a leading IT Consultancy firm, is always in search of ways to improve its efficiency and productivity. To achieve this, they've decided to incorporate **Microsoft Copilot for Microsoft 365** into their operations. With its extensive range of features and the ability to streamline tasks, automate workflows, and enhance collaboration, Contoso is confident that Copilot will be a game-changer.

As part of the lab, you've been given access to Contoso's Microsoft 365 environment to test and demonstrate the capabilities of **Microsoft 365 Copilot**. You have the access to Contoso's data present in various SharePoint sites, namely Human Resource, Marketing and Finance, which you will utilize in future in the lab. You also have been provided the access to Teams environment as an employee of the **Contoso Ltd.** By the end of this lab, you'll have a thorough understanding of how **Microsoft 365 Copilot** can transform an organization's productivity and efficiency, just as it's doing for **Contoso Ltd**.

## Objective

Learn to leverage an OpenAI model to extract data and create embeddings, by end of this lab you will be able to:

- **Introduction to M365 Copilot** : Learn about the capabilities of Microsoft 365 Copilot.
- **Understanding M365 Copilot Architecture** : Explore how M365 Copilot is designed and integrated.
- **Preparing for M365 Copilot Deployment** : 
   - **Organizing Sharepoint teams and files** : Structure SharePoint for efficient collaboration.
   - **Understand Semantic Index** : Learn how Semantic Index improves search and context in M365.
- **Using Copilot in M365 Applications** :
   - **Using Microsoft 365 Copilot in Word** : Automate content creation and editing.
   - **Using Microsoft 365 Copilot in Outlook** : Draft and manage emails efficiently.
   - **Using Microsoft 365 Copilot in Powerpoint** : Create impactful presentations with AI.
   - **Using Microsoft 365 Copilot in Excel** : Analyze data and generate insights quickly.
   - **Using Microsoft 365 Copilot in Teams** : Enhance collaboration and manage tasks with AI.
   - **Using Microsoft 365 Copilot in Loop** : Collaborate seamlessly with real-time updates.
   - **Using Microsoft 365 chat** : Centralize conversations and integrate insights.
- **Administer M365 Copilot** :
   - **Managing Microsoft 365 Copilot Licenses in Admin Center** : Allocate and monitor licenses effectively.
   - **Managing Microsoft 365 Copilot Services** : Configure and manage Copilot services for optimal performance.
   - **Managing Public web content access** : Control Copilot's access to web content for compliance.
   - **Change update channel of Microsoft 365 Apps to enable Copilot** : Adjust update settings for Copilot functionality.
- **Reviewing Security and Compliance in Copilot** : 
   - **Reviewing Security and Compliance in Copilot using Sensitivity Labels** : Protect content with appropriate labels.
   - **Implementing sensitivity label** : Apply labels to classify and secure data.
   - **Reviewing Security and Compliance in Copilot Using Data Classification** : Organize data based on sensitivity and usage.
   - **Reviewing Security and Compliance in Copilot Using Customer Keys** : Use customer keys for data encryption.
   - **Reviewing Security and Compliance in Copilot Using Communication Compliance** : Monitor and manage communication policies.
   - **Reviewing Security and Compliance in Copilot Using Audit** : Track user activities and system changes.
   - **Reviewing Security and Compliance in Copilot Using Content Search** : Perform advanced searches for compliance and security.
   - **Reviewing Security and Compliance in Copilot Using eDiscovery** : Manage legal and investigative workflows.
   - **Reviewing Security and Compliance in Copilot using Retention Policies** : Retain and manage important data efficiently.
- **Exploring Microsoft Copilot Lab** : Gain deeper insights through practical labs.
- **Try Out Your Organizational Use Cases with M365 Copilot Capabilities** : Experiment with Copilot to address specific business needs.

## Prerequisites

Participants should have:

- **Basic Knowledge of Microsoft 365 Services**: Familiarity with core M365 applications such as Word, Excel, PowerPoint, Teams, and SharePoint.
- **Azure Active Directory (Azure AD) Basics**: Understanding of user management, groups, and access permissions in Azure AD.
- **Administrative Access to Microsoft 365 Tenant**: Ensure you have admin privileges to configure Copilot services, licenses, and compliance settings.
- **Access to Microsoft 365 E5 License**: A Microsoft 365 E5 license or equivalent is required for accessing advanced Copilot features.
- **Set Up of Microsoft 365 Environment**: A fully configured M365 environment with necessary applications installed, including SharePoint, Teams, and Outlook.
- **Knowledge of Security and Compliance in Microsoft 365**: Familiarity with sensitivity labels, retention policies, and compliance tools like eDiscovery and audit logs.

## Architecture

Microsoft 365 Copilot's architecture seamlessly integrates advanced AI capabilities with Microsoft 365 applications to enhance productivity and user experience. It uses Microsoft Graph to provide real-time insights and contextual understanding across apps like Word, Excel, PowerPoint, Teams, Outlook, Loop, and SharePoint. The Semantic Index is a key component, optimizing data retrieval by structuring and indexing files and conversations for Copilot. Integration with Azure Cognitive Services enhances capabilities such as personalized recommendations and language understanding. The architecture also incorporates Microsoft Purview to ensure security and compliance, leveraging tools like sensitivity labels, data classification, retention policies, and eDiscovery. This architecture supports robust management features, including licensing and service configurations, while maintaining adherence to organizational policies, creating a unified framework for deploying, managing, and exploring M365 Copilot capabilities effectively.

## Architecture Diagram

![](./media/copilot-for-microsoft-365-architecture.png)

## Explanation of Components

- Word: Automate document creation, editing, and summarization.
- Outlook: Streamline email drafting, responses, and scheduling.
- PowerPoint: Generate professional presentations with AI-powered design and content suggestions.
- Excel: Analyze data, build charts, and gain insights with AI.
- Teams: Enhance collaboration, summarize chats, and manage tasks efficiently.
- Loop: Enable real-time collaboration with dynamic and adaptive content blocks.
- M365 Chat: Consolidate insights and facilitate conversations using data from Microsoft 365.
- Managing Microsoft 365 Copilot Licenses in Admin Center: Allocate, monitor, and manage user licenses efficiently.
- Managing Microsoft 365 Copilot Services: Configure Copilot services for optimal use across the organization.
- Managing Public Web Content Access: Ensure compliance by controlling access to public content sources.
- Sensitivity Labels: Apply labels to classify and protect sensitive data.
- Data Classification: Organize and manage data based on its sensitivity and use cases.
- Customer Keys: Enhance encryption with customer-managed encryption keys.
- Communication Compliance: Monitor and enforce organizational communication policies.

## Getting Started with Microsoft Copilot for Microsoft 365

Welcome to your **Microsoft Copilot for Microsoft 365** lab! We've prepared a seamless environment for you to explore and learn about **Microsoft Copilot for Microsoft 365**. Let's begin by making the most of this experience:

## Accessing Your Lab Environment

Once you're ready to dive in, your virtual machine and lab guide will be right at your fingertips within your web browser.

## Virtual Machine & Lab Guide

In the integrated environment, the lab VM serves as the designated workspace, while the lab guide is accessible on the right side of the screen.

**Note**: Kindly ensure that you are following the instructions carefully to ensure the lab runs smoothly and provides an optimal user experience.

  ![](./media/main.png)

## Exploring Your Lab Resources

To get a better understanding of your lab resources and credentials, navigate to the **Environment** tab. You will find your credentials under **M365 Copilot User Details**. The value before the **|** will be your User ID and the value after **|** will be your User password to log into Microsoft 365 applications and utilize the lab environment.

  ![](./media/labguideupdategettingstarted.png)

Copy and paste the credentials in the notepad **Username (1)** & **Password (2)**

  ![](./media/copy.png)

## Utilizing the Split Window Feature

For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the Upper right corner.

  ![](./media/main-1.png)

## Lab Guide Zoom In/Zoom Out
 
To adjust the zoom level for the environment page, click the **A↕ : 100%** icon located next to the timer in the lab environment.

![](./media/n21.png) 

## Managing Your Virtual Machine

Feel free to start, stop, or restart your virtual machine as needed from the **Resources** tab. Your experience is in your hands!

  ![](./media/vm-run.png)

Now, click on Next from the lower right corner to move on to the next page.

  ![](./media/nxt.png)

## Support Contact
The CloudLabs support team is available 24/7, 365 days a year, via email and live chat to ensure seamless assistance at any time. We offer dedicated support channels tailored specifically for both learners and instructors, ensuring that all your needs are promptly and efficiently addressed.

Learner Support Contacts:

* Email Support: cloudlabs-support@spektrasystems.com
* Live Chat Support: https://cloudlabs.ai/labs-support

## Happy Learning!!
