---
layout: post
title: A Practical Guide to Execution Level Dashboarding
description: "Baselines for constructing development dashboards"
date: 2018-11-07
cover:  "/assets/img/2018-11-07/header.png"
tags: [monitoring, instrumentation, dashboarding]
comments: false
share: true
---

---
<center>
<h3> Part 1 - Baselines for constructing development dashboards. </h3>
</center>
---
<br/>


> **DISCLAIMER:**
This chapter is written from my personal experience with dashboarding. Monitoring is a vast field and though I've touched upon various bits, the majority of my experience is in backend development, and I am learning more about operations (which is all very interesting and exciting). As such, the discussed "baselines" will be for backend work. I will not be covering frontend monitoring, performance monitoring, or other forms of monitoring in this current series of posts. They may be broached in future posts as I become older and wiser.

In the last series, _Creating & Maintaining Impactful Dashboards_, numerous things were covered. The importance of dashboards, and how they are crucial for transparency, unity and clear communication across businesses and teams. The different areas of a business that dashboarding can be useful for, and how to ensure that your dashboards remain useful and unignored. Finally, some of the signs that dashboards may need work, and what to do when the crisis signs are spotted. 

This next chapter / series of posts will cover some more hands on a practical guides to dashboarding. The focus will be on development dashboarding and the series will cover topics such as suggested baselines for development dashboarding, an example of a monitoring infrastructure for a playground and in production, and some useful tools provided by the likes of Grafana and Docker that will make your monitoring life going forward, easier

This first post will echo points in the  _Creating & Maintaining Impactful Dashboards_ series, but with hopefully cover the paradigms in more depth.

## Metrics VS Diagnostics

Before diving into these next few chapters, I think it's important that the information being covered is relating to metrics over diagnostics.

Metrics are high level measures of a system, project or business. They are primarily used for seeing how the measured environment is behaving in order to then have a future affect on them. Depending on the type of measurements, metrics are useful for spotting or preventing erroring behaviour or seeing bottlenecks and areas for improvement. The information used for metrics is usually aggregated into time specific chunks, which include larger periods of time as records get older. When being used they are often kept in a present line of site, such as a screen on an office wall.

Diagnostics, on the other hand, are used once a problem or area for improvement has already been determined. These are often used along side high-level metrics but have a different purpose. Examples of diagnostic information includes logs. Information is often lower level and not aggregated. Diagnostic information is often used for debugging or tracing, finding out the specifics of a problem or area of improvement at the point that it is assumed it is occurring. Often the recordings put in place aren't kept for a long period of time, and once their usefulness is outlived, they are removed. There are exceptions to this rule, such as behaviours which can't be fixed or areas which 

## Baselines & What's Great About Them

Let's talk about my favourite dashboard - the car dashboard. Anybody who drive can get into any car and determine how to get the information they need in little to no time. This is because there is a baseline to what information is displayed, where and how. 

We need the same things from our system dashboards as we do from our car dashboards. We need to know the state of our systems and if there is anything we need to react to. It needs to be presented in a way that's quick to read & easy to understand. If we have a standard format for our dashboards then, like with a car dash, we can read and understand system dashboards with minimal effort.

_Are there existing, well tried out patterns for these dashboards?_ Yes! 
_Am I preaching someone else's knowledge without trying it out?_ No!

## Dashboards for Services

There is a pattern proposed by Brendan Gregg which is great for services :[U.S.E](http://www.brendangregg.com/usemethod.html). These stand for Utilisation, Saturation and Error. I've used this pattern in a couple of the places I've worked in and it's avoided catastrophe.

* _Utilisation_

This refers to how long a service takes to do it's process, the work it needs to do. It's the time from input to outcome. It tell us by itself how long it is taking to process the work. This may align to KPI's. In combination with the other measures, it can tell us how to act to fix utilisation times.

---
_Analogy: a person clocking in and out of work. The time from when they clock in, to after they've done their work and clocked out._

---

* _Saturation_

This is the degree to which work is queued. This could be in a literal queue in the case of services - RabbitMQ, SQS or similar. There a couple of measures for this - the depth of queue, and the oldest message.

---
_Analogy: When a toilet is occupied it can't take on any more "work". As such the queue gets longer outside. The degree to which the "toilet service" is saturated is the degree to which that queue builds up._

---

* _Error_

Errors are pretty much what you would expect - but there are different levels and types of errors. There errors internal service errors, custom errors or the whole service could go down. These are the ones we normally consider. Harking back at my previous posts - there aren't just technical errors but also business concerns contextual to the service. The service is built for some business need and there may be behaviour which technically works, but is not desired behaviour for the businesses needs. These should be measured as well.

---
_Analogy: Well... there's no need for an analogy here..._

---

These used in combination are incredibly powerful. A slower utilisation and a higher saturation could point to a couple of causes. Maybe we have an increased load to our application and the service can't cope with it. It might be that we need to scale or look into how we can improve the performance of the system. We would have to find out if there was an event that might have lead to this increase and if a short or long term fix would be required. 

Another cause could just be the service is having issues. We should be able to see this from an increase in errors.

It might be that utilisation is still good but the saturation has increased. Here, we would scale as the problem doesn't seem to be with the service itself, especially if there isn't an increase in errors, and do some further investigations.

There are more combinations than those listed here, but over time you learn the patterns of unusual behaviour in your system and how to react. All from less than 5 baseline metrics.

## Dashboards for API's

For API's there are two main patterns I use for reference. Google's Four Golden Signals and R.E.D.

**[Googles Four Golden Signals](https://landing.google.com/sre/sre-book/chapters/monitoring-distributed-systems/)**

The Four Golden Signals are mentioned in the Monitoring Distributed Systems chapter of the Google SRE book. Used in combination, the four metrics discussed are incredibly powerful.

* _Latency_ 
the time between request and response but with a focus of the difference between successful and erroring requests.

* _Traffic_ 
requests per second. A measure of the load on the API.

* _Errors_
same as before, a count of errors.

* _Saturation_ 
what percentage of your systems resources is currently in use.


**[R.E.D](https://peter.bourgon.org/blog/2016/02/07/logging-v-instrumentation.html)**

RED, which is discussed in this blog written by Peter Bourgon, is a mnemonic coined by Tom Wilkie. Much like Brendan's Gregg USE methods for measuring system resources and services, RED is suggested as baseline measurements for API's.

* _Rate_
 - a count of requests over time

* _Error_
 - a count of error over time

* _Duration_
 - the time between request and response.


## Applying alerts


## Managing Stakeholder Concerns

---
## Links

#### Blogs by Jessica:

_Chapter 1 - Creating & Maintaining Impactful Dashboards Series_

* Part 1 - [Creation of impactful dashboards](https://jesswhite.co.uk/impactfuldashboardspart1-post/)

* Part 2 - [Continuous Maintenance.](https://jesswhite.co.uk/impactfuldashboardspart2-post/)

* Part 3 - [Danger Signs and Don'ts.](https://jesswhite.co.uk/impactfuldashboardspart3-post/)

_Chapter 2 - A Practical Guide to Execution Level Dashboarding_

* **Part 1 - [Baselines for constructing development dashboards](https://jesswhite.co.uk/practicaldashboardingpart1-post/)** (_you are here_)

#### Referenced Blogs

1. [RED](https://peter.bourgon.org/blog/2016/02/07/logging-v-instrumentation.html)
2. [Four Golden Signals from the Google SRE book](https://landing.google.com/sre/book/chapters/monitoring-distributed-systems.html)
3. [USE](http://www.brendangregg.com/usemethod.html)
#### Videos 

---


<br/>
<div style="text-align:center; width:80%; margin-left: 10%;" markdown="1">
![step 1](../assets/img/logo.png)
</div> 
<br/>