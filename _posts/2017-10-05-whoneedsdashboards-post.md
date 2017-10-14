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


MI (Management Information) contains information that can be used to measure the health of the business financially. This can include monitoring of sales, losses or attendance. These are the statistics that cause the results shown on the BI dashboard. Examples of data can include:

* Generated leads
* Money gained from each integrated third party
* Number of users or monetary gain for each type of product
* Results from marketing release or AB test
* Losses - temporary or permanent.
* Reported performance of competitors.

> Departments such as sales, finance and risk can use MI dashboards to guide the priority of  current work, help to plan future work and to monitor performance of recent releases.

Both of these types have their own uses and are equally brilliant. They can also be combined to be of interest to a wider audience and have added uses! Not unlike a very cool transformer. By having a combined BI/MI dashboard the company can have a united vision on what the company is trying to achieve. This may be a financial goal, a number or users or something completely different. No matter what it is, the work employees do are normally guided in some way to achieve this goal. By showing this progress in a easy to understand format, everyone in the company can see the companies health, it's progress and how likely they are to get their bonus if its tied to performance.

> Combine MI & BI and the whole business can make use of it.

There is quite a bit of information that can be displayed on the mixed form of dashboard. For instance, by having a graph which shows the target aims for the quarter, where the company is at on achieving that monthly goal and the major events that may have impacted the companies progress. It can show the impact of different departments contributions to achieving this target. Major events on the dashboard can include anything that can impact company in any way. Examples can include:

* A marketing initiative.
* A new feature.
* Implementation of a new policy.
* Outage of a third party.
* Integration with a new third party.

> Insert picture of example graph here.

By doing something like this it is easy to the company's progression as a whole, the company's eventual aim and some of the contributing factors to the current state of play. Other high level statistics can be added to this board. For instance, I've seen it where by hovering on a point you could see details such as estimated financial impact. Another feature as by hovering on a date you could see dispersed and gained money. 

Good rules for these kinds of Keep it simple. Keep it high level. Keep it focused towards that one goal.

### Operational and Development Dashboards

#### Operational information

#### Development information

#### Who needs them?


### Reading

1. [Zen and the Art of Systems Monitoring](https://www.scalyr.com/community/guides/zen-and-the-art-of-system-monitoring)

2. [6 Golden Rules to Successful Dashboard Design](https://www.geckoboard.com/blog/building-great-dashboards-6-golden-rules-to-successful-dashboard-design/#.WdKS62hSyUl)

3. [Executive Dashboards - What they are and why every business needs one](https://www.forbes.com/sites/davelavinsky/2013/09/06/executive-dashboards-what-they-are-why-every-business-needs-one/#25b577fe37d1)


### Thanks to: