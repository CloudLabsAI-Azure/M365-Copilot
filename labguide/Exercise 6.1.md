# Exercise 4: Overview of M365 Copilot App

### Estimated time: 30 minutes

## Overview:

In this exercise, we will explore the Copilot interface, understand the concept of reusable no-code agents, and create two powerful agents – Researcher and Analyst – without writing any code. These agents are designed to assist with tasks such as content summarization, document synthesis, data analysis, and insight generation, using data already available in your Microsoft environment.

## Objective: 

In this exercise, we will complete the following tasks

- **Understand the M365 Copilot App interface and capabilities:** Get familiar with the layout, features, and functions of the Microsoft 365 Copilot App.

- **Learn about No-code agents and discuss use cases in M365 Copilot:** Explore how no-code agents work in Copilot and identify scenarios where they can be effectively applied. And execute sample actions with Researcher and Analyst agents to understand their practical business applications.

- **Create and experiment with **Researcher** No-code agent:** Build a Researcher agent to summarize documents and extract key insights without writing any code.




### Task 1: Introduction to M365 Copilot App

Walk through of M365 Copilot:

1. Open your browser and go to: https://www.office.com.

1. Sign in with your Microsoft 365 account with the credentials below if required.

    **Email/Username:** <inject key="AzureAdUserEmail"></inject>
 
    **Password:** <inject key="AzureAdUserPassword"></inject>

1. Locate the **Chat** in the app launcher (waffle menu) or search bar.

   ![](./media/Office2.png)

1. Other M365 functionalities

    - **Search:** You can search for documents, meetings, emails, notes, chats, or even tasks using AI-driven contextual results from Microsoft Graph.
        > **Example:** "Find the latest project update from XYZ” or “Show me Q2 financial reports".

    - **Chat:** Use this area to ask Copilot questions, summarize content, draft emails, or retrieve insights from your documents or organizational data.
        > **Example:** “Summarize the last meeting with the marketing team” or “Draft a follow-up email for the sales pitch.”

    - **Notebooks:** You can combine AI-generated content, summaries, and your own notes into organized sections — similar to a digital binder powered by Copilot.
        > **Example:** Ideal for organizing research findings, training materials, or long-term planning documents collaboratively.

### Task 2: Understanding No-Code Agents in Copilot

1. In the Copilot app, navigate to the **Agents** section.

1. There should be some agents already available.

    ![](./media/Office.png)

1. Discuss use cases.

    - **Researcher Agent:** Synthesizes large volumes of information.

        - Click on the **Researcher (1)** agent from the menu, then click on **+ (2)**, and then click on **Add Content (3)**
        
            ![](./media/Researcher1.png)

        - Select **Market_Trends_Report_Q2_2025.docx (1)** and then enter one of the prompts from below.
            
            - “Summarize these documents into key bullet points.”

            - “What are the key takeaways from this report?”

            - “Identify common themes across these files.”

                ![](./media/Researcher2.png)
        > **Note:** The responses from the agent may vary.

    - **Analyst Agent:** Performs calculations, summarizes data, and creates visual reports.

        - Click on the **Analyst (1)** agent from the menu, then click on **+ (2)**, and then click on **Add Content (3)**
        
            ![](./media/Analyst1.png)

        - Select **Sales_Data_Q1_2025 (1)** and then enter one of the prompts from below.
            
            - “Summarize the monthly revenue trends.”

            - “Which products performed best last quarter?”

            - “Create a pie chart of total sales by region.”

                ![](./media/Analyst2.png)
            > **Note:** Copilot should generate summary insights and create visualizations directly in Excel or as a report.


### Task 3: Creating a No-Code Agent

Build and test an agent that can summarize documents and compile findings.

1. Click **Create Agent**

    ![](./media/Agent1.png)

1. Click on **Configure**

    - Give your agent a name: **Market Trends Researcher**

    - **Description:** This intelligent agent is designed to help users analyze documents and extract key insights — such as summaries, common themes, and trends — without needing to write any code or use custom logic.

    - **Instructions:** 
        - Summarize all documents into concise bullet points

        - Identify trends and common themes across the uploaded content

    - **Knowledge:**

        - Click on **Attach cloud files** button.
        
            ![](./media/Agent2.png)
        
        - Click on **Finance** SharePoint site.

            ![](./media/Agent3.png)
        
        - Select **Market_Trends_Report_Q2_2025.docx (1)** file and click **Select (2)**.

            ![](./media/Agent4.png)


1. Leave all other settings as default and click on **Create**.

    ![](./media/Agent5.png)


> **Notes:** You don’t need to code or script. The configuration is based on task type and data input. Mention security and data compliance through Microsoft 365’s boundaries