---
episode: "Transcript Making security easier for developers"
permalink: /easier-security
status: publish
type: transcript
---

[00:00:00] **Michaela:** Hello and welcome to The Software Engineering Unlocked 
Podcast. I'm your host, Dr. McKayla. And today I have the pleasure to talk to 
Harshit Chitalia. But before I start, let me tell you about my latest project, 
awesomecodereviews.com. Yeah, all my work on contributes has now its dedicated 
home.

At [awesomecodereviews.com](https://www.awesomecodereviews.com), you will find 
articles about code review best practices, code review checklists, news about 
the latest research on code reviews, and of course workshops and courses that I 
offer around this topic. So, please hop over to 
[awesomecodereviews.com](https://www.awesomecodereviews.com) and check out my 
latest work.

But now, back to Harshit. Harshit is the co-founder and CTO of Tromzo. And he's 
on today to share his knowledge on how to make security easier for developers. 
Before starting Tromzo, Harshit spent eight years as director of engineering at 
Juniper Networks where he experienced first-hand how frustrating security can 
be for developers. So I'm super, super thrilled to have Harshit here with me 
today.

Harshit, welcome to the show.

[00:01:04] **Harshit:** Thank you for having me. I'm really excited.

[00:01:08] **Michaela:** Yeah, I'm really happy that you're here. So, Harshit, 
what makes it hard for developers or frustrating for developers if you think 
about security?

[00:01:18] **Harshit:** I think, there are several aspects to it. I mean, if I 
think I've had, I, myself, have been a developer for a very long time before I 
jumped the, to the management train and, you know, started taking up more 
leadership positions. And being a developer is like wearing multiple hats, 
right?

Basically, you are writing software, then making sure that you ship that 
software, writing tests, and as we've now gone into the DevOps and, you know, 
CI/CD, and Agile methodologies, now we are no longer just looking software for 
the application. But we are writing software for infrastructure as well, right?

So, we are managing microservices, we are managing the cloud, and we are 
managing the end-to-end lifecycle. So now, a lot has been asked from one 
developer, right? So it's no longer you asked for somebody who's full stack. 
You ask somebody who's full stack, plus DevOps, plus SRE, and plus presales or 
post-sales, right? Like, doing support as well.

Now, to mix all of these things with security is completely new ball game. 
Because earlier, security was all about firewalls, right? You protect your 
application by deploying a firewall, making sure there's no DDoS attacks and 
you can buy an application from Cisco or Palo Alto, and that's it.

But these days, most of the hacks that you see are all software 
vulnerabilities. Dependencies, which are vulnerable, or software that you write 
is vulnerable. So, how do you kind of go and mitigate all of that? And it 
becomes really, really challenging for somebody who's new, to kind of even 
understand what the Attack Office is. What all possible things can be, kind of 
wrong?

So, to give you an example, one of our customers, they use, they have a 
standard stack. Python on the backend, React on the frontend, deploy it in 
microservices in the cloud. Now, just this standard application, they use eight 
different security tools to kind of make sure that the application is good 
enough that they can ship.

So, these are basically secret scanning, code dependency scanning, 
infrastructure scanning, container scanning. Then, you have just your source 
code analysis scanning. And so, you could keep on, just making sure that you 
are covered across all your bases. Now, if a developer, as a developer, you ask 
me, okay, in addition to everything that I'm doing now, you want me to go and 
look at eight tools and figure out the hundreds of vulnerabilities that exist 
in my environment and something is coming from a dependency, which I don't even 
know what to do about, it becomes like a big mess, right?

So that's why I would say security has become so difficult for developers, and 
there has to be better ways to kind of manage these things.

[00:04:11] **Michaela:** So, I heard you talk mostly about scanning tools, 
right? Using tools and automatically detect security vulnerabilities.

What about manually, actually checking those? It's also a hard problem? I'm all 
about code reviews. And part of code review could also be to look a little bit 
as input validation. For example, are there sequel injections? Are there, is 
there, is Cross-site Scripting possible? Do I have some parameters, you know, 
in, as get set, for example, and so on?

Is that still necessary? And are developers struggling with that in your 
experience as well? And because the tools somehow look at the different tech 
surface, right? They look at different kind of problems. They find a subset of 
those problems as well.

But is there still this need also for developers to understand how to manually 
check for those problems and know about secure coding practices?

[00:05:04] **Harshit:** Oh, a hundred percent. Everything that you mentioned 
about your manually checking, going through code reviews, looking for things 
that can be inputted are all valid concerns.

And that has to go through code training and making sure, you know, developers 
are even aware that these problems can be fixed. But if I look at the whole, 
broader perspective of a developers project today, with all these open source 
technologies out there, developers are just writing, if, just purely from a 
line of code perspective, let's say.

So, only 30% of the code is what developers write. The rest 70% is coming in 
from third party libraries of some sorts, or any of the infrastructure that 
you're already using. So, even if you manually code review, things that your 
project are doing and your peers are doing, and that also in a very fast pace 
environment, it becomes really difficult to kind of keep that happening.

[00:06:05] **Michaela:** Mm-hmm.

[00:06:06] **Harshit:** So, what we've observed is that very few 
vulnerabilities get caught because somebody's doing a code review and, you 
know, they point it out, unless it's right out there, right? Typically, it's 
through automation that people find with these vulnerabilities.

And the other thing is, people use a lot of pen testing tools as well, right? 
There is third party pen testers. There are in-house pen testers. And though 
pen testers, they work very differently, but at the same time, their model is 
that we want to replicate how an attacker would see it.

Because the attacker typically won't have access to your source code. So they 
take it as a black box, and they're trying to kind of go and really hammer your 
application. So, that's also one kind of a scan tool, if you think about it. 
It's a security tool, pen testing tool that will go and hammer your application 
as well.

But as I was saying, today, in pretty much every leading organization, you take 
Netflix, Coinbase, yeah, you know, Airbnb, everybody does security through 
automation. I mean, if you are starting on a new project, there's no way that 
you can go ahead and say that, "Okay, I'm gonna manually go and find out 
vulnerability."

It's just a very large surface area. And today, even with all these tools, it's 
difficult to manage risk. I mean, there's no software out there today that is, 
I would say, a hundred percent secure, right? We have 4,500 customers who have 
over, I would say, half a million vulnerabilities in their environment, overall.

But now, that doesn't mean that, "Okay, you can go and hack any bank that you 
want today," right? Because they are managing risk. They are managing, okay, 
what needs to get fixed, how that needs to get fixed, what is the priority? 
There are dedicated teams for those things. And so, but, the way those things 
are, I mean, we can talk more about it from a security perspective as well, but 
the way some of those things are done is not the most efficient way.

And even for smaller teams, we're just starting out, it becomes even more 
difficult to kind of manage some of these things as well. And I can talk about 
a survey that we did recently to kind of figure out what do application 
developers feel overall about security as well as we continue on this.

[00:08:22] **Michaela:** Yeah, it would be really interesting. One thing that 
I was wondering, especially if you are mentioning these large organizations, 
right? So, for small organizations, I totally understand that, you know, one 
dev has to wear so many hats. And I also see this shift, right? That the person 
has to, developer is not only a full stack developer, but this DevOps, you 
know, requirements, and the security requirements, and so on.

But aren't companies like the ones that you mentioned, especially the large 
organizations like Microsoft or Google or, well, Coinbase is not in that 
( *laugh* ) in that sphere, but still, I think a larger organization, same as 
Airbnb, I think they have dedicated security teams, right? And so, are the 
developers really responsible? When I'm working with teams, especially from 
large organization, and I bring up security and that they should think about it.

They're like, "What our thing (??)," right? ( *laugh* ) And to really try to 
get rid of this additional responsibility and say, "Well," you know, "We have 
a team that actually does that." What's your experience here? Do you see that?

[00:09:28] **Harshit:** Yeah. Yeah. I mean, we've definitely seen it, but 
you'll be very surprised that things are changing, okay?

And it's no longer about we have a separate security team. And especially in 
the space that Tromzo or my work currently kind of goes into. So, security has 
different facets. There's cloud security, there is application security, and 
then there is other areas about security as well.

So, within application security, there is no way that the security team can go 
and fix the issues, because they don't know anything about the code. The 
developers are the one who are writing the code. Whether it's their own 
software, or application logic that they're writing, or dependencies and 
containers that they're bringing up to kind of run their services.

It's all the application developers. So even at Google or at Airbnb, it's now, 
that's why we talk about the shift left. Everybody's trying to shift left, 
which essentially means that the developers now definitely have that 
responsibility. And I cannot totally understand. It's like a cultural shift as 
well, right?

So we, if you go back in the day, we used to have QA engineers, right? We used 
to have testers who would basically be responsible for testing the application. 
Now, if you look at it, most modern teams don't have a QA engineer. More 
software teams just don't have that position anymore because the developer has 
taken the role.

In some bigger organizations, you'll hear somebody doing SDET, which is 
basically software developer in test, which is writing infrastructure to manage 
these tests, making sure the performance of these tests is good. You can run as 
many tests excessively (??). Now, what we are seeing in security teams is 
security teams are managing the risk in your application.

So they will define what we call a security guardrails where you can say, 
"Okay, this is the container image that you can use for our container services. 
This is what you can kind of push into your environment. Or this is what you 
cannot do within, you cannot push out any secrets in your code." So, those kind 
of become security guardrails as you're developing code.

And that is what the security team manages. But on a day to day basis, the 
vulnerabilities that come out of your software need to be addressed by the 
developers, right? And, yeah, developers, I know some of them are get really 
excited about security, and some of them are like, "Hey, not me," you know?

And so, that is a big cultural change. And so, and there are, we can talk about 
how we can mitigate some of that changes as well, because we've seen companies 
go through that transformation, right? Couple of things that have really worked 
well over there is, you know, push from the top.

If your CEO is emphasizing, "Okay, security is important for us," if your top 
level executors are telling you that, "Okay, we need to kind of do more about 
security," a large organizations have this position of a CSO, which is 
basically a VP level position or even higher. And typically, if they have a 
board seat, that means that, you know, they are part of the executive team.

They have a position there and they are mandating security, right? So, it 
becomes like one of the pillars in an organization. And it's always good to see 
that. On the lower level, on the engineering side itself, we have seen teams go 
ahead and do gamification, right? So now, there are leaderboards happening.

Okay. This team introduced these many issues today. And this is how they are 
trending week-on-week or one-on-one. Now, that kind of, you know, most 
engineers are gamers as well, right? So, you kind of put in all this 
gamification within fixing issues, and finding issues. Then, it kind of 
increases the visibility, as well as make sure that people are driven to kind 
of achieve a certain goal because it becomes like a community kind of a feel.

And so, we've seen a couple of organizations do that really well and where they 
are doing some of these gamification. They have a leaderboard where they track 
these things and everybody's made aware of what's happening in their 
environment.

[00:13:49] **Michaela:** Yeah. And what about tools? You were talking about 
tools, right? And that there are many tools and that the developers have to, 
you know, understand them. But aren't we just, you know, set, you know, if we 
have, let's say some automated tool in our GitHub, in the CI/CD pipeline, 
thinking about Snyk, for example, or, you know, DeepSource, some study analysis 
tools here, is that enough?

Or what do we need?

[00:14:14] **Harshit:** Yeah, yeah. That's a good question. What do we need? 
So, the thing is this. That security is one of those fields where you can never 
be sure that, you know, it's like protecting your home, right? Is a camera on 
the front door enough or do you need one on the back door?

If you have both of these, do you need a motion detector? So now, it depends 
on what you are guarding, right? What are your crown jewels? Let's say, it's a 
bank. Then you need a camera every other place. You want to make sure that 
there's things everywhere. But let's say, it's a public library or something 
else where people are going to have access to everything.

So you, so it's all about managing risk, right? And then from a tooling, just 
tooling perspective, you need a different kind of a tool for everything that 
you are really trying to protect against. So, some companies are API companies. 
For example, Postman, or let's say, Apigee, or things.

To, for them, API security becomes the most important thing, right? So they 
would not just have one tool doing API security. They may have three different 
tools doing all different kinds of API security. But if I'm talking about 80% 
of the organizations, the seven, eight tools are basically what we call as SaaS 
tools which do source code analysis, dependency, checking contain, secret 
scanning, so, in which Snyk comes in.

And there are a bunch of other players as well like Veracode, and Checkmarx, 
and, I mean, the list can go on and on. Then the other side comes, which is the 
infrastructure scanning, where people are scanning for your Terraform code or 
your CloudFormation code.

They're looking at your container images. So things like Aqua Security is there 
for container images. There are open source ones as well. The new thing that 
has come out is something called a supply chain security.

[00:13:49] **Michaela:** Mm-hmm. Mm-hmm.

[00:16:10] **Harshit:** Like, how do you kinda make sure about not just 
everything that you are importing, but how much of the supply chain, so as to 
say, of the software is also being imported in your environment?

Making sure that is all there, so there's this whole angle of supply chain 
security. And then, you know, just finally, it's all about your code, as I 
said. Either your APIs, if you're using Python, then there will be a Python 
Analyzer, if you're using React or JavaScript, there'll be a child, there'll be 
a language specific thing as well.

And then, a lot of security typically goes with compliance as well. So, you 
have licenses as well, that people need to monitor for. So there are license 
based checks and license based scanners as well, making sure you're not 
importing something, which is unofficially not a good license that you want to 
have in your enterprise product.

So, there are all these different variations of things that you would need to 
make sure that you're running a good application security program.

And in a survey that I was talking about, we, well, basically there's, it came 
out to, like, 62% of the developers are using today, 11 or more sec 
application, security tools in their environment. So you can see that that 
number is high and it is going higher and higher as we kind of make everything 
software.

[00:17:31] **Michaela:** So, what can we do to make it easier for developers? 
So, we are talking about the, you know, we have this shift left, there, they 
need to be more responsible for it, we are talking about that also 
infrastructure is now code, right? We are talking about that there are so many 
tools.

So, what can we do to make it easier for them? What can we do to reduce the 
friction?

[00:17:52] **Harshit:** Yeah, absolutely. And I think, there are three things 
here. It's technology, process, and people. And we can talk about all three of 
them and how all of that can change to kind of aid in making this thing easier 
for everybody.

So, let's talk about the technology perspective first. So, clearly, if you have 
eight things that you need to do, the human mind is not capable of doing that. 
So, it's easier if there is one thing that tells you what to do, right? So, you 
would need sort of an orchestrator or a management platform that makes sure 
that, you know, you are getting these reports from these eight or 11 things, 
and they are bagging reported in a way that is meaningful to you.

So, not that you have to go to a dashboard. But if the message is coming to you 
on a Slack channel, or coming to you directly on your GitHub PR. There's no 
point in telling me, "Okay, I filed a JIRA ticket because I introduced a secret 
in the code."

It should come right there in the PR. So it should block the PR with, it should 
not allow me to kind of go and merge something, which I should not be merging. 
So, that whole notion about shifting left and taking it to as much left, right? 
Even going as further as going inside your IDE, having a good pre-commit hook, 
like today, to kind of validate some of those things as well.

So, if I have to really talk about from a tech perspective, we need three 
things there. One is visibility of what all things I have in my environment and 
why all of this is secure or not secure, and what do I stand right now, and 
kind of measure that on an ongoing basis.

The second thing I need is automation, right? Making sure that if I have 
hundred thousand things, you know? Typically in container worlds, right? You 
will have 500 vulnerabilities come up. And typically, the fix will be, "Okay, 
go ahead and upgrade your OS image."

And that will just solve 500 things. Now, I can't go and file 500 tickets in 
JIRA, for example, for that one thing. It has to be one thing and just tell me 
exactly what to do. And then, as a developer, I can just go ahead and do that. 
So, just managing that process, what the scanner is telling you, and what the 
JIRA ticket is, and how do I go and mitigate it, that whole process can be 
totally automated.

And so, there are many of these workflows that can be automated out, in your 
environment. So then, workflow automation becomes a key thing from a tech 
perspective. And then the last thing is being able to just constantly monitor 
this, making sure that there is an assistant bot, so I use to say.

Like, your co-pilot, your co-developer is constantly on your shoulder, just 
nudging you to do the right thing and making sure that it tells you right there 
and there when you're about to commit a mistake or do something. That, "Okay. 
No, no, no, that is wrong. You can't do that," right?

So, solving these three things from a tech perspective, I think become really 
good. And there are a lot of other things that individually can be done in all 
of these three things. But I feel like just having that shift left mindset and 
being able to kind of go and finish that, would really help solve, I would say, 
60 to 70% of this.

Then, the rest comes into the process and the people, right? When I said 
people, let's talk about people first. Security needs to be in the culture, 
right? It needs to come down from the top that, you know, security is something 
that is important, you are allocated time, right?

It can't be like engineers are asked to kind of, of course ship features, but 
they also need to be allocated certain time to fix security issues inside, and 
inside their sprint planning, right? It can't be like, "Okay, we'll do security 
last." Security needs to be at the forefront. In fact, even before, if you're 
launching a completely new service, you should do security reviews before 
launching that new service.

Not that, "Hey, I'm now already built that. Now, what do I do about it? Now, I 
have a big gap in this." So, having that kind of a mindset is very, very 
important. And then, having processes defined. How do you kind of ask for 
exceptions, for example, right? Let's say, the developer is really busy right 
now.

And he wants to ask for an exception. "Okay, give me couple of weeks before I 
can get to this issue." How can the security team manage that risk and make 
sure that, you know, that is kind of documented? Because the ratio of security 
people to developers is really bad, right? If there's one security engineer to 
200 developers.

If even 10% of them ask for an exception, there's no way that security engineer 
can even just manage that process, right? So, how do you manage those workflows 
and that processes, and define them in your organization about what is 
considered, say, P0? And what is, how do you manage exceptions?

How do you manage due dates? And how do you track SLAs? All of those things, 
if you have a good defined process, then things become really, really smooth, 
right? You can think about this being very similar to how DevOps today works. 
You have Datadog and Century doing this really day in, day out because they had 
to move it from dedicated DevOps people to engineers who are now managing 
infrastructure.

So, it's a very similar process that I think even security needs to get into, 
right? Where it's going to be continuous. You will have SLAs that you need to 
meet, and you will have pager duty alerts that need to get addressed as soon as 
the security issues found.

So, I think, there is enough equivalent that we can see in other fields that 
has happened, and I'm pretty sure we can embed some of those learnings within 
the security teams too.

[00:23:42] **Michaela:** Yeah. So, especially the thing that you said at the 
beginning, triggered a couple of thoughts for me. So, if you have so many 
tools, obviously, they're reporting so many issues and we have to assign them 
a priority, right? We are also have to find duplications ( *laugh* ) because 
if we have tools, they are, normally, they are not scanning for very dedicated 
things and they are overlapping, right?

So one tool finds a little bit more in this area, but a lot also in the same 
area as, you know, the other tool. And so, you know, I'm getting, let's say, 
you are mentioning 11 tools. I probably get five times the same issue from all 
of those tools, right? And so, it would be good to have them together and then 
also assign some priorities so that I know what to look for.

I mean, it's already starting with studying analysis, right? I get all these 
errors and I don't even know where to look at or what to do first. So, is that 
also what you are hinting at? It, you know, it's really important to help wade 
through all of those information that we are getting from all of those tools, 
and especially from different tools, right?

Because within one tool, people obviously thought about, you know, how to 
package it and how to make it more adjustable. But if you have 11 tools, 
they're not made in a way, you know, that they're used together.

[00:25:03] **Harshit:** Absolutely. You are a hundred percent correct. And 
that's the biggest problem today, right?

Because now you have 11 tools telling you some things which are different, but 
there are enough number of things which are overlapping as well. And so, how do 
you kind of make sense of it? And the bigger thing is this. That, how do you 
even manage risk? How do you kind of go ahead and prioritize it?

As I was saying, that one of our customers has over 3,500 repos. There are 200 
engineers in the team and there are 3,500 repos. I mean, it's a, it's been, the 
company has been around for a long time. So, of course, you know, you go 
through these phases. But as a security team, how do you even know what needs 
to happen to that 3,500 repos?

Who's actually using those 3,500 repos? Or they are even deployed in 
production, right? So, if I go and scan everything, then I'm going to find, as 
I said, over 200, 300 thousand issues across all of these tools. Then, if I 
just have to go manually do one issue per day, I'm looking at years ( *laugh* ) 
before I get to it.

And by that time, there'll be 300,000 more issues, right? So, absolutely, you 
know? Combining all of these together, correlating it, de-duplicating it, and 
at the same time, making sure that we can automatically prioritize all these 
things becomes a piece of priority for a security team itself as an imperative 
of how do you kind of manage risk. And, yeah.

I mean, that's the fundamental problem that people are kind of facing. I mean, 
that's exactly the problem. That was the thesis before we started Tromzo. I 
mean, that is what I was facing back at Juniper as well when I was leading my 
team. I had three products, over a hundred engineers, and it was a big issue 
for me.

And when I basically went out and talked to other engineers, and some of my 
peer in the industry, and security folks, it became like, "Yeah, it's a problem 
for my team as well." And when I heard that over, you know, several times, I 
said, "Okay, let's start a company and solve this problem."

[00:27:14] **Michaela:** Yeah. So another thing that I want to, you know, 
briefly talk about and you mentioned it at very, at the beginning was only 30% 
or something around this number is written in-house, right? And the rest, we 
are relying on more and more services. And, you know, we are all that happy 
that, you know, it's in the cloud and, you know, I don't have to think about 
authentication because there are services doing it for me.

And I don't have to think about logging because there's an open source system 
that can do it at already for me, a package that I can use, right? And then, 
we have ( *laugh* ) Log4j, and the vulnerabilities, and so on, right? And 
suddenly, we are all facing, you know, real issues, real travels. But on the 
other hand, I mean, I have some scanners running for my little projects, and 
they're just, you know, they're not high risk.

They're not, you know, bringing in millions or something. So I don't feel that, 
you know, I have a big issue with not updating them frequently or with some 
vulnerabilities. So I get, weekly, I'm getting, you know, "You are using some 
unsecure version over here. You should do something over here."

And it's really hard to keep up with that. Is that also something that you 
think can be improved?

[00:28:29] **Harshit:** Yeah. No, that's a really, really good question. And 
definitely we need to kind of, you know, think more about that, right? At the 
end of the day, as you're saying, you are running some of those projects, and 
you are running some scanners, and they are reporting some things to, you need 
to go and fix them.

Now, that's I feel like if I'm a purist, then I would say, "Yes, you have to go 
and fix them," right? Now, but at the same time, you have to kind of manage the 
risk of it. For example, if you have something what we call as RCE, which is 
Remote Code Execution, that pretty much means that that kind of vulnerability, 
if it exists in your system, then anybody can basically go and do anything in 
your environment, right?

What happens is this. That there are few that come in, and then they become a 
big deal, like the examples that you took of, about Log4j. So, one of the real 
use cases for using Tromzo for our customers was trying to find out where all 
Log4J exist in their environment.

Because they had, today, no way to kind of figure out, before Tromzo, across 
all their services and assets and everything that they're using, how and where, 
if I even, if I'm using that library or not. So, it becomes really critical to 
kind of identify what you want to kind of fix. Because if the tool is just 
reporting, "Okay," that, "Okay, you have a very critical severity."

But let's say you only using it in your test environment. It's not even used in 
production, you're not shipping that software anywhere, then probably you don't 
need to fix it as soon as it's there, right? But at the same time, if you have 
something critical and it is internet facing, then you probably want to kind of 
fix it, right?

So, it's not, it's one thing that the tool is giving you some information. But 
at the same time, you want to make sure that, you know, you have a way to 
manage that risk and you define what is okay in your environment. And that is 
the most important thing here. Because you cannot, and I can stress double 
there, that you pretty much cannot fix everything that the tool is reporting to 
you.

There is no way you will have bandwidth to do that. So then, it's all about 
managing risk and how do you kind of go about managing all of that.

[00:30:56] **Michaela:** So, you run this survey that you already mentioned, 
right? The voice of the modern developer. What was the main finding that was 
surprising to you?

[00:31:04] **Harshit:** So, the key things that came out of the voice of the 
developer survey, some of the key things that were a little surprising for me 
were that one of, let me start with the first one. Developers are, I mean, 
we've been talking about this. But even developers know about it, that they are 
fixing only 32% of the vulnerabilities that exist in the environment today.

So, out of three vulnerabilities that are being found, only one third is, I 
mean, only one is getting kind of fixed. I would say not a surprising factor, 
but the ratio is quite surprising, right? I mean, we knew that we are not 
fixing everything, but just one third, it seems like quite a bit. Especially 
these are all B2B applications or B2C applications where, you know, is actually 
generating a lot of money and revenue.

The other thing that came out of this is a one third of the overall 
vulnerabilities that are reported by some of these scanners are also just 
noise. So now, clearly, the scanning companies also need to do a lot better 
here because if they feel that they're reporting false positives on that high 
level, right?

Because at the end of the day, most scanners are just rules, right? They kind 
of check for patterns or check for things. And so, if those are not really 
highly accurate or don't cover a lot of cases, then it becomes a problem as 
well. So we see that, you know, developers are not too happy about it, that, 
you know, there are so many vulnerabilities which are just basically noise.

And then, the other thing was that, you know, they found that they are actually 
pushing code, which is vulnerable. Like, 42% of the developers push vulnerable 
code once per month. So now, this was also something interesting that they know 
that the code is vulnerable, but they still are going and pushing it.

Because it's, they need to kind of go and deliver features at the end of the 
day. And they don't have enough bandwidth to kind of go ahead and fix some of 
these things as well, right? So we are seeing all these different things 
pointing out to the same problem where the problem is massive.

There's not enough resources to fix it. And the problem being massive itself is 
a problem in it itself. You know what I mean? ( *laugh* ) So it's all coming 
together in such a way that, clearly, if not mitigated or not addressed, it can 
really blow up to be a major, major thing.

[00:33:50] **Michaela:** Yeah, I totally see that. Especially with studying 
analysis tools, right? We have the same thing, right? So some people just turn 
them off or drastically reduce the rules, so that it becomes, first of all, 
manageable, but also meaningful, right? Because if you have all these false 
positives or little issues, you know, that are, you know, not that critical, it 
takes away from your attention, right?

And so I think that, especially this prioritization and making sure that you 
know this is really something you should fix here. And those, you know, because 
you said, well, one third is only addressed, right? But one third is noise, 
right? So there's this in the mid, another third, right?

Which we should actually look at, or at least wade through, and make sure that 
those important issues from this one third are, you know, covered or shifted 
somewhere. Yeah. I totally see that.

[00:34:42] **Harshit:** Yeah, exactly. And I think, you read the numbers right. 
So, that's the gap here. I mean, and attackers just need one way to get in, 
right?

I mean, they don't need one third or they don't have too many things that they 
go for. They just need one way. And so, for you, it's like, how do you kind of 
mitigate it. And also, the thing is that it's not that they're going to use the 
same thing year in, year out, right? So, earlier it was SolarWinds, now it was 
Log4j, now it was Spring4Shell, and by December in Christmas, that would be 
something else, right?

[00:35:21] **Michaela:** Yeah. Yeah.

[00:35:22] **Harshit:** So, it's, I mean, we definitely know that something's 
going to come up. So, how prepared are you for this Christmas is, essentially, 
is the question the security team needs to ask themselves.

[00:35:33] **Michaela:** Yeah. Thank you so much, Harshit, for, you know, all 
your wisdom and your insights into security. I think now is the time that you 
also tell a little bit more about Tromzo. It's the end of the show, right? And 
so, maybe if people want to check it out, you're working on this, right? You're 
the co-founder and CTO of this startup.

So, I think I understood quite a bit of the ideas behind of the motivations, 
you know, why you are on this path. But maybe you can share a little bit of 
this path to, you know, wrap this episode up. Maybe also, how long have you, 
you know, have you been doing this? Have you developed Tromzo, and what's your 
solution?

What do you think is the right way to do that in a, I guess, softer way 
( *laugh* ).

[00:36:18] **Harshit:** Yeah, absolutely. And thank you for asking that. So, 
yeah. We started Tromzo about, I would say, 15 months back. So we are a, I 
would say, a relatively new company. But at the same time, both me and my 
co-founder have years of experience, both in engineering and as well as 
security.

So, we are not new to the space or new to the problem. The problem, as I said, 
just intensified in the last couple of years, with everything becoming 
software. As I was saying, that network, it became software. Your 
infrastructure became software, your microservices, just to cough (??), right?

And you have now a per (??) repo. Earlier, everything used to be a monorepo. 
Now, you have a repo for every small little thing as well, right? Everything 
became, I would say, a node module, right? You write a function, it becomes a 
node module, right? And then, nobody really knows you need a node module or not.

But so, then, dependencies really to cough (??). So, a lot of these things 
exponentially scaled in the last few years. And so, this problem that we talked 
about, about how do you go ahead and manage risk in your environment, which is 
essentially looking at all the security findings that you have in your 
environment.

Figuring out what all, even software assets that you have. Forget the 
vulnerabilities first. What are software assets that you have, which we call as 
SBOM or Software Bill of Materials? What do you even have over there? How, what 
is the different tools that you are running? Do you, are you even scanning for 
all of these things, which are kind of important in your environment? And then, 
also then, going and looking at, okay, what are those tools reporting, right?

Combining all of this just gives you the visibility, right? So it gives you a 
pretty dashboard, but again, that is not the end. I mean, that's good to know 
that I have something, that's the first step. But then, how do you kind of go 
and automate some of the prioritization that you need to do with it?

So, building in that context about what is important, why this is important for 
me to kind of fix environment and being able to prioritize it in a way which is 
automated, becomes really, really key. And that's where Tromzo comes in. And 
that's why we bought, built Tromzo to help you kind of figure out, "Here is 
everything that all the tools are reporting, but this is what I'm going to 
prioritize."

And then, just prioritizing it also doesn't solve the needle, right? The key 
needle is that, how do you influence developers to kind of go and fix them? 
So, we've built out all the things that I talked about, like leaderboards.

Going and talking to engineers in the workspaces that they work in, making sure 
that we automatically comment in PRs, sending them Slack messages, and making 
sure that, you know, they have the full context of how something needs to get 
fixed. There's no need opening a JIRA ticket or telling them something if 
there's no fix available, right?

What are they going to do? Yeah, it is there, right? You know, big deal. So, 
making sure, you know, you make software security really easy for developers 
and having the tool that does that is essentially what we kind of, say, that 
that's what our vision is, and that's what we are driving towards.

And so, we've kind of built out, I would say, the initial framework of doing 
all of these things. And we have a lot of, I would say, thought leaders in this 
space where kind of helping us as well. We have 26 CSOs from leading 
organizations like Coinbase, Robinhood, and Lemonade, and a lot of other folks 
who are kind of coming and helping us build this thing in the right way as well.

So, the goal for us is to kind of make every software security team successful 
and, you know, they become the heroes of the company. And that's our really 
goal in making Tromzo.

[00:40:12] **Michaela:** It is sound really exciting. And well, I, I've been 
doing a lot of data mining at Microsoft. And, you know, Pack detection, finding 
duplicate Packs, and so on.

And I know, you know, it's quite a tricky task. So, how good are you? I mean, 
15 months in is probably not that long, right? So, do you see initial results 
that people are really happy with what you can do automatically? How you can 
group those things? How you can find applications, reduce that, prioritize 
that, and do that all automatically?

Is that working already really good? And what do your first bit of (??) users 
say? Your users? How far are you with this mission?

[00:40:49] **Harshit:** Yeah. I mean, so, we are very far, I would say, in 
making sure that, you know, there's adoption of the platform itself. So, we 
have paying customers today. And they're being, so, we started with high-end 
midmarket kind of, where, you know, there are at least like a thousand plus 
people in the company, at least, you know, 500 plus engineers.

So they have dedicated security team working towards resolving that. Because, 
as I said, we wanna make them heroes. So, they are really happy with the 
product. We've, what we started with was definitely the visibility piece, and 
then the automation.

And now, we are getting more and more entrenched into the developer workflows. 
Because every engineering team and every engineering culture is a little 
different, right? Some of our teams are customers that we work it, everything 
is open, right? They know everything about everything. Everybody is okay in 
learning about somebody else's vulnerabilities.

And it's like a, I would say, total open culture. There is another customer 
where everything is closed, right? Like, you can only show this to this person 
or you cannot even know what other services somebody else is working on. So, we 
are working through some of those workflows right now and building out those 
features.

And then the other big thing that we are doing now is also helping customers 
run some of these tools. So, for example, as I said, there are 11 tools that 
customers are using, but at the end of the day, they're not still doing 
everything that they could be doing, right?

So, maybe they're not looking at Go dependencies, or maybe they're not looking 
for secrets in code, or maybe they're not doing something else. So, there is 
always that gap in which that you have left something out, because A, you 
didn't have money, or B, you didn't have resources. So we are helping them 
bridge that gap as well.

So, because it's good to manage what you have, but it's also good to, or I 
would say, great to kind of actually make sure that you covered the entire 
office, right? So now, we are working with more security teams out there to 
kind of bridge the gap of what they have and what they want or where they want 
to be, and continue to that journey.

So our goal is, at the end of the day, if you ask me five years from down the 
line, what do you want Tromzo to be? We want it to be the platform that 
application security team goes to for all the application security needs. So 
today, if you think about an equal, it would be like a Salesforce.

For every sales engineer or every salesperson out there, they have Salesforce 
as their system of record that basically coordinates, manages everything to do 
with sales, right? Today, in security, there is, something like that doesn't 
exist, right? So that's what our vision is, to kind of build that system of 
record and system of engagement for all of security folks.

And then, also making sure that the developers also feel bought into it and 
they kind of work together with security on this platform.

[00:43:54] **Michaela:** It is sounds really exciting. I'm so happy for your 
journey. I, you know, I'm getting really like, wow, I would jump in in that as 
well. So, I'm going to link Tromzo, obviously, in the show notes so people 
should definitely check it out.

And I will also link your voice of the modern developer survey, and, yeah. 
Maybe some other links that you want me to put. And, yeah, I'm really happy 
that you have been here, Harshit, today. It was great to talk to you.

[00:44:19] **Harshit:** Thank you very much. And you too. Thank you.

[00:44:24] **Michaela:** Yeah, bye bye. I hope you enjoyed another episode of 
the Soft Engineering Unlocked Podcast.

Don't forget to subscribe, and I talked to you again in two weeks. Bye.
