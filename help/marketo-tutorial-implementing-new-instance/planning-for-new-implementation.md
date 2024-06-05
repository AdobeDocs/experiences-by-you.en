---
title: Planning for a new Marketo Engage implementation
description: Learn more about the essential planning and cross-functional team collaboration for successfully implementing a new Marketo Engage instance. This tutorial provides sample milestones, team engagements, and resource allocations for a seamless Marketo Engage implementation.
role: Admin
level: Beginner
doc-type: Article
solution: Marketo Engage
duration: 0
last: substantial-update- 2024-05-01
jira: KT-14808
thumbnail: KT-14808.jpeg
---

# Planning for a new Marketo Engage implementation

Implementing a new Marketo Engage instance involves meticulous planning, collaboration across teams, and continuous optimization. While there's no perfect recipe for implementing a new instance, most Marketo Engage administrators who have gone through it can agree that planning ahead will make the process a lot smoother.

In this tutorial, we will dive into the specific milestones, team engagements, and resource allocations crucial for a successful Marketo Engage rollout.  

## Key milestones during the new Marketo Engage implementation

### Phase 1 - Discovery and planning

- Conducting marketing and sales needs assessment
- Defining objectives or Key Performance Indicators (KPIs)

### Phase 2 - Technical setup and configuration

- Configuring admin settings including CNAMEs and Munchkin Code.
- Configuring lead management processes
- Testing automation workflows and data sync

### Phase 3 - Program library creation and campaign setup

- Developing email templates and landing pages. Starting with [importing starter programs](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program) from the [Program Import Library](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/program-library/program-import-library-overview).
- Setting up Segmentation and Personalization rules
- Creating initial campaigns for lead generation and nurturing

### Phase 4 - Training and user adoption

- Conducting training sessions and/or materials for Users
- Establishing instance governance policies and best practices
- Monitoring user adoption metrics and stakeholders feedback

### Phase 5 - Go-Live and optimization

- Final system testing and quality assurance
- Launching initial campaigns and monitoring performance
- Implementing iterative Improvements based on reporting and analytics

## Stakeholders engagement and resources needed

Implementing a new instance requires careful planning and execution to maximize its benefits. Getting the right stakeholders involved at the beginning will help tailor the implementation to your organization's overall needs. Reference the sample of key stakeholders and their potential role(s) in the project below to help you find the right internal partners to implement Marketo Engage.   

<table>
 <thead>
    <tr>
        <th>Stakeholder</th>
        <th>Potential Role(s) and Responsibilities  </th>
    </tr>
 </thead>    
 <tbody>
    <tr>
        <td>Marketing Operations Director/Manager</td>
        <td>
        <li>Main point-of-contact on project</li>
        <li>Instance governance rules</li> 
        <li>Data analysis for reporting and analytics </li> 
        </td>
    </tr>
    <tr>
        <td>CRM Admin</td>
        <td>
        <li>CRM Sync </li>
        <li>Lead flow</li> 
        </td>
    </tr>
     <tr>
        <td>IT Admin</td>
        <td>
        <li>Munchkin</li>
        <li>SPF/DKIM </li> 
        <li>Web domain setup</li> 
        <li>CNAMEs</li> 
        <li>Email Deliverability</li>
        </td>
    </tr>
    <tr>
        <td>Engineering</td>
        <td>
        <li>Development for custom services integration work </li>
        <li>Data engineering for data mapping and migration</li> 
        </td>
    </tr>
     <tr>
        <td>Marketing </td>
        <td>
        <li>Program templates creation and design</li>
        <li>Channels </li>
        <li>Lead/person scoring and lifecycle</li> 
        <li>Reporting and feedback for program effectiveness</li> 
        </td>
    </tr>
     <tr>
        <td>Sales</td>
        <td>
        <li>Lead/person scoring modeling</li>
        <li>Lead flow/routing</li>  
        <li>Lifecycle Service Level Agreements (SLAs)</li> 
        </td>
    </tr>
     <tr>
        <td>C-Suite</td>
        <td>
        <li>Overall project direction  </li>
        <li>High-level implementation goals</li> 
        </td>
    </tr>
</table>

## Peer perspective - Marketo Engage implementation

Hear Marketo Engage Champion (2019), Kyle McCormick, about his onboarding and implementation experiences at Palotos Networks. You'll learn about the challenges he faced and his advice on how to successfully and efficiently drive your onboarding process.

