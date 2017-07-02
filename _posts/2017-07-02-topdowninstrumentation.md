---
layout: post
title: "Driving Instrumentation From The Top Down"
description: "A case study on driving monitoring through AC"
date: 2017-07-02
tags: [monitoring, instrumentation]
comments: true
share: true
---
 
_A proposed approach on how to make the most of instrumentation, uniting the development and business overview of products. Mostly academic, but this has been applied at work to test the theory._
 
##### The theory.
 
Monitoring is an expansive topic which I have gained a strong interest in this year. How to effectively log, instrument and alert is discussed at length and there seems to be no one true answer.
 
My experience so far with instrumentation had been dashboards built purely by developers. They decided the metrics to be measured, and what was to be shown on the dashboards. Sensible considering the dashboards were primarily used for diagnosis and to determine what needed to be alerted upon. There were however some issues including:
 
+ _Noisy dashboards_: In some cases, where there was no direction on what should be instrumented, dashboards contained unnecessary information. This made them busy and hard to read. Sometimes they would be trimmed down, but often this wasn't the case.
<br/><br/>
+ _Missing information_: In other situations the dashboards did not contain the information needed to spot problems early on.
<br/><br/>
+ _Neglected dashboards_: Dashboards were used in the short term. Once the feature was considered stable, they were only really used if considered useful for diagnosing the cause of an alert.
 
The full power of instrumentations wasn't being utilised. To address this we had a look into how dashboards can be useful to us. Some of the reasons we use dashboards include:
 
+ _Observing features are behaving as expected_.
+ _Observing the health of a feature_.
+ _Checking SLA's are being adhered to_.
+ _Being able to identify where problems are arising with ease_.
+ _Identifying areas to be optimised_.
 
Dashboards are useful not only to development teams, but also to other departments. A lot of the information we need on the dashboards align closely to the acceptance criteria of the epics driving feature development. If we were to build dashboards based from the acceptance criteria of these epics it avoids the issue of missing information. Further, it restricts the information to what is useful to those using the dashboards, decreasing unnecessary noise on the dashboards as well.
 
Finally, it was thought that we could change access to the dashboards. When features are first released, dashboards are monitored closely by development and are incredibly useful. Further, when there are alerts showing something has gone wrong in the system, dashboards are useful for quick diagnosis. If the dashboards are built from AC, we could provide access to the dashboards to teams the features matter to. This makes it more likely for abnormal behaviour to be spotted. As the teams invested in the features are more likely to recognise unusual behaviour they are more likely to notice strange behaviour. This helps the development team create effective alerts around things like how many customers hitting a service is extraordinarily high or low.
 
##### The application.
 
To try this theory out, first we had to get buy in from the business. The product owner was required to write extra acceptance criteria in order for this to work. They needed to get requirements from the stakeholders about what they want to know about each feature. This could include metrics such as the number of applications in a time period, time to process each application or whether we are sticking to third party / internal SLA's.
 
Once gained, the product owner included AC for instrumentation covering these requirements. By doing this, it ensured that these metrics would be included as part of the development work.
 
##### The results.
 
This process has been followed for a couple of projects now. In our case, it has worked well.
 
The first project was a backend feature integrating with a third party. The dashboard was shared with development and another team. It enabled both teams not only to spot bugs easily but also react to anomalous behaviours. Further, we could answer questions about response times with the third parties.
 
By driving our dashboards through business need, they are evolving in a way that benefits us, they are being viewed by those who need to see them, they have information that is useful to the business and greater buy in all round. Instrumentation is no longer a second class citizen & is being utilised again.
 
By no means do I think this is the right solution for all business'. Indeed I believe it still has a way to evolve where it is presently being used. Nonetheless, it has been undeniably useful in this case.
 
##### The future of this project.
 
These dashboards have been built using existing software, and as we move to using the Elastic Stack and its increased functionality, there is a lot more we can do.
 
The aim is to eventually build team specific dashboards as well as feature specific dashboards. For example, it would be great if the people on the phones have a dashboard they can understand that shows when certain features of the website goes down. These could be built based on stakeholder needs, and would give the whole company a clear overview on what is happening in the system.