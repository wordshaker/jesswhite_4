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

SLOs are measurable, numerical values of system availability.

### Determining SLO's

There are a number of factors when defining and determining SLOs. As mentioned SLOs have tie in business and product need, as well as the technical considerations such as feasibility of measurement and cost. 

<strong>Not a measure of perfection</strong>

As mentioned previously, SLOs are measures of what is expected of the service. Common mistakes with SLOs are to set them too high or too low. SLOs are meant to be achievable, not set as stretch goals or what the system can achieve in a perfect world. If you are rarely or never achieving an SLO, it defeats the purpose of having it as a measure of if the service is meeting it's expected behaviours to be "available".

Likewise they should be a measure that is too low. When a service is demonstrating behaviours which are considered problematic or broken to users or a business need, SLOs shouldn't pass.

<strong>Simple and discrete</strong>



<strong>Costs versus reliability</strong>

<strong>Flexibilities of measures</strong>

<strong>Accounting for error budgets</strong>


### Setting SLO's


### Transparency


----------


- "However, if you simply start with what’s easy to measure, you’ll end up with less useful SLOs. As a result, we’ve sometimes found that working from desired objectives backward to specific indicators works better than choosing indicators and then coming up with targets."


- "Keep in mind that the more reliable the service, the more it costs to operate.  Define the lowest level of reliability that you can get away with for each service, and state that as your SLO."

- "whether your service needs to be made more reliable (increasing cost and slowing development) or less reliable (allowing greater velocity of development)."

- "It’s both unrealistic and undesirable to insist that SLOs will be met 100% of the time: doing so can reduce the rate of innovation and deployment, require expensive, overly conservative solutions, or both. Instead, it is better to allow an error budget—a rate at which the SLOs can be missed—and track that on a daily or weekly basis."

- "Choosing targets (SLOs) is not a purely technical activity because of the product and business implications, which should be reflected in both the SLIs and SLOs (and maybe SLAs) that are selected."

- Don’t pick a target based on current performance
While understanding the merits and limits of a system is essential, adopting values without reflection may lock you into supporting a system that requires heroic efforts to meet its targets, and that cannot be improved without significant redesign.

Keep it simple
Complicated aggregations in SLIs can obscure changes to system performance, and are also harder to reason about.

Avoid absolutes
While it’s tempting to ask for a system that can scale its load "infinitely" without any latency increase and that is "always" available, this requirement is unrealistic. Even a system that approaches such ideals will probably take a long time to design and build, and will be expensive to operate—and probably turn out to be unnecessarily better than what users would be happy (or even delighted) to have.

Have as few SLOs as possible
Choose just enough SLOs to provide good coverage of your system’s attributes. Defend the SLOs you pick: if you can’t ever win a conversation about priorities by quoting a particular SLO, it’s probably not worth having that SLO.17 However, not all product attributes are amenable to SLOs: it’s hard to specify "user delight" with an SLO.

Perfection can wait
You can always refine SLO definitions and targets over time as you learn about a system’s behavior. It’s better to start with a loose target that you tighten than to choose an overly strict target that has to be relaxed when you discover it’s unattainable.

SLOs can—and should—be a major driver in prioritizing work for SREs and product developers, because they reflect what users care about. A good SLO is a helpful, legitimate forcing function for a development team. But a poorly thought-out SLO can result in wasted work if a team uses heroic efforts to meet an overly aggressive SLO, or a bad product if the SLO is too lax. SLOs are a massive lever: use them wisely.

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
