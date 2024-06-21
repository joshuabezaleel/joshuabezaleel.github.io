+++
title = "Platform: why now?"
date = "2024-05-27"

#
# Why platform?
#
# description = "An optional description for SEO. If not provided, an automatically created summary will be used."

tags = ["software","devops","sre","platform"]
+++

Platform engineering has taken the infrastructure community by the storm in the recent days. Various talks on the recent KubeCons are mostly all about platform, on par with talks on AI. And as all hype should be, I am usually on the more skeptic side and I believe we should've taken them more objectively, not as is. Even though that I am currently working on the infrastructure and platform on day-to-day basis, I can really understand the POV of the people that are skeptic on this one and I believe that both gave really good perspectives on their corresponding point of views so it results in a healthy discussion in the community. One of the best take of platform was put by the one and only Kelsey [here](https://x.com/kelseyhightower/status/1760712390252089518).

On the benefit of establishing platform engineering, there are already a bunch of blogposts that talks about this, and perhaps you already have enough. The question was, if it might seem obvious that platform engineering practices will bring benefits not only to the infrastructure team, but also to the devops culture, delivery and developer experience, and the whole software engineering field, then why do we just have this now and not earlier? 

1. Product management has just reached its maturity state. The IT boom was not as old as we think and so does the science and art of how to build a software product. It started with the user-facing applications, which makes sense since it's what needed to keep the business afloart and the company running. 

2. In the past building software and maintaining it (operations) were used to be handled by 2 separate roles, the former by software engineer and the latter by sysadmin, which I am grateful of that we are past that era. And thanks to the growth of cloud computing field, we now are able to establish the DevOps culture of "you build it you run it" as coined by Werner Vogels. Even if we're getting better at handling infrastructure, most of the work are still being done ad-hoc without proper tracking and measurement through JIRA tickets and Slack messages which I think will easily burn infrastructure people out as it's not scalable, repetitive, it doesn't give a sense of achievement nor vision. Two of the articles that I really liked that talk about this was the "Human scalability of DevOps" by Matt Klein [here](https://medium.com/@mattklein123/the-human-scalability-of-devops-e36c37d3db6a) and "Everyone is not Ops" by Cindy Sridharan (copyconstruct) [here](https://copyconstruct.medium.com/the-death-of-ops-is-greatly-exaggerated-ff3bd4a67f24).

3. We just got the abstraction matured recently, which is the building block needed to be able to make thing that we call platform. Blob storage, DNS, compute engine, databases, and other abstractions through an API that is accessible for us to be used. Every part of the infrastructure could be weaved by us LEGO-like to cater to our company's custom usecase and needs.

Those three reasons in my opinion makes the reason of why platform engineering boomed the past few months and in the recent year. Companies has been building custom implementation of infrastructure engineering in their own companies and through open source communities and conferences, we are enabled to share knowledge between one another.

One of the caveat is that what comes to mind when people talk mostly about platform engineering was mostly an Internal Developer Portal (or what is known as IDP). Or is it the only way to implement platform? I'll try to talk about this in the next post as the reflection on personally a year and a half building one and 4 year since the team started their first commit.
