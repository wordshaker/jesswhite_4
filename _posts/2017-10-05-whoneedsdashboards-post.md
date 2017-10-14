---
layout: post
title: Who Needs Dashboards?
description: "An overview of the different types of dashboards and what they are for"
date: 2017-10-05
img: ./2017-10-05/header.jpg
tags: [monitoring, instrumentation]
comments: false
share: true
---

> An overview on the different forms of dashboards, what they are useful for and for whom.

Monitoring is an expansive topic from instrumentation to logging in all it's forms. One part of instrumentation is dashboards - the visualisation of your metrics and measurements. Dashboards can have numerous purposes from enabling a clear view of the important parts of a software system, to measuring the overall health of a business.

It's no secret that I am fascinated by the topic of monitoring. I want to find out what people do in their companies, pain points, how to do it well and the awesome things that can come from having a well monitored system. As part of my work in this area previously I tried something to get more departments in the company I worked for invested and bought into what was begin instrumented in our system. You can read the blog covering that experiment [here](https://jesswhite.co.uk/instrumentationforbusiness-post/). I think dashboards are powerful, often underutilised and that there isn't enough resource talking about them out there. 

> "If you don't measure it, you cant improve it" - Randy A. Steinberg

There are a lot of common questions around dashboards including how long they should live and what should be on them. These questions aren't going to be addressed in this post. Instead, we are taking a step back to examine what types of dashboards there are, what they are for, and who needs them. Hopefully, by the end of this, you'll want to learn more about how dashboards can be used in your company, but also how to do them well. Dashboards are beautiful and powerful tools. They come in many forms, each with their own strengths, purpose and evolution. There is a bit of overlap on these categories and how they are used, which will be covered.

The information in this post uses a cumulation of my own experience (I have been involved in the development of developer, MI and BI dashboards), talking to those with more experience than myself and extensive reading. Any resources I used and people who kindly gave me their time to discuss dashboards with are listed at the end.

### MI and BI Dashboards

These dashboards are primarily for business use. The data on them are relatively high level. They are used for measuring the health of a business and for planning the future direction of the company. 

First of all, let's explore BI (aka Business Intelligence) dashboards. These show data that can be used to inform business strategy. These may include any major events that have had an effect on the business to help structure future plans. Is the business meeting their Key Performance Indicators (KPI's)? Are these begin met on schedule? If not, is there any clear reason why they may have not been met? Can the measurements we have be extrapolated to estimate when we are going to meet overarching goals? Using BI dashboards, you can see the effectiveness of past efforts to help guide future ones, as well as judging if the business is healthy overall. Metrics on these dashboards may include:

* Real time achievement vs business / board goals.
* A unit important to the business across time. I.e. customer numbers over the last year. This can be used to judge if the customer base is on the rise, if there are times of year which effect the performance of the business and therefore any planned initiatives.

These types of boards are principally aimed to assist executives, managers and other corporate stakeholders.

> Upper management can use BI dashboards to help structure future business plans, so monitor the health of the business and to negotiate with / report to stakeholders.

As I am not the primary audience for this kind of dashboard, I talked to a couple of people heading up companies.  These people use dashboards already, so I enquired to what information is important to them, but also in board meetings. 

> Add Notes From Discussion with Michael etc.

The other high level type of dashboard is the Management Information (MI) dashboard. These contains information that can be used to measure the health of the business financially. They may include monitoring of sales, losses or attendance. It can also cover how well a company is managing their costs while trying to increase their revenue. These are the statistics that cause the results shown on the BI dashboard. This cost / profit balance is crucial to all companies. Get it wrong, and the company won't exist for long. Examples of data can include:

* Generated leads
* Money gained from each integrated third party
* Number of users or monetary gain for each type of product.
* Results from marketing release or AB test
* Losses - temporary or permanent.
* Cost of resource. This could be departmental costs from software required to salaries paid out.
* Reported performance of competitors.

