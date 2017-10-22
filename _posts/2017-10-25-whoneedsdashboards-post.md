---
layout: post
title: Who Needs Dashboards?
description: "An overview of the different types of dashboards and what they are for"
date: 2017-10-25
img: ./2017-10-25/header.jpg
tags: [monitoring, instrumentation, dashboard]
comments: false
share: true
---

----
#### An overview on the different forms of dashboards, what they are useful for and for whom.
--- 

### What is a dashboard?

Dashboarding is part of the instrumentation portion of monitoring. The main purpose of a dashboard, no matter its type, is to enable the ability to quickly process information that a user might need. This may be to understand the current situation, to aide in decision making, or to inform that a reactive action is needed.

In the [Google SRE book](https://landing.google.com/sre/book/chapters/monitoring-distributed-systems.html) dashboards are defined as following:

> _"An application (usually web-based) that provides a summary view of a service’s core metrics. A dashboard may have filters, selectors, and so on, but is **prebuilt to expose the metrics most important to its users**. The dashboard **might also display team information** such as ticket queue length, a list of high-priority bugs, the current on-call engineer for a given area of responsibility, or recent pushes."_

This description is probably aimed at the more 'technical' dashboards but there are two elements of this definition which support the definition just given which I have placed in bold.

There are a lot of common questions around dashboards including how long they should live and what should be on them. These questions aren't going to be addressed in this post. Instead, we are taking a step back to examine what types of dashboards there are, what they are for, and who needs them. The following four categories of dashboard will be covered:

- Business Intelligence (Strategic)
- Management Information (Tactical)
- Operational Information (Execution)
- Development Information (Execution)

I'm my opinion, dashboards are both beautiful and powerful. They come in many forms, each with their own strengths, purpose and evolution. I hope by the end, you will be considering who needs dashboards, and why, in your place of work.

### Business Intelligence Dashboards

Business Intelligence (BI) dashboards are also known as strategic dashboards. They contain information that show the overall health of a business and are used to help generate business strategy. There is a lot of number crunching and statistical analysis involved in working out if the business is making the right decisions and what future decisions need to be made. As such there is a lot of information that can be on a BI dashboard.

Some of the responsibilities covered by BI dashboards include:

- **Measuring and monitoring trends that show how the business is performing.**

   Shows if the current understanding of how the business is performing is accurate. This can help inform what kind of decisions need to be made.

- **Comparisons of the businesses performance over previous time frames.**

   Helps show any trends. If the business is under-performing, why? Has there been a trend like it previously and what did we do to mitigate it? Has there been a shift in performance over time?

- **Measures demonstrating the accuracy of the statistical models used for giving a competitive advantage to their customer base.**

   Some companies have models of what a customer may need. For example, a gas company may expect higher income in winter months, especially in households with very young or elderly people. Are they selling their product at the right price? Are those that use their services likely to pay their bills?

BI dashboards answer the questions of _'how is the business performing?'_ and _'what can be done to improve the performance?'_. They can be used to help structure future business plans, monitor the health of the business and provide transparency to stakeholders.

A business needs to meet goals and Key Performance Indicators (KPIs). An example is having quarterly goals to increase revenue or customer base. Dashboards can be useful for indicating a business's progress to reaching these targets. For example, by showing real time achievement vs estimated progress that should have been made. 

There is a lot that can be covered in BI dashboards. The best way to display this information or the information to be shown is a whole different topic for a different day. Today, we are covering who needs these dashboards.

BI dashboards are needed by upper management including executives, managers and other corporate stakeholders. They need them to help make informed decisions.

### Management Information Dashboards.

Next we have Management Information (MI) dashboards. These contain information that can be used to measure the health of the business financially and the progress of initiatives to help reach the business goals. These are the statistics that cause the results shown on the BI dashboard. For example, MI dashboards may include monitoring of sales, losses or attendance. It can also cover how well a business is managing their costs while trying to increase their revenue. 

This cost/profit balance is crucial to all businesses. Get it wrong, and the business won't exist for long. Examples of data can include:

* Generated leads
* Money gained from each integrated third party
* Number of users or monetary gain for each type of product.
* Results from marketing release or AB test
* Losses - temporary or permanent.
* Cost of resource. This could be departmental costs from software required to salaries paid out.
* Reported performance of competitors.

Departments with a direct cost/profit impact such as marketing, finance, product and (in some businesses) data analytics need MI dashboards to guide the priority of current work, help to plan future work, and to monitor performance of previous work.

Dashboards are useful to these departments for numerous reasons. First of all it is a really accessible way to display a lot of information. For example, a marketing team may have a number of initiatives happening at one time and by using a dashboard they can see which initiatives appear to be having the biggest impact without sifting through Excel sheets of numbers. 

Dashboards also make it easier to communicate what is going on to other areas of the business. If a product team have a dashboard displaying the number of customers, the type of product they are using, the business outgoings and incomings, and competitor performance it can not only help demonstrate the impact of the team, but direct their upcoming focuses. 

### MI and BI are closely linked. What happens if you combine the two?

Both of these types have their own uses and strengths. By combining the two, you can create a dashboard that's of interest to an even wider audience. By having a combined BI/MI dashboard, a united vision on what the business is trying to achieve and their progress to that goal can be shown. 

<div style="text-align:center; width:80%; margin-left: 10%;" markdown="1">
![MI BI](../assets/img/2017-10-25/MIBI.JPG)
_Above: A mock of a combined MI and BI dashboard._
</div>

Pick a key KPI. This may be a financial goal, a number of users or something completely different that is expected to be achieved in a certain time frame. No matter what it is, work that is put forward to departments as a priority is normally guided in some way to achieve this goal. 

By showing the progress in reaching the BI aim in a easy to understand format, everyone in the business can see the business's health, it's progress and how likely they are to get their bonus if it's tied to performance. When I've seen this done the boundaries for the events shown on these dashboards are set by the business. Major events on the dashboard can include anything that can impact business in any way. Examples can include:

* A marketing initiative.
* A new feature.
* Implementation of a new policy.
* Outage of a third party.
* Integration with a new third party.

Using a combined MI/BI dashboard it is easy to the business's progression towards it's goal and the impact of ongoing work. Other high level statistics can be added to this board. For instance, I've seen examples where by hovering on a point you could see details such as estimated financial impact.

It could also display the performance in a previous time frame. This can demonstrate temporal effects that might need to be planned for. An example would be Christmas for many companies. Some see a rise in use, others will find it a tougher time to make money in. 
<!--  -->
Good rules for MI/BI and business level dashboards: Keep it simple. Keep it high level. Keep it focused towards that one goal.

## Execution Information.

The final two categories to be explored in this post are operational and development dashboards. These can be referred to as 'execution information' as they cover a lot of overlapping questions about how the business problems defined by strategic and tactical decisions are tackled in a technical fashion.

Some of the questions they answer are:

* What is the health of the system?
* Could it be better? (performance/stability) 
* If it's unhealthy, what is broken or performing poorly?
* What is running? 
* Where is the system most fragile?

Depending on your business size and structure, these dashboards can also be combined as both types of work are interlinked. Hardware and software can have a big impact on each other. In larger companies, the teams and their dashboards seem to be split. In this case, there is a reliance on clear communication and transparency.

### Operational Information
The primary focus of operation information is to monitor interactions with hardware, be it physical or virtual. In order to have software that runs well you need to have an infrastructure that is healthy and running effectively.

Some of what is covered by operational dashboards include:

* Services
* CPU
* RAM
* Disk Space - space, latency, read & write

Both operations teams (AKA. IT teams) and developers need dashboards covering operational information. Operations want to keep the system healthy, and when something isn't behaving as expected - they want to determine where the problem my lie. Development teams software runs off this infrastructure. They want to know if peculiarities they are seeing in their software my be down to what it is running on or if their software may be causing problems for the hardware. They want to know if their current hardware is suitable for work that is prioritised. The better the communication between these two teams, the easier it is not only to keep the system alive, but also to determine ways in which to make it better.

### Development Information

Being a developer, this final category to dashboard I am exposed to a lot. For both operations and development, dashboarding has been used as a tool for a very long time. As such, there are a lot of different ways in which they can be used and structured. 

An example of some of the uses for development dashboards include: 

- Monitoring the health of your system and aiding debugging issues

   Probably the first reason that might come to mind when thinking about dashboards is their use for checking whether the system is working or not. Being able to see what parts of the system are up, what parts might be affected by poor performance of a third party or what is behaving unusually is imperative. When debugging something going wrong with the system, a dashboard displaying the behaviour of each component can help speed up the process of diagnosing and fixing the issue.

- Performance monitoring
   You can also create dashboards at different levels to see how each area of your system is performing. This can show where the bottlenecks are, whether software or hardware needs improving and how the system is coping with it's current load. We can use performance monitoring to guide future work to improve the system, as well as seeing the effect of other pieces of work on the system. The more performant your product is, the faster the experience for your user.

- Guiding improvement
   Linked to the points above, a business can use monitoring to see where their software may need work. Software systems can get old and creaky. They may be fit for purpose when first build, but like with anything in engineering, these systems need love and maintenance. Through monitoring you can see where bottlenecks are. Do you need to scale? Could the code do with another look at if it has not been touched in awhile? Are messages staying in the queues too long? Again, this applies to both development and ops.


Though developers are the main audience for development information dashboards, there are situations where operations, product owners and stakeholders benefit from these dashboards too. The work done in operational and development teams can highly impact each other and as such clear communication and standardised understanding of how the systems are working are beneficial. I have seen it where product have used development information dashboards instead of having their own to see information they need as well. An example is to see if SLA's are being met for a third party.

### Who Needs Dashboards?

There are more categories of dashboard than those written about here, and even for those mentioned I could go into much more depth of who needs them and why.

In answer to the main question of 'who needs dashboards?' - everyone does. In my opinion, when done well, dashboards can make your life easier. They can help direct work. They help show the effects of your investment. They can improve communication and transparency in a business.

 It also doesn't hurt that they are easy to look at. 

 This following quote from [Measuring ITSM](https://www.amazon.co.uk/Measuring-ITSM-Reporting-Management-Executives/dp/1490719458/ref=pd_cp_14_1?_encoding=UTF8&psc=1&refRID=NERK3B79N4A24C5GJN7E) sums up why everyone needs dashboards quite nicely

> "If you don't measure it, you can't manage it" <br/>
> "If you don't measure it, you can't improve it"<br/>
> "If you don't measure it, you probably don't care"<br/>
> "If you can't influence it, then don't measure it"<br/>
> -- _Randy A. Steinberg_

In order to make informed decisions you need a baseline and to measure progress. In order to fix or improve things, you need to be able to see when something is broken or can be improved. 

Dashboards could be used to a further extent than what is covered in this post. How great would it be if those with direct customer contact had a dashboard of which parts of the product was down for maintenance or how many calls/emails were waiting? Or if sales had a board with their running totals versus aimed profit? Not only do dashboards make it easier to work with information, be reactive and plan well; but it can help increase openness and communication across business.

**Who needs dashboards?**

   You do.

## Thanks

To build upon my knowledge in these areas, I talked with a number of people who had worked with a variety of dashboards. My aim was to not only write from my own experience but to gather the uses of dashboards from different departments, different professions and different sized companies. 

Thank you to: Darren Whitworth, Michael Woodburn, Karl Bagci, Jonathan Relf, Chris Taylor, Moreton Brockley and anyone else who has encouraged my enthusiastic monitoring related babble. I now have enough information for a year's worth of posts.

## Some Further Reading

- [Zen and the Art of Systems Monitoring](https://www.scalyr.com/community/guides/zen-and-the-art-of-system-monitoring)
- [6 Golden Rules to Successful Dashboard Design](https://www.geckoboard.com/blog/building-great-dashboards-6-golden-rules-to-successful-dashboard-design/#.WdKS62hSyUl)
- [Executive Dashboards - What they are and why every business needs one](https://www.forbes.com/sites/davelavinsky/2013/09/06/executive-dashboards-what-they-are-why-every-business-needs-one/#25b577fe37d1)
- [Measuring ITSM](https://www.amazon.co.uk/Measuring-ITSM-Reporting-Management-Executives/dp/1490719458/ref=pd_cp_14_1?_encoding=UTF8&psc=1&refRID=NERK3B79N4A24C5GJN7E)
- [Karl Bagci's blog posts around ITSM ](https://medium.com/@karlbagci)
- [Peter Bourgon - Logging v. Instrumentation](https://peter.bourgon.org/blog/2016/02/07/logging-v-instrumentation.html)
- [Brendan Gregg - USE Method](http://www.brendangregg.com/usemethod.html)
- [Google SRE book](https://landing.google.com/sre/book/chapters/monitoring-distributed-systems.html)
- [From Strategy to Business Models and to Tactics ](http://www.hbs.edu/faculty/Publication%20Files/10-036.Pdf)
- [Defining Strategy, Implementation, and Execution](https://hbr.org/2015/03/defining-strategy-implementation-and-execution)