>[!VIDEO](https://video.tv.adobe.com/v/3428771/?quality=12&learn=on)

## What's Next?

Create a new implementation project plan and timeline. Below is a sample project timeline including sections for sample milestones, tasks, responsible teams, deadlines, and dependencies. Use it to streamline your Marketo Engage implementation journey and ensure a successful rollout across the organization.

You can also download the example for editing and tracking specific milestone tasks [HERE](/help/marketo-tutorial-implementing-new-instance/assets/adobe-marketo-engage-implementation-milestones-project-management-template.xlsx).

<table>
 <thead>
    <tr>
        <th>Topic</th>
        <th>Milestone</th>
        <th>Status</th>
        <th>Anticipated Date</th>
        <th>Actual Date</th>
        <th>Resources Needed</th>
    </tr>
 </thead>    
 <tbody>
    <tr>
        <td><em>Use these general onboarding topics to organize the stages of your milestones.</em></td>
        <td><em>Write out your specific milestone tasks.</em></td>
        <td><em>What is the current status of your task?</em></td>
        <td><em>What is the aniticipated completion date of this task?</em></td>
        <td><em>When was this task actually completed?</em></td>
        <td><em>What resources will you need to complete this task and which team(s) will you need them from?</em></td>
    </tr>
    <tr>
        <td rowspan=2>Technical Setup</td>
        <td><em>EXAMPLE -</em> Install MunchkinID on the company website</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>9/5/24</td>
        <td>9/12/24</td>
        <td>Web Development team</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Set up Domain Keys Identified Mail (DKIM) and 2 separate CNAMEs for deliverability and email tracking links.</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>9/15/24</td>
        <td>9/18/24</td>
        <td>Support and setup from the IT Team</td>
    </tr>
    <tr>
        <td rowspan=4>Adobe Admin Console & Admin Setup</td>
        <td><em>EXAMPLE -</em> Create Marketo Engage users and roles</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Information from marketing teams on who needs access to Marketo Engage.</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Create additional Marketo Engage Product Admin in Adobe Admin Console</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Information from marketing operation team on who needs admin access to Marketo Engage.</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Set up Support Administrators</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>8/27/24</td>
        <td>9/15/24</td>
        <td>Information from marketing operation team to confirm the main contacts for support. Support from System Admin to assign Support Admin users.</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Define folder structure and naming conventions</td>
        <td bgcolor="c6f0cf">Complete</td>
        <td>9/7/24</td>
        <td>9/12/24</td>
        <td>Input from each team using Marketo Engage on program types and organization needs.</td>
    </tr>
    <tr>
        <td rowspan=2>CRM Integration (if apply)</td>
        <td><em>EXAMPLE -</em> Determine field mapping prior to sync</td>
        <td bgcolor="ffeb9c">In Progress</td>
        <td>10/22/24</td>
        <td>N/A</td>
        <td>Support from CRM admin to understand available fields.</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Conduct a data audit</td>
        <td bgcolor="ffeb9c">In Progress</td>
        <td>10/26/24</td>
        <td>N/A</td>
        <td>Support from CRM admin or budget.</td>
    </tr>
    <tr>
        <td rowspan=2>Operational Program Build</td>
        <td><em>EXAMPLE -</em> Create program to standardize incoming data</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>11/9/24</td>
        <td>N/A</td>
        <td>Support from the Sales Ops and CRM teams to determine a data management strategy.</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Create an email subscription center</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>11/19/24</td>
        <td>N/A</td>
        <td>Input from the marketing teams on content types and segmentation for mailing lists.</td>
    <tr>
        <td rowspan=2>First Marketing Program Build</td>
        <td><em>EXAMPLE -</em> Set up basic email program</td>
        <td bgcolor="ffeb9c">In Progress</td>
        <td>11/12/24</td>
        <td>N/A</td>
        <td>Creative assets from digital team for emails and landing pages.</td>
    </tr>
    <tr>    
        <td><em>EXAMPLE -</em> Create program for quarterly newsletter</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>11/30/24</td>
        <td>N/A</td>
        <td>Content from marketing team for newsletter email and creative assets/content from the design team.</td>
    </tr>
    <tr>
        <td rowspan=2>LaunchPoint Integration Setup</td>
        <td><em>EXAMPLE -</em> Create API only user and role</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>11/23/24</td>
        <td>   </td>
        <td>Scope out the services needed for the new instance with the marketing teams.</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Create a custom service for Google Ads</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>12/7/24</td>
        <td>   </td>
        <td>Support from Web and Paid Media teams to authenticate Marketo Engage to access Google Ads.</td>
        <td>
    </tr>
    <tr>
        <td rowspan=2>User Training and Documentation</td>
        <td><em>EXAMPLE -</em> Create a governance guide for internal users</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>12/2/24</td>
        <td>N/A</td>
        <td>Create a Marketo Engage governance team to build supporting governance documentation or budget to contract the governance project out.</td>
    <tr>
        <td><em>EXAMPLE -</em> Train 4 users and provide them with Standard Marketo User access</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>12/13/24</td>
        <td>N/A</td>
        <td>Support from VP of Marketing to make trainings mandatory for access to Marketo Engage.</td>
    <tr>
        <td rowspan=2>Go-Live</td>
        <td><em>EXAMPLE -</em> Send first newsletter</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>12/9/24</td>
        <td>N/A</td>
        <td>Marketing Operations team to QA, schedule, and send.</td>
    </tr>
    <tr>
        <td><em>EXAMPLE -</em> Pull the first Email Performance Report.</td>
        <td bgcolor="ffc7cf">Not Started</td>
        <td>12/16/24</td>
        <td>N/A</td>
        <td>Marketing Operations team to QA, schedule, and send.</td>
    </tr>
 </tbody>    
</table>

>[!NOTE]
>Examples provided are not based on a real implementation timeline. Do not rely on these as a standard timeline for your onboarding with Marketo Engage, as every implementation is unique with different milestones and requirements according to your organization's needs.

For hand-in-hand assistance in implementing and customizing your Marketo Engage for your instance, please contact the Adobe Account Team or reach out to [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}. 

### Author

{{amy-chiu}}
