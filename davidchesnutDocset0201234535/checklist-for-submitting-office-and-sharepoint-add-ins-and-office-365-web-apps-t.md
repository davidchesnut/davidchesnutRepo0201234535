---
title: Checklist for submitting Office and SharePoint Add-ins and Office 365 web apps to the Seller Dashboard
ms.prod: MULTIPLEPRODUCTS
ms.assetid: 6114a720-77c0-438f-9be9-4d9a3c970bd4
---



# Checklist for submitting Office and SharePoint Add-ins and Office 365 web apps to the Seller Dashboard
Prepare to add and submit Office and SharePoint Add-ins and Office 365 web apps using Azure AD to the Seller Dashboard for approval and inclusion in the Office Store. 
Before you submit Office and SharePoint Add-ins or Office 365 web apps in the Seller Dashboard: 
  
    
    


- Review the current  [Validation policies for apps and add-ins submitted to the Office Store (version 2.1)](validation-policies-for-apps-and-add-ins-submitted-to-the-office-store-version-2.md). This will help you avoid common mistakes and verify that you're fully compliant with the current validation requirements, and ensure that your app or add-in will pass validation when it is submitted to the Office Store for approval. 
    
  
- Check the  [Regional Information for the Microsoft Seller Dashboard](http://msdn.microsoft.com/library/7f8445c7-f4f6-4cd7-888f-b0936aa8785b.aspx) to verify that you reside in a country or region that the Seller Dashboard supports.
    
  
- For Office Add-ins, validate your add-in manifest. You can validate your add-in manifest in two ways: 
    
  - In Visual Studio, go to Build > Publish, and choose **Perform Validation check**. 
    
  
  - Download the  [Office App Compatibility Kit](https://www.microsoft.com/en-us/download/details.aspx?id=46831) and run it on your add-in.
    
  

## Checklist for submitting apps or add-ins
<a name="bk_add"> </a>


****


|**Ready**|**What you need**|**Notes**|
|:-----|:-----|:-----|
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|App type | The following Office Types are available: Office Add-in Outlook Add-in SharePoint Add-in Web app using Azure AD|
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|App title |Your **App Title**appears in the listing on the Office Store. For title guidelines, see [Create effective Office Store apps and add-ins](create-effective-office-store-apps-and-add-ins.md). Office Add-ins that are available on iOS cannot include "app" in the **App Title**. > [!TIP]  > The **App Title**appears on the**overview**page in the Seller Dashboard. The**App Name**appears on the**details**page.          |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|App name |To offer your apps or add-ins in multiple languages, you can provide an **App Name**in each language. For a list of the languages that the Seller Dashboard currently accepts, see Table 2 later in this article.> [!TIP]  > The **App Name**appears on the**details**page for each language in the Seller Dashboard.          |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Version |The version number you provide for the **Version**must exactly match the version number in the add-in manifest file of the add-in you submit. For more information, see [Validation policies for apps and add-ins submitted to the Office Store (version 2.1)](validation-policies-for-apps-and-add-ins-submitted-to-the-office-store-version-2.md). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Release date |The date your app or add-in is released and listed in the store. The release date does not determine the date on which the app or add-in is available in the Office Store. > [!IMPORTANT]  > If you are submitting an update and you select a release date that is in the future, your app or add-in will not be discoverable in the Office Store until the date you select. If your app or add-in was available in the Office Store, it will be hidden from users until the release date for the updated version.           |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Category |Choose at least one category to use as a filter in the Office Store to help customers find your app or add-in. You can choose up to three categories. If you choose the Education category for your app or add-in, you'll need to comply with policy 7.18 of the  [validation policies](validation-policies-for-apps-and-add-ins-submitted-to-the-office-store-version-2.md). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|App logo | Include a picture you want customers to associate with your app or add-in that will appear in the store listing. For Word, Excel, and Project add-ins, you are required to link to an image using the [IconUrl](http://msdn.microsoft.com/en-us/library/c7dac2d4-4fda-6fc7-3774-49f02b2d3e1e%28Office.15%29.aspx) element in the add-in manifest. The image specified must be 32 pixels by 32 pixels. For Outlook add-ins, you are required to link to an image using the [IconUrl](http://msdn.microsoft.com/en-us/library/c7dac2d4-4fda-6fc7-3774-49f02b2d3e1e%28Office.15%29.aspx) element in the add-in manifest. The image specified must be secured with HTTPS. This image is shown as the 64 pixels by 64 pixels image associated with your add-in in the**installed add-ins**dialogue. For best customer experience, specify a 64 pixel by 64 pixel image for the**IconUrl**element. For validation, this image must be between 64 pixels by 64 pixels and 128 pixels by 128 pixels. The image must be in one of the following file formats: .gif, .jpd, .png, .exif, .bmp, or .tiff. For SharePoint Add-ins, you are required to include an icon in the add-in's package. The image included must be 96 pixels by 96 pixels. The image that you include must match the image that you submit via the Seller Dashboard form. Scan your logo with a current version of virus detection software, and upload it to the Seller Dashboard only if it passes the virus scan. If you need virus detection software, visit the [Microsoft Safety &amp; Security Center](http://go.microsoft.com/fwlink/?LinkId=248711).  Only one logo is associated with your app or add-in. If your logo requires localization, create separate submissions for each language and use a different logo for each.|
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|App package |The binary file or manifest file that you upload to the Seller Dashboard. Your add-in manifest must conform to the add-in manifest schema. Make sure that you have not omitted elements or included incorrect elements, and that the order of the elements is correct. The ID in your add-in manifest must be unique. The title that you specify in the add-in manifest must be the same as the title you specify in the Seller Dashboard. For detailed manifest schema information, see  [Schema reference for Office Add-ins manifests (v1.1)](http://msdn.microsoft.com/library/7e0cadc3-f613-8eb9-57ef-9032cbb97f92%28Office.15%29.aspx). > [!TIP]  >  If you have a SharePoint Add-ins, the file name extension should be .app. If you have an Office Add-in, the extension should be .xml (add-in manifest file).>  Scan your app or add-in with a current version of virus detection software, and upload it to the Seller Dashboard only if it passes the virus scan. If you need virus detection software, visit the [Microsoft Safety &amp; Security Center](http://go.microsoft.com/fwlink/?LinkId=248711).           For more information about maintaining consistency between the logo image and the one you include in the app package, see  *Create a consistent visual identity for your add-in*  in [Create effective Office Store apps and add-ins](create-effective-office-store-apps-and-add-ins.md). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|OAuth Client ID (if required) |If your app or add-in is a service and requires server-to-server authorization, you will need a client ID and client secret. You create the client ID and secret in the Seller Dashboard. For more information, see  [Create or update client IDs and secrets in the Seller Dashboard](create-or-update-client-ids-and-secrets-in-the-seller-dashboard.md). > [!NOTE]  >  To submit a SharePoint Add-in that uses OAuth and that you want to distribute to China, you must:>  Use a separate client ID and client secret for China.>  Add a separate add-in package specifically for China.>  Block access for all countries except China.>  Create a separate add-in listing for China.>  For more information, see [Submit SharePoint Add-ins for Office 365 operated by 21Vianet in China](submit-sharepoint-add-ins-for-office-365-operated-by-21vianet-in-china.md).           |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Testing notes |Provide instructions, links to resources, or a video demonstrating the app or add-in that will help validation testers validate your submission as part of the approval process.. For example, provide valid credentials or a password if your add-in requires them. The credentials or password are not for public use and will only be used by Microsoft. For web apps, use the testing notes to supply the Single Sign-On URL to help the validator find the app. For apps or add-ins using the Education category, provide subject and age range details. For more information, see policy 7.18 of the  [validation policies](validation-policies-for-apps-and-add-ins-submitted-to-the-office-store-version-2.md). Your testing notes are for validation purposes only and will not be published in your store listing. If you provide complete testing notes, they can assist in the validation and approval of your add-in. |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Cryptography and encryption information |Specify whether your app or add-in calls, supports, contains, or uses cryptography or encryption. For more information about encryption, see  [EAR Controls For Items That Use Encryption](http://go.microsoft.com/fwlink/?LinkId=268130). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Apple developer ID |If your add-in is iOS-compatible and you want to make it available in the Office Add-in Catalog on iPad, you will need to provide your Apple developer ID. |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|App description |This includes a **Short Description**and a**Long Description**that will appear in the store listing for your app or add-in. For description guidelines, see [Create effective Office Store apps and add-ins](create-effective-office-store-apps-and-add-ins.md). Office Add-ins that are available on iOS cannot include "app" in the **Short Description**. If you want a tailored experience for users in a regional store, you can add other languages so that your app or add-in appears in other language stores with localized metadata. If you add a language, you must write a **Short Description**and a**Long Description**in that language.|
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Screenshots | Provide at least one screenshot of your app or add-in. You can provide up to five screenshots for customers who want to learn more. Customers will be able to see these images in the store listing, so do not include any private or personal information that you don't want customers to see. If you add other languages to your app or add-in submission, you can add language-specific screen shots. Screenshots that match each language provide the best customer experience. Your screenshots must be in one of the following file formats: .png, .jpg, .jpeg, or .gif. They must be 512 x 384 pixels, and can be no greater than 300 KB. Screenshots must be unmanipulated images of your app or add-in running in a licensed copy of Office. Scan your images with a current version of virus detection software, and upload them to the Seller Dashboard only if they pass the virus scan. If you need virus detection software, visit the [Microsoft Safety &amp; Security Center](http://go.microsoft.com/fwlink/?LinkId=248711). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Support document link |Provide a link to your support documentation, including  `http://` or `https://` in your URL. The support link should include contact details so that users can contact you or a support person about your add-in.For Office Add-ins, make sure that you include the  [SupportUrl](http://msdn.microsoft.com/library/61cff5aa-929f-7d6a-2ce9-0b92b2d6e0a7%28Office.15%29.aspx)****element in your manifest file. You might need to add this element to the manifest file, because it is not included by default.This entry should be of the form:  `<SupportUrl DefaultValue="http://www.<yoursupportURL>.com/" />`|
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Privacy policy notification link |Provide a link to a privacy policy. > [!NOTE]  > If your app or add-in enables access to and use of Internet-based or mobile services, or collects and/or transmits user information to you or a third party, you must provide a link to a privacy statement that contains privacy details that will be published with your app or add-in. > The Seller Dashboard now requires a link to your privacy document. If you submitted your app or add-in before a link to your privacy document was required in the Seller Dashboard, the link to privacy information on the listing page will call out that a privacy statement was not provided:  [Privacy Statement](http://office.microsoft.com/en-us/privacy-statement-HA103998772.aspx). > To add the link to a privacy policy to an approved app or add-in, you can edit your Seller Dashboard submission, add the link, and submit it for approval again. For more information, see  [Update, unpublish, and view app and add-in metrics in the Seller Dashboard](update-unpublish-and-view-app-and-add-in-metrics-in-the-seller-dashboard.md).           |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Video link (optional) |You can create and submit a link to a video that explains how to use and get the most out of your app or add-in. This video will appear in the listing page for the add-in. Make sure that your video walks the user through the most useful features of the app or add-in. We recommend that you keep your video under three minutes. |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Customized end-user license agreement (optional) |If you have a customized license agreement, you can upload it. If you do not, the store will provide a license agreement for your app or add-in. For more information, see  [Office Store Standard Application License Terms](http://office.microsoft.com/en-us/store/office-store-standard-application-license-terms-HA102821243.aspx). For more information about licensing, see  [License your Office and SharePoint Add-ins](license-your-office-and-sharepoint-add-ins.md),  [Licensing your SharePoint Add-ins](http://blogs.msdn.com/b/officeapps/archive/2012/11/09/licensing-your-apps-for-sharepoint.aspx), and  [Creating and verifying licensing in a paid Office Add-in](http://blogs.msdn.com/b/officeapps/archive/2012/11/01/creating-and-verifying-licensing-in-a-paid-app-for-office.aspx). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Pricing information | The price is set at the app or add-in level. You don't set a price for each language. You set a price tier. The price shown to customers is in the currency associated with the store the app or add-in is being sold in. You can list your app or add-in for free, for a one-time purchase, or as a perpetual monthly subscription. For a paid or subscription app or add-in, you can also choose whether you want to offer it as a trial, and if so, the duration of that trial. For SharePoint Add-ins, you can also set two additional pricing options:**Number of trial users**- This limits the total number of users on a given site who can use the add-in as a trial.**Price threshold**- This sets a limit on the amount a single buyer pays for purchasing multiple add-in licenses. For example, if you set the price threshold at ten users, the user is only charged for the first ten licenses they purchase. You can add this information at any time, so if you decide to list your add-in for purchase at a later date, you can add pricing information at that time. You can't change the pricing from subscription to one-time charge, or vice versa, after you have submitted the add-in listing. This includes add-ins you submitted before the subscription pricing option was available. For more information, see [Decide on a pricing model for your Office or SharePoint Add-in or Office 365 web app](decide-on-a-pricing-model-for-your-office-or-sharepoint-add-in-or-office-365-web.md). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Trial information |If your app or add-in supports a trial, you will need to specify the duration of the trial, and the number of users. You also need to consider licensing. For more information, see  [License your Office and SharePoint Add-ins](license-your-office-and-sharepoint-add-ins.md),  [Licensing your SharePoint Add-ins](http://blogs.msdn.com/b/officeapps/archive/2012/11/09/licensing-your-apps-for-sharepoint.aspx), and  [Creating and verifying licensing in a paid Office Add-in](http://blogs.msdn.com/b/officeapps/archive/2012/11/01/creating-and-verifying-licensing-in-a-paid-app-for-office.aspx). |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|Payout and tax information |To list your app or add-in for purchase, either for one-time purchase or as a subscription, you must also provide payout and tax information. This information must be validated. |
|
  
    
    
![Seller Dashboard checklist checkbox](images/17bacc50-19b6-45fc-81ae-1097bdb3c928.gif)
  
    
    

  
    
    

  
    
    
|App appropriately localized |If your app or add-in supports multiple languages, verify that it has been appropriately localized, or it will not pass validation and won't be approved. For more information, see  [Localization for Office Add-ins](http://msdn.microsoft.com/library/5a1a1cd7-b716-4597-b51f-fa70357d0833%28Office.15%29.aspx) and [Localize SharePoint Add-ins](http://msdn.microsoft.com/library/907a9189-7ce3-469a-8c87-4cef26f03c73%28Office.15%29.aspx). |
   

## Additional resources
<a name="bk_addresources"> </a>


-  [Validation policies for apps and add-ins submitted to the Office Store (version 2.1)](validation-policies-for-apps-and-add-ins-submitted-to-the-office-store-version-2.md)
    
  
-  [Update, unpublish, and view app and add-in metrics in the Seller Dashboard](update-unpublish-and-view-app-and-add-in-metrics-in-the-seller-dashboard.md)
    
  
-  [Create or update client IDs and secrets in the Seller Dashboard](create-or-update-client-ids-and-secrets-in-the-seller-dashboard.md)
    
  
-  [Submit SharePoint Add-ins for Office 365 operated by 21Vianet in China](submit-sharepoint-add-ins-for-office-365-operated-by-21vianet-in-china.md)
    
  
-  [Decide on a pricing model for your Office or SharePoint Add-in or Office 365 web app](decide-on-a-pricing-model-for-your-office-or-sharepoint-add-in-or-office-365-web.md)
    
  
