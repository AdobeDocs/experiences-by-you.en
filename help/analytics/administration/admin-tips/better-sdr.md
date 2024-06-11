---
title: Building Data Culture and a Better Solution Design Reference
description: Revolutionize your data strategy and empower your team to create a solid Solution Design Reference (SDR) document. Eliminate measurement gaps and foster a collaborative data culture through step-by-step methodologies.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25
jira: KT-15338
thumbnail: KT-15338.jpeg
exl-id: 99fcf68f-5698-4270-9055-ab224e6323a1
---
# Building data culture and a better solution design reference

_Revolutionize your data strategy and empower your team to create a solid Solution Design Reference (SDR) document. Eliminate measurement gaps and foster a collaborative data culture through step-by-step methodologies._

It's finally time. You put together a solid SDR. An SDR is the guide that you use to implement your metrics and dimensions. You've defined what they're called, when they fire, and your developers love it. You went through the entire process of deployment, wrote acceptance criteria, went through your sprints, tested it, and it's done! Your instance of [!DNL Adobe Analytics] should be getting marketing and product teams celebrating as they dig into the data, get new revelations about your customers, and find all the areas of success and, well, areas of less success. But you're not hearing the accolades that you were expecting. 

From one team, you hear complaints like:

"Why can't I figure out the conversion rate on this funnel?"

"Why isn't there a metric for this?"

"I need more detail! A metric alone isn't enough. There are at least three different dimensions that I need to understand performance. Why didn't you put them in?"

But it's the other team that's an even bigger cause of concern. From them, you don't hear anything at all. Worse, you see charts that were clearly taken from your old analytics solution (the one that's no longer maintained, and every day is falling further into a swamp of decrepitude and dirty data). A sense of dread fills you as you consider the decisions that might be made with that original mess. 

_What went wrong?_ 

_Why are there gaps in measurement?_ 

_Why aren't your team members embracing this?_

I'll start by letting you off the hook slightly. There's _always_ going to be some revision. If your site or application is complex enough to need an enterprise analytics solution, it's guaranteed that you will miss something. But in this case, you did not miss enough to explain the measurement gaps I'm describing. 

What went wrong is a lot harder to put into a spreadsheet. Essentially, you missed out on your first chance to build a collaborative data culture while you built your SDR. 

I want to walk you through a method that my colleagues and I developed to both build a better SDR with fewer gaps, and to get end users invested (and even occasionally excited) about their new instance of [!DNL Adobe Analytics]. Let's go over how and why you should consider this method.

## The how

_Learn about the measurement conference. Use a funnel map to visualize each step of your plan. Create mock dashboards to review as a group. Create a data dictionary for users._

### The measurement conference

1. Get your stakeholders together, either in person or virtually, with the goal of finding out what to measure. This meeting should include some executives.
1. Have obvious examples already on the board on sticky notes, such as revenue, sales, or leads, the core key product indicators (KPIs) you know will be measured. Repeat with dimensions like logged-in state, product categories, or search terms.
1. Have everyone add their own sticky notes, grouping as necessary.
1. Ask people to vote on the ones that they think are important. These are unlimited votes because all of these metrics and dimensions probably matter.
1. For any metrics and dimensions that have low votes, have the stakeholders who asked for them explain why these components would be used. If there's a good use case, keep these components. If there is a better way of getting that data, or nobody can explain how these data are actionable, or if there's another good reason to remove the metrics and dimensions, do so.
1. Add these metrics and dimensions to your SDR for an initial review by the stakeholders who were present.

### The funnel map

