---
title: Log CRM Sync Errors for Easy Troubleshooting
description: Learn how to use a log of CRM Sync errors to investigate CRM sync issues and keep it running smoothly.
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16
jira: KT-13875
thumbnail: KT-13875.jpeg
hide: no
---

# Log CRM Sync Errors for Easy Troubleshooting

As a Marketo Engage administrator, checking if your instance is in sync with your CRM should be a key part of your [daily routine](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (find it on the top right corner of your Marketo Engage interface) is where you will start to find and investigate frequent syncing issues, there is a pro tip that could help you manage the instance health in an organized manner. Adobe Marketo Champion (2019-2022), Amy Goldfine recommends admin users keep a log of CRM Sync errors to make troubleshooting easier.

![Screenshot of the Sync Errors tab](/help/tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Why keep a record of CRM Sync Errors? 

By logging the CRM Sync errors, Marketo Engage admins can review the issues and trends with the CRM administrators to fix the root cause. Follow the steps below to document your CRM Sync issues for your instance.  

## How to keep a log of CRM Sync Errors 

Before you get started, download the [CRM Sync Errors Log template](/help/tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx). 

**Step 1:** Go to the *[!UICONTROL Admin] section* in Marketo Engage. Under *[!UICONTROL Integration]*, click *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]*, or *[!DNL Veeva]*, depending on which [!DNL CRM] you use, then the *[!UICONTROL Sync Errors]* tab. 

**Step 2:** You can choose to [export the records of errors as a [!DNL CSV] file through the [!UICONTROL Filter] panel](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. If you only have a few hours, copying and pasting directly from the *[!UICONTROL Sync Errors]* tab would be the way to go. 

**Step 3:** Note the date that the error occurred.   

**Step 4:** Enter the number of person records affected by that error. (Sometimes your CRM will only throw an error for one person. Sometimes there will be many people with the same error at once.)   

**Step 5:** Note the email address of one person affected by the error. This makes it easy for you to reference and discuss the errors with the CRM administrator.   

**Step 6:** Paste links to the person record in [!DNL Marketo Engage] and [!UICONTROL CRM Lead/Contact] record of that person.   

**Step 7:** In the last column, paste the actual text of the error.

## What's Next?  

**Identify Error Codes:** To understand the error codes, look up the descriptions in the developers documentation [Response-Level Error Codes table](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} and find typical next steps to resolve the errors.  

## Authors

**Amy Goldfine**  
Adobe Marketo Champion(2019-2022)
*Founder, MarketingOpsAdvice.com*

![Amy Goldfine](/help/tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Adoption & Retention Marketing Manager at Adobe* 

![Amy Chiu](/help/tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
 
