---
layout: post
title: A Practical Guide To Dashboarding Part One
description: "Introduction To Baselines for Dashboards"
date: 2019-01-30
cover:  "/assets/img/2018-04-23/header.png"
tags: [monitoring, instrumentation, dashboard]
comments: false
share: true
---

----
<center>
<h3> Introduction To Baselines for Dashboards. </h3>
</center>
--- 
<br/>

Everybody uses dashboards and graphs in every day life. From using modern banking apps like Monzo or Starling which display your spend rate graphically, to people managing their heating using an app.

### Learning from car dashboards

In previous posts I've written about how the car dashboards are, in my opinion, one of the best designed visual displays of information. I've written about a couple of aspects of car dashboards we can learn from and adapt to improve the visualisations we create to display the state of our systems - software, hardware, business or otherwise.

#### Previously, we've explored that information on a dashboard should have the following properties:

- **The way in which information is shown should be clear.**

When you sit in a car, you know the big dial is the speedometer. You know this information is displayed in real-time and what that dial is showing. You know how to read the speed you are going at in real time.

This is the same for the majority of information on a car dashboard. You have an idea of where the information you need is displayed, how to interpret the way in which it is displayed and this doesn't take much time or cognitive effort to figure out. 

The information on dashboards should be clear and unambiguous.

- **Information should be actionable.**

There are a couple of aspects to this. Firstly, the information displayed on a car dashboard is the information you need in order to drive safely and keep the maintenance of the car up. There isn't any information displayed that is for _interest_. Only information that is necessary and actionable.

Secondly, information is displayed in a way that the driver knows:

- What the information means.

- What action needs to be taken.

- How quickly the situation needs to be reacted to.

- The rough impact/effects if the information is not reacted to.

This helps with prioritising the actions to the information being provided. Speeding - you need to react quickly, you need to slow down, if you don't the consequences can be severe. If your indicator lights are on and you aren't turning - you don't need to react as quickly, you need to turn the indicator of, the consequences are less severe than speeding, but still not great.

#### In my impactful dashboard talks I've also hinted upon:


- **The urgency of the action should have an effect on how it's displayed.**

- **Dashboards should be contextual**

#### There is another characteristic of car dashboards that I'd like to explore.

If you are familiar with cars, whether that's as a driver, a passenger or otherwise, when you look at a car dashboard you know what the information displayed to you means very quickly. Car's do differ slightly on the design of their dashboards, but you know what the speedometer will look like, and roughly where to look for it. It's easy to find the oil gauge, the notification lights, the warning lights. No one needs to explain the dash to you, where to find the information you need, or what each dial and light is representing.

> Car dashboards have a base level of information they always provide.

This is a powerful characteristic of car dashboards. There is a standard baseline of information. There is a standard way in which certain information is displayed. Because of this, it is easy to get the information you need when driving any car, even when there are slight differences in design. 

What if we applied a similar idea to the dashboards and visualisations that tell us about the state of our software, infrastructure? It could be the case that by having standards for how we demonstrate information, we can make it easier to share information or work across teams. For example, a developer could go from one team to another and be able to understand the high level state of domain by looking at their dashboards, because API/service metrics are displayed the same way in the other teams they have worked in. Likewise other teams and other technical departments would be able to interpret these boards easily, and without assistance if needed.

### Standardised Baselines

This is not a new idea. Personally, I have used baseline information in teams I have worked in. In infrastructure, it's even more common. If you are using AWS or Azure for example, they have in-built standards for monitoring certain things which you an use.

In this series of posts, I will talk through baselines that I have tried and practiced as Software Developer. With reference to the original authors of these patterns, I'll explain why the information is powerful and how it can be used. As with all my posts, this is personal experience. I'm not saying it's right or wrong, but it's something I have found valuable.

I plan to only talk through API's and Services for now, as these are the areas I have the most experience in. There are similar standards out there for other areas of monitoring - front end, security, databases etc. If you are intrigued by the idea of having standards for dashboards, I encourage you to look into what is applicable for your needs and maybe send good resources my direction.

### Metrics vs Diagnostics


---

_Chapter 2 - A Practical Guide To Dashboarding Series_

* <strong><a href="{{site.baseurl}}/2019/03/30/practicaldashboardspart1-post.html">Part 1 - Introduction To Baselines for Dashboards</a></strong>

* Part 2 - Baselines for Services. _coming soon_

* Part 3 - Baselines for API's. _coming soon_

---

---

_Chapter 1 - Creating & Maintaining Impactful Dashboards Series_

* <a href="{{site.baseurl}}/2018/04/09/impactfuldashboardspart1-post.html">Part 1 - Creation of impactful dashboards</a>

* <a href="{{site.baseurl}}/2018/04/22/impactfuldashboardspart2-post.html">Part 2 - Continuous Maintenance.</a>

* <a href="{{site.baseurl}}/2018/04/23/impactfuldashboardspart3-post.html">Part 3 - Danger Signs and Don'ts.</a>

---

<div style="text-align:center; width:20%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/logo.png" alt="Logo">
</div>