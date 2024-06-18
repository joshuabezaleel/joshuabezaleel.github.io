+++
title = "1 Year in Infrastructure and Developer {Tooling,Efficiency,Productivity}"
date = "2024-04-10"

#
# A reflection of a year working in infrastructure and developer {tooling,efficiency,productivity}
#
# description = "An optional description for SEO. If not provided, an automatically created summary will be used."

tags = ["software","infrastructure","sre","platform"]
+++

Back in my previous company, I felt stuck. It's not my intention to point fingers but I was in a team where there were various features being built that it wasn't used even once after being pushed to production, and for me it's weirded since it was an internal tooling team expected to be used by other operations coworkers so I thought that this kind of problem should have a lesser chance to exist in the first place since the user is nearer to us. 

A team was then being created called the platform team with the main users of other engineers to help increasing the efficiency of the engineering flow. I applied to the team, going through the usual team-transfer flow, present project and alike, being interviewed, and got accepted. I felt thrilled since it has been a passion of mine to work in developer {tooling,efficiency,productivity} because I think that it (1) would be able to expose me to a more fun and exciting technical challenges and (2) the feedback loop is much faster and we're nearer to our users since it would be the other engineers that we interact on a daily basis, it's even much easier for us to dogfood what we're building ourselves. Even more, I believe lots of us enjoy being in the engineering role for the enjoyment of building things from scratch and to enable people in achieving that easier, for me it doubles the fun. 

Unfortunately, because of the company's situation, the team had to pause recruiting more members. 

Then I remembered I knew a senior from my university since I was involved in the Kubernetes community. The initial intention was to just have a coffee chat to at least have someone to talk with about me feeling stuck but turns out he had a vacancy on his team. I was sure that I wouldn't be able to get accepted in the team since there are a lot of people that I look up to. They are known, they have a voice, and they give back to the community, but above all, I knew they are kind, decent human being. Hence, I tried to make the leap of faith.

Fast forward a year (and a half, actually, since I joined on November 2022) from then. As someone who was thinking to start their career in non-engineering roles because he just wasn't born with the technical skill - which I finally did simply just because I don't want to die with what ifs - I would've never imagined I could say to myself that I am enjoying what I am working on a daily basis.

## What the team is working on
The team started as what was known as Payment Infrastructure, since it was responsible for the infrastructure of the "solely" Consumer Payment product on GoTo Financial subsidiary (of GoTo), which is mainly the GoPay digital wallet. Since (1) GoTo Financial comprises of various acquired companies ranging from Point of Sales, lending and installments, merchant gateway, and various other companies, with started with their own infrastructure and (2) our team had the considerably more mature infrastructure offering among others, we were also tasked to consolidate all of the other companies' services, databases, and all other product components to be onboarded on our infrastructure, hence renaming ourselves as GoTo Financial (GTF) Infrastucture.

We are comprised of 5 smaller teams. There is a Foundation team that handles all of the foundational (duh) layer of our infrastructure: Kubernetes, DNS, network, cert, service mesh, the list goes on. Automation is tasked for all of the stateful components - databases, cache, message queue - the applications are using. Governance governs the security, access, and cost. Observability offers and maintain the logging, metrics, alerting, tracing, and everything that helps the product engineering team to observe whatever is happening on the services that they are writing. And last, I was initially planned to be on the Developer Tooling team that should've maintain the centralized scheduler, libraries, and all other common things that the developers are using but no one is owning and maintaining it, but it was eventually merged to the Developer Experience team, where we also are responsible for the main CI/CD deployment tool and the Internal Developer Platform, where not only it is the (1) one-stop place for product engineers to start, build, and maintain their services, but also we enable (2) other team under the Infrastructure department to integrate their infrastructure offerings, out-of-the-box, on the platform that we maintain.

As a result, today, product engineers could start a codebase for their services, get various offerings of infrastructure starting from service mesh, publicly internet-accessible domain, PostgreSQL database and Redis, ELK logging and Prometheus metrics and alerting, cost visibility, secure and compliant, along with various deployment features like canary deployment and deployment preview, in just a few minutes.

