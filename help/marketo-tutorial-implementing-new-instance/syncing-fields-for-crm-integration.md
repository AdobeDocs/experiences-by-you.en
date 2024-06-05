---
title: Syncing Fields for the Native CRM Connectors
description: Learn how to streamline your initial CRM integration by strategically selecting the essential CRM fields for Marketo Engage to use. Conduct the Data Dictionary exercise to identify the fields you need for a smooth CRM sync that helps sales and marketing teams stay aligned.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-04
jira: KT-14811
thumbnail: KT-14811.jpeg
exl-id: 42b7ca3d-e445-4c11-ad3d-d4e70c101c8e
---
# Syncing Fields for the Native CRM Connectors

Are you using Salesforce or Microsoft Dynamics within your organization? If so, with Marketo Engage's native CRM connectors (i.e. Salesforce, Microsoft Dynamics, and Veeva), you can coordinate marketing and sales activities by seamlessly sharing relevant information between Marketo Engage and CRM. Before you configure the initial CRM sync, make sure you identify the fields you'd like to sync between the two systems to keep your Marketo Engage database clean.  

Learn more about how to conduct this exercise with best practices suggested by Adobe Professional Services. Follow along to understand Standard Fields and Custom Fields and document their relationships between Marketo Engage and your CRM. 

## Identify fields to sync before integrating your CRM with Marketo Engage

When integrating your CRM with Marketo Engage, you probably won't need to sync all your CRM fields to Marketo Engage. Being strategic about the fields you need can help your Marketo Engage instance process the data flow more efficiently.  

The initial sync between your Marketo Engage and CRM system will automatically make associations for most existing standard fields (i.e. Email, First/Last Name, Company, etc.). Additionally, the connector also syncs [Custom Fields](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} for your Leads, Contacts, Accounts, and Opportunities by creating new fields in Marketo Engage that are automatically mapped to those fields from your CRM. 
 
Identifying and organizing the fields that you'd like to sync from your CRM prior to performing the initial sync is a critical step in the Native Connector setup process. We refer to this as a Data Dictionary exercise, which helps you minimize the number of duplicate fields that get created and make any subsequent remapping steps go as smoothly as possible. This exercise typically involves input from the Marketing and Sales teams and your CRM Admin to ensure that only relevant fields are synced to your Marketo Engage instance. 
 
## How to build your Data Dictionary

Generally, the best practice is to only sync CRM fields that will be needed for marketing purposes. Start with this exercise to organize the fields from your CRM that will need to be mapped to Marketo Engage and run the initial CRM sync correctly the first time.

>[!NOTE]
>If you have custom fields in your CRM that already have an equivalent custom field in Marketo Engage before beginning the initial sync, a new "duplicate" field will be created in Marketo Engage for the CRM field. You can re-map the CRM field to the original Marketo Engage field and hide the duplicate field once the initial sync is complete, but you will need to contact [Adobe Customer Support](https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console){target="_blank"} to do so. See step 7 for more details.

**Step 1:** Build a rough list of fields currently available in your CRM and mark whether you would like them to appear in Marketo Engage.  

* Include feedback from your CRM admin, marketing, and sales teams in the decision-making process. 
* Document the API names and field types for each field 
* Determine what level of access Marketo Engage should have for these fields (i.e. Read-Only or Read-Write) 


**Step 2:** Review the [Admin > Field Management section](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/view-field-mappings-between-marketo-and-salesforce){target="_blank"} of your Marketo Engage instance to Identify any custom fields previously created directly in the system that you would like to include in the sync.

* Document the API names and field types for each field.
* Denote fields that already have an equivalent field in your CRM. 
* Denote fields that do not already have an equivalent field in your CRM.
 

**Step 3:** Start building the Data Dictionary with the default map fields

* Since Marketo Engage uses a flat database, it's recommended that you format your Data Dictionary as follows: 

  * First Column: Marketo Engage Field Names 
  * Second Column: Marketo Engage API Names 
  * Third Column: [Marketo Engage Field Type](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} (i.e. Boolean, Currency, Date, etc)  
  * In subsequent columns, repeat for the CRM object types (Lead, Contact, Account, Opportunity) with an additional column for the level of access you'd like Marketo Engage to have (i.e. Read, Write, Edit) 
  <br>

  Here's a sample of what it would look like: 
    ![Data Dictionary Table](/help/marketo-tutorial-implementing-new-instance/assets/data_dictionary.png){width="100%" zoomable="yes"}


* Start by adding the default fields that will be automatically mapped for your CRM:

  * [Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/default-salesforce-field-mapping){target="_blank"}
  * [Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/default-dynamics-field-mapping){target="_blank"}
  * [Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/veeva-crm-sync/sync-details/default-veeva-field-mapping){target="_blank"}

