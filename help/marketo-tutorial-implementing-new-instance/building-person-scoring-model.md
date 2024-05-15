---
title: Building person scoring models for Marketo Engage programs
description: Adobe Marketo Engage allows you to build your scoring model(s) from the ground up. Before you jump right in Marketo Engage to build your scoring programs, you will have to set up the essential score fields such as Demographic Score, Behavioral Score, and Total Person Score. Learn more about the strategies used by Marketo Engage Champions for developing Scoring Models that your business needs.
role: Admin
level: Beginner
doc-type: Article
duration: 0
last-substantial-update: 2024-05-04
jira: KT-14810
thumbnail: KT-14810.jpeg
---
# Building a person scoring model

Person scoring helps you identify the people who are most engaged with your company and are your Ideal Customer Profile so that you can share those leads with your sales team and close deals! Together with sales, you determine which leads you want to hand off to them by using a lead/person scoring program in Adobe Marketo Engage. This can either be determined by a minimum of behavioral scoring, demographic scoring, or both.

In this tutorial, we will walk you through three exercises suggested by Marketo Engage Champions Christina Zuniga and Katja Keesom. Follow along to determine which activities and characteristics are important indicators that a prospect is interested in purchasing (behavioral scoring) and is the right fit for you (demographic scoring), and account for the nuances across markets.

## Why develop and use a person scoring model?

You may have many leads in your database, but how do you know which ones are ready to buy your products and services now? As your marketing organization seeks to optimize lead quality and sales readiness, this is where the scoring model comes into play.

By scoring people in your Marketo Engage database, you can measure how qualified your generated leads are and set criteria for when they are sales-ready. That allows your sales team to focus on the leads that are most likely to close while the marketing team continues to nurture the other people in the database via their marketing programs.

## Exercise 1 - Determining Buyer Interest with Behavioral Scores

Behavioral scoring is giving a numerical value to trackable actions a prospect takes that indicate interest in your products and services and intent to buy. For example, visiting the website shows interest, and visiting the pricing page may show intent. In contrast, visiting the careers page may indicate the person is not going to purchase.

**Step 1** - Make a list of prospect activities that matter to your sales process or are valuable to your organization. It can be helpful to work with your sales team to determine which activities indicate a lead has the intent to purchase, helping you align the criteria with sales and prioritize based on their observations of closed deals. Here are a few suggested questions that you can ask your sales team:

* Which activities indicate a good or bad lead to you?
* What type of content consumed by a lead has a stronger intent to purchase?

**Step 2** - List actions that indicate a prospect is not interested in your product. Be sure to list activities that are trackable through Marketo Engage.

**Example 1a - Activities indicating intent to buy**

| **Activities indicating intent to buy** | **Activities indicating NO intent to buy** |
| --- | --- |
| Visit pricing page | No interaction in last 90 days |
| Attend annual customer event | Visit careers page |
| Register for webinar | Unsubscribes |
| Download white paper |     |
| Fill out request demo form |     |

**Step 3** - Analyze and choose a sales handoff threshold score.

* Once a lead indicates enough interest by performing some of the activities you defined in Step 1 and the total score surpasses this threshold, you will hand them off to sales. This threshold will simply be a number that helps set a benchmark for the scores you assign to individual behaviors.
* Your threshold number should be large enough so that a person needs to complete multiple interactions with your brand to meet it. For example, one email open is unlikely to be a sufficient qualifier. If you just started, try working with a threshold of 100 and building out your person scoring from there.
* Setting a high or low threshold depends on which leads your sales team is most interested in receiving and developing into business opportunities. If you have any existing data about your recent sales deals, analyze it and see what actions people took in successful deals. This can help you to determine how many touch points go into a qualified sales lead and help you extrapolate from there what your threshold number should be.

**Example 1b – Threshold for sales handoff:**

| Average number of touchpoints for qualified lead | 4   |
| --- | --- |
| Threshold for sales handoff | 50  |

**Step 4** - Assign a score to each activity listed in ‘Example 1a - Activities indicating intent to buy’.

* Use a positive behavior score for the activities that indicate interest to boost a prospect’s overall lead score, and a negative score to indicate disinterest.
* Using your threshold from ‘Example 1b – Threshold for sales handoff’ as a benchmark, determine your behavior scores relative to the importance of their actions. For example, prospects who request a demo should go straight to sales. Assigning that action a point value equal to your prospect handoff threshold will make the most sense. Meanwhile, downloading a white paper is not as strong an indicator of buying interest and therefore should be worth fewer points.