My coworker already mentioned when they interviewed me that in my current role on the Developer Experience team that it would be comprised of 70% software engineering and 30% operations, whereas the other team would be perhaps the opposite of that, but one funny thing working in the Infrastructure department was that I would never be able to say exactly what is the exact term of my current role. I scoured LinkedIn and could see more than 5 variations of the term being used by my coworkers. DevOps engineer? People would've say DevOps is a culture not a role. Some says SRE. Other says Cloud Platform Engineer. Others are just Infrastructure Engineer. In another companies they have Developer Experience engineer. But in the end, it's a Software Engineering role that focused on improving the Developer Experience, and I enjoy it. 

## Infrastructure
When I was in university I wouldn't expected that I would be in engineering role, let alone to be in the infrastructure side of the software since I always had an impression that the infrastructure people are the special one among the rests, to be able to have knowledge down to the most complex ones enabling things to run smoothly. But turns out working in infrastructure, and especially with the intersection of Developer Experience, is something that I am enjoying for the following reasons.

1.  It lets you peek of the magic under the hood

    Alfred Aho said that computer science is a science of abstraction and I do believe, and grateful, that where we're all today are possible because we're standing on the shoulder of giants. Libraries, frameworks, and especially the gargantuan size of the infrastructure underneath. Working on this field gave me a chance to learn the things that we as product engineer usually take for granted. How are our services communicate with each other? Securely? What does it take to store and process enormous amount of data? How much does running software actually cost? How is metrics being scraped from what we've defined? And I must say, it's a heck lot of fun.

2.  Less prone to BS

    I am indeed positioned in one of the more opinionated side of the IT (I despise it generalized being called tech) community but there are lots of overglorification and hype in it followed by dramas and whatnots, solutions looking for problems, and things being built without having the societal impact to even be considered. Not that I'm saying that we should overlooked the social and other various aspects of IT - in fact we need way more of it - but sometimes the combination of it with how people are greedy with capital is what make me feel like it's an unhealthy one. 

    Whereas I think infrastructure folks are focused in making things work, making software run, accessible by users, reliable, and scalable. 

3.  Sharing - and enhancing - the joy of building

    This goes back to the one I mentioned in the early part of the article but I believe one of the things that makes people stay in this industry (aside from the pay, which is a very valid reason to be so) is the joy that they got in being able to just create and build things, which I think is something that is innate with being human.

    Being in infrastructure and developer experience/tooling enables you to also multiply that joy, since what you're building will be used by other engineers so they could get that feeling of joy so they can focus in what exactly they want to build. Regardless of whether you are in internal tooling team or a Developer Tooling SaaS, I think this feeling of joy is universal and something that I am really grateful of. 

4.  People and community

    Since the people are more focused on practicality (when I'm saying more, it doesn't mean that they don't have the hype here as well, we'll get that on different post) on getting things to run, and it's less likely that it will contain something that is business and application specific, I observe that the infrastructure people and community is much more open to be in discussion and sharing with one another, which we can see from the number of conferences and communities available regarding infrastructure. 

    I am also inbdebted for my career to the infrastructure community, specifically CNCF. I got both my previous job and also the current one partly because I - as a newbie - was very much welcomed to contribute to one of the CNCF projects, Porter, which I would want to pay a homage to the ever amazing late Carolyn Van Slyck. 

5.  Nearer to the whole company's system and culture

    Infrastructure - and developer experience - team members will be handling and maintaining the components and tooling that will be used by most, if not all, software engineers in your company. This enables us to take a broader look of how engineering is being run in the company. How services are being maintained by the wealth of teams, how it differs from one another and its overall architecture. The rituals, routines, SDLC, and characteristics on each and every teams. And moreover if you are lucky to be in a place where you're serving a lot of end-user, you'll get a chance to see various approaches on how to scale the system and where the system hits the liimt.


## Closing
I should've also mentioned that apart from being in the infrastructure team itself, I also enjoyed to be in where I am now because of the really great culture that the team proudly upholds. Everyone is not just technically brilliant but also kind and open and supportive. I am grateful to be where I am now and will enjoy the journey as much as possible.
