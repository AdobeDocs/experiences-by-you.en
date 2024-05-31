---
title: Designing omnichannel conversational marketing with Dynamic Chat
description: Get a quick start to design conversational marketing with Adobe Dynamic Chat, the native conversational engagement channel within Adobe Marketo Engage. This tutorial offers actionable recipes to implement use cases such as sales meeting booking, website content engagement, and events/webinar promotion.
role: Admin
level: Beginner
doc-type: Article
duration: 0
last-substantial-update: 2024-05-23
jira: KT-14814
---

# Designing omnichannel conversational marketing with Dynamic Chat

Marketers, your website is essential for generating leads, boosting conversions, and accelerating sales cycles. Engaging with visitors in real-time on your website allows your sales team to qualify buyers more efficiently. Adobe Dynamic Chat, the native chat channel within your Adobe Marketo Engage subscription, enables you to automate conversations to extend Marketo Engage's capabilities. 

This tutorial outlines the thought process and primary use cases shared by Sara Barriuso, Marketing Operations Manager at Cornerstone OnDemand, during the "Learn from Your Peers". She explained how her organization used Dynamic Chat to maximize Marketo Engage's capabilities. 

## Integrating conversational engagement in your demand generation strategy 

Visitors browse your website for a reason. They might be seeking content on your product(s) or service(s) or looking for contact information to speak to your sales representatives. They could also be your customers looking for additional product information. Chat enables your website visitors to self-serve and self-qualify if they are ready to speak to your sales team.  

When Sara Barriuso implemented Dynamic Chat, she was drawn by its seamless integration with Marketo Engage and the [prebuilt activity triggers](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-activities){target ="_blank"} that activate Marketo Engage programs and vice versa. She developed her conversational engagement strategies with three audience segments in mind:  

1. Unknown prospects: proactively offer demo calls to generate new leads.
2. Known leads/customers: extend visitors' time spent browsing content and offer demo calls to generate upsell and cross-sell opportunities.
3. Prospects/customers: provide personalized experiences by extending the efforts of marketing campaigns.  


## Key use cases to start building your Dialogues  

To implement these strategies, Sara built her Dynamic Chat Dialogues around the following use cases:  

1. Default Catch-all Dialogue: give an initial option to all visitors, guiding them to accomplish their tasks more efficiently.  

2. Promoting event and webinar registration: drive website visitors to register for events and webinars to funnel them into the buying stage more quickly. 

3. Extending campaign content engagement: offer additional context or address potential questions when visitors browse content on the website. 

Let's see these use cases in action as Sara showcases her process, from mapping out the conversational flow to configuring the Dialogues and targeting in Dynamic Chat and Marketo Engage. 

### Use case 1: Default catch-all Dialogue for all site visitors 

This Dialogue provides five initial options for site visitors to choose from, creating a self-guided experience that helps them find the information they need based on their persona. To start, you might want to explore your 'Contact Us' email inbox to identify common themes and categorize them into Dialogue options that apply to your site visitors. Watch the demo and follow the steps below to create your default catch-all Dialogue:  

