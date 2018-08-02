---
title: "Communicate with Teams users in another organization"
ms.author: tonysmit
author: tonysmit
manager: serdars
ms.topic: article
ms.tgt.pltfrm: cloud
ms.service: msteams
ms.collection: Strat_MT_TeamsAdmin
ms.audience: Admin
appliesto:
- Microsoft Teams
localization_priority: Normal
description: "See how to configure Teams to let users communicate with users in another organization."
---

# Let your Teams users chat and communicate with users in another Teams organization

Use the steps in this article when:
  
- You have users in different domains in your business. For example, Rob@ContosoEast.com and Ann@ContosoWest.com.
    
- You want the people in your organization to use Teams to contact people in specific businesses outside of your organization.
    
-You want anyone else in the world who uses Teams to be able to find and contact you, using your email address. If the both of you enable External Access and allow each others domains, this will work. If they don't, then they need to make sure their configuration isn't blocking your domain.

Follow these steps:

## Let your Teams users chat and communicate with users in another Teams organization

### Step 1 - Make sure to set up the ports and URLs that are needed.

**The most common issue people encounter when setting up business-to-business communication is getting their [Office 365 URLs and IP address ranges](https://docs.microsoft.com/en-us/microsoftteams/office-365-urls-ip-address-ranges) right.**

### Step 2 - Enable your organization to communicate with another Teams organization

Note: External access hasn't been fully rolled out, and so you may not see all of the below options within your tenant.

![teams-logo-30x30.png](media/teams-logo-30x30.png) **Using the Microsoft Teams and Skype for Business Admin Center**

   1. In the left navigation, go to **Org-wide settings** > **External access**. 

   2. At the top of the **External access** page, click **External access** to **On**. 

   3. Add the other organization's domain to the allowed list by clicking **Add domain**. In the **Add a domain** pane, put in the domain name click **Allowed** and then **Done**.

   4. Click **Save**. 

   5. Then make sure the admin in the other Teams  organization does these same steps. For example, in their **allowed domains** list, their admin needs to enter the domain for your business.

### Step 3 - Test it
To test your setup, you need a Teams user who's not behind your firewall.
  
   1. After you and the admin from the organization have changed the **External access** settings, you should be good to go.
    
   2. In the Teams app, search for the person by email address, and send a request to chat.
    
   3. Ask your Teams contact to send you a request to chat. If you don't receive their request, the problem is your firewall settings (assuming they've already confirmed their firewall settings are correct).
    
   4. Another way to test whether the problem is your firewall is to go to a wifi location not behind your firewall such as a coffee shop, and use Teams to send a request to your contact to chat. If the message goes through there, but not when you're at work, then you know the problem is your firewall.

## Communicate with users in a Skype for Business Online organization

If you are setting it up to let your Teams users find and contact users that are in a Skype for Business organization, you will the admin in that organization to follow these steps.

![sfb-logo-30x30.png](media/sfb-logo-30x30.png) **Using Skype for Business admin center** 

Have the admin in that organization do these steps:
    
1. In the Office 365 admin center, go to **Admin Centers** > **Skype for Business**.
  
2. In the **Skype for Business admin center**, choose **Organization** > **External communications**.
    
3. To set up communication with a specific business or with users in another domain, in the drop-down box, choose **On only for allowed domains**.
    
    OR, if you want to enable communication with everyone else in the world who has open Skype for Business policies, choose **On except for blocked domains**. This is the default setting.
    
4. Under **Blocked or allowed domains**, choose **+** and add the name of the domain you want to allow. Make sure the admin in the other organization does these same steps. For example, in their **allowed domains** list, their admin needs to enter the domain for your business.
    
### Related topics

[Sign in teams](sign-in-teams.md)
[End user training for Teams](enduser-training.md)

