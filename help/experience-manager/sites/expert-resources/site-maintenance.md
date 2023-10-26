---
title: Your Routine Site Maintenance Guide
description: Whether you're an admin, author, or developer, site maintenance touches every aspect of your AEM Sites instance. Use this guide to ensure your strategy is set up for success.
role: Admin
level: Beginner, Intermediate
topic: Administration
audience: author, marketer, developer
feature: Learn From Your Peers
---
# Site Maintenance Tips and Tricks

There are three options when it comes to installing and maintaining an AEM instance 

* AEMaaCS (cloud service) - the system is always on, up to date, and scales dynamically as you need it
* Adobe Managed Services where Adobe Customer Service Engineers do all the daily/weekly/monthly maintenance and ensure all service packs are installed and the system is always secure and running smoothly
* running it on-premises, where you have to take care of the entire system, including backups, upgrades, and security.

If you choose to implement your own system on-premises, here are a few things to keep in mind to ensure you have a secure, performant system. In addition to the "care and feeding" items, this paper will also point out several items AEM Developers ought to keep in mind to assist in keeping the system running well.

## Admins

Backups - ensure you have complete and/or partial backups on a frequent schedule:

* daily
* weekly
* monthly

Many customers do snapshot backups, which only take a few minutes assuming the underlying operating system supports such backups. Make sure these backups are stored properly (off the AEM system). Ensure the backups are functional and can be used to recreate a working system periodically - there's nothing worse than having the system crash and your backups are corrupt for some reason!

There are several items you need to monitor to ensure trouble-free operation:

### Routine Maintenance

#### [index maintenance](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/practices/best-practices-for-queries-and-indexing.html?lang=en)

Indexes allow queries to run as quickly as they can, freeing up resources for other operations. Ensure your indexes are in tip-top shape! AEM cancels queries that travere instead of using an index to keep one bad query from affecting overall AEM performance.

#### [Tar Compaction/ Revision cleanup](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/deploying/revision-cleanup.html?lang=en)

Each update to the repository creates a new content revision. As a result, with each update the size of the repository grows. To avoid uncontrolled repository growth, old revisions need to be cleaned up to free disk resources.

#### [Lucene binaries cleanup](https://experienceleague.adobe.com/docs/experience-manager-65/administering/operations/operations-dashboard.html#automated-maintenance-tasks)

Purge lucene binaries and reduce the running data store size requirement.

#### [Data Store Garbage](https://experienceleague.adobe.com/docs/experience-manager-65/administering/operations/data-store-garbage-collection.html)

When an asset in AEM is deleted, the reference to the underlying data store record may be removed from the node hierarchy, but the data store record itself remains. This unreferenced data store record becomes "garbage" that need not be retained. In instances where a number of unreferenced assets exist, it is beneficial to get rid of them to, preserve space, optimize backup, and filesystem maintenance performance.

#### [Workflow Purge](https://experienceleague.adobe.com/docs/experience-manager-65/administering/operations/workflows-administering.html)

Minimizing the number of workflow instances increases the performance of the workflow engine, so you can regularly purge completed or running workflow instances from the repository.

#### [Audit Log Maintenance](https://experienceleague.adobe.com/docs/experience-manager-65/administering/operations/operations-audit-log.html

AEM events that qualify for audit logging generate a lot of archived data. This data can quickly grow over time due to replications, asset uploads and other system activities.

#### [Security](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security-checklist.html?lang=en)

Ensure the Security Checklist best practices are followed closely to ensure the most secure instance of AEM.

#### Diskspace

Monitor diskspace to ensure you have enough for the JCR Repository, plus about half again as much space - the tar compaction uses extra space when it runs. Running out of diskspace is the number one reason for JCR corruption!

## Developer

Try not to use custom components - use [core components](https://www.aemcomponents.dev/). Your goal should be to use core components 80-90% of the time and custom components only sparingly. This often requires a new way of looking at the components on a page - you must realize the components can be restyled easily by a front-end developer using CSS. Also keep in mind that those core components can be embedded in each other to achieve quite complex results. Get creative!

### [Style Systems](https://experienceleague.adobe.com/docs/experience-manager-65/authoring/siteandpage/style-system.html?lang=en)

Style systems allow the core components, and even custom components, to have their look and feel change at the Authors discretion to create completely new looking components. These stylistic changes generally only involve a front-end designer and a knowledgeable author (often referred to a 'Super Author')

### [Launches](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/launches/overview.html?lang=en) 

Launches allow for work to be completed for a new Promotion, Sale, or website rollout without impacting the currently deployed pages. In addition, they can be scheduled to go live automatically, without attendance or supervision, allowing Authors to do next week's (or next quarter's) work today and not rush into page development the day before it should go live - it's truly the gift of TIME!)

### [Content Fragments](https://experienceleague.adobe.com/docs/experience-manager-65/assets/fragments/content-fragments.html)

Content fragments are customizable "chunks" of information that can be easily reused all over the site. If you need a change you just change the original chunk and the update is seen everywhere it's used - immediately!

### [Experience Fragments](https://experienceleague.adobe.com/docs/experience-manager-learn/sites/experience-fragments/experience-fragments-feature-video-use.html?lang=en)

While sounding almost identical to Content Fragments, Experience Fragments are small, visible, pieces of a page. These can also be reused widely across your site and maintained in a central location within AEM to ease the task of making potentially global changes across your site in seconds, not days or weeks.

Think ahead and see what might be reused. A footer? A disclaimer? A Header? Certain types of content? All these can be shared across an entire site while keeping maintenance at a minimum. Need to update a date in a disclaimer, but it's on 1,000 pages on your site? It's a 5 second operation if you used an Experience Fragment!

## General

Stay abreast of changes AEM through continued learning - don't get stuck in the past. Use [Experience League](https://experienceleague.adobe.com/docs/experience-manager-learn/sites/overview.html?lang=en) and [Adobe Digital Learning Services (ADLS)](https://learning.adobe.com/) to hone your skills.

## Conclusion

AEM can be a large system, and it takes many types of people to make it "sing". From Admins to Developers (both front-end and hardcore Java developers) to Authors - there's something for everyone! And if you don't feel like handling the day to day Administration, there's always AMS and AEM as a Cloud Service.