>[!VIDEO](https://video.tv.adobe.com/v/3429194/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

1. Build the Dialogue and create a testing link. 
2. Add a goal to track the conversions (e.g. demo request submission).
3. Have 2-3 people test it and collect feedback. 

#### Phase 2

1. In "Audience", add a web page URL in "Target" to indicate where the Dialogue will show up. 
2. In "Settings", add the campaign name, description, priority, and language. 
3. Click "Publish"

>[!TAB Marketo Engage]

#### Phase 1

1. Create your tracking Smart Campaign.
2. In "Smart List", use a "Reaches Dialogue Goal" trigger. Use the same goal (e.g. Demo Request) you used Dialogue
3. In "Flow", include a "Change Program Status" step to track conversion. 
4. The source will show as 'dynamicChat'. You can create a Smart Campaign to update the source to a name that makes sense to you. 

#### Phase 2

1. Re-test your tracking Smart Campaign when it is live. 

>[!ENDTABS]

#### Level up: Account-based marketing 

You can further enhance the default catch-all Dialogue by incorporating industry-targeted content, making the conversations even more useful for visitors. For example, suggest industry-specific whitepapers or case studies for your visitors to download. Watch the demo and follow the steps below to create a default catch-all Dialogue for account-based marketing:

>[!VIDEO](https://video.tv.adobe.com/v/3429195/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Clone the "default Dialogue" and rename it. 
2. In "Stream Designer", adapt Dialogue messages to the target industry (only one stream + the initial question).
3. Have 2-3 people test the Dialogue and collect feedback.
4. Create a testing link and share it.
5. In "Audience", add a web page URL where the Dialogue will display and update the target to the industry you want.
6. In "Settings", add the campaign name, description priority, and language.
7. Click "Publish". 

>[!TAB Marketo Engage]

1. Create your tracking Smart Campaign and test the goal.
2. Re-test the tracking Smart Campaign after publishing the Dialogue. 

>[!ENDTABS]

### Use case 2: Promoting event and webinar registration 

Events and webinars are popular marketing tactics for B2B businesses to generate demand. They offer engaging experiences and rich information that attract prospective customers. Connecting your website visitors to upcoming events and webinars enables you to qualify prospective customers even faster. Creating this Dialogue is low effort and low cost, and can quickly demonstrate success, helping you gain support from marketing stakeholders to add conversational engagement to your omnichannel automation plan. Watch the demo and follow the steps below to create your event/webinar promotion Dialogue:

>[!VIDEO](https://video.tv.adobe.com/v/3429196/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

#### Phase 1

Build a template for "event registration" Dialogue for ongoing campaign use. 

#### Phase 2

1. Clone the template.
2. Copy and paste text to the Dialogue message for a new event
3. Update UTM parameters used in your event link (e.g. utm_medium=website&utm_source=adobe). 
4. Create a testing link, click "Publish", and share it with the requestor.
5. Peer review and apply feedback. 


>[!TAB Marketo Engage]

#### Phase 1

1. Create your tracking Smart Campaign within the webinar/event program template and test it.

#### Phase 2

1. Add your campaign name to the tracking Smart Campaign within Marketo Engage and test it. 

>[!ENDTABS]


#### Level up: Register known people  

You can offer an even better experience to website visitors by registering them for your events and webinars without having them fill out a form. Personalized experiences build trust and show visitors that you remember them. Let's see how to level up your event and webinar promotion Dialogue in action.

>[!NOTE]
>Please consider the potential security risk involved in certain protective states/countries and implement this personalization carefully by consulting with your Legal team. 

>[!VIDEO](https://video.tv.adobe.com/v/3429197/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Clone the Event/Webinar promotion Dialogue.
2. In Stream Designer, after the user answers "Yes", add a question card "Is this your email address?"
3. If they answer "Yes" – add a message card "You will receive a confirmation email in your email with the event/webinar details". 
4. If they answer "No" –  add a message card "Please fill out the form on the registration page". 
5. Create a testing link, click "Publish", and share it with the requestor. 
6. In the Audience tab, add [email is not empty]. 


>[!TAB Marketo Engage]

1. Add this new Dialogue to the tracking Smart Campaign within Marketo Engage and test it. 

>[!ENDTABS]

### Use case 3: Extending campaign content engagement 

Imagine a captivating window display catches your eye and draws you into a store. If a receptionist then helps you select products or answers your questions, you might feel more comfortable making a purchase. To replicate this experience online, you can have your Dynamic Chat dialogue appear on the web pages where your marketing campaigns direct visitors. As users engage with the web content, Dynamic Chat immediately displays relevant conversations, suggesting additional content or addressing potential questions. This is achieved by leveraging automation triggers to activate Dynamic Chat campaigns based on user engagement within Marketo Engage programs. Now, let's see how to bring this use case to life.

>[!VIDEO](https://video.tv.adobe.com/v/3429199/?learn=on)

Extending Campaign Content Engagement - Configuration:

>[!VIDEO](https://video.tv.adobe.com/v/3429200/?learn=on)

>[!BEGINTABS]

>[!TAB Dynamic Chat]

1. Generate new leads for your campaigns via email and social campaigns' touchpoints. In this example, the Talent health index survey is hosted on the brand's website.
2. Clone an existing Dialogue template (e.g. default catch-all Dialogue) to create three Dialogues for the following scenarios and update the "Target URL" in the 'Audience' tab accordingly:
   * When web visitors came from your marketing channels and land on your webpage.
   * On the thank you page
   * Any visitors who return to your website within 45 days of engaging in the marketing campaign (retargeting)

>[!ENDTABS]

## What's Next? 

* Map out your conversational flow in [Stream Designer](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer){target ="_blank"} or a flow chart offline.
* Create a default catch-all Dialogue in Dynamic Chat. 
* Activate the conversations post-campaign engagement by using automation triggers in Marketo Engage.


## Authors

{{sara-barriuso}}

{{amy-chiu}}