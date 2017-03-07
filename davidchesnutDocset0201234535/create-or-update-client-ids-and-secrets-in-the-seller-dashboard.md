---
title: Create or update client IDs and secrets in the Seller Dashboard
ms.prod: MULTIPLEPRODUCTS
ms.assetid: f7852781-922f-4499-9dd4-c266907a8c14
---


# Create or update client IDs and secrets in the Seller Dashboard
Create or delete client IDs and secrets, update or replace expiring client secrets, and associate them with your add-ins in the Seller Dashboard to enable OAuth in your SharePoint Add-ins.
To update expiring client secrets in SharePoint Add-ins: 
  
    
    


1. Generate and add a new client secret in the Seller Dashboard to associate with that particular add-in client ID. For specific steps, see  **To generate additional client secrets** in [Update the client secret associated with your client ID](#bk_update) later in this article.
    
  
2. Update your remote web application to use the new client secret. For information about how to do this using Microsoft Office Developer Tools for Visual Studio, see  **Update the remote web application in Visual Studio to use the new secret** in [Replace an expiring client secret in a SharePoint Add-in](http://msdn.microsoft.com/library/369d14f0-75c1-4383-8a2d-05b4030c44ea%28Office.15%29.aspx). 
    
  
3. Republish your remote web application.
    
  

> [!Important]  
> Microsoft Office Developer Tools for Visual Studio supports setting a secondary client secret that you can use to update your expiring client secret.
  
    
    


## Using OAuth to authenticate and authorize add-ins
<a name="bk_usingoauth"> </a>

Open Authorization (OAuth) is an open protocol for authorization. OAuth enables secure authorization from desktop and web applications in a simple and standard way. It lets users approve an application to act on their behalf without sharing their user name and password. For example, users can share their private resources or data (contact list, documents, photos, videos, and so on) that are stored on one site with another site, without having to provide their credentials (typically user name and password). 
  
    
    
With OAuth, users can authorize a service provider (for example, SharePoint 2013) to provide tokens instead of credentials (for example, user name and password) to their data that is hosted by a given service provider (for example, SharePoint 2013). Each token grants access to a specific site (for example, a SharePoint document repository), for specific resources (for example, documents from a folder), and for a defined duration. Users can then grant a third-party site access to information that is stored with another service provider (for example, SharePoint), without sharing their user name and password and without sharing all the data that they have on SharePoint.
  
    
    
If your add-in requires this type of authorization, you have to associate OAuth client ID and client secrets with your add-in. You can generate OAuth client ID and client secrets in the Microsoft Seller Dashboard, and then add them to the code of your add-in.
  
    
    
When a user installs an add-in that has an associated client ID and client secret, a consent dialog box appears. If the user gives consent, the add-in can act on behalf of the user to access the data that the add-in requires. Users can only grant the permissions that they have. Grants represent the permissions that a user has delegated to an add-in. 
  
    
    
For example, your add-in could be a trip calendar add-in that opens as an  **IFRAME** on an Office 365 SharePoint site. OAuth would allow the add-in to identify the user to whom the trip calendar belongs, or if the trip calendar add-in needed to access other aspects of Office 365, such as resources or calendar information, it could access those on behalf of the signed-in user.
  
    
    

> [!Note]  
> For more information about OAuth, client ID and client secrets, see  [Authorization and authentication of SharePoint Add-ins](http://msdn.microsoft.com/library/bde5647a-fff1-4b51-b67b-2139de79ce4a%28Office.15%29.aspx),  [Context Token OAuth flow for SharePoint Add-ins](http://msdn.microsoft.com/library/526c8c4a-5cbb-4efc-87d9-23ac73655cf4%28Office.15%29.aspx), and  [Register SharePoint Add-ins 2013](http://msdn.microsoft.com/library/be41a5dc-2af9-4fd9-bf4e-ad6dfa849524%28Office.15%29.aspx).
  
    
    


## Add a client ID and client secret
<a name="bk_addclientid"> </a>

You can associate only one client ID with your add-in, but you can associate multiple client secrets with a client ID. For security and administrative purposes, we recommend limiting the number of client secrets associated with a client ID.
  
    
    

> [!Important]  
>  To submit a SharePoint Add-in that uses OAuth, and distribute it to China, you must use a separate client ID and client secret for China. You also must:
>  Add a separate add-in package specifically for China.
>  Block access for all countries except China.
>  Create a separate add-in listing for China.
>  For more information about submitting apps or add-ins and blocking access, see [Use the Seller Dashboard to submit Office and SharePoint Add-ins and Office 365 apps to the Office Store](use-the-seller-dashboard-to-submit-office-and-sharepoint-add-ins-and-office-365.md). For more information about distributing add-ins for China, see  [Submit SharePoint Add-ins for Office 365 operated by 21Vianet in China](submit-sharepoint-add-ins-for-office-365-operated-by-21vianet-in-china.md). 
  
    
    

Inbound data to your add-in will be signed using only one signing client secret. In the Seller Dashboard, this is the client secret with a green check mark next to it. If you delete the signing client secret that your add-in uses, the next valid client secret will be used instead.
  
    
    
Your add-in can use any valid client secrets as passwords to communicate with Microsoft. When a client secret expires, it can no longer be used as a password. If there is only one client secret associated with your client ID, deleting that secret can prevent your add-in from accessing the data it needs.
  
    
    
If your add-in is a service and it will need OAuth client IDs and client secrets, follow these steps.
  
    
    

### To add a client ID


1. Sign in to the  [Seller Dashboard](http://go.microsoft.com/fwlink/?LinkId=248605) with your Microsoft account.
    
  
2. On the  **Client ids** tab, choose **Add a new oauth client id**.
    
  
3. On the  **Provide details** page, provide the following information.
    

|**Item**|**Information to provide**|
|:-----|:-----|
|Friendly client ID Name|Choose a name to help you recognize which add-in will use this client ID; for example, "calendar app".|
|App domain|Provide the domain on which your add-in will run. For example:  `app.contoso.com`This must be a valid domain name that you own; it must not include  `http://` or `https://`; and it must not be an international domain name (IDN).|
|App redirect URL|Provide the redirect URL to send users to after they agree to your add-in's access requirements in the consent dialog box. This URL must start with  `https://`.|
|Client secret valid for|Choose how long your client secret will be valid. The recommended time period is one year, because this might be easier to track within your business processes than longer periods. However, there is no security impact to choosing a longer period of time. When the client secret is expiring, you will need to update your add-in.|
|Client ID and secret availability|Choose  **This Client ID will be used for an add-in that is available worldwide**, or  **This Client ID will be used for an add-in that is available in China only**.|
4. Choose  **Generate client ID**.
    
  
5. On the  **obtain client secret** page, copy your client ID and client secret to a secure location so that you can refer to it later.
    
    > [!Important]  
>  The client secret is associated with your client ID, but it will not be shown in the Seller Dashboard again.
>  You should also record the start and end dates, so that you will be aware of the client secret period of validity and its expiration date.
>  If your client secret is close to expiring, you will need to generate a new client secret and update your add-in. For more information, see [Update the client secret associated with your client ID](#bk_update) in this topic.
6. Choose  **DONE**.
    
  
7. If you didn't copy your client secret to a secure location, choose  **Cancel** in the **Have you copied your client secret?** dialog box. Otherwise, choose **YES**.
    
  

### To associate your client ID and secret with your add-in
<a name="bk_associate"> </a>

After you create your client ID and client secret, you can add them to the code of your add-in and then associate your client ID with your add-in to the Seller Dashboard.
  
    
    

> [!Note]  
> You can add the client ID and client secret to your code at any point in your add-in development process: during development, before testing, or before adding your add-in to the Seller Dashboard. However, to fully test your add-in, we recommend that you add them before you test. You can use the same client ID and secret throughout your add-in development process.
> If you are unsure where to place the client ID and client secret in your code, refer to the documentation provided for the add-in type you are developing.
  
    
    


### To associate the client ID and client secret with your add-in in the Seller Dashboard


1. When you're adding or editing your add-in, on the  **Overview** page, select the **My add-in is a service and requires server to server authorization** check box.
    
    > [!Important]  
>  If you are submitting a SharePoint Add-in that uses OAuth, and you want to distribute it to China, you must use a separate client ID and client secret for China:
2. Select the friendly name of the OAuth client ID that you want your add-in to use. 
    
    For more information, see  [Use the Seller Dashboard to submit Office and SharePoint Add-ins and Office 365 apps to the Office Store](use-the-seller-dashboard-to-submit-office-and-sharepoint-add-ins-and-office-365.md).
    
  

## Update the client secret associated with your client ID
<a name="bk_update"> </a>

Update your client secret in the following situations:
  
    
    

-  **Your client secret is expiring**
    
    We recommend that you add a new client secret in the Seller Dashboard while your current client secret is still valid. Update your add-in with the new client secret, and then delete the client secret that is close to expiring from the Seller Dashboard.
    
    > [!Note]  
> To update expiring client secrets in SharePoint Add-ins, follow these steps. Note that Microsoft Office Developer Tools for Visual Studio supports setting a secondary client secret that you can use to update your expiring client secret.
-  **The security of your client secret is compromised**
    
    To respond to a security compromise quickly, you can delete the compromised client secret from the Seller Dashboard first, add a new client secret, and then update your add-in with the new client secret.
    
  

> [!Important]  
> After the compromised client secret is deleted and before the new client secret is added, your add-in might temporarily be unavailable. This might be acceptable depending on the severity of the business impact of a lost or stolen client secret.
  
    
    


### To generate additional client secrets


1. Sign in to the  [Seller Dashboard](http://go.microsoft.com/fwlink/?LinkId=248605) with your Microsoft account.
    
  
2. On the  **Client ids** tab, choose the client ID with which you want to associate additional client secrets.
    
  
3. On your client ID summary page, choose  **ADD NEW CLIENT SECRET**.
    
  
4. Choose  **GENERATE CLIENT SECRET**.
    
  
5. Copy your client secret to a secure location so that you can refer to it later.
    
    > [!Important]  
>  The client secret is associated with your client ID, but it will not be shown in the Seller Dashboard again.
>  Record the start and end dates so that you will be aware of the client secret period of validity and its expiration date.
6. Choose  **DONE**.
    
  
7. If you didn't copy your client secret to a secure location, choose  **Cancel** in the **Have you copied your client secret?** dialog box. Otherwise, choose **YES**.
    
    > [!Note]  
> The new client secret will be active within 15 minutes.

### To delete a client secret


1. Sign in to the  [Seller Dashboard](http://go.microsoft.com/fwlink/?LinkId=248605) with your Microsoft account.
    
  
2. On the  **Client ids** tab, choose the client ID that has the client secret you want to delete.
    
  
3. On your client ID summary page, under  **Client secrets**, choose the  **X** next to the client secret you want to delete.
    
    > [!Important]  
>  Deleting a client secret can prevent your add-in from accessing the data it needs, unless you created additional secrets that are valid and that are associated with your add-in, and you configured it to use these additional client secrets.
>  If you have only one client secret associated with the client ID, you might want to generate an additional client secret before you delete it.
4. In the  **Are you sure you want to delete this client secret?** dialog box, choose **NO**, if you are not ready to delete this client secret. If you are ready to delete the client secret, choose  **YES**.
    
  

## Delete a client ID
<a name="bk_deleteclientid"> </a>

You might want to delete a client ID in certain situations, for example:
  
    
    

- You no longer want to offer your add-in.
    
  
- You want to offer a new version of your add-in and no longer want to offer the previous version. In this situation, you might want to delete the client ID you associated with the previous version of your add-in.
    
  

> [!Caution]  
> Deleting a client ID that is associated with your add-in deletes all associated client secrets and prevents it from accessing the data it needs. Any customer using your add-in will experience downtime after you delete a client ID that is associated with it.
  
    
    


### To delete a client ID


1. Sign in to the  [Seller Dashboard](http://go.microsoft.com/fwlink/?LinkId=248605) with your Microsoft account.
    
  
2. On  **Client ids** tab, choose the client ID that you want to delete.
    
  
3. On your client ID summary page, under  **OAUTH CLIENT ID**, choose  **DELETE**.
    
    > [!Caution]  
> Deleting a client ID that is associated with your add-in deletes all associated client secrets and prevents it from accessing the data it needs. Any customer using your add-in will experience downtime after you delete a client ID that is associated with it.
4. If you are not ready to delete this client ID, in the  **Are you sure you want to delete <your client ID's name>?** dialog box, choose **NO**. If you are ready to delete this client ID, choose  **YES**.
    
  

### To delete a client ID, but continue offering your add-in


1. Add another client ID and at least one valid client secret. 
    
    For more information, see  [Add a client ID and client secret](#bk_addclientid).
    
  
2. Delete the client ID from your code.
    
    > [!Note]  
> Customers using your add-in will experience downtime after you delete a client ID that is associated with your add-in.
3. Delete the client ID from the Seller Dashboard, as described in the previous procedure.
    
  
4. Add the new client ID and client secret to your code.
    
  
5.  [Submit your updated add-in for approval](use-the-seller-dashboard-to-submit-office-and-sharepoint-add-ins-and-office-365.md) in the Seller Dashboard.
    
    > [!Caution]  
> Customers using your add-in will experience downtime during the update to your code and the Seller Dashboard approval process.

## Additional resources
<a name="bk_addresources"> </a>


-  [Submit Office and SharePoint Add-ins and Office 365 web apps to the Office Store](submit-office-and-sharepoint-add-ins-and-office-365-web-apps-to-the-office-store.md)
    
  
-  [Authorization and authentication of SharePoint Add-ins](http://msdn.microsoft.com/library/bde5647a-fff1-4b51-b67b-2139de79ce4a%28Office.15%29.aspx)
    
  
-  [Context Token OAuth flow for SharePoint Add-ins](http://msdn.microsoft.com/library/526c8c4a-5cbb-4efc-87d9-23ac73655cf4%28Office.15%29.aspx)
    
  
-  [Validation policies for apps and add-ins submitted to the Office Store (version 2.1)](validation-policies-for-apps-and-add-ins-submitted-to-the-office-store-version-2.md)
    
  
-  [Checklist for submitting Office and SharePoint Add-ins and Office 365 web apps to the Seller Dashboard](checklist-for-submitting-office-and-sharepoint-add-ins-and-office-365-web-apps-t.md)
    
  

