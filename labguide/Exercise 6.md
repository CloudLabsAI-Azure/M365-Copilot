# Exercise 6: Manage Copilot

You can assign or remove Microsoft 365 Copilot licenses for users in your tenant through the Microsoft 365 Admin Center.

## Task 1: Managing Microsoft 365 Copilot Licenses in Admin Center

### Task 1.1: Assign a Copilot licenses to user

Follow these steps to assign a Copilot license for an existing user from the admin center:

1. Go to [Microsoft 365 Admin Center](admin.microsoft.com) and sign in with your admin credentials.


1. From the left side navigation pane, click on **Users (1)** and then choose **Active users (2)**.

    ![](../labguide/media/M8.png)

1.  In the Active users page, search or find the user you want to manage Copilot license. Click on **<inject key="AzureAdUserEmail"></inject>**.

    ![](../labguide/media/M9.png)

1. In the user's profile page, on the right side click on **Licenses and apps** to go to their licenses details.

    ![](../labguide/media/M10.png)

1. To assign, expand the **Licenses (1)** section, select the boxes for the licenses that you want to assign, then select **Save changes (3)**.

   >**Note:** In this case, we have already assigned the licences to the account.

    ![](../labguide/media/M11.png)

 All license changes are saved automatically after you make an assignment change.

### Task 1.2: Remove a Copilot licenses

To remove an already assigned Copilot license:

1. Follow steps above to open the user's **Licenses and apps**.

    ![](../labguide/media/M10.png)

1. Uncheck the **Microsoft Copilot for Microsoft 365** under the licenses section.

    ![](../labguide/media/M18.png)

    >**Note:** In this case, you don't need to remove the licenses.

1. Changes apply automatically after saving.

Now the user's Copilot license assignment status will be updated.

### Task 1.3: Manage Microsoft 365 Copilot Services

Microsoft 365 Copilot comes with different services that can be enabled or disabled as per your preferences. This can be configured from the Microsoft 365 Admin Center.

1. Login to [Microsoft 365 Admin Center](admin.microsoft.com).


1. Go to **Billing (1)** > **Licences (2)**.

    ![](../labguide/media/M14.png)

1. Scroll down and click **Microsoft Copilot for Microsoft 365**.

    ![](../labguide/media/M15.png)

1. Select the **<inject key="AzureAdUserEmail"></inject> (1)** and select **Manage apps & services (2)**. 

   ![](../labguide/media/M16.png)

1. If you want to **Turn apps and services on or off**, uncheck any of the apps and services and click **Save**.
 
   ![](../labguide/media/M17.png)


### Task 2: Public web content access

Microsoft Copilot for Microsoft 365 chat experiences in Bing, Microsoft Edge, and the Microsoft Teams app has a feature that allows Copilot to reference web content when responding to user prompts. Allowing Copilot for Microsoft 365 to reference web content enhances the end user experience and productivity with Copilot. The feature is automatically turned on when you first start using Copilot. You can turn off this feature by following these steps:

1. In the Microsoft 365 admin center, go to **Settings (1)** > **Search & intelligence (2)**.

    ![](../labguide/media/M19.png)

1. On the **Configurations** page, select **Improved responses with web content in Copilot for Microsoft 365**.

    ![](../labguide/media/M20.png)

1. Select **Change**.

1. Uncheck the checkbox for **Allow Copilot to reference web content**.

    ![](../labguide/media/m21.png)

    >**Note:** In this case, you don't need to uncheck this option.

1. Select **Save**.

All admin setting updates may take up to 24 hours to reflect any changes.


### Task 3: Enable Plugins