> Departments such as marketing, finance and risk can use MI dashboards to guide the priority of  current work, help to plan future work and to monitor performance of recent releases.

So why do marketing, finance and risk care about these dashboards? Numerous reasons. First of all it is a really accessible way to see a lot of information. Marketing may have a number of initiatives happening at one time and by using a dashboard they can see which initiatives appear to be having the biggest impact without sifting through excel sheets of numbers. Dashboards also make it easier to communicate what is going on to other areas of the business. When discussing the metrics that effect BI, a stakeholder can be shown a dashboard, or be provided access to one. It enables them to see what is going on without much explanation and can start needed conversations earlier. Even by having a high level dashboard of number of customers, the type of product they are using, the business outgoings and incomings, and competitor performance can not only help demonstrate the impact of the team, but direct their upcoming focuses. 

_What happens when you combine the two?_

Both of these types have their own uses and strengths. By combining the two, you can create a dashboard that's of interest to an even wider audience. By having a combined BI/MI dashboard, a united vision on what the company is trying to achieve and their progress to that goal can be shown. 

Pick a key KPI. This may be a financial goal, a number or users or something completely different that is expected to be achieved in a certain time frame. I've seen this being split from a yearly KPI down to quarterly stages to aim for. That's a short enough time frame that the future goal doesn't seem as unachievable. No matter what it is, work that is put forward to departments as a priority is normally guided in some way to achieve this goal. By showing the progress in reaching the BI aim in a easy to understand format, everyone in the company can see the companies health, it's progress and how likely they are to get their bonus if its tied to performance. Further, if you mark some of the departmental events that have contributed to the companies performance, it is easier to recognise the impact a departments work has on the grand aim.

> Combine MI & BI and the whole business can make use of it.

There is quite a bit of information that can be displayed on the mixed form of dashboard. As mentioned, the impact of different departments contributions to achieving the company target, but also external factors having an impact. Major events on the dashboard can include anything that can impact company in any way. Examples can include:

* A marketing initiative.
* A new feature.
* Implementation of a new policy.
* Outage of a third party.
* Integration with a new third party.

By doing something like this it is easy to the company's progression as a whole, the company's eventual aim and some of the contributing factors to the current state of play. Other high level statistics can be added to this board. For instance, I've seen it where by hovering on a point you could see details such as estimated financial impact. Another feature as by hovering on a date you could see dispersed and gained money. 

As well as showing the company's next big target and how they are progressing on reaching that target, some choose to show a line of what the performance of the company was like a year earlier. In some cases this may show how much a company has grown financially or in popularity over the last year. It not only shows if the company as a whole is likely to hit their next target, but also the impact of the past work, or if there were any externally impacting events that might want to be planned for. An example would be Christmas for many companies. Some see a rise in use, others will find it a tougher time to make money in. 

Good rules for MI / BI and business level dashboards: Keep it simple. Keep it high level. Keep it focused towards that one goal.

### Operational and Development Dashboards

#### Operational information

#### Development information


#### ITSM

#### Who needs them?


### Reading

1. [Zen and the Art of Systems Monitoring](https://www.scalyr.com/community/guides/zen-and-the-art-of-system-monitoring)

2. [6 Golden Rules to Successful Dashboard Design](https://www.geckoboard.com/blog/building-great-dashboards-6-golden-rules-to-successful-dashboard-design/#.WdKS62hSyUl)

3. [Executive Dashboards - What they are and why every business needs one](https://www.forbes.com/sites/davelavinsky/2013/09/06/executive-dashboards-what-they-are-why-every-business-needs-one/#25b577fe37d1)

4. [Measuring ITSM](https://www.amazon.co.uk/Measuring-ITSM-Reporting-Management-Executives/dp/1490719458/ref=pd_cp_14_1?_encoding=UTF8&psc=1&refRID=NERK3B79N4A24C5GJN7E)

5. [Karl Bagci's blog posts around ITSM ](https://medium.com/@karlbagci)


### Thanks to: