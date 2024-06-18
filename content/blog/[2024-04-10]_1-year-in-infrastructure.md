+++
title = "1 Year in Infrastructure"
date = "2024-04-10"

#
# A reflection of a year working in infrastructure
#
# description = "An optional description for SEO. If not provided, an automatically created summary will be used."

tags = ["software","infrastructure","sre","platform"]
+++

Back in my previous company, I felt stuck. It's not my intention to point fingers but I was in a team where there were various features being built that it wasn't used even once after being pushed to production, more so because it was an internal tooling team expected to be used by other operations coworkers so I thought that this kind of problem should have a lesser chance to exist in the first place since the user is nearer to us. 

A team was then being created called the platform team with the main users of other engineers to help increasing the efficiency of the engineering flow. I applied to the team, going through the usual team-transfer flow, present project and alike, being interviewed, and got accepted. I felt thrilled since it has been a passion of mine to work in developer {tooling,efficiency,productivity} since I think that it (1) would be able to expose me to a more fun and exciting technical challenges and (2) the feedback loop is much faster and we're nearer to our users since it would be the other engineers that we interact on a daily basis, and also it's much easier for us to even dogfood what we're building ourselves. Even more, I believe lots of us enjoy being in the engineering role for the enjoyment of building things from scratch and to enable people in achieving that easier, for me it doubles the fun. 

Unfortunately, because of the company's situation, the team had to pause recruiting more members. 

Then I remembered I knew a senior back in my university from the Kubernetes community. The initial intention was to just a coffee chat to at least have someone to talk with about me feeling stuck but turns out he had a vacancy on his team. I was sure that I wouldn't be able to get accepted in the team since there are a lot of people that I look up to. They are known, they have a voice, and they give back to the community, but above all, I knew they are kind, decent human being. Hence, I tried to make the leap of faith.

Fast forward a year (and a half, actually, since I joined on November 2022) from then. As someone who was thinking to start their career in non-engineering roles because he just wasn't born with the technical skill - which I finally did simply just because I don't want to die with what ifs - I would've never imagined I could say to myself that I am enjoying what I am working on a daily basis.

## What the team is working on
The team started as what was known as Payment Infrastructure, since it was responsible for the infrastructure of the "solely" Consumer Payment product on GoTo Financial subsidiary (of GoTo), which is mainly the GoPay digital wallet. Since (1) GoTo Financial comprises of various acquired companies ranging from Point of Sales, lending and installments, merchant gateway, and various other companies, with started with their own infrastructure and (2) our team had the considerably more mature infrastructure offering among others, we were also tasked to consolidate all of the other companies' services, databases, and all other product components to be onboarded on our infrastructure, hence renaming ourselves as GoTo Financial (GTF) Infrastucture.

We are comprised of 5 smaller teams. There is a Foundation team that handles all of the foundational (duh) layer of our infrastructure: Kubernetes, DNS, network, cert, service mesh, the list goes on. Automation is tasked for all of the stateful components - databases, cache, message queue - the applications are using. Governance governs the security, access, and cost. Observability offers and maintain the logging, metrics, alerting, tracing, and everything that helps the product engineering team to observe whatever is happening on the services that they are writing. And last, I was initially planned to be on the Developer Tooling team that should've maintain the centralized scheduler, libraries, and all other common things that the developers are using but no one is owning and maintaining it, but it was eventually merged to the Developer Experience team, where we also are responsible for the Internal Developer Platform, where not only it is the (1) one-stop place for product engineers to start, build, and maintain their services, but also we enable (2) other team under the Infrastructure department to integrate their infrastructure offerings, out-of-the-box, on the platform that we maintain.

As a result, today, product engineers could start a codebase for their services, get various offerings of infrastructure starting from service mesh, publicly internet-accessible domain, PostgreSQL database and Redis, ELK logging and Prometheus metrics and alerting, cost visibility, secure and compliant, along with various deployment features like canary deployment and deployment preview, in just a few minutes.

## Infrastructure
