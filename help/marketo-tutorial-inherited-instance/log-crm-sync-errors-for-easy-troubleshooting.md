---
title: Log CRM Sync Errors for Easy Troubleshooting
description: Learn how to use a log of CRM Sync errors to investigate CRM sync issues and keep it running smoothly.
feature-set: Marketo Engage
feature: Administration
role: Admin
level: Intermediate, Experienced
doc-type: Tutorial
last-substantial-update: 2023-10-16T00:00:00.000Z
jira: KT-13875
thumbnail: KT-13875.jpeg
exl-id: 6a38f5dd-5d25-43d8-a1d3-e75ab396e555
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
    internal-label: Experience Manager
  - id: c68cd75e-5bca-4bc3-a60e-9e183f816441
    internal-label: Experience Manager Cloud Manager
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
---
# Log CRM sync errors for troubleshooting

As a [!DNL Marketo Engage] administrator, checking if your instance is in sync with your CRM should be a key part of your [daily routine](https://nation.marketo.com/t5/champion-program-blogs/my-marketo-morning-routine-tips-for-driving-marketing-operation/ba-p/247508){target="_blank"}. While the [Notifications section](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/notification-types.html){target="_blank"} (find it on the top right corner of your [!DNL Marketo Engage] interface) is where you will start to find and investigate frequent syncing issues, there is a pro tip that could help you manage the instance health in an organized manner. [!DNL Adobe] Marketo Champion (2019-2022), Amy Goldfine recommends admin users keep a log of CRM Sync errors to make troubleshooting easier.

![Screenshot of the Sync Errors tab](/help/marketo-tutorial-inherited-instance/_assets/Marketo_Engage_Admin_Salesforce_Sync_Errors_Tab.png)

## Why keep a record of CRM Sync Errors? 

By logging the CRM Sync errors, [!DNL Marketo Engage] admins can review the issues and trends with the CRM administrators to fix the root cause. Follow the steps below to document your CRM Sync issues for your instance.  

## How to keep a log of CRM sync errors 

Before you get started, download the [CRM Sync Errors Log template](/help/marketo-tutorial-inherited-instance/_assets/downloads/Adobe-Marketo-Engage_CRM-Sync-Error-Log-Template.xlsx).

**Step 1:** Go to the *[!UICONTROL Admin] section* in [!DNL Marketo Engage]. Under *[!UICONTROL Integration]*, click *[!DNL Salesforce]*, *[!DNL Microsoft Dynamics]*, or *[!DNL Veeva]*, depending on which [!DNL CRM] you use, then the *[!UICONTROL Sync Errors]* tab. 

**Step 2:** You can choose to [export the records of errors as a [!DNL CSV] file through the [!UICONTROL Filter] panel](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.html#filter-sync-errors){target="_blank"}. If you only have a few hours, copying and pasting directly from the *[!UICONTROL Sync Errors]* tab would be the way to go. 

**Step 3:** Note the date that the error occurred.   

**Step 4:** Enter the number of person records affected by that error. (Sometimes your CRM will only throw an error for one person. Sometimes there will be many people with the same error at once.)   

**Step 5:** Note the email address of one person affected by the error. This makes it easy for you to reference and discuss the errors with the CRM administrator.   

**Step 6:** Paste links to the person record in [!DNL Marketo Engage] and [!UICONTROL CRM Lead/Contact] record of that person.   

**Step 7:** In the last column, paste the actual text of the error.

## What's next?  

**Identify error codes:** To understand the error codes, look up the descriptions in the developers documentation [Response-Level Error Codes table](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes){target="_blank"} and find typical next steps to resolve the errors.  

## Authors

**Amy Goldfine**  
[!DNL Adobe] Marketo Champion(2019-2022)
*Founder, MarketingOpsAdvice.com*

![Amy Goldfine](/help/marketo-tutorial-inherited-instance/_assets/authors/Customer_Author_Amy_Goldfine.png){width="25%"}

**Amy Chiu**
*Adoption & Retention Marketing Manager at [!DNL Adobe]* 

![Amy Chiu](/help/marketo-tutorial-inherited-instance/_assets/authors/Adobe_Author_Amy_Chiu.png){width="25%"}
