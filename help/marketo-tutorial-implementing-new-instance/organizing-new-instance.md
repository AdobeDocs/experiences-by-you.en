---
title: Organizing a new instance and establishing naming conventions
description: Learn how to set up a good organization within your Marketo Engage instance, allowing future marketers within your organization to easily navigate through the programs, modify the assets, and pull reports.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last-substantial-update: 2024-05-03
jira: KT-14813
thumbnail: KT-14813.jpeg
---
# Organizing a new instance and establishing naming conventions

As an administrator implementing a new Marketo Engage instance, you are laying down the groundwork allowing future marketers within the organization to easily navigate through the instance. Getting familiar with the tree folder structure and naming conventions will keep your instance tidy and set up for long-term success. This tutorial encompasses examples recommended by Adobe and Marketo Engage Champion(2019-2020), Natalie Kremer, to help you [organize the folders and name assets consistently](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630){target="_blank"}. 

## Why is structuring folders and applying naming conventions necessary?

Staying organized in your instance makes it easy for you and your colleagues to keep track of campaigns, programs, and assets and report program performance. To organize the navigation tree in your instance and build at scale, it is recommended to use [folders](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders){target="_blank"}, [standard naming conventions](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#naming-schemes){target="_blank"}, and features such as [cloning](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs#cloning){target="_blank"}.

## How to organize a Marketo Engage instance

>[!VIDEO](https://video.tv.adobe.com/v/3421577/?quality=12&learn=on)

### Step 1 - Setting up a folder structure to put your programs in order

The first step to organizing your instance is to [set-up a folder structure](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html) house your program and assets in an easy to find and orderly manner.

Here are some quick tips when structuring the folders in tree:

* Maintain a flat folder structure for discoverability.
* Structure your folders to reflect your organization's team structure (e.g. Region or Team) or initiatives (e.g. Newsletters).
* Include time-based labels to enable searchability and signal appropriate timing for archiving (e.g. 2024).
  * Administrators are recommended to archive folders at least once a year. Using an annual folder name, you can easily deactivate live Smart Campaigns and archive the entire folder at the end of the year.

Below are folder examples of putting these tips into practice.

**Folder Name in Tree**

>[!BEGINTABS]

>[!TAB Marketing Activities]

![Folders Marketing Activities](/help/marketo-tutorial-implementing-new-instance/assets/folders-marketing-activities.png)

>[!TAB Design Studio]

![Folder Design Studio](/help/marketo-tutorial-implementing-new-instance/assets/folders-design-studio.png)

>[!TAB Database]
  
![Folder Database](/help/marketo-tutorial-implementing-new-instance/assets/folders-database.png)

>[!ENDTABS]

### Step 2 - Building folders within the programs

Now, let's apply the folder structure at the program level. As a best practice, housing the local assets in sub-folders will help you keep the programs tidy and allow internal users to modify or report on the programs efficiently. Common sub-folders include emails, landing pages, Smart Campaigns, Lists, Reports, etc..

**Folder Name inside Programs**
* Campaigns - *Folder for all campaigns managing interactions and status tracking.*
* Local Assets - *Folder for all assets that are specific to this Program.*
  * Emails
  * Landing Pages
  * Smart Campaigns
  * Lists - *Only needed when there are Program specific Lists.*
  * Forms - *Only needed when there are Program specific Forms; most Forms are Global Assets.*
  * Reports - *Only needed when there are Program specific Reports.*

### Step 3 - Create naming conventions for your programs and assets

Once you have the folder structure in Tree, you will want to name the programs and assets consistently. This is when standardizing naming conventions would be helpful to scale up the naming process internally. Here are a few components that you can use to establish naming convention to ensure searchability:

* Program Type Abbreviation - Email, Content, Nurture, Webinar, etc.
* Category - Type of Program - Standalone Email, Newsletter, etc.
* Dates - Program launch date
* Short Description - Brief description about the Program

Now, let's put the values into the formula and generate the program names for various program types.

#### Program Naming Formula

| **Abbreviation of Program Type** | **YYYY** | **\-** | **MM** | **\-** | **DD(Optional)** | **Category** | **\-** | **Brief Description of Program** |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| EM - Email Send (Email Program) | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| NL – Newsletter | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| ENG – Engagement Program | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| WBN - Webinar | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| IW – Interactive Webinar | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| TS – Tradeshow | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| LE – Live Event (Roadshow) | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| UG - User Group | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| WC – Website Content | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| CS – Content Syndication | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| LI – List Import | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| OA – Online Advertising | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |
| PPC – Pay Per Click | YYYY | \-  | MM | \-  | DD(Optional) | Category | \-  | Brief Description of Program |

| **Examples** |
| --- |
| ES 2023-10 Gated Content - XYX Whitepaper |
| WC-2023-10- Monthly Webinar - ABC Case Study |

#### Asset Naming Formula

Going one level down to naming assets, it's best that you do not repeat the Program name and use short and generic identifiers for future cloning use. Here are a few quick tips for you to keep in mind:

* Number the assets based on their sequence in the program process.
* Use "-" (hyphen) to separate the naming components instead of "."(dot) or "\_"(underscore).
  * Why? Marketo Engage uses a dot to separate the Program Name from the Campaign Name. Using "\_" will prevent you rom seeing it when the asset is hyperlinked.
* Use standard acronyms in the asset names to shorten the reference and still allow easy recognition.

With these in mind, we will apply these tips to the following assets and create formulas to generate names:

##### Name the assets based on sequence in program process

| **Sequence in Program Process** | **\-** | **Description** |
| --- | --- | --- |
| 01  | \-  | Description |
| 02  | \-  | Description |
| 03  | \-  | Description |

| **Examples: Smart List** |
| --- |
| 01-Send Email |
| 02-Opened |
| 03-Clicked |
| 04-Filled-out Form |
| 05-Influenced (Program Success) |
| 06-Unsubscribed |

##### Name the assets with abbreviation of asset type

| **Abbreviation of Asset Type** | **Asset Type** | **\-** | **Description of Goal** |
| --- | --- | --- | --- |
| LP - Landing Page | LP  | \-  | Description of Goal |
| EMAIL - Email (outbound) | EMAIL | \-  | Description of Goal |
| ALERT - Email Alert | ALERT | \-  | Description of Goal |
| WF - Web Form | WF  | \-  | Description of Goal |
| EXCL - Exclusion List | EXCL | \-  | Description of Goal |
| SLST - Smart List | SLST | \-  | Description of Goal |
| LST - Static List | LST | \-  | Description of Goal |

| **Examples** |
| --- |
| LP-Registration |
| LP-ThankYou |
| EMAIL-Outbound |
| EMAIL-Newsletter |
| EMAIL-Invitation |
| EMAIL-Reminder |
| EXCL-Competitors |

##### Name the downloadable files(.pdf) with abbreviation of asset type

| **Asset Type** | **Content Description** | **\-** | **Abbreviation of Asset Type** | **.** | **PDF** |
| --- | --- | --- | --- | --- | --- |
| WP - White Paper | Content Description | \-  | WP  | .   | pdf |
| CS - Case Study | Content Description | \-  | CS  | .   | pdf |
| DS - Data Sheet | Content Description | \-  | DS  | .   | pdf |

| **Examples: Downloadable PDF files** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

>[!CAUTION]
>
>When naming files in the above examples, do not use spaces and avoid the use of underscores "\_"

## What's Next?

* Download the Worksheet: [Marketo Engage Organization and Naming Conventions](./assets/adobe-marketo-engage-organization-and-naming-conventions.xlsx){target="_blank"} to support the creation of the folder structure and naming conventions.
* Once you determine the necessary components in your standard naming convention, consider building formulas into a Google Sheet or Microsoft Excel. For future use, simply input your values in the spreadsheet to generate your Program names.
* Once you align on an overall folder structure, it is time to think through the templates you need based on the most frequent use cases and the most common requests your team receives. Then start building your first program template. Read on to get started with [Adobe Marketo Engage program templates](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates){target="_blank"}.
  
### Authors

{{natalie-kremer}}

{{amy-chiu}}
