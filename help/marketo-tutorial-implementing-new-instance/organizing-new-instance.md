---
title: Organizing a new instance and establishing naming conventions
description: Learn how to set up a good organization within your Marketo Engage instance, allowing future marketers within your organization to easily navigate through the programs, modify the assets, and pull reports.
role: Admin
level: Beginner
doc-type: Article
duration: 0
last-substantial-update: 2024-05-03
jira: KT-14813
thumbnail: KT-14813.jpeg
---
# Organizing a new instance and establishing naming conventions

As an administrator implementing a new Marketo Engage instance, you are laying down the groundwork allowing future marketers within the organization to easily navigate through the instance.

Getting familiar with the tree folder structure and naming conventions will keep your instance tidy and set up for long-term success. This tutorial encompasses examples recommended by Adobe and Marketo Engage Champion alumnus, Natalie Kremer [Keep Marketo Engage Organized with Folders and Naming Conventions](https://nation.marketo.com/t5/champion-program-blogs/keep-marketo-engage-organized-with-folders-and-naming/ba-p/245630) and [Get started with Adobe Marketo Engage program templates](https://business.adobe.com/blog/how-to/get-started-with-marketo-engage-program-templates) to help you organize the folders and name assets consistently.

## Why is structuring folders and applying naming conventions necessary?

Staying organized in your instance makes it easy for you and your colleagues to keep track of campaigns, programs, and assets and report program performance. To organize the navigation tree in your instance and build at scale, it is recommended to use folders, standard naming conventions, and features such as cloning.

## How to organize a Marketo Engage instance

>[!VIDEO](https://video.tv.adobe.com/v/3421577/?quality=12&learn=on)

### Step 1 - Setting up a folder structure to put your programs in order

The first step to organizing your instance is to [set-up a folder structure](https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.html) house your program and assets in an easy to find and orderly manner.

Here are some quick tips when structuring the folders in tree:

* Maintain a flat folder structure for discoverability.
* Structure your folders to reflect your organization’s team structure (e.g. Region or Team) or initiatives (e.g. Newsletters).
* Include time-based labels to enable searchability and signal appropriate timing for archiving (e.g. 2024).
  * Administrators are recommended to archive folders at least once a year. Using an annual folder name, you can easily deactivate live Smart Campaigns and archive the entire folder at the end of the year.

Below are folder examples of putting these tips into practice.

>[!NOTE]
>
>**FOR THE BELOW TABLE** --> Please see the NOTE blocks in step 2 that reference the table options.  I will make this table match whatever you decide for step 2.

| **Folder Name in Tree** |     |     |     |     |     |     | **Description** |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **Marketing Activities** |     |     |     |     |
|     | Active Marketing Programs |     |     | Programs that are currently interacting with your audience or are currently being built to do so. |
|     |     | Emails |     |     |
|     |     | Events |     |     |
|     |     |     | Live Events / Roadshows |     |
|     |     |     | Trade Shows |     |
|     |     |     | Webinars |     |
|     |     | Newsletters |     |     |
|     |     | Nurture |     |     |
|     |     | Web Content |     |     |
|     |     | Web Forms |     |     |
|     | Program Template Library |     |     |     |
|     | Operational |     |     | This folder is a centralized location for any of your on-going operational programs such as scoring, person source, etc. |
|     |     | Data Management |     | Program with campaigns that normalize data or fix data issues. |
|     |     | Lead Lifecycle |     | Program to track the progress of leads in the funnel. |
|     |     | Scoring |     | Program to score leads on behavior and demographic attributes. |
|     | Sales Insight |     |     |     |
|     |     | Interesting Moments |     | Marketo Interesting Moment Program and Campaigns. |
|     |     | Sales Request |     | Program with Campaigns that sales can add a lead or contact to. |
|     |     | Sales Email |     | Program with Emails that sales can send through Sales Insight. |
|     | \_Archive |     |     | Place where Programs got deactivated reside, after they are no longer interacting with your audience. |
|     |     | \_Learning |     | Place where all Training Exercises would be stored - if you want to keep them. |
|     |     | \_Testing |     | Place where the administrators can test and learn new things and all Test Programs would be stored - if you want to keep them. |
|     |     | \_2022 |     |     |
|     |     | \_2023 |     |     |
| **Design Studio** |     |     |     |     |
|     | Landing Pages |     |     |     |
|     |     | Landing Page Templates |     |     |
|     |     |     | \_Archive | Place for landing page templates that are no longer in use. |
|     |     | Global Landing Pages |     | Place for landing pages that are used in multiple programs or not associated with programs. |
|     |     | \_Archive |     | Place for global landing pages that are no longer in use. |
|     | Forms |     |     |     |
|     |     | Global Forms |     | Place for forms that are used in multiple programs or not associated with programs. |
|     |     | \_Archive |     | Place for global forms that are no longer in use. |
|     | Emails |     |     |     |
|     |     | Email Templates |     |     |
|     |     |     | \_Archive | Place for email templates that are no longer in use |
|     |     | Global Emails |     | Place for emails that are used in multiple programs or not associated with programs |
|     |     | \_Archive |     | Place for global emails that are no longer in use |
|     | Snippets |     |     |     |
|     | Images and Files |     |     |     |
|     |     | Template Graphics |     |     |
|     |     | Logos |     |     |
|     |     | Downloadable Assets |     |     |
|     |     |     | Case Studies |     |
|     |     |     | Product Literature |     |
|     |     |     | Whitepapers |     |
| **Database** |     |     |     |     |
|     | System Smart Lists |     |     |     |
|     | Group Smart Lists |     |     |     |
|     |     | Exclusion Lists |     |     |
|     |     | Operational Lists |     |     |
|     |     |     | Email Deliverability |     |
|     |     | \_Archive |     | Place for Smart Lists that are no longer in use |
|     | Group Lists |     |     |     |
|     |     | Internal Lists |     |     |
|     |     | \_Archive |     | Place for Static Lists that are no longer in use |

### Step 2 - Building folders within the programs

Now, let’s apply the folder structure at the program level. As a best practice, housing the local assets in sub-folders will help you keep the programs tidy and allow internal users to modify or report on the programs efficiently. Common sub-folders include emails, landing pages, Smart Campaigns, Lists, Reports, etc.

>[!NOTE]
>
>**PLEASE READ - we have options here** --> Tables are very problematic and not easy to replicate from MS Word to HTML.  These are 2 options for the below content.  It doesn't appear that this content 'needs' to be in a table and seems to format clearly as a list.  However, if a table is required, I included a compromise table option.  Will use which ever one you prefer.

**Folder Name inside Programs**
* Campaigns - Folder for all campaigns managing interactions and status tracking.
* Local Assets - Folder for all assets that are specific to this Program
  * Emails
  * Landing Pages
  * Smart Campaigns
  * Lists - Only needed when there are Program specific Lists.
  * Forms - Only needed when there are Program specific Forms; most Forms are Global Assets.
  * Reports - Only needed when there are Program specific Reports.

| Folder Name inside Programs | Description |
| --- | --- |
| Campaigns | Folder for all campaigns managing interactions and status tracking. |
|Local Assets | Folder for all assets that are specific to this Program |
|<ul><li>Emails</li><li>Landing Pages</li><li>Smart Campaigns</li><li>Lists - Only needed when there are Program specific Lists.</li><li>Forms - Only needed when there are Program specific Forms; most Forms are Global Assets.</li><li>Reports - Only needed when there are Program specific Reports.</li></ul>| |

>[!NOTE]
>
>**PLEASE READ - we have options here** --> Tables are very problematic and not easy to replicate from MS Word to HTML.  These are 2 options for the above content.  It doesn't appear that this content 'needs' to be in a table and seems to format clearly as a list.  However, if a table is required, I included a compromise table option.  Will use which ever one you prefer.

### Step 3 - Create naming conventions for your programs and assets

Once you have the folder structure in Tree, you will want to name the programs and assets consistently. This is when standardizing naming conventions would be helpful to scale up the naming process internally. Here are a few components that you can use to establish naming convention to ensure searchability:

* Program Type Abbreviation - Email, Content, Nurture, Webinar, etc.
* Category - Type of Program - Standalone Email, Newsletter, etc.
* Dates - Program launch date
* Short Description - Brief description about the Program

Now, let’s put the values into the formula and generate the program names for various program types.

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

Going one level down to naming assets, it’s best that you do not repeat the Program name and use short and generic identifiers for future cloning use. Here are a few quick tips for you to keep in mind:

* Number the assets based on their sequence in the program process.
* Use “-” (hyphen) to separate the naming components instead of “.”(dot) or “\_”(underscore).
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

| **Examples: Downloadable PDF files (DO NOT USE SPACES, avoid underscores "\_")** |
| --- |
| XYZ-Gadget-DS.pdf |
| Acme-Company-CS.pdf |
| How-XYZ-Gadgets-make-life-easier-WP.pdf |

## What’s Next?

* Download the Worksheet: [Marketo Engage Organization and Naming Conventions](https://experienceleague.adobe.com) **LINK TO DOWNLOADABLE FILE** to support the creation of the folder structure and naming conventions.
* Once you determine the necessary components in your standard naming convention, consider building formulas into a Google Sheet or Microsoft Excel. For future use, simply input your values in the spreadsheet to generate your Program names.

### Authors

{{natalie-kremer}}

{{amy-chiu}}