---
title: Troubleshooting for Marketers
description: Knowing the most common errors can help with faster problem-solving and boost your productivity. These troubleshooting tips to help you effectively resolve similar errors as they occur.
version: Standard
feature: Workflows
role: User
level: Beginner, Intermediate, Experienced
doc-type: Article
last-substantial-update: 2023-05-18
jira: KT-13256
thumbnail: KT-13256.jpeg
exl-id: 24a6815b-52d1-4bd6-9d27-522720a91f83
---
# Troubleshooting for Marketers: 5 Common Workflow and Delivery Errors 

By: [Suraj Patra](https://www.linkedin.com/in/suraj-p-51612053/){target="_blank"}, Senior Consultant, Meijer 

As a Senior Engineer and customer expert on Adobe Experience Cloud products for the past five years, I enable business users at [Meijer](https://www.meijer.com/){target="_blank"}, an American supercenter chain founded in 1934, to run complex marketing and transactional campaigns with ACS. A few projects that I've worked on include customized campaigns to store offers and order details for personalization, integrated with Adobe Audience Manager, and customer insight for segment ingestion.  


In my time using ACS, I've run into errors which can be time consuming and frustrating to solve. Knowing the most common errors can help with faster problem-solving and boost your productivity. Below are my troubleshooting tips to help you effectively resolve similar errors as they occur. 

## Data Type Mismatch Error  

**Error Code:** 
`PGS-220000 PostgreSQL error: ERROR: operator does not exist: character varying = bigint` 

**Cause:** 
These types of errors appear in a workflow when you try to reconcile using fields of different data types. For example, when you upload a file using load file which has a string field, and you try to reconcile the string field with a profile field that has data type of int.

![data-type-mismatch-error](/help/assets/kt-13256/data-type-mismatch.png)

**Solution:**
 Change the data type of the field in "Load file" activity to the one that you are matching with. Open the "Load File" activity. Move to the "COLUMN DEFINITION" tab and change the data type of the desired field.


![data-type-mismatch-solution](/help/assets/kt-13256/data-type-mismatch-solution.png)

## Delivery Personalization Error    

**Error Code:** 
`The schema for profiles specified in the transition ('') is not compatible with the schema defined in the delivery template ('nms:recipient'). They should be identical.` 
 
**Cause:** 
This error appears when you are sending an email to an address, but the email or any other identifier is not reconciled with a profile. To send an email communication, the email or the identifier should be always linked to a profile.  

![workflow with reconciliation activity](/help/assets/kt-13256/del-persn-error-wf.png)

**Solution:**
A common ID must exist from the loaded file with the recipient table. This common key joins the load file to the recipient table within the reconciliation activity. Emails may not be sent to records that do not exist in the recipient table which requires this reconciliation step within the workflow. In doing so, you would reconcile the incoming load file activity with an identifier like email ID from the profile. The `nms:recipient` schema refers to the profile table and reconciling the incoming records with profile makes it available during email preparation. 

Refer to the screenshot for reconciliation activity as shown below. 

![workflow with reconciliation detail](/help/assets/kt-13256/del-persn-error-wf-solution.png)

Learn more about [reconciliation](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/data-management-activities/reconciliation.html?lang=en). 

## Common Field Dataset Error

**Error Code:** 
`The document types of inbound events (''and'') are incompatible (step 'Exclusion'). Unable to perform the operation. `

**Cause:** 
This issue occurs while using the **exclusion activity** in ACS workflows, when performing an exclusion based on the ID, when the Primary set and the excluded set don't have the same field names. 


![Common Field Dataset Error](/help/assets/kt-13256/dataset-error.png)

**Solution:**

There are two ways to resolve this error: 

1. Use the same field name in both the primary and excluded and use that field as ID 

    OR 

2. Use the JOINS exclusion method to select the field based on which you want to exclude the records. 

![Common Field Dataset Error - Solution ](/help/assets/kt-13256/dataset-error-solution.png)

## Field Name Dropped Error  

**Error Code:** 
`XTK-170036 Unable to parse expression 'i__name'`

**Cause:** 

Failure points may occur in an **enrichment activity**. One of the most common is displayed below. 

![Field Name Dropped Error](/help/assets/kt-13256/field-name-dropped-error.png)

This happens when you manually edit an expression name in the activity. The image shows that the expression was modified from `name `to `i__name`. 

**Solution:**

You can resolve this error in three ways: 

1. Change the name back to the expression that was originally present. 

2. If you want to use a new name, change the values in the **enrichment activity**. 

3. If you don't remember what has changed, your best bet would be to recreate the activity. 

## Temporary Table Dropped Error 

**Error Code:** 
`XTK-170024 The temporary schema "temp:deliveryEmail1" is not defined in the current context.`

**Cause:** 
This is a common error in complicated workflows involving enrichment or other activity. It probably means some of the activity workflows are not correctly saved during multiple changes to the workflow. 

![Temporary Table Dropped Error ](/help/assets/kt-13256/temp-table-dropped-error.png)

**Solution:**
There are many ways that this error can occur, so there is not a simple fix. If it is a simple workflow, then it would better to reconfigure the activity. In a complicated workflow, it is better to copy the workflow activities to a new workflow, save, and rerun it.