1. Get a visualization of all the funnels, step by step with every state included.
1. With the designers and product managers, go through each step and discuss what everyone considers success in that funnel. Is it the conversion rate? Is it choosing a particular path? Is it using certain features?
1. Ask questions about what metrics and dimensions are necessary to understand funnel performance on each step of the funnel and overall.
1. Above each step of the funnel, add the metrics and dimensions that are measured on that step, including the calculated metrics.
1. At the beginning of each funnel, write out the reports that go in the dashboard that the product manager can use to track performance. These reports include a [fallout report](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/fallout/fallout-flow), [current month](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/components/calendar-date-ranges/custom-date-ranges), [trended conversion rates](https://experienceleague.adobe.com/en/docs/analytics/analyze/analysis-workspace/visualizations/line), and anything more specific to that funnel.
1. Add the new metrics and dimensions you've discovered to the SDR and send it to the stakeholders for a second review.

### The preview dashboards

1. Using the funnel map as a guide, create mockup dashboards.
1. There should be an overall view, such as an [Executive Summary Dashboard](driving-success-with-executive-summary-dashboards.md), and dashboards for each of the funnels.
1. There will also be some more specific to your site or app, such as product performance or content performance.
1. Distribute these to the relevant stakeholders and get feedback on the design.
1. Make any updates requested and if new metrics or dimensions are needed, add them to your SDR.
1. Send out the updated preview dashboards and SDR for a final review.

### Data democratization tools

1. Create a data dictionary. The SDR is for your developers, but the data dictionary is for your end users. Make it readable so that everyone can easily look up what data is available and know how to use it. Your end users should be the final approvers of this.
1. Annotate. In every organization, there are certain dates that matter every year and others that will come up. Ensure that you gather the relevant dates from your stakeholders and add them in as annotations to increase the understanding of the data they see. 
1. Curate. If your SDR is big, it might be overwhelming. Paralysis of choice doesn't just apply to your clients. See what matters to each group of users and curate the elements they'll see.

## The why

_Learn about gathering requirements, building a data culture, sparking deep thought about data, creating a sense of ownership about the data, and simplifying the data._

### Gather requirements

Gathering requirements is an obvious one, but there are several effective ways of doing it. I've used one-on-one interviews, questionnaires, and reviews of existing reports. Those strategies work, but not as well as the methods I just outlined. however, I don't think that the difference between the methods for requirements gathering is significant. The method I've described gets you 95% of the way there, and these other methods get you 90% of the way. 

So, what is the _why_?

### Build data culture

Ih this process, you:

* Spark deep thought about how to measure success
* Create a sense of ownership in your stakeholders
* Make it easier for stakeholders to understand their data

### Spark deep thought about data

For many of the people at your company, data is something they consume. They use it. They analyze it. They don't think deeply about it. Some people inherited reports and processes from their predecessors but have not altered them for continuity's sake. Perhaps these people never needed to think about the _why_ of the data.

This process gives them an opportunity to really _understand_ data. Asking questions like, What is success? How would you know if you were successful? How would you know what to change if you weren't successful? These questions must be answered at the beginning of creating every site, application, and product--but far too often they aren't. By asking these questions, you help deepen a person's understanding of not only the data, but also their product.

### Create a sense of ownership over the data

A sense of ownership is not something that a person easily acquires. It's not found in that thirty-minute meeting the attended three months ago. It's not created by that an annoying questionnaire they answered too quickly because of other pressing work issues like demos and sprint release dates. 

Ownership is the product of someone's deep thought and their work with you and colleagues. It's the thing they've looked over several times, provided ongoing feedback for, and what they've approved after that feedback was incorporated. It's theirs! The fact that it's useful is due to them. It's _their_ data and it's that process that made it theirs.

### Simplify the data

You've also shown them how they'll use the process and what it will look like through the [preview dashboards](#the-preview-dashboards). Any new solution is _hard_. There's so much to learn, and given the tremendous customizability of [!DNL Adobe Analytics], the learning curve can be steep. You've removed 80% of that though. Even before the first line of code has been written, your stakeholders know what their dashboards will look like. They'll know how to read them and get meaning from them. They'll know what success literally looks like because they've told you what metrics and dimensions define success. And, you've told them how that success will be visualized for them. The delivery of the actual dashboards is a refresher, not a scary new learning task. 

This isn't necessarily the quickest way of getting an SDR together. It's a lot of work and requires a lot of coordination of schedules, especially since it's vital you have some executives in the mix. In the end, though, an enterprise analytics solution is a huge investment of time and money, and you want to make sure adoption and satisfaction are high. This method goes a long way toward making that happen.

**Author**

This document was written by: 

![gitai-headshot](assets/gitai-headshot-150.jpg)

Gitai Ben-Ammi, Business Architecture Associate Manager at Accenture

[!DNL Adobe Analytics] Champion
