---
title: Building data culture and a better solution design reference
description: Revolutionize your data strategy and empower your team to create a solid Solution Design Reference (SDR) document. Eliminate measurement gaps and foster a collaborative data culture through step-by-step methodologies.
feature: Implementation Basics
topic: Administration
role: User
level: Experienced
doc-type: Article
duration: 72000
last-substantial-update: 2024-04-25
jira: KT-15338thumbnail: KT-15338.jpeg
---

# Building data culture and a better solution design reference

**Revolutionize your data strategy and empower your team to create a solid solution design reference (SDR) document. Eliminate measurement gaps and foster a collaborative data culture through step-by-step methodologies.**

It's finally time. You put together a solid Solution Design Reference (SDR). This is the guide you use to implement your metrics and dimensions, what they're called, when they fire, and your devs loved it. You went through the entire process of deployment, writing acceptance criteria, going through your sprints, QAing the entire thing, and it's done! It was a lot of work, and now it's done. Your instance of Adobe Analytics should be getting marketing and product jumping up and down as they dig into the data, get new revelations about your customers, and find all the areas of success and, well, areas of less success. But you're not hearing the accolades you were expecting. 

From one camp, you hear complaints.

"Why can't I figure out the conversion rate on this funnel?"

"Why isn't there a metric for this?"

"I need way more detail about this! A metric alone isn't enough. There are at least three different dimensions I need to understand performance. Why didn't you put them in?"

But it's the other camp that's an even bigger cause of concern. From them, you don't hear anything at all. But much worse, you see charts that were very clearly taken from your old analytics solution, you know, the one that's no longer being maintained, and every day is falling further into a swamp of decrepitude and dirty data. A sense of dread fills you as you think about the decisions that might be made with that mess.

What went wrong? Why are there gaps in measurement? Why aren't your team members embracing this?

I'll start by letting you off the hook a little bit. There's *always* going to be some revision. If your site or app is complex enough to need an enterprise analytics solution, it's basically guaranteed that you'll miss something. But not enough to explain the measurement gaps I'm talking about here. What went wrong is a lot harder to put into a spreadsheet. You missed out on your first chances to build a collaborative data culture at the same time you built your SDR. I want to walk you through a method that I and my colleagues have developed to both build a better SDR with fewer gaps, and to get end users invested and even occasionally excited about their new instance of Adobe Analytics. Let's go over the hows and the whys.

**The How**

***The Measurement Conference:***

1. Get your stakeholders together, either in person or virtually with the goal of finding out what to measure. This should include some execs.
1. Have some obvious examples on the board on sticky notes already, things like revenue, sales, or leads, the very core KPIs you know will be measured. Repeat with dimensions, things like logged in state, product categories, or search terms.
1. Have everyone add their own sticky notes, grouping as necessary
1. Have people vote on the ones that they think are important. These are unlimited votes since maybe all of these metrics and dimensions matter.
1. For any that have low votes, have the stakeholders who asked for them explain what they'll use them for. If there's a good use case, keep it in. If there's a better way of getting that data, they can't explain how it's actionable, or there's another good reason to leave it out, strike it from the board.
1. Add these metrics and dimensions to your SDR for an initial review by the stakeholders who were present

***The Funnel Map***

1. Get a visualization of all the funnels, step by step with every state included
1. With the designers and product managers, go through each step and talk through what they consider success on that funnel. Is it conversion rate? Is it choosing a particular path? Is it using certain features?
1. Ask questions about what metrics and dimensions are necessary to understand funnel performance on each step of the funnel and overall.
1. Above each step of the funnel, add the metrics and dimensions that will be measured on that step, including the calculated metrics.
1. At the beginning of each funnel, write out the reports that will go in the dashboard that the product manager will use to track performance, things like a fallout report, current month and trended conversion rates, and anything more specific to that funnel.
1. Add the new metrics and dimensions you've discovered to the SDR and send it to the stakeholders for a second review.

***The Preview Dashboards***

1. Using the Funnel Map as a guide, create mockup dashboards.
1. There should be an overall view, such as an Executive Summary Dashboard, and dashboards for each of the funnels.
1. There will also be some more specific to your site or app, such as product performance or content performance.
1. Distribute these to the relevant stakeholders and get feedback on the design.
1. Make any updates requested and if new metrics or dimensions are needed, add them to your SDR.
1. Send out the updated preview dashboards and SDR for a final review.

***Data Democratization Tools***

1. Create a Data Dictionary. The SDR is for your devs. The Data Dictionary is for your end users. Make it readable for end users so they can easily look up what data is available and know how to use it. Your end users should be the final approvers of this.
1. Annotations. In every organization, there are certain dates that matter every year and others that will come up. Make sure that you gather the relevant ones from your stakeholders and add them in as annotations to increase the understanding of the data they see. 
1. Curation. If your SDR is big, it might be overwhelming. Paralysis of choice doesn't just apply to your clients. See what matters to each group of users and curate the elements they'll see.

**The Why**

***To Get Requirements***

This is an obvious one but there are other effective ways of getting requirements. I've personally used one on one interviews, questionnaires, and reviews of existing reports. Those will work, though I think not as well as the methods I've just outlined. I honestly don't think the gap in requirements gathering is that big though. The method I've described will get you 95% of the way there, and these other methods will get you 90% of the way. So, what's the big why?

***To Build Data Culture***

With this process, you:

- Spark deep thought about how to measure success
- Create a sense of ownership in your stakeholders
- Make it easier for stakeholders to understand their data

***Sparking Deep Thought about Data***

For many of the people at your company, data is something they consume. They use it. They analyze it. They don't think deeply about it. Some of them inherited reports and processes from their predecessors they have not altered because of the need for continuity. They've never needed to think about the why of the data.

This process gives them an opportunity to really *understand* data. Asking the questions, what is success? How would you know if you were successful? How would you know what to change if you weren't successful? This is an exercise that should be done at the beginning of creating every site, app, and product, but far too often is not. By asking these questions, you help deepen their understanding of not only the data, but also their own product.

***Creating a Sense of Ownership over the Data***

This is not something that was handed down from on high. This is not something that was a thirty-minute meeting three months ago. This is not that annoying questionnaire that they were hounded for a week to answer and that they did so in a hurry because they had a demo to get to so they could make the sprint release date. This is the product of their deep thought and their work with you and their colleagues, the thing they've looked over several times, provided ongoing feedback for, and that they've approved after that feedback was incorporated. It's theirs! The fact that it's useful is due to them. It's *their* data and it's the process that made it theirs.

***Making the Data Easier to Understand***

You've also shown them how they'll use it and what it will look like through the preview dashboards. Any new solution is *hard*. There's so much to learn and given the tremendous customizability of Adobe Analytics, the learning curve can be quite steep. You've removed 80% of that though. Even before the first line of code has been written, your stakeholders know what their dashboards will look like. They'll know how to read them and get meaning from them. They'll know what success literally looks like because they've told you what metrics and dimensions define success, and you've told them how that will be visualized for them. The delivery of the actual dashboards is a refresher, not a scary new learning task. 

This isn't the quickest way of getting an SDR together. It's a lot of work and requires a lot of coordination of schedules, especially since it's vital you have some execs in the mix. In the end though, an enterprise analytics solution is a huge investment of time and money, and you want to make sure adoption and satisfaction are high. This method goes a long way toward making that happen.

**Author**

This document was written by: 

![gitai-headshot](assets/gitai-headshot.png)

Gitai Ben-Ammi, Business Architecture Associate Manager at Accenture

Adobe Analytics Champion


