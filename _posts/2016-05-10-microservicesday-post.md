---
layout: post
title: "Microservices Day"
description: "Microservices Day London 2016"
date: 2016-05-10
cover: "/assets/blog_header.jpg"
categories: [event, review]
comments: false
share: true
---
<br/>

----
<center>
<h3>Overview of Microservices Day London 2016</h3>
</center>
--- 
<br/>

### Common Themes:

* [Docker](https://www.docker.com/)
* [Cloud / AWS](https://aws.amazon.com/)
* [Canary Testing / Release](http://martinfowler.com/bliki/CanaryRelease.html)
* [Blue-Green Deployment](http://martinfowler.com/bliki/BlueGreenDeployment.html) 
* [SWIM](https://www.cs.cornell.edu/~asdas/research/dsn02-swim.pdf)

### Agenda

The [Agenda](http://microservicesday.com/#agenda) of the day included:
* [Fred George](https://twitter.com/fgeorge52) - How to enable organizations to go faster
* [Adrian Trenaman](https://twitter.com/adrian_trenaman) - Fighting the Good Fight at the Hot Gates of Micro-Services
* [Richard Rodger](https://twitter.com/rjrodger) - Solving service discovery: how Node.js microservices can find each other without a registry
* [Jason Melo](https://twitter.com/jasonmelo) - Microliths: how to avoid traps in your stack and your culture
* [Clifton Cunningham](https://twitter.com/clifcunn) - Micro-transformation
* [Anne Currie](https://twitter.com/anne_e_currie) - Microservices and Containers. How much faster than a VM
* [Valentine Gogichashvili](https://twitter.com/valgog) &  Fabian Wollert - Data integration in the world of microservices

### Ones To Watch

All of the talks are available on [Youtube](https://www.youtube.com/playlist?list=PL0CdgOSSGlBZkM4ZSGO0fjkNTXEIteQy9"). 

Below is a list of a few of my favourites:
#### [Richard Rodger](https://www.youtube.com/watch?v=9VC6YeQeZVk) - Solving service discovery: Node.js microservices without a registry:

This talk went through the lessons learnt by Nearform in there 5 years of working with microservices. Richard first stated that automated deployment is essential to be able to work efficiently with microservices. He also went on to praise [Netflix Eureka](https://github.com/Netflix/eureka) as an example of intelligent load balancing.

He argued that 'service discovery' is now an anti-pattern and that we should make message first class citizens, using them to define patterns. In this it should not matter where a message ends up or how it got there, only that a service is interested in something it contains.

He went on to discuss that each service should have a local view of itself, but there should be a self-updating global view using
                            [SWIM](https://www.cs.cornell.edu/~asdas/research/dsn02-swim.pdf) (Scalable Weakly-consistent Infection-style Process Group Membership Protocol). In this each service pings random services. This knowledge is then shared on to the next set of pings, and so the process continues. Using this process we can see which services are up and which are not. At convergence you get complete knowledge of the entire system and all this happens in milliseconds. This is useful for scalability and composability.    
An example of the implementation of a microservices architecture using Node.JS written by Richard can be found [here](https://github.com/senecajs/ramanujan). This is a Twitter like app that uses the Seneca microservices framework that is also a good example of the SWIM protocol for peer-to-peer discovery.

#### [Fred George](https://www.youtube.com/watch?v=WKTtnVb83mQ) - How to enable organizations to go faster:
Fred George is a pretty well known speaker, so admittedly I was excited to see him speak. In this talk he explored the hot topics surrounding microservices, which pretty much covered the common themes throughout the whole day. He then went on to discuss the [Cynefin Framework](https://en.wikipedia.org/wiki/Cynefin_Framework) and how it can be used to judge how profitable a solution to a problem may be as well as whether a company should use traditional or non-traditional methods to solve it.

He went on to discuss the 5 points which can help an organisation progress:
1. Understand your problem.
2. If it is a complex problem, you need to be able to fail fast as "experimentation drive innovation".
3. If it is a complex problem, re-think interactions - consider the interaction with customer at feature level rather than story level.
4. Measure what matters - expose developers to business success metrics, customer retention, clicks. Make the impact of their work visible.
5. Mitigate organisational inhibitors - this includes over-specialisation and too many managers, none of which have a clear overall picture.

Fred George also explored the hierarchy of development. Thought I saw his vision here, personally I am still a strong advocate for a flat structure.

A flat structure encourages the idea that everyone's view is valid, as the only difference between a senior / junior is their experiences, and as such both can have a valid point of view. Fred explored a much more hierarchical structure which rewarded knowledge - but personally I find such structures can introduce bad attitudes. 

####  [Jason Melo](https://www.youtube.com/watch?v=UAJuYs5PNqk) - Microliths: how to avoid traps in your stack and your culture

I love the term 'Microlith' which Jason used to refer to tightly coupled microservices. This is definitely a danger when moving from a monolith to a microservices architecture. In this talk Jason Melo discussed the journey from monolith to microservice in the following phases:

##### Phase 1a - Cultural mindshift: EMBRACE THE CHAOS! 
Everyone is involved in DevOps and it is not an individuals role! There will be well defined service ownership and LOADS of databases! Multiple run times!
These are factors which some may have difficulty with in the beginning.   

##### Phase 1b - Strangling the monolith:
Teams control their services with domain boundaries, guard rails and build pipelines. You can expect very high amounts of network chattiness dependent on synchronous REST. Elegant service discovery can make this process more smooth.

##### Phase 2 - Event Messaging over REST + Logging and Analytics:
Decoupling the microlith us difficult and investment in logging is VERY important. A transaction tracer can also be useful for seeing flow and can be used in conjunction with logs.

[Elasticsearch, Logstash and Kibana](https://www.elastic.co/products),  [Kafka](http://kafka.apache.org/), [Spark](http://spark.apache.org/) & [S3](http://docs.aws.amazon.com/AmazonS3/latest/dev/Welcome.html) are all examples of aggregated logging solutions. If you are using Blue-Green deployment, you can do real time log analytics on deployment using the same analytics platform.

##### Phase 3 - Scheduling and Orchestration:</b> 
[Jenkins](https://jenkins.io/), [Docker UCP](https://www.docker.com/products/docker-universal-control-plane), [Swarm](https://docs.docker.com/swarm/) on AWS, [Cloud Formation](https://aws.amazon.com/cloudformation/) and [Ansible](https://www.ansible.com/) - you need to work hard at getting persistence and scaling right! These can run distributed data streaming, messaging and analytics pipelines seamlessly.

It was interesting seeing how another company has approached the monolith to microservices journey and the tools they found useful. There seems to be many variations of this journey but a lot of the same difficulties are faced in each.

### Overview
Overall, for a free event, the quality of the speakers was surprisingly high. The venue was fantastic, the staff friendly and the general vibe was very open. As a conference, I would recommend it for both those wanting to explore moving into a microservices architecture and those that are established. It is good to learn from other companies wins and mistakes, but also there are a lot of practices and tools that may be useful.

Microservices Day did feel a bit like a practice for NodeConf, but it was free so I cannot complain about that. The talks all followed similar themes and towards the end of the day it started to feel like you had heard the same thing three times over - but I guess that it what comes from having a small area to talk about. 

It was interesting to hear about how companies had dealt with the transition to a microservices architecture and it was the first time I had come across SWIM protocol which I found a particularly interesting concept. The use of Docker in production, and the way in which companies were testing new functionality was slightly different from what I have experienced. There were a few things throughout the day that I think are worthy of further investigation, with the aim of eventually trying out some of them in my own work.                        


<br/>
<div style="text-align:center; width:20%; margin-left: 10%;" markdown="1">
<img src="{{site.baseurl}}/assets/img/logo.png" alt="Logo">
</div>