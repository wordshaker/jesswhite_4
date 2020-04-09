---
layout: post
title: Service Levels.
description: "Objectives, Agreements and Indicators"
date: 2020-04-09
cover: "/assets/blog_header.jpg"
categories: []
comments: false
share: true
---

----
<center>
<h3>  </h3>
</center>

---
<br/>

In order to know if a system is working, we have to know what working looks like and how to measure it. This is not only a technical concern, but also includes if a system meets a product or business need. The user and client experiences of interacting with these systems also need to be factored. 

How can we measure a system in a way that satisfies all these concerns? This is where Service Level Objectives (SLO), Service Level Agreements (SLA) and Service Level Indicators (SLI) come into play. These measures are explored <a href="https://landing.google.com/sre/sre-book/chapters/service-level-objectives/" target="_blank">in Chapter 4 of the Google SRE (Site Reliability Engineering)</a>

Determining these measures can be more difficult than first anticipated and they will change over time. Nonetheless, the are important to track.

> _"These tools aren’t just useful abstractions. Without them, you cannot know if your system is reliable, available or even useful. If they don’t tie explicitly back to your business objectives, then you don’t have data on whether the choices you make are helping or hurting your business." - Google SRE Book_

In this post, we will go through how these measurements are linked, what they are and how they can be defined and measured. 

### Quick definitions

- **SLO :** Measures of expected behaviours of the service. These are measured by SLIs.
- **SLA :** Contracts of the consequences of missing the SLO's agreed with consumers, users and other parties.
- **SLI :** A quantifiable measure of some level of service provided. Help to measure if SLAs are met.

### How these are linked

SLOs are agreed in terms of business and product requirements. They are how the a service is expected behave as a good average, and not be a measurement of perfection or stretch goals. 

These help when agreeing SLAs. By knowing what the expected behaviour of a service or system is, you can then set reasonable and achievable SLAs with your users, clients, consumers and third parties.

Whether SLAs and SLOs are met and achieved are measured using SLIs.

<br/>

---


# Diving into each 

Now we have established the basics of what each are and how they are connected; lets dive into each of them in a bit more detail. 

## Service Level Objective (SLO)

The top tier of these measurements and contracts is the Service Level Objective (SLO). An SLO sets the expectation for how available a service is and how it should perform. by no means are SLO's purely technical measurements. They require the input of a business and should be linked to both product and overall business expectation.

SLOs are measurable, numerical values of system availability/reliability. They go hand in hand with error budgets, which are targets for the maximum amount of time a service is unavailable/unreliable in a quarter.

When it comes to discussing work, a team and product can refer back to SLO's to help determine it's value and purpose. This is assuming it is a well defined "good" measure which doesn't increase work for a team because it's too stretched.

### Determining SLO's

There are a number of factors when defining and determining SLOs. As mentioned SLOs have tie in business and product need, as well as the technical considerations such as feasibility of measurement and cost. 

<strong>Simple and discrete</strong>

Ideally, there should be a limited number of these measures and they should be measures that aren't over complicated. The more complex the measurement and the more moving pieces, the more likely it is that something will be missed or misinterpreted. Likewise, too many measures hide what it is important and can be difficult to keep track of. 

<strong>Not a measure of perfection</strong>

As mentioned previously, SLOs are measures of what is expected of the service. Common mistakes with SLOs are to set them too high or too low. 

SLOs are meant to be achievable, not set as stretch goals or what the system can achieve in a perfect world. If you are rarely or never achieving an SLO, it defeats the purpose of having it as a measure of if the service is meeting it's expected behaviours to be "available".

As with everything in life, perfection is always impossible. There will be downtime due to errors, deployments and more which call lead to a loss in availability. Likewise, the expectation that things will never fail can cripple innovation and experimentation, which can be detrimental to progression. It's worth accounting for these as part of determining your SLOs.

Likewise they should be a measure that is too low. When a service is demonstrating behaviours which are considered problematic or broken to users or a business need, SLOs shouldn't pass.

<strong>Costs versus reliability</strong>

One of the reasons why perfection is unattainable is that is it is expensive. Operation costs increase the more reliable and available you want your service to be. As such, it is suggested in the Google SRE book that the lowest level of reliability that can be achieved while still making dependants, clients etc happy with the level of service should be stated as an SLO.

Likewise with other SLOs, the cost of achieving them should be accounted for. If to achieve an SLO the service needs rewriting, a system rearchitecting or an unachievable budget requirement - it's not a suitable SLO.

<strong>Flexibilities of measures</strong>

Over time a services purpose can change as can the expectations of that service. For example change in code or tooling could change the level of average performance. Likewise, there can be additional or reduced features from product. Over time it is best to review and adjust SLOs and related SLAs and SLIs. 

<strong>Accounting for error budgets</strong>

Error budgets are explored <a href="https://landing.google.com/sre/sre-book/chapters/embracing-risk/#xref_risk-management_unreliability-budgets" target="_blank">in Chapter 3 of the Google SRE (Site Reliability Engineering) Book.</a> They are closely tied to SLOs. It is a metric covering how much time in a quarter a service can be "unreliable".

This budget accounts for down time due to deployments, production issues and unexpected events. As previously mentioned, an SLO of 100% availability and reliability isn't possible, but we can plan and aim for achievable goals and measures.

### Setting SLO's

### Transparency

----------------

## Service Level Agreement (SLA)

### Setting SLA's

## Service-Level Indicator (SLI)

### Setting SLI's

---

# Worked Example



# References

- <a href="https://landing.google.com/sre/sre-book/chapters/service-level-objectives/" target="_blank">Google SRE - Chapter 4 Service Level Objectives</a>

- <a href="https://cloud.google.com/blog/products/gcp/sre-fundamentals-slis-slas-and-slos" target="_blank">SRE fundamentals: SLIs, SLAs and SLOs</a>

- <a href="https://cloud.google.com/blog/products/gcp/availability-part-deux-CRE-life-lessons" target="_blank">SLOs, SLIs, SLAs, oh my - CRE life lessons</a>

- <a href="https://docs.honeycomb.io/working-with-your-data/slos/" target="_blank">Define and manage Service Level Objectives (SLOs)</a>

- <a href="https://www.circonus.com/2018/07/a-guide-to-service-level-objectives/" target="_blank">A Guide To Service Level Objectives, Part 1: SLOs & You</a>

---

_Jess_

---


<div style="text-align:center; width:20%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/logo.png" alt="Logo">
</div>
