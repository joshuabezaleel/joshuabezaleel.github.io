+++
title = "How might you platform"
date = "2024-06-02"

#
# How might you platform
#
# description = "An optional description for SEO. If not provided, an automatically created summary will be used."

tags = ["software","platform"]
+++

This is some observation that I got on the practices that either infrastructure people that is going to start the journey in platform engineering or for people that have been practicing for a while that is looking for some lesson-learned from other companies. Will keep this list alive for a while in case there are new ones that I got.

1.  Proper width of abstraction

    Premature optimization is the root of all evil. And so does chunky abstraction.

    We as the infrastructure team would have used some method of abstraction as the point of interaction with our customers, product engineers, as our means to organize and maintain the whole underlying infrastructure. Some use a JIRA ticketing, some use documentation and Pull Request, some use a centralized repository and pipeline template, and even a Slack channel and conversation is a valid abstraction and means of interaction. The hippiest thing nowadays? You guess it. Internal Developer Portal maintained by Platform Engineering team. By the time you are reading this article I hope you have already came across and read or watch any talk about how platform is not necessarily have to be a portal.

    But unfortunately, chunky abstraction could also even exist in our .

    Kubernetes Operator.

    Cari yang paling bermasalah dan time-consuming. Drill down on that. Built a PoC, the thinnest and MVP one. Iterate on it. Only add abstraction if necessary. 

2.  Captive audience

    TBA

3.  Shared responsibility model

    TBA

4.  Keep your allies (power-users) close

    TBA

5.  Usually they already had an existing something to scratch their own itch

    TBA

6.  Standardization with golden path, but be open to experimentation and ideas

    TBA
