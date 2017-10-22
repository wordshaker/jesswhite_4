---
layout: post
title: Who Needs Dashboards?
description: "An overview of the different types of dashboards and what they are for"
date: 2017-10-15
img: ./2017-10-15/header.jpg
tags: [monitoring, instrumentation, dashboard]
comments: false
share: true
---

----
#### An overview on the different forms of dashboards, what they are useful for and for whom.
--- 

### What is a dashboard?

Dashboarding is part of the instrumentation portion of monitoring. The main purpose of a dashboard, no matter its type, is to enable the ability to quickly process information that a user might need. This may be to understand the current situation in order to aide in decision making, or to inform that a reactive action is needed.

In the [Google SRE book](https://landing.google.com/sre/book/chapters/monitoring-distributed-systems.html) dashboards are defined as following:

> _"An application (usually web-based) that provides a summary view of a service’s core metrics. A dashboard may have filters, selectors, and so on, but is **prebuilt to expose the metrics most important to its users**. The dashboard **might also display team information** such as ticket queue length, a list of high-priority bugs, the current on-call engineer for a given area of responsibility, or recent pushes."_

This description is probably aimed at the more 'technical' dashboards but there are two elements of this definition which support the definition just given which I have placed in bold.

There are a lot of common questions around dashboards including how long they should live and what should be on them. These questions aren't going to be addressed in this post. Instead, we are taking a step back to examine what types of dashboards there are, what they are for, and who needs them. The following four categories of dashboard will be covered:

- Business Intelligence (Strategic)
- Management Information (Tactical)
- Operational Information (Implementation)
- Development Information (Implementation)

I'm my opinion, dashboards are both beautiful and powerful. They come in many forms, each with their own strengths, purpose and evolution. I hope by the end, you will be considering who needs dashboards, and why, in your place of work.

### Business Intelligence Dashboards

Business Intelligence (BI) dashboards are also known as strategic dashboards. They contain information that show the overall health of a business and are used to help generate business strategy. There is a lot of number crunching and statistical analysis involved in working out if the business is making the right decisions and what future decisions need to be made. As such there is a lot of information that can be on a BI dashboard.

Some of the responsibilities covered by BI dashboards include:

- **Measuring and monitoring trends that show how the business is performing.**

   Shows if the current understanding of how the business is performing is accurate. This can help inform what kind of decisions need to be made.

- **Comparisons of the businesses performance over previous time frames.**

   Helps show any trends. If the business is under-performing, why? Has there been a trend like it previously and what did we do to mitigate it? Has there been a shift in performance over time?

- **Measures demonstrating the accuracy of the statistical models used for giving a competitive advantage to our customer base.**

   Some companies have models of what a customer may need. For example, a gas company may expect higher income in winter months especially in households with very young or elderly people. Are they selling their product at the right price, and are those that use their services likely to pay their bills?

> BI dashboards answer the questions of 'how is the business performing, and what can be done to improve the performance. They can be used to help structure future business plans, monitor the health of the business and provide transparency to stakeholders.

A business needs to meet goals and Key Peformance Indicators (KPIs). Looking at the short term, most businesses have quarterly goals be it to increase revenue or customer base. Dashboards which can be useful as indicators for how a business is doing to reach these goals may show real time achievement vs estimated progress to meeting a businesses quarterly goal. 

There is a lot that can be covered in BI dashboards. The best way to display this information or the information to be shown is a whole different topic for a different day. Today, we are covering who needs these dashboards.

> BI dashboards are there to assist upper management including executives, managers and other corporate stakeholders. 


### Management Information Dashboards.