**Example 1c – Scoring activities indicating intent to buy:**

| Threshold for sales handoff = 50 points |     |
| --- | --- |
| Activity | Score |
| Filled out “request a demo form” | +50 |
| No interaction in last 90 days | \-10 |
| Download a white paper | +5  |
| Visit us at a tradeshow | +15 |

**Step 5** - Remember, scoring is an iterative process! Continuously review and adjust scores and thresholds as you gather more data for analysis.

## Exercise 2 - Identifying the right fit with Demographic Scores

Now that you have defined the activities indicating buying intent, you should complete the scoring model with your Ideal Prospect Profiles. To identify whether a prospect is the right fit for further sales conversation, it’s important to assign demographic scores in addition to behavioral scores so that the model helps determine the best leads in terms of fit and intent.

**Step 1** - Make a list of characteristics for your ideal prospects.

* Consider listing attributes such as their industry, company, department, and role. Be sure that these characteristics correspond to available demographic fields in your Marketo Engage instance.
* Work with your sales team to determine which leads respond most to sales inquiries and are key contacts during sales opportunities.
  * It can be helpful to analyze recent closed won opportunities to see what characteristics your best customers have. For example,
    * Digging through closed lost opportunities for patterns can lead you to find demographic data you want to avoid.
    * Identify decision-makers and internal champions that drive your selling efforts. Deep dive into the data and bring your findings to a workshop with some of your sales team to validate or refine your conclusions.
  * You can also interview your sales team with the following sample questions:
    * Which department are they usually engaging with?
    * What are the job titles of the people involved in product demos and who are the people that need to sign off on the purchase?

**Example 2a – Ideal prospect characteristics**

| **Category** | **Ideal Prospect Characteristics** |
| --- | --- |
| Industry | Aerospace, Manufacturing |
| Company size | 100 – 999, 1,000 – 9,999 |
| Job title | Director, Vice President, C-Level |
| Department | HR  |

**Step 2** - Assign a score to each characteristic according to its relevance in your ideal prospect profile. Use positive scores for desirable traits and negative scores for traits that make the lead less of a fit for your product.

**Example 2b – Assigning scores to ideal and undesirable prospect characteristics**

| **Characteristic** | **Score** |
| --- | --- |
| Industry – Aerospace | +10 |
| Industry – Manufacturing | +5  |
| Company size – 100 - 999 | +5  |
| Company size – 1,000 – 9,999 | +10 |
| Company size – <10 | \-10 |

## Exercise 3 - Incorporating local flexibility in your scoring model

With the basic behavioral and demographic scoring models you have completed, you could take it to the next level by allowing local flexibility. Business values may vary in different markets when an organization operates globally. In the following exercise, you will learn how to apply scores to reflect the real business value of the lead activities or characteristics in different situations.

**Step 1** - Take the activities and characteristics from exercises 1 and 2 and determine for each item whether they vary by location or product line.

**Example 3a – Signals in global and local markets:**

| **Signal** | **Global** | **Local** |
| --- | --- | --- |
| Activities | <ul><li>Filled out “Request a demo” form</li><li>No interaction in last 90 days (about 3 months)</li></ul> | <ul><li>Visit us at tradeshow</li><li>Download a white paper</li></ul>
| Characteristics | <ul><li>Department</li><li>Job title</li></ul> | <ul><li>Industry</li><li>Company size</li></ul> |

**Step 2** - Define your scoring matrix for local markets:

* Set up a different matrix for demographic and behavior elements.
* Determine the topics of priorities for you to ask for the local team's input on.
* Define the number of values used to rate within your topics.
* Assign individual values by aligning relative worth with global scores.
* Consider defining common scenarios when prospects interact with your brand and test your overall scoring for them.
  * For example, a common prospect journey you see would be for a person to enter your website on a content page, then click through to a product page and download a brochure. You would target them with a webinar invitation, and they respond to it by registering, but not attending. Consider if your sales already want to speak with this person or not and evaluate if your scoring model gets these prospects to the right overall score to reflect that level of interest.

**Example 3b – Demographic scoring matrix:**

| **Demographic matrix** | **Priority 1** | **Priority 2** | **Priority 3** |
| --- | --- | --- | --- |
| High values | 20 points | 10  points | 7  points |
| Medium values | 10  points | 7  points | 3  points |
| Low values | 5  points | 3  points | 1 point |

