---
title: Mapping fields for CRM integration
description: Learn how to streamline your initial CRM integration by strategically selecting the essential CRM fields for Marketo Engage to use. Use our field mapping worksheet to map the necessary fields accurately for a smooth CRM sync that helps sales and marketing teams stay aligned.
role: Admin
level: Beginner
doc-type: Article
duration: 0
last-substantial-update: 2024-05-04
jira: KT-14811
thumbnail: KT-14811.jpeg
---

# Mapping fields for integrating with your CRM

Are you using CRM within your organization? If so, with Marketo Engage’s native CRM connectors (i.e., Salesforce, Microsoft Dynamics, and Veeva), you can coordinate marketing and sales activities by seamlessly sharing relevant information between Marketo Engage and CRM. Before you configure the initial CRM sync, make sure you map out the fields between the two systems properly to keep the database clean.

Learn more about how to conduct this field mapping exercise suggested by Julz James, Adobe Marketo Engage alumnus (2015) to document Standard Fields, Custom Fields, and their relationships between two systems.

## Why should you map fields before integrating your CRM with Marketo Engage?

When you initially sync your Marketo Engage account with CRM, Marketo Engage automatically makes these associations between your built-in CRM and Marketo Engage fields. Marketo Engage will also sync your Custom Fields such as your Leads, Accounts, Opportunities, and Contacts.

Mapping out the relationships between fields upfront is critical and it will save you from remapping when duplicated fields are created in Marketo Engage. To orchestrate the data exchange between your marketing and sales team, you need to ensure your CRM admin, marketing, and sales teams understand what fields are important to map or not and the purpose of having them in synced in Marketo Engage and your CRM.

## How to map the CRM fields

When integrating your CRM with Marketo Engage, you probably don't need to sync all your CRM fields to Marketo Engage. Being strategic about the fields you need can help your Marketo Engage instance process the data flow more efficiently.

Start with this exercise to determine which fields from your CRM will need to be mapped over to Marketo Engage to run the initial CRM sync correctly the first time.

>[!NOTE]
>
>While it is possible to re-map the fields between CRM and Marketo Engage after initial sync, you will need to contact Marketo support with a request for your current field mapping and your desired field mapping. You will need to provide the Marketo Engage Field(s) and the API Name(s) as this example [here](https://nation.marketo.com/t5/knowledgebase/re-mapping-sfdc-marketo-fields/ta-p/299284){target="_blank}.

**Step 1**: List out fields available in CRM and mark whether transferring them to Marketo Engage.

* Include feedback from your CRM admin, marketing, and sales teams in the decision-making process to help keep only useful fields in Marketo Engage.
* Add the fields to Marketo Engage that are required to create a contact in your CRM.
  * Reference Add Marketo Fields to Salesforce [Enterprise/Unlimited](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited#add-marketo-fields-to-salesforce){target="_blank} or [Add Marketo Fields to Salesforce](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional#add-marketo-fields-to-salesforce){target="_blank} for the required fields.
  * Reference the [Create a Contact in Microsoft Dynamics](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/microsoft-dynamics/microsoft-dynamics-sync-details/create-a-contact-in-microsoft-dynamics){target="_blank} for the required fields.

**Step 2**: Document the API names for the CRM fields to which you want to map your Marketo Engage fields. These should be the underlying API name of field as it appears in CRM.

**Step 3**: Label the field types for each field that you decide to map between Marketo Engage and your CRM. Choose from [a list of types available in Marketo Engage](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/custom-field-type-glossary){target="_blank}. You will need to use this information as you create Custom Fields.

**Step 4**: Consolidate the fields mapped on paper to avoid duplicated fields. In some cases, you will want to map multiple fields from your CRM to single Marketo Fields. For example, Email Address in Marketo Engage would map to both Lead Email Address and Contact Email Address in your CRM.

**Step 5**: As you wrap up this exercise, consider including the Marketo-Engage-only fields and fields that are syncing from CRM to Marketo Engage into a ‘Data Dictionary’ for your Marketo Engage users to reference.

## Exercise sheet: Field mapping for Marketo Engage and CRM integration

Below is a sample exercise sheet with the necessary attributes for you to get started with mapping the fields. Download the sample for your offline use \[LINK TO DOWNLOADABLE FILE\].

| Fields available in CRM | Field API Name in CRM | Object Type | CRM Field Type | Transfer Over to Marketo Engage? | Field Name in Marketo | API Name in Marketo Engage | Marketo Engage Field Type |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Name of field as it appears in CRM (Account Name, Billing City, Marketing Suspended, etc.) | Underlying API Name of field as it appears in CRM (account_name_a, billing_city, etc.) | Object Type in CRM (Lead, Contact, Account, Opportunity, etc.) | Field format (string, text, datetime, etc.) | Y/N | What is the field called in Marketo? | API Name will help map to CRM | Field format (string, text, datetime, etc.) |
| EXAMPLES |     |     |     |     |     |     |     |
| Company Name | company_name | Lead | string | Y   | Company Name | Company Name | string |
|     | company_name_a | Account | string | Y   | Company Name (A) | Company Name | string |

## What’s Next?

* Download the [exercise sheet](./assets/field-mapping-for-marketo-engage-crm-integration.xlsx){target="_blank} to map fields for CRM integration.
* Finalize the fields mapped with CRM, sales, and marketing teams to ensure the selection serves the purposes for each team.
* With the final mapping sheet, go to Admin > Field Management and [create a Custom Field](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo){target="_blank} in Marketo Engage. If you want the fields to be kept in sync with your CRM, create them in the CRM and they will automatically be created in Marketo Engage.
* Take the next steps to configure the initial CRM sync and select the fields to sync:
  * Watch the [Salesforce sync demo](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup){target="_blank}
  * Watch the [Microsoft Dynamics demo](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup){target="_blank}

### Authors

{{julz-james}}

{{amy-chiu}}
