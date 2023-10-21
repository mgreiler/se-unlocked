---
episode: "Transcript Episode 75 Luca Galante"
permalink: /platform-engineering
status: publish
type: transcript
---

[00:00:00] **Michaela:** Hello and welcome to the Software Engineering Unlocked 
Podcast. I'm host Dr. Greiler, and today I have the pleasure to talk to Luca 
Galante, who will talk with me about platform engineering. 

But before I start, let me tell you about an amazing opportunity that allows you, yes, you, 
to earn additional income! 

Do I have your attention? Yes? Great. So, Userinterviews.com is a company that connects researchers 
with study participants. And they especially are looking for developers that share 
their feedback on products. 

So, share your opinion with top brands such as Spotify, Amazon, Adobe, and many many more, and get paid. 
Most studies take less than one hour to participate and pay over $60. 

So, sign-up today - It’s totaly free - apply to give feedback for products that interest you, 
and make a nice side income. Additionally, you help to shape the future of the tools we all use. 
So, What’s not to like, right? So, are you ready to earn extra income by sharing your expert opinion?head over to [userinterviews.com](https://www.userinterviews.com/hello) to signup and participate today.

But now back to Luca. Luca is leading 
product at Humanitech and so hundreds of DevOps and platform setups, and he 
condensed all his learnings into his weekly newsletter that's called Platform 
Weekly, which has, which has 10,000 subscribers.

He's also the core contributor to the platform engineering community that has 
more than 10,000 meet up, uh, members, more than 8,000 Slack members. And 
they're also having a platform con. This is a conference about platform 
engineering that has over 6,000 and attends in just one day. Well, so I think he 
knows

He knows a lot about platform engineering. I will pick his brain today. So I'm 
so, so happy that you're here, Luca with me today. Welcome to the show. 

[00:01:24] **Luca:** Thank you. Thank you for having me. 

[00:01:26] **Michaela:** So, um, I asked people today before having this, uh, 
conversation with you, I asked them, so what do you think about platform 
engineering

And they were like, what? platform, what?what is that? Platform engineering. 
Yeah, exactly. Um, so can you maybe outline a little bit what is platform 
engineering? And um, I actually noted it's a little bit of a hype now. Why is 
that? What is it and why is it a hype right now? 

[00:01:53] **Luca:** Yeah, absolutely. Um, so platform engineering, I, I define 
it as the science, but really the art as well of designing and really bringing 
together all the different tech and tools that you have in an organization, 
especially you're kind of mid-size, large size enterprise engineer organizations and bring 
all of that tech and tools into one golden path that enables, um, developers 
sell service and at the same time reduces the cognitive load on the individual 
developer and the individual contributor. And so these golden paths, um, are 
most often referred to as an internal developer platform or IDP.

and that IDP is built by a platform engineering team or internal platform team, 
or platform team. And uh, the, the kind of like the key principle of of platform 
engineering is platform as a product, which means you have a platform team that 
is really a, works as a product team and ships a product, which is the platform 
to the rest of the engineer organizations.

Um, who are their customers? The, the developers. So developers are their 
internal customers, and that is really one of the, kind of like the key 
differences to something like SRE, which is mainly focused on, you know, 
reliable production systems, really, and DevOps, which is a culture or 
philosophy. Um, never meant to be, it was never meant to be a job role technically.

Um, and platform engineering is really a, a new, a new discipline, 
right? That actually hopes to. Um, bring to live, uh, the, the initial tenant of 
DevOps, which is you build it, you run, and, and so, If we, you know, if we 
think about, you know, DevOps, uh, cause I think this is important context to, 
to understand, you know, where platform engineering fits in the, in the, kinda 
like in the broader scope of things.

You know, DevOps, you know, it came up more than probably 10 years ago at this 
point. And, and when it did, the word was at very, very different place. Right? 
We, we were mainly working on monoliths, running on bare metal. Um, the 
infrastructure that we were running. Insanely less complex than it is right now.

You didn't have Kubernetes GitHubs, you didn't have, you know, the CNCF Cloud 
native tooling landscape, which is like hundreds or thousands of different tools 
that nobody really understands how they fit together and, You know, and, and so 
the, the time is really different, right? And, and the initial idea behind 
DevOps is quite simple and, and is great, right?

It's, is to remove barriers between developers and operations and facilitate 
collaboration between them. But the issue is, in reality for many organizations, 
uh, what that turned into when you consider all this converging trends of GitHubs, 
cloud Native Kubernetes, iac, and so on and so forth, is a world where, you 
know, developers are overwhelmed.

You know, they are overwhelmed by this extra cognitive load that is created by 
all these tools, very complex tool chains, where now just to do a simple 
deployment. To, you know, a preview environment. You wanna just like, say those 
two things in one sentence. In some engineer organizations, especially at large 
scale, that can take, you know, weeks.

Cause you need somebody to provision your, uh, you know, a database and set up 
your, um, you know, your preview environment. And then, you know, and, and only 
then you can like start touching like 10, 15 different like tech tools or 
complicated scripts just to do one simple deployment, right? And so what that 
results into is on the one hand, you know, waiting time and frustrated 
developers that are just like too afraid of touching all this, you know, 
spaghetti configuration stuff that they don't wanna mess up.

And on the flip side of that, you have operations or DevOps in some cases, 
teams. That are completely overwhelmed and you know, are basically just trying to put 
out fires and fighting constantly taking ups and, and so when we at Humanitech 
looked at this, you know, our, our funding team comes from, you know, people who 
built, uh, the platform, Xing, which is a big, you know, kind of like LinkedIn 
competitor in Europe that never really took off, but it's still a very new company.

Um, our CTO actually built one of the platforms at Google and you know, we 
realized that in this whole DevOps revolution, what leading. Engineering 
organizations were doing was building platforms cuz they immediately realized, 
hey, there is no way that we can, you know, onboard hundreds or even thousands 
of developers like they were doing every day.

Um, but, um, you know, and expecting everybody to understand this full, you 
know, super complex, increasingly complex cloud native setup. And so we need 
some sort of platform layer here to enable developer self service on the one 
hand, and then make ops slightly easier on the other. and that's kind of where platform 
engineering was started.

And this is where we started also doing the work on our community that happy to 
talk more about. 

[00:07:13] **Michaela:** Okay. So, um, let's, let's dig a little bit deeper and 
I want to, you know, decompartmentalize a little bit what you were saying right 
now. Um, So we have DevOps on one end, right? Where, um, there was this strive 
that developers also run the code, right?

So that you're not throwing code over and then another person or another team is 
reliable for even to test it, right? So I think everything came a little bit 
more closer together over the last, let's say 15 years, right? So, uh.
Developers took over more responsibility for testing the code, but also for 
running the code, but then for shipping the code, right?

Um, and so now that we have this so close to us, uh, but we have more tooling, 
it becomes extremely complex. Right. So , if, if you are a developer, you should 
be good, let's say in in in JavaScript and React. And you should know maybe some 
backend, and then you should know some databases. And then you should also know 
Kubernetes.

And I think then already your, your world explodes, right? Um, right. And then 
maybe some monitoring and some observability and so on. So it becomes extremely 
complex and I think there's not one person that can know everything. And even 
for teams, it becomes a complex, uh, way to do it. . And what you are telling 
me, I think, is that there are all these tools and then we put them together 
like pieces and puzzles and then maybe have some scripts that, you know, glue 
that together.

Um, and then it becomes brittle also and difficult. And so platform engineering 
teams emerged a little bit out of this need of making that more structured, more 
systematic, and also having an owner that. Takes over the architecting such 
systems that are based on tools and, and, and, and already, you know, 
technologies, whole technologies that are actually coming into that.

Is that, is that a correct understanding of what platform engineering is? 

[00:09:06] **Luca:** Yeah, you said it really well, . Okay. I have another 
question for you. I couldn't said it said it better myself. , 

[00:09:13] **Michaela:** what you are also talking is DevOps and then site 
reliability. Site reliability, engineering, right? Mm-hmm. . But another thing 
that comes up in my mind, especially because I've worked on that over the last 
two years, is develop experience.

And I see a lot of, um, platform teams that you're talking about, right? Those 
platform from teams also being interested in develop developer experience, 
right? Because we want to make the life of developers easier, right? We want, we 
want them not to sweat because, you know, uh, they can't deploy, right? They 
want, we want them to ship code really, really fast.

Um, but I think the idea of really calling it something. Straight out like 
telling, saying it's it's developer experience and we are also responsible for 
that. Um, is another task. Do you see that, that people are really interested in 
that or is it only a part of the developer, uh, the, the platform engineering 
folks that are interested in Devero developer experience?

What's your perspective on, uh, perspective on that? 

[00:10:13] **Luca:** Absolutely. Yeah. That is, I think the most important thing 
that platform teams need to care about is, you know, building that really tight 
feedback loop with their developer teams, the development teams and, um, you 
know, make sure that they really optimize for their day-to-day developer 
experience.

Right. And that is where it's so important that you treat your platform as a 
product that you're shipping. and you treat developers as your internal customers. Cause 
otherwise that flow, that feedback loop breaks. Um, and so, you know, what we 
see in the community and in the marketing in general, successful platform 
engineering teams do is.

You know, they treat the platform as a product. As we said, they have this 
really tight feedback loop with developers. They also have a really clear 
mission and role, which is stated and almost internally marketed, as you know, 
clearly different from a DevOps or SRE team, right? So, um, your mission is not 
simply.

Um, which is not necessarily simple things, right, but, um, is not to, you know, 
worry about maintenance and reliability of your systems is to, you know, 
improve, you know, the dev developer experience continuously of all the 
development teams, whatever it is, you know, that is, there needs to be a clear 
mission.

That is communicated to the rest of the engineer organization to position the 
platform team and make sure and set them up for success. That's really 
important. Um, the other thing that we see Plat, you know, successful platform 
teams do is. Um, you know, focus on common problem and really focus on this like 
minimum and common denominator across the engineering organization, right?

And so when you're thinking about rolling out a platform, you know, how do you 
win over your, your developers, like of course you wanna focus on developer 
experience, but you know, How do you, um, how do you make sure, you know, you 
can't, you can't usually roll out to like hundreds or thousands of developers or 
at once.

And so it's really important to focus on that set of problems that you see 
across, you know, the board there is where, where the, the most pain lines, and 
again, that only comes from like surveys. You know, just general, you know, 
traditional product research, really talking to your customers and then, you 
know, iterating on the features, iterating on the features, and make sure that 
you don't reinvent the wheel all the time.

Um, but you know, you brought up earlier this idea of glue that's actually. A 
really, really valuable part, um, of, of the job, of platform teams is really 
gluing together their, you know, what is a very complex tool chain into one 
golden path that makes sense. And I think crucially. , you wanna provide 
developers with a choice of what is the right golden path for a path, right?

So as an example, what you said, right? You have, you might have, you know, a 
lot of, um, you know, front-end, like a junior front-end engineer that really 
wants to worry about react JavaScript and nothing, and not too much more than 
that. , right? So they don't care whether you're running on E Ks, G K E, which 
region, like they don't care about any of that, right?

And so for them, you might want to build a really, you know, high level, high 
obstruction, golden path that just lets them, you know, easily deploy a test, a 
small change to their dev environment. And that's it. But then you also might 
have somebody like a, you know, senior backend engineer that really loves 
messing out, messing around with her helm charts and um, you know, yamo files 
and so on.

And so what you wanna provide to them in that case is, you know, the ability of 
going off path, the ability of, you know, messing around with like lower level 
stuff. And so, you know, What we advocate for in the platform engine community 
is really a, you know, a toolbox that, um, you know, platform teams use.

There is an opinionated toolbox to build opinionated golden path. Why? 
Because you, there's no better person than your platform, your own platform team 
to understand what is the right level of instruction and what does a golden path 
really means for, um, our organization. 

[00:14:44] **Michaela:** So I have, uh, many questions. I wrote down actually 
four that are really important, so we have to cover all of them.

Um, the first one I started with, the first one is that, Uh, how long is it to 
go ? 10 years ago? You know, uh, I, I would say I was in the platform team a 
little bit different. I think it's not exactly the same. Um, maybe I was more in 
a, ah, it, it's really early days right? Back then. Right. So, but I was working 
at Microsoft and um, at that point it was called, um, tools for software 
engineers team.

Right? So we were providing mm-hmm. , the tools for the software engineers. Um, 
but what I have seen there, and then actually my team was. Reorged, uh, because 
it grew and grew and grew, right? It became more and more important into one ES 
one engineering system, which I think, you know, it's a little bit, this idea of 
first we wl were responsible, responsible for making the build faster 
for, for, you know, the large organization, which sounds trivial, but if you're 
running Microsoft, uh, for example, a Windows, it's not that, right?

Uh, you know, you can really spend some time to optimize this build time or we 
were making testing faster or more reliable or, So we were working with 
different teams really on those problems that they were seeing with testing, 
with build, um, with, with, uh, code ownership and so on. Um, and then it was, 
uh, because it was becoming more important, it became this a large one ES team, 
right?

One engineering platform. And I have seen at that point that a lot of companies 
tried to, especially larger companies, tried for from this very scattered 
landscape, right? This team is doing it that way. This team is doing it a 
little bit different. They are using a very different tool, Jane, into this one 
engineering system where you say, well, an organization with 200,000 people 
should all have the same tools, right?

Right. I think people went a little bit away from that. Uh, but there's still a, 
a, a little bit of, of this idea, which is I think, different from what you were 
saying. Right. So, um, you were saying listen to your customers. Um, where, what 
I have seen, um, in the early days, it was more a top-down approach, right?

It was like we want Git, for example, right? So now we have, you know, this tool 
or we have this hammer, let's, let's put it that way, right? We have this 
hammer, uh, that works very well and we want everybody to use it, right? 
Independent of their situation. Um, or we want, you know, that everybody does 
this, uh, you know, does something this way so that we can keep knowledge and 
you know, it.

Stream, like processes and so on. Um, do you still see that or, um, is there 
really this focus on, well, uh, depending on what our, you know, customers need 
and how is our internal developers within a com company I can have as scattered 
or a, a complex and, you know, uh, a landscape as it's not uniform, not 
coherent.

[00:17:37] **Luca:** Yeah, so it can definitely not be a top-down approach. 
Right. And in fact, I was having an interesting conversation this morning with 
somebody about this, where, you know, we were saying, hey, would the ideal 
scenario for a platform for a new platform team. Be, um, Greenfield, right? And 
it's like, kind of like, cuz from a, a purely theoretical standpoint, you, you'd 
argue yet, right?

Like, oh, you can choose everything, right? You can pick your perfect stock and 
like design all the flows and so on. But the issue is, the, the issue with that 
is then you're already going kind of like the password, which is basically 
saying, , I know what's best. Mm-hmm. , right? Um, and then you, you'll all need 
to like, kind of just like fit into this like, mold that I've created for, for 
this platform.

Whereas the, I think the, the ideal scenario actually, and, and frankly what we 
see in the vast majority of cases in practice is, you know, you have a, a 
brownfield complex enterprise setup and now you wanna roll out the platform 
initiative, which means we already have, you know, tens of development teams with 
their own stack, right?

Like these people prefer using, um, you know, Argo cd. These people prefer using 
Argo plus Jenkins. This is like Circle CI and something else, right? So, Um, now 
that's where you understand as a platform team, if you listen right and, and 
you, and you look closely, that's where you start understanding, okay, um, I can 
see some pattern, I can see some preferences.

I understand I talk to them, right? And this is where you start formulating an 
idea of what this like minimum common denominator is. And that is the starting 
point of your platform. And I would argue that it's probably actually a better 
starting point. It might be a more difficult one and a more, a more laborious one than, 
Hey, we can start from scratch and just dream up the ideal platform.

But I think is something is, is, is one that in the long run will probably, um, 
you know, come closer to what the developers actually want. And so I think 
that's actually the, the, the best way of, of approach. 

[00:19:45] **Michaela:** Another trend and I think, yeah, something that evolved 
over time. When I look at, you know, how, how platform engineering or whole this 
industry somehow, uh, formed itself, is that like 10 years back, I only saw 
people doing what I'm doing.

At large organizations, you know, I saw people at Microsoft. Yes. I saw them at 
Google. Even Spotify was too small at that point. Right, right. And now I see 
platform engineering teams and the interest for that also at medium size 
companies or startups. Um, maybe not at two person show right. . Um, um, but uh, 
you know, like if they have.

I don't know, what's the numbers? 50 people. It could be that there is already 
somebody responsible for, for doing that. Right. 50 engineers or something. Um, 
do you see the same trend? Is it also, is it something that just large 
organizations do or is uh, is platform engineering and thinking about developer 
experience and this common denominator and so on, is that something that smaller 
organizations should care?

[00:20:49] **Luca:** Yeah, it's a great question. Um, and actually you said I 
think the right number, uh, it's about 50 , I would say, uh, you know, 30, 50. 
That's when I think you start seeing the things breaking, right? Because you 
have two, I think you have two scenarios below that threshold, right? Like, 
either you have, you know, people are saying, all right, like, I'm just gonna go 
with the path, like something that, you know, maybe like five or 10 years ago 
could have been like in Heroku for instance.

Now you have a bunch of other solutions for that. Or like, As a service type of 
things. Um, and that, those are great for, you know, those, those like smaller 
use cases, the problem is they don't really scale, right? Like when you start 
wanting to have those different golden paths that we were talking about earlier, 
then it becomes really hard because that toolbox is just not flexible enough, 
right?

Um, and then the other scenario is basically you just have your like 10, 15, 
senior backing engineers and everyone is kinda like you know, really comfortable 
handing, handling your IAC modules and your Kubernetes like helmet charts and, 
and stuff like that. Right? And that's also fine, but that's also doesn't scale.

Cause you can't just hire those people Right. Forever. Um, you'll, you'll hire 
more junior people, especially as a scale and, um, you just can't expect 
everybody to be familiar with that, especially if they weren't. In the early 
stages of building it. And so that's where we start seeing then a, a trend 
towards platform teams forming.

Um, and, and you're absolutely right, um, you know, it trickle down from very 
large companies to, you know, smaller and smaller companies. And I think the 
threshold, the, the, kinda like the cutting point is a, is around us like 30, 50 
engineers. I think also important to mention. You know, the very, um, then, then 
I think the question becomes, what is the, you know, minimum common denominator?

What are the, what are the, um, you know, patterns that you see in, in, um, 
platform building that you can replicate across the board so that you avoid 
people inventing the wheel over and over again? And that's kinda like what we 
worry about when we think about constantly humanity. . And so, you know, in that 
cases I always say, Hey, if you're like a Google, like of course Google will 
build your own platform.

Cause they have like very, and in fact they have many different platforms 
internally, right? Because they have like very specific requirements and they're 
just like at a huge scale, right? But, um, if you are not at that scale of a 
Salesforce over Google, where you actually have like multiple platform teams 
internally competing with each other.

Um, but you just have like one platform team. Then you wanna provide that 
platform team with the best possible toolbox to make them succeed. And you don't 
wanna, and you wanna make sure they don't reinvent the wheel and just like build 
the whole thing from scratch, but leverage a combination of, you know, either 
open source or open source and, and, and commercial offerings that give them 
that initial kind of, you know, foundation.

That, that then can be that sort of opinionated, um, you know, toolbox that 
we're talking about to go build your own opinionated platform and your own 
opinionated workflows on top. But I think it's important that you kind of focus 
as a platform team on that serve like last mile optimization and not on let me 
build the entire, uh, thing from scratch, which is something that unfortunately 
we see a lot of people doing.

It can be extremely resource intensive and extremely time consuming. And, you 
know, sometimes it's worth it. And a lot of times it's, it's not. And, and we 
see a lot of organizations underestimate the effort of, you know, not just 
building a platform , which can be like one or two years, uh, at any, you know, 
considerable size of company, but also maintaining and improving that platform.

And we see actually a lot of organizations making this mistake where they say. Hey, 
you know, we had this platform, initiative's gonna run for a year, then we're 
gonna, this platform is gonna be great. And actually, you know, when you ship 
the v1 that's when the work starts, like, like with every other product, right?

And so, um, it's, it's, it's a lot of work. And, and, and we want the 
engineering, the platform teams to focus on that optimization part and try and 
provide them with an initial toolbox to get started. 

[00:24:55] **Michaela:** Okay, so let's. Let's step a little bit back and look 
at what's the outcome, right? What's the product really?

How can I imagine that, right? So, um, I would say probably in the purest form, 
it's infrastructure is code. Um, but I think probably to, to reach that there 
are probably many steps. Maybe it's a document at the beginning, , um, maybe 
it's, uh, maybe it's GitHub's actions. I don't when, when we are really small, 
right?

So, uh, Uh, C I C D pipeline run. Right? And we have some GitHub action scripts, 
or we have some, um, maybe I. , could we say we are a, a platform engineering 
team if we have Sapir, , you know, take over things from one system to the 
other. Is that, is that, is that an engineering platform, , or, or how, you 
know, what, what's the form that we are striving for?

What's the, you know, the golden rule? How, how should that look like? Is it the 
document? Is that enough? Can we say that's already a platform that we build, 
that we describe. Which tool boxes are, you know, going in or that we are using. 
And maybe, you know, there is a Titan script and there is is a back script and 
you know, this is how you run them with those commands or you know, I think 
there's a.

A large, uh, virality of forms, how we could actually have that from quite 
manual to extremely automated. So, so what, what is the toolbox that you are 
talking about? Do, do I go to GitHub and is there a repository and I download, 
you know, uh, uh, a standard, um, platform engineering, um, polar plate coat, , 
and then I start customizing that to my needs?

Or how, how does that work. 

[00:26:34] **Luca:** Yeah, I love this question. This is such a good question 
because. It's actually something where I think we see the largest gap right now 
in the, both in the community and the market broadly, which is, um, you know, 
obviously, you know, the, the history of software engineering really is a 
history of, of progressive obstruction and platforms, right?

So, Everything is a platform. Everyone wants to be a platform, right? Every tool 
like markets themselves is a platform. So, um, but I think what we see, you 
know, specifically around platform engineering is a focus around two main areas, 
which is application configurations and infrastructure, uh, configurations, 
right?

And so having those two as the kind of like the core pillars of your delivery 
setup, right? And yeah, your delivery setup kind of like, you know, starts in 
your get base system, then goes into your ci, your c. and then touches all the 
parts of the infrastructure and you know, from dev to production. And, um, but 
you know, the, one of the, I think like fallacies and sort of like anti patterns 
that we see out there is um, especially when there is a top down initiative 
around, hey, we need to build a platform.

Cause it's cool and, you know, people say we should do it. Um, then kind of like 
people go into looking at what is the, you know, looking at developer workflows 
chronologically, right? And so then they analyze it, right? Where, where does a 
developer start when, you know, she wants to create a new application, a new 
service.

And it's like, oh, they go get and like, um, and so then they start looking at 
um, you know, they look at this workflow and they're like, alright, this is 
where we're gonna start building the top right. And so then the answer a lot of 
times becomes, For instance, in turn, developer portals or you know, servers, 
catalogs like backstage, which don't get me wrong, it's a great product.

They're, they're huge contributors to the community. We're, you know, we're big 
fans and we weren't closely with them. But the issue a lot of times, especially 
if you're not a massive in the organization, which is the vast majority of 
cases, is that is not where the value lies. , right? If you're trying to think 
about where, where is the painful thing, what is the painful bit for developers 
within your, uh, application and infrastructure configuration world within your 
delivery and C I C D setup?

It's usually the configuration management bit. It's not the, you know, let me 
start with the, with the, you know, with which template and so on for the 
services of reach, scaffolding and. Um, that's, that's where we see, um, most of 
the focus. And that's where we promote a, an approach to configuration 
management that we call dynamic configuration management.

Um, and is really focused on dynamically generating conflict files. On the fly 
at deployment time for developers in a way that, you know, basically removes 
everything that is like the, the entire kind of like, uh, cognitive overload of 
trying to figure out what are the dependencies, what do I need do in specific 
environment and so on.

And really just like have them work against one single, um, Uh, configuration 
format that then can work environment in an environment agnostic way across 
their entire setup. Um, and yeah, so that's, that's kind of where we, where we 
see, you know, the, the, the focus in terms of, you know, platform engineering.

But you bring up a really good point, which is, um, you know, I think apart from 
engineering community, Gone through, you know, multiple phases. One was in the 
last couple of years, which was like the, the initial, the nascent phase of, um, 
you know, hey, The promise, the initial tenant of Dells, because you build it, 
you run, it can actually be, um, you know, uh, executed in practice through 
platform engineering.

Right? And it was about hammering that idea here and there and, you know, 
platform engineer really exploded last year. We had, you know, Gartner putting 
it on the hype cycle, the, our community, you know, quadrupled or more in size. 
and, and really there was like a lot of debates. There was a whole controversy 
on Twitter around Dell is that long platform engineering, happy to get into that 
as well, but like really the, um, you know, platform engineering exploded.

Um, and so. Now, you know, there are a lot of people that are coming into the 
community that are coming into this trend and going, okay, like, I get it. I'm 
sold. This is cool. I'm in, where do I go? Right? And, and then there's 
crickets, right? There is no good place for people to get started. There's no 
blueprints.

There's no reference architectures, there is no, um, you know, just starting 
points for people. And so this is something that from a community perspective in 
the platform engineering community, Focusing heavily on this year. And really, 
and, and it's also gonna be, in fact, one of the, the, the trucks that I'm 
personally really excited about, uh, platform Con 23, which is really just 
platform blueprints and, and just bring the practitioners and try and start 
building, you know, phase one was about building a, a, uh, if you will, a 
shared framework for how to think about these things now is about, you know, building 
and sharing actual blueprints and architectures. And so this is what we're 
focusing on now. Yeah. Yeah. 

[00:31:52] **Michaela:** And, um, coming back to these blueprints and, and how 
can I imagine them, are they, is that code, is that, is that, as I said, saper 
actions?

Is it a GitHub action? Is that already, you know, is that enough or, or how does 
that, how does that look like? And, and, and how is it stored? How, how do we 
make sure that it's, you know, um, updated? Like especially these glue, you 
know, between the systems? Yes. How, how, what do we do with them? How do you 
evolve?

Are there smells that I can have with them? Right. And, and are diversion and so 
on. 

[00:32:28] **Luca:** Absolutely they are version, and it goes back to what I was 
saying earlier, right? They're really like, if you think about it, the two 
pillars are the application configuration and infrastructure management bit, 
right? So, um, what that means in practice is, you know, yamo files and helm 
charts on the one hand and IC modules on the other, right?

And those live in a, uh, you know, in your get based system. Um, and that's 
something that is really important and something that. You know, we are have, 
have spent a long amount of a lo a long amount of time, sort of like debating 
within the community because the initial kind of instinct of a lot of people 
when they think about a platform is a dashboard effectively, right?

Is having this like really nice UI that makes especially management really 
happy. Um, cuz they can like see what, you know, the door metrics for the teams 
are and like click around and so on and so forth. But the reality set is the 
value really lies into, you know, version code. Right. Um, to be clear and, and 
that is what developers want.

Right? So to go back to what we were saying earlier, um, you know, we've seen 
many platform teams. At rolling out their platform because they focus on this 
kind of like click ops approach. Mm-hmm. to, you know, build a, a, a pretty ui 
and, and, and developers will use it. Well, that actually doesn't work in the 
vast majority of the cases.

Why? Because developers really enjoy, you know, their, you know, their code 
based workflows, right? Like they work and get, they push something and so they 
don't wanna. Jump out into this clunky ui, try and figuring out, ok, what do I 
need to do now? Like, um, and then, and then you go back to what you were doing 
earlier, which is black, your ops or platform team, and like, Hey, how do I do 
this again?

Right. And so instead is really like the, the, you know, the most, some of the 
most successful platform initiatives that we've see in the market. Have really 
embraced, you know, again, they listen to developers. They figured out, hey, 
what do they want? They want code based. This is what they're used to. Alright, 
let's let, let's build an interface which is fully code based.

And, um, and, and that's the way to go in our opinion. . Yeah. Yeah, 

[00:34:31] **Michaela:** that sounds good. So another question that I have for 
you to understand the role and the responsibility of a platform engineering team 
is, mm-hmm. , what about, uh, education? Do you provide also education within 
your organization? Would you go and, you know, um, Yeah, tell people how to, to 
use certain tools or for example, how to spin up test environments, how to write 
those configurations, how to adjust those configurations.

Um, or is that something that's outside of the platform? Engineering, um, 
responsibilities, shop role. 

[00:35:05] **Luca:** No, it's very much, uh, in within the, the, the, the set of 
responsibilities. And I think it's a great question because it, it kind of, it 
hints at something I think that a, a trend that, that we've seen. So, you know, 
if you, if you look at us from a historical perspective, right?

The, you know, you look, you go all the way back to kind of like the cis Adam 
Day, which was, you know, this poor person, you know, in the basement trying to 
actually like, install real servers and, and you know, then, you know, develop 
people. Throw over the mythical fans and they tried to like, all right, now I 
need to like actually deploy this thing and, and make it all work.

Right? Um, and so the communication was, was extremely limited. And, and, and I 
think like as you go through like, you know, DevOps access and so on, you see a, 
just like in a, a correlation of increase in needed communication skills, and I 
think this is even more. When you look at sort of like the next iteration, which 
is the platform engineer, communication skills become extremely important in 
this role because you need to not only, you know, build that really tight 
feedback loop that we're talking about with developers.

You also need to get, you know, management and executive by end. You need to 
really being able to like sell this thing internally and. and work in this 
multi-stakeholder environment with different teams. Right. Um, and then as you 
said, train, train and educate people is that isn't sorry, is an extremely 
important part of the job.

Right. Um, and so for sure, um, I think, you know, the, the, the key kind of. 
Um, skillset of the platform engineer is on the one hand this like product 
mindset, which maybe not all traditional infrastructure folks necessarily have. 
You know, I'm sure everybody can adopt it, but it requires a mindset, a mindset 
shift.

Towards that. And then the other bit is communication, training, education, um, 
and really just evangelize, right? And I mean, you see this as extremely true 
in, you know, very large organizations. We had, um, we have a couple of talks 
that I can, I can share with, with your audience later. Um, one is from, uh, gal 
Navarro.

He gave it at the last platform in 2022, and is about, you know, the salesman. 
Of, of the platform engineers and how, how do you, how do you sell internally? 
And another one that I think is really interesting is by Aaron Erickson. He 
built one of the, that, that actually will ended up being the successful, um, 
platform initiative at Salesforce.

And at Salesforce it was like an interesting, you know, situation where you had 
actually multiple platform teams competing with the chat. And if you think about 
that scenario, you, your communication skills need to be like on, you know, on, 
on I, on Hyperdrive. , it's a little bit like you're in a, a startup in an open 
market.

You can't just worry about, you know, the product that you're building, you 
really need to worry about like, what's your go-to-market, what's your 
distribution of your product? Right? And so you really need to become like a 
marketing and salesperson educator. 

[00:37:56] **Michaela:** Yeah. And so, um, because I'm also training, uh, 
software engineering teams, I want to know is.

Part of the platform engineering or is that a boundary? You know, there must be 
some boundary where, where we say, well, you know, training, um, engineers is, 
is okay for let's say CI and CD pipeline, but we are not training them how to 
test their systems or I'm specializing on code reviews, right? Because they're 
big.

Pain point for, for many, many organization. Right. And there is actually a lack 
of training. So is that also something that the platform engineering team would 
take over or would worry about how people conduct code reviews and how they do 
that? Or is that outside, let's say testing code reviews, let's say secure 
coding practices.

Right? We can spend that even further. Right. So where, where is the boundary of 
what is still you? Part of a platform engineering team and their education to 
the organization and, and what's outside of that? 

[00:38:53] **Luca:** Yeah, I mean, a bit of a cop out answer maybe, but it 
depends, right? So if, if, if you're, I think if you are a small platform 
organization, obviously you're not gonna have, you know, a ton of resources to 
kinda, everybody needs to wear all their hats, right?

Um, we've definitely seen very large companies where they have dedicat. You 
know, evangelists and trainers just for their platform initiative, right. So I 
think it's a question of resources. Um, but in general, I think, you know, it's 
not necessarily the actual engineer. Maybe that, um, is, you know, the people 
actually building the platforms and shipping features for it that are the main, 
uh, evangelists.

I would say, you know, a, a really active role is played by the product. And, 
and I think the PM of the platform is actually an extremely interesting 
position. And in fact, you know, in the platform engineering Slack, one of the 
most active channels is the product management channel. Um, cuz there's so many 
dimensions to, you know, PMing a platform, you know, is all this, everything 
that we talked about is like, you wanna be the glue you, you wanna, you, you 
need to position yourself with executives, not as a cost center.

As a, as a value driver, you need to evangelize it. Right? And, and a lot of 
that needs to be driven on a, on a product management level. And so I think, you 
know, to answer your question at a, at a, at a small scale, for sure, the PM in 
a larger scale, you know, you're gonna have, the PM is gonna be supported by a 
dedicated, sort of like evangelist.

[00:40:27] **Michaela:** Yeah. Yeah. So I ha I have another, another question 
for you, . For example, when I was doing this study on developer experience, 
right? Um mm-hmm. , there were some concerns, you know, and, and I hear that 
over and over again. There are concerns that engineers. Do not know best. Right. 
So you were saying at the beginning you were saying, oh, you go to your 
customers because they know best what they need and so on.

Right. But sometimes, you know, it's coming up over and over when I'm talking 
with people, uh, there are some skeptics that say, well, maybe they don't know 
best. , not all of them know best because they, maybe they haven't been exposed 
to something else, right? Maybe they haven't seen faster review cycles.

Maybe they haven't seen how, you know, a, a fully automated C I C D works. Like 
maybe they are working against a standard or a status quo. Um, where, uh, if 
you're not bringing outside, you know, you know, ideas, we will get stuck into, 
you know, Doing things, how we always did them. Right. Um, do you see that as 
well, that, that that can happen?

That, uh, you know, that, um, you know, shipping, I don't know, shipping, uh, 
every three months is seen as normal and actually fast, but actually we, what we 
want to know, and if we compare and benchmark with, you know, the successors and 
the leading companies, we should ship three times a day. Right. . 

[00:41:48] **Luca:** Right, right.

Yeah, absolutely. And that's, I think, um, that's where. Really, you see whether 
you have a good platform team or not. Right? Because, you know, building a tight 
feedback loop with developers doesn't mean blindly listening to them, right? It 
means, you know, listening and, and like weighing. And I think one of the 
advantages that platform teams have right now is if your platform engineer, you 
are very likely to be, you know, Um, quite like probably an early doctor and, 
and, and pretty much on the cutting edge of, you know, the whole cloud native 
and, and sort of like textile conversation right now.

So in that case, you have somebody that usually is somebody you know that is 
driving already in a victim by, you know, by default and then can sort of like 
find what's the right. Of drive and how far, how far I can push with developers 
listening to them. Right. Um, that's certainly something that could change.

Um, and, and I and I over time, and I think, you know, the key is what is this 
system of checks and balances that we can put into place? Because, you know, 
what is true of developers can also be true platform engineers themselves. 
Right. You know, we have seen certainly platform teams that have fallen for, you 
know, Fallacy of, oh, this like shiny new tech that came out and I'm really 
excited about, and everybody is saying it's amazing, you know, and it's gonna 
solve all our problems and let me just like try to like fit it somehow as a, you 
know, square in a rod hole.

Um, Into our platform design and, and that obviously can create more, more harm 
than good. And so, um, yeah, it, I don't think there is a perfect answer. Just, 
uh, be thoughtful . Yeah. So 

[00:43:40] **Michaela:** maybe for beginners. Right? And also to round up our, 
our interview today. Um, If I'm a beginner, uh, or maybe new to platform 
engineerings, and I'm wondering, is that actually something for our 
organization?

Would that help us? Should we start something like that? What's a good place for 
me to go and, uh, find resources about platform engineering and even make up my 
mind if, you know, that will be a good, a good investment of our. 

[00:44:08] **Luca:** Yeah, absolutely. I think, you know, platform engineer.org 
is probably the best place to start.

You, you have a blog there with a lot of resources. Internal developer 
platform.org as well is, is an actual repo where, you know, it is open source. 
People can, uh, do their own PRS and commits and, and we see. You know, there's 
a really good rundown of what are all the tools, what are the problems, what are 
the core principles?

Um, so those are two extremely good places to start. Platform, platform. Then 
from there you can join, you know, the Slack channel and really just get into 
the weeds of it. You know, there are 8,000 plus. Platform practitioners, some 
extremely experienced that have built, you know, the platforms at Walmart, at 
Apple, you know, and, and, and some that are just getting started just like you.

Right? And so that's a perfect place, I think, to just get a feeling for delay 
of the land. Um, and I think also platform platform.com, you know, we just 
updated the, the website. Um, you know, with the new, with the new addition. 23 
is gonna happen in. We're expecting 150 to 200 talks by some of the best 
leading, you know, DevOps and platform practitioners.

And so that's free. Um, and it's virtual so people can join from anywhere. So 
that's also a really good place. Oh, that's pretty cool. 

[00:45:22] **Michaela:** Yeah. Yeah. I will link all of that in my show notes. 
Um, yeah, the last question that I have for you is what are, and it must be a 
short. What are the three benefits that people get out of, um, you know, the 
three main benefits that people get out of if they are investing in platform 
engineering?

What do you think? 

[00:45:42] **Luca:** Um, self-service. No frustration. And no ticket ops. 

[00:45:51] **Michaela:** No. Ticket ops. 

[00:45:52] **Luca:** What? What's that? Oh, ticket ops is just, you know, um, 
Ops team basically being like bombarded with inbound ops requests. By the 
development teams, right? And so the idea is like, um, you know, the benefits of 
of platform, the benefits of a platform are on the developer side.

I don't need to wait any longer. I don't need to slack my ops. I, I can just 
self-serve what I need to run my and services independently. So no frustration, 
self service. And on the other side of the equation is no ticket ops, no. You 
know, living my life as a glorified, stressed out help desk, and, um, and just 
working frankly on better problems, like more interesting problems.

Optimize your production setup. Not stand up the same Postgre sequel for the 
10th time. 

[00:46:38] **Michaela:** Yeah. Yeah. Will AI do that for us in two years? , 

[00:46:43] **Luca:** who knows? It seems like AI is gonna 

[00:46:45] **Michaela:** do everything, can do a lot, right? Yeah. We are all, 
actually, they will do the, the interview that we just did, just better. 
Exactly. Okay.

Well, look, I thank you so much for being on my show. I really, uh, thank you. 
Enjoyed talking to you and learning all about platform engineering and, uh, 
yeah. Thank you so much. 

[00:47:02] **Luca:** Okay. Thank you so much for having me. I hope people find 
it interesting. Yeah. 

[00:47:05] **Michaela:** Bye-bye. All right. This was another episode of the 
Engineering Unlocked Podcast.

If you enjoyed the episode, please help me spread the word about the podcast. 
Send the episode to a friend via email, Twitter, LinkedIn. Well, whatever 
messaging system you use, or give it a positive review on your favorite 
podcasting platform such as Spotify or iTunes, this would mean really a lot to 
me.

So thank you for listening. Don't forget to subscribe and I will talk to you in 
two weeks. Bye.