**Step 3** - Collect input from your local or regional sales teams to develop a holistic view. You will notice that no individual scores are included in example 3c. This allows the sales team to focus on the relative worth of the different topics during the review process. However, you should have your full model documented as background materials for other Marketo Engage administrators.

* Lock down what cannot be adjusted for global consistency (here in the “Implement topic?” column). 
* Mark (here in "Priority" and "Score" columns) what can be adjusted for local influences.

**Example 3c – Relative worth of scoring topics:**

<table>
 <tr>
    <th>#</th>
    <th>Implement topic</th>
    <th>Demographic / Behavioral</th>
    <th>Topic</th>
    <th>Priority</th>
    <th>Values</th>
    <th>Scores</th>
 </tr>
 <tr>
    <td rowspan=6>1</td>
    <td rowspan=6>REQUIRED</td>
    <td rowspan=6>Demographic</td>
    <td rowspan=6>Industry</td>
    <td rowspan=6>2</td>
    <td>Technology</td>
    <td>High</td>
  </tr>
  <tr>
    <td>Fashion</td>
    <td>High</td>
  </tr>
  <tr>
    <td>Retail</td>
    <td>Medium</td>
  </tr>  
  <tr>
    <td>Manufacturing</td>
    <td>Medium</td>
  </tr>
  <tr>
    <td>Healthcare</td>
    <td>Low</td>
  </tr>
  <tr>
    <td>...</td>
    <td>Low</td>
  </tr>
<tr>
    <td rowspan=3>2</td>
    <td rowspan=3>Yes</td>
    <td rowspan=3>Demographic</td>
    <td rowspan=3>Company size (employees)</td>
    <td rowspan=3>3</td>
    <td>>1000 employees</td>
    <td>High</td>
  </tr>
  <tr>
    <td>250-999 employees</td>
    <td>Medium</td>
  </tr>
  <tr>
    <td>1-249 employees</td>
    <td>Low</td>
  </tr>  
<tr>
    <td rowspan=3>3</td>
    <td rowspan=3>No</td>
    <td rowspan=3>Behavioral</td>
    <td rowspan=3>Page visits on your website</td>
    <td rowspan=3>2</td>
    <td>>Product information pages</td>
    <td>Low</td>
  </tr>
  <tr>
    <td>Pricing pages</td>
    <td>Medium</td>
  </tr>
  <tr>
    <td>Demo request page</td>
    <td>High</td>
  </tr>
</table>

## What's Next?

* Download the [person scoring exercise sheet](./assets/build-person-scoring-model-and-local-flexibility-in-adobe-marketo-engage.docx){target="_blank} to develop your scoring model offline.
* Build out your person scoring in Marketo Engage. Check this [tutorial](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/lead-and-data-management/lead-scoring-watch){target="_blank} and [demo](https://experienceleague.adobe.com/en/docs/events/marketo-and-mochas-recordings/2023/lead-scoring){target="_blank} to get started. You can import a lead/person scoring program [template](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program){target="_blank} from the Marketo Engage Reference Library to accelerate the program build.
* Create two versions of the scoring program:
  * A central program that runs all scoring that cannot be updated locally.
  * A local copy with the scoring elements that are configurable.
* Set up your scoring values as tokens within your scoring program. This ensures consistency even as you adjust scores over time.
  * A common example of tokenized scores is having a token for high-value activities that automatically meet your threshold, such as requesting a demo or booking a meeting with your sales team. Even if you alter the minimum score required to meet your threshold, you can easily update all high-value activities at once by updating one token.
* Adjust your local Smart Campaign for each location:
  * Determine which demographics and behavioral activities should only score once (i.e. Industry) and which should score every time a prospect qualifies (i.e. Attended a webinar). This ensures potential contacts triggered by the data value change are relevant for sales.
  * Make sure your choices are mutually exclusive.
  * Make your updates in both flow steps so the Person Score is updated in an identical way to the Demographic Score. That way, the Person Score stays in line with the combination of behavior score and demographic score.
* Test the Smart Campaign once you’ve finished building your program. For example, go to your demo form, fill it out with a test email, and check your test person’s score in [Marketo Engage database](https://experienceleague.adobe.com/en/docs/marketo/using/getting-started-with-marketo/quick-wins/simple-scoring#step-view-the-person-info){target="_blank}.
* After you build your model, consider setting up an alert to go out to sales once the person’s score has reached your sales handoff threshold. Learn more about setting up an alert with this [tutorial](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert){target="_blank}.

### Authors

{{christina-zuniga}}

{{katja-keesom}}

{{amy-chiu}}