* Confirm each default field in Marketo Engage matches the field in your CRM that you would like to sync with. For example, the "Unsubscribed" field in Marketo Engage could be the "Email Opt Out" field in your CRM.  
* Adjust the CRM API name, privileges, and [data type](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank"} where necessary. 

**Step 4:** Add additional fields to the Data Dictionary 

* Include the Display Name, desired CRM privileges and data type for each field.
* If a field exists in CRM but not Marketo Engage, fill the Marketo Engage display and API names with the same values from the CRM field. 
* If a field exists in Marketo Engage but not the CRM, fill the CRM display name with the desired value but leave the CRM API name blank until after the field is created. 
* If equivalent fields exist in both systems, include them on the same line and indicate that they will need to be remapped in the "Notes" section at the far right of your Data Dictionary sheet. 

>[!NOTE]
>If you're planning on creating a Sync Filter field ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}), make sure to include it in this step but leave the API names blank until the field is created in your CRM.  

**Step 5:** Review the Data Dictionary with your CRM Admin 

* Create fields in CRM for those that already exist in Marketo Engage and update the Data Dictionary with the Display and API names for the new CRM field. 
* Perform field mapping between Lead and Contact objects in your CRM ([Salesforce](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"} | [Microsoft Dynamics](https://community.dynamics.com/blogs/post/?postid=8a91d93e-2181-45dd-a8fb-1092010bc8f1){target="_blank"}). When a Lead is converted into a Contact, this ensures the fields can be consolidated into a single field in Marketo Engage.  
* Ensure that the Marketo Sync Profile has appropriate privileges to each field as noted in the Data Dictionary:
  * [Set profile permissions in Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited#set-profile-permissions){target="_blank"} 
  * [Set profile permissions in Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"}
  * [Set profile permissions in Veeva](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up#create-application-user-in-microsoft){target="_blank"} 

**Step 6:** Perform the initial sync 

* Ensure that all fields you would like to sync with Marketo Engage have the appropriate privileges in your CRM as defined by the Data Dictionary. 
* Ensure that all fields you would  ***not*** like to sync with Marketo Engage are [hidden from the Marketo Sync Profile](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync){target="_blank"}. It is much easier to add new fields to the sync later than it is to remove fields that were unintentionally synced. 
* Are you connecting your CRM with the Sync Filter field? If you sync to Salesforce, contact Adobe Customer Support to ensure the filter functionality is turned on before starting your initial sync. 
 

**Step 7:** Review the Field Management section in Marketo Engage 

* Confirm/update the Display & API Names for the new synced fields. 
* Identify any duplicated fields that may require remapping. Duplicated fields occur in a few scenarios:  
  * Custom fields in the CRM would create a new (potentially duplicate) field in Marketo Engage the first time they sync down if an equivalent field already existed in Marketo Engage. 
  * Marketo-Engage-Only custom fields (i.e. a field created directly in Marketo Engage) and you may have an equivalent field synced from the CRM. 

 

**Step 8:** Contact Adobe Customer Support to perform remapping if duplicated fields appear 

* Contact Support with the following information for fields that need to be remapped: 
  * Display & API names for new duplicate fields created by the CRM. 
  * Display name for Marketo Engage field that you would like the CRM field to map to. 
  * Please refer to this example [HERE](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank"}. 
* Once remapping is complete, review the API names for the remapped fields in Marketo Engage and update the values in your Data Dictionary's "API Name" column to ensure it contains the most accurate information. 

## What's Next? 

* Build your Data Dictionary to organize your fields for the CRM integration.   
* Familiarize yourself with the initial sync process for your CRM 

>[!BEGINTABS]

>[!TAB Salesforce]
  
Learn how Marketo Engage and Salesforce go together to keep your sales and marketing data in sync.

>[!VIDEO](https://video.tv.adobe.com/v/3424719/?learn=on)

+++**Links used in the video:**

* [Understanding the Salesforce Sync](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.html){target="_blank"}

* [Add Marketo Fields to Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.html){target="_blank"}

* [Create a Marketo User in Salesforce (Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.html){target="_blank"}

* [Connect Marketo and Salesforce(Enterprise/Unlimited)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.html){target="_blank"}

* [Users would need to Set Up the Connected App on the Salesforce side before they proceed to Marketo and Salesforce Sync.](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.html){target="_blank"}

* [Salesforce Sync Status](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/salesforce-sync-status.html){target="_blank"}

* [Hide and Unhide a Field](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/hide-and-unhide-a-field.html){target="_blank"}

* [Tutorial: Learn about syncing Marketo to your CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!TAB Microsoft Dynamics]

Learn how the Microsoft Dynamics 365 sync works and configure the setup properly to allow the two systems to speak to each other.

>[!VIDEO](https://video.tv.adobe.com/v/3424737/?learn=on)

+++**Links used in the video:**

* [Understanding the Microsoft Dynamics Sync](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/understanding-the-microsoft-dynamics-sync.html){target="_blank"}

* [Download the Marketo Lead Management Solution](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/download-the-marketo-lead-management-solution.html){target="_blank"}

* [Update the Marketo Solution for Microsoft Dynamics](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.html){target="_blank"}

* [Grant Consent for Client Id and App Registration](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/grant-consent-for-client-id-and-app-registration.html)

* [Validate Microsoft Dynamics Sync](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/validate-microsoft-dynamics-sync.html){target="_blank"}

* [Sync Status](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/sync-status.html){target="_blank"}

* [Fix Dynamics Validation Sync Issues](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/fix-dynamics-validation-sync-issues.html){target="_blank"}

* [Create a Custom Dynamics Sync Filter](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/custom-dynmaics-sync-filter-details/create-a-custom-dynamics-sync-filter.html){target="_blank"}

* [View the Organization Service URL](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/sync-setup/view-the-organization-service-url.html){target="_blank"}

* [Editing Fields to Sync Before Deleting Them in Dynamics](https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/editing-fields-to-sync-before-deleting-them-in-dynamics.html){target="_blank"}

* [Tutorial: Learn about syncing Marketo to your CRM](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/crm-sync-learn.html){target="_blank"}

+++

>[!ENDTABS]

### Authors

{{peter-livadas}}

{{amy-chiu}}
