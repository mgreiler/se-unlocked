# Harshit Security

[00:00:00] **Michaela:** Hello and welcome to the software engineering unlocked 
podcast. I'm your host, Dr. McKayla. And today I have the pleasure to talk to 
Harshit Chitalia. But before I start, let me tell you about my latest project. 
Awesome co reviews.com. Yeah, all my work on contributes has now its dedicated 
home at [awesomecodereviews.com](https://www.awesomecodereviews.com).

You will find articles. About code best practices, code checklists news about 
the latest research on code reviews and of course workshops and courses that I 
offer around this topic. So please hop over to 
[awesomecodereviews.com](https://www.awesomecodereviews.com) and check out my 
latest work. 



But now back to Harshit, Harshit is the co-founder and CTO of Tromzo and he's on 
today to share his knowledge on how to make security easier for developers. 
Before starting Tromzo Harshit spent eight years as director of engineering and 
Juniper networks where he experienced firsthand, how frustrating security can be 
for developers. So I'm super, super thrilled to have harsh here with me today.

Harshit, welcome to the show. 

[00:01:04] **Harshit:** Thank you for having me. I'm really excited.  

[00:01:08] **Michaela:** Yeah, I'm really happy that you're here. So Harshit, 
what makes it hard for developers or frustrating for developers?  

[00:01:18] **Harshit:** If you think about security I think there are several 
aspects to it. Right. I mean, if I, I think I have, I myself have been a 
developer for a very long time before I jumped the, to the management train and, 
and, you know, started taking up more leadership positions and, and being a 
developer is, is like wearing multiple hats, right?

Like basically you are writing software then making sure that you ship that 
software writing. And as we've now gone into the DevOps and, you know, C I C D 
and agile methodologies. Now we are no longer just looking software for the 
application that we are writing software for infrastructure as well.

Right? So we are managing microservices. We are managing the cloud and we are 
managing the end to end life cycle. So now a lot has been asked from one 
developer, right? So it's no longer, you asked for somebody who's full stacked. 
You ask somebody who's full. Plus DevOps plus SRE and plus presales or postsales 
right.

Like doing support as well now to mix all of these things with security is like 
completely new ballgame right now, because earlier security was all about 
firewalls. Like you protect your application by deploying a firewall, making 
sure there's no DDoS attacks and you can buy an application from Cisco or Palo 
Alto and, and.

But these days, most of the, the, the hacks that you see are all software 
vulnerabilities, right. Dependencies, which are vulnerable or software that you 
write is vulnerable. Right. So how do you kind of go and mitigate all of that? 
And it becomes really, really challenging for somebody who's new to kind of even 
understand like what the attacks office is like, what all possible things can be 
kind of wrong.

Right. So to give you an example, one of our customers. They use, like they, 
they have a standard stack, right? Like Python on the back end react on the 
front, end, deploy it in microservices, in the cloud right now, just this 
standard application. They use like eight different security tools to kind of 
make sure that the application is, is good enough that they can ship.

Right. So these are basically secret scanning code dependency, scanning 
infrastructure scanning, container scanning. Then you have just your source core 
analysis scanning, right? And, and so you could keep on like, just making sure 
that, that you are covered across all your bases. Now, if a developer, as a 
developer, you ask me, okay, in addition to everything that I'm doing now, you 
want me to go and look at eight tools and figure out like the hundreds of 
vulnerabilities that exist in my environment and, and something is coming from a 
dependency, which I don't even know what to do.

It becomes like a big mess. Right? So that's why like I would say security has 
become so difficult for developers and, and, and there has to be better ways to 
kind of manage these things. 

[00:04:11] **Michaela:** So I heard your talk mostly about scanning tools, 
right. Using tools and automatically. Security vulnerabilities.

What about manually actually checking those, right. It's also a hard problem. 
I'm all about code reviews and part of code review could also be to look a 
little bit as input validation, for example, are there sequel injections? Are 
there like, is there is cross site scripting possible? Do I have some.

Parameters you know, in as get set for example, and so on. Is that still 
necessary and are developers struggling with that in your experience as well? 
And because the, the, the tools somehow look at the different tech surface, 
right? They, they look at different kind of problems. They find a subset of 
those problems as well.

But is there still, this need also for developers to understand how to manually 
check for those problems and know about secure coding practice. 

[00:05:04] **Harshit:** Oh a hundred percent, right? Like everything that you 
mentioned about like your manually checking, going through quarter reviews 
looking for like things that can be inputted are all valid concerns.

And, and, and that has to go through like core training and, and making sure, 
like you're not, developers are even aware that these problems can be fixed. But 
if I look at the whole broader perspective of, of like a developers. Project 
right today. With all these open source technologies out there, developers are 
just writing if just purely from a line of code perspective, let's say, right.

So only 30% of the code is what developers write. The rest. 70% is coming in 
from third party libraries. Of some sorts or any of the infrastructure that 
you're already using. Right? So even if you manually record a view, things that 
your project are doing and your peers are doing, and that also in a very fast 
pace environment, it becomes really difficult to kind of keep that.

Happening, right. Mm-hmm so what, what we've observed is that like very few 
vulnerabilities get caught because somebody's doing a code code review and, and, 
and, you know, they, they point it out unless it's like right out there. Right. 
Typically it's through automation that people find with these vulnerabilities.

Right. And the other thing is like, people use a lot of pen testing tools as 
well, right? Like there is third party pen testers. There are in-house pen 
testers. And though pen testers, like they. Very differently. But at the same 
time there are model is that we want to replicate how an attacker would see it.

Right. Because the attacker typically won't have access to your source score. So 
they take it as a black box and they're trying to kind of go and, and really 
hammer your application. Right. So that's also one kind of, of a scan tool. If 
you think about it, like it's a security tool pen testing tool that will go and, 
and hammer your application as well.

But as I was saying, right, like today, In pretty much every leading 
organization. Right. You take Netflix, Coinbase. Yeah. You know, Airbnb, 
everybody does security through automation, right? Like, I mean, if you are 
starting on a new project, there's no way that you can go ahead and say that, 
okay, I'm gonna manually go, go and find out vulnerability.

It, it's just a very large surface area. And, and today, even, even with like 
all these tools, it's difficult to manage risk, right? I mean, there's no 
software out there today. That is, I would say a hundred percent secure. Right. 
We have like fortune 500 customers who have over, I would say half a million 
vulnerabilities in their environment.

Overall. Right. But now that doesn't mean that, okay, you can go and hack any 
bank that you want today, right. Because they are managing risk, right. They are 
managing, okay, what needs to get fixed, how that needs to get fixed, what is 
the priority? They are dedicated teams for those things. Right. And so, so, but, 
but the way those things are, I mean, we can talk more about it from a security 
perspective as well, but the way some of those things are done is, is not the 
most efficient.

Even for smaller teams, right? Like we're just starting out. It becomes even 
more difficult to kind of manage some of these things as well. And I can talk 
about like a survey that we did recently to kind of figure out, like, what do 
application developers feel overall about security as well as, as we continue on 
this.

[00:08:22] **Michaela:** Yeah, it would be really interesting. One thing that I 
was wondering, especially if you are mentioning these large organizations, 
right? So for small organizations, I totally understand that, you know, one deaf 
has to wear so many hats and I also see this shift, right. That the person has 
to like developer is not only a full stack developer, but this DevOps ops, you 
know requirements and the security requirements and so on.

But aren't companies like the ones that. Mentioned, especially the large 
organizations like Microsoft or Google or, well, Coinbase is not in that. in 
that sphere, but still I think a larger organization, right? Same as Airbnb. I 
think they have dedicated security teams. Right. And so are the developers 
really responsible when I'm working with teams, especially from large 
organization and I bring up security and, and that they should think about it.

They're like, What our thing. Right. and, and to really try to get rid of this 
additional responsibility and say, well, you know, we have a team that actually 
does that. What's your experience here? Do you see that? 

[00:09:28] **Harshit:** Yeah. Yeah. I mean, we've definitely seen it, but you'll 
be very surprised that things are changing.

Okay. And and it's no longer about like, we have a separate security team. 
Right. And especially in, in the space that proso, or like my work currently 
kind of goes into, so, so security has like different facets, right? Like 
there's cloud security. There is application security and, and then there is 
like other areas about security as well.

So within application security, there is no way that the security team can go 
and. Like the issues, because they don't know anything about the code, right? 
The developers are the one who are writing the code, whether it's, they are own 
like software or application logic that they're writing or dependencies and, and 
containers that they're bringing up to kind of run their services.

It's all the application developers. So even at Google or, or at P. It's it's 
now that's why we talk about the shift left. Right. Everybody's trying to shift 
left, which essentially means that the developers now definitely like have that 
responsibility and I cannot totally understand. Right. It's like, like a 
cultural shift as well.

Right? So we, if you go back in the day, we used to have QA engineers, right? 
Like we used to have testers who would basically be responsible for testing the 
application. Now, if you look at it, most modern teams. Don't have a QA 
engineer, like more software teams just don't have that position anymore because 
the developer has taken the role in some bigger organizations.

You'll hear somebody doing S D E T, which is basically software developer in 
test, which is writing infrastructure to manage these tests. Right. Making sure 
the performance of these tests is good. You can run as many tests as similarly, 
like now what we are seeing. And security teams is security teams are managing 
the risk in, in your application, right?

So they'll define what we call a security guard. Where you can say, okay, this 
is the container image that you can use for our container services. This is what 
you can kind of push into your environment, or this is what you cannot do 
within, like, you cannot push out any secrets in your code. Like, like, so those 
kind of become security guard rails.

As, as you're developing code, and that is what the security team manages, but 
on a day to day basis, the vulnerabilities that come out of your software need 
to be addressed by the developers. Right. And, and yeah, developers, I know like 
some of them are, get really excited about security and some of them are like, 
Hey, not me, you know?

And, and so that is a big cultural. and, and so, and, and there are, we can talk 
about like how we can mitigate some of that changes as well, because we've seen 
companies like go through that transformation, right? Couple of things that, 
that have really worked well over there is, you know, push from, from the top, 
right?

Like if, if your CEO is emphasizing, okay, security is important for us. If your 
top level executors are telling you that, okay, we need to kind of do more about 
security. A large organizations have this position of a CSO, which is a, 
basically a VP level position or even higher. And, and typically if they have a 
board seat, that means that, you know, they are part of the executive team.

They have a position there and they are mandating security, right. So it becomes 
like one of the pillars in an organization. And it's always good to see that on 
the lower level, like on the, on the engineering side itself, we have. Teams go 
ahead and do gamification. Right? So now there are leaderboards happening.

Okay. This team introduced these many issues today. Okay. And this is how they 
are trending week on week or one on one right now that kind of. , you know like 
most engineers are gamers as well. Right? So you kind of put in all this 
gamification within, within like fixing issues and, and finding issues, then, 
then it kind of increases like the visibility as well as make sure that people 
are driven to kind of achieve a certain goal.

Right. Because it becomes like a community kind of a feel. And, and so we've 
seen a couple of organizations do that really well and where they are doing some 
of these gamification, they have a leader. Where, where they track these things 
and, and, and everybody's made aware of, of like what's happening in their 
environment.

[00:13:49] **Michaela:** Yeah. And what about tools? You were talking about 
tools, right? And that there are many tools and that the developers have to, you 
know, understand them, but aren't, we just, you know, set, you know, if we have, 
let's say some automated. Tool in our GitHub, in the CI CD pipeline, thinking 
about sneak for example, or, you know, deep source, some study analysis tools 
here.

Is that enough? Or 

[00:14:14] **Harshit:** what do we need? Yeah, yeah. That's a good question. 
Right? Like what do we need? So the thing is this, that security is one of those 
fields where you can never be sure that, you know it like it's like protecting 
your home. Right. Is a camera on the front door enough or do you need one on the 
back door?

Right. If you have both of these, do you need a motion detector? Right. So now 
it depends on like what you are guarding, right? What are your crown jewels? 
Right. Like, let's say it's a bank, then, then you need a camera every other 
place. Like you want to make sure that there's things everywhere. But let's say 
it's like a public library or something else where, where people are going to 
have access to everything.

So you, so it's all about managing risk, right? And then from a tooling, just 
tooling perspective. You need a different kind of a tool for everything that, 
that you are really trying to protect against. Right? So some companies are like 
API companies, right? Like for example, postmen, or like, let's say a Apigee or 
things.

So for them, API security becomes the most important thing. Right? So they would 
not just have one tool doing API security. They may have like three different 
tools doing all different kinds of API security. Right. But, but if I'm talking 
about like 80% of the organiz. Right. The seven, eight tools are basically what 
we call as SAS tools which do like source code analysis, dependency, checking 
contain like secret scanning.

Right? So in which like sneak comes in and there are a bunch of other players as 
well, like VR code and check marks and, and, and I mean, the list can go on and 
on, right. Then then the other side comes, which is like the infrastructure 
scanning, right. Where people are scanning for your Terraform code or your cloud 
formation code.

They're looking at your container images. Right? So things like Aqua security is 
there for container images. There are open source ones as well. The new thing 
that has come out is something called a supply chain security, right? Like how 
do you kinda. Make sure about like, not just everything that you are importing, 
but how much like of the supply chain.

So as to say of the software is also being, being imported in your environment, 
right? Like, so making sure that is all there. So, so there's this whole angle 
of supply chain security. And then you know, just finally it's, it's all about 
like your core, right? As I said, like either your APIs, if you're using Python, 
then there will be a Python.

Analyzer, if you're using react or Java script, there'll be a child. There'll 
like be a language specific thing as well. And then a lot of security typically 
goes with compliance as well. So you have like licenses as well that people need 
to monitor for, right? So there are license based checks and license based 
scanners as well.

Making sure you're not importing something, which is unofficially, like not a 
good license that you want to have in your enterprise product. Right? Like, so, 
so there are like all these different variations of things, right? That, that 
you would need to make sure that you're running a good application security 
program.

And, and in a survey that I was talking about, right. We. Well, basically 
there's, it came out to like 62% of the developers are using today 11 or more 
sec application security tools in their environment. Like, so you can see that 
that that number is high and it is going higher and higher as we kind of make 
everything software.

[00:17:31] **Michaela:** So what can we do to make it easier for developers? So 
we are talking about that, you know, we have this shift left there, they need to 
be more responsible for it. We are talking about that also infrastructure is now 
code, right? We are talking about that. There are so many tools, so what can we 
do to make it easier for them?

What can we do to reduce the friction? 

[00:17:52] **Harshit:** Yeah, absolutely. Like. And I think, I think there are 
three, three things here, right? Like it's it's technology process and people. 
Right. And we can talk about all three of them and, and how all of that can 
change to kind of aid in, in making this thing easier for everybody.

Right. So let's talk about the technology perspective first, right? So clearly, 
like if you have eight things that you need to. Like the human mind is not 
capable of doing that. Right. So it's easier that if there is one thing that 
tells you what to do, right. So you would need like in sort of an orchestrator 
or a management platform that makes sure that, you know, you are getting.

These reports from like these eight or 11 things and, and they are begging 
reported in a way that is meaningful to you. Right? So not that you have to go 
to a dashboard, but if the message is coming to you on a slack channel, right. 
Or coming to you directly on your PR, right. There's no point in telling me, 
okay, I filed a JIRA ticket because I introduced a secret in the.

It should come right there in the PR, right. So it should block the PR with it 
should not allow me to kind of go and merge something, which, which I should not 
be merging. So, so that whole notion about shifting left and taking it to, to as 
much left, right. Even going as further as like going inside your IDE.

Right. Having a good pre-commit hook, right. Like today to kind of validate some 
of those things as well. If, if I have to really talk about from a tech 
perspective, we need three things there. Like one is visibility of like what all 
things I have in my environment and why all of this is secure or not secure.

And like, what do I stand right now? And, and kind of measure that on an ongoing 
basis. The second thing I need is automation, right? Like making sure that if I 
have hundred thousand. Right. You know, typically like in, in container worlds, 
right? Like you will have like 500 vulnerabilities come up and typically the fix 
will be okay.

Go ahead and upgrade your O S. Right. And that will just solve 500 things. Now I 
can't go and file 500 tickets in JIRA. For example, for that one thing, it has 
to be like one thing and, and just tell me okay, exactly what to do. Right. And 
then as a developer, I can just go ahead and do that. So just managing that 
process, what the scanner is telling you and what the JIRA ticket is and how do 
I go and mitigate it.

That whole process can be totally automated. Right? And so there are many of 
these workflows that can be automated. In your environment. Right? So, so then 
workflow automation becomes a key thing from a tech perspective. And then the 
last thing is, is being able to just constantly monitor this, right? Like making 
sure.

There is a, an assistant bot. So as to say like, like your co-pilot, like your 
co-developer is constantly on your shoulder, just nudging you to do the right 
thing. Right. And making sure that it tells you right there and there, when 
you're about to commit a mistake or do something. That. Okay. No, no, no, no, 
that is wrong.

You can't do that. Right. So, so solving these three things from, from a tech 
perspective, I think become like really good. And there, there are a lot of 
other things that individually can be done in all of these three things, but I 
feel like just having that shift lit like mindset and, and being able to kind of 
go and, and finish that would, would really.

So, like, I would say 60 to 70% of this, then the rest comes into like the 
process and, and the people, right. Like when I said people let's talk about 
people first, right? Like security needs to be in the culture. Right? Like it 
needs to come down from the top that, that, you know, security is something that 
is important that you, you are allocated time.

Right? It can't be like, like engineers are asked to kind of, of course ship 
features, but they also need. We allocated certain time to fix security issues 
inside and inside their sprint planning, right. It can't be like, okay, we'll do 
security last, right. Security needs to be at the forefront. In fact, even bef 
if you're launching a completely new service, you should do security reviews 
before launching the new service.

Not that, Hey, I'm now already built that now, what do I do about it now? Have a 
big gap in, in this, right? So, so having that kind of a mindset is, is, is 
very, very important. And then having processes defined, right? Like how do you 
kind of ask for exceptions, for example? Right. Let's say the developer is 
really busy right now.

And, and he wants to ask for an exception. Okay. Give me couple of weeks before 
I can get to this issue. How can the security team manage that risk and make 
sure that, you know, that is kind of documented because the ratio of like 
security people to developers is really bad, right? Like if there's one security 
engineer to 200 develop.

If E like even 10% of them ask for an exception, there's no way that security 
can even just manage. Process. Right. So how do you manage those workflows and 
that processes and define them in your organization about like, what is 
considered like say P zero and what is like, how do you manage exceptions?

How do you manage due dates and how do you track SLAs? Right. All of those 
things. If you have a good defined process, Then things become really, really 
smooth. Right. You can, you can think about this being like very similar to how 
DevOps today works, right? Like you have Datadog and century doing this really 
day in, day out because they had to move.

It from dedicated DevOps, people to engineers who are now managing 
infrastructure. Right? So, so it's a very similar process that I think even 
security needs to get into, right. Where, where it's going to be continuous. You 
will have SLAs that you need to meet and you will have page duty alerts that 
need to get, get addressed as soon as the security issues found.

Right? So, so I. There is enough equivalent that we can see in other fields that 
has happened. And, and I'm pretty sure we can, we can embed some of those 
learnings within, within the security teams too.

[00:23:42] **Michaela:** Yeah. So especially the thing that you said at the 
beginning triggered a couple of thoughts for me, right? So if you have so many 
tools, obviously they're reporting so many issues and we have to assign them a 
priority. Right? We are also have to find because if we have tools, right, they. 
Normally, they're not like scanning for very dedicated things and they're 
overlapping, right?

So one tool finds a little bit more in this area, but a lot also in the same 
area as you know, the other tool. And so, you know, I'm getting, I'm getting, 
let let's say you are mentioning 11 tools. I probably get. Five times the same 
issue from all of those tools. Right. And so it would be good to have them 
together and then also assign some priorities so that I know what to look for.

I mean, it's already starting with studying analysis, right. I get all these 
errors and I don't even know where to look at or, or what to do first. So is 
that also what you are, what you are hinting at that, you know, it's really 
important to help Wade through all of those information that we are getting from 
all of those tools and especially from different tools, right?

Because within one tool, people obviously thought about, you know, how to 
package it and how to make it more adjustable. But if you have 11 tools they're 
not made in a way, you know, that they're used together. 

[00:25:03] **Harshit:** Absolutely right. You, you are a hundred percent 
correct. And, and that's, that's like the biggest problem today, right?

Because now you have 11 tools telling you some things which are different, but 
there are enough number of things which are overlapping as well. And so how do 
you kind of make sense of it? And the bigger thing is this. How do you even 
manage risk? Right? Like how do you kind of go ahead and prioritize it?

As I was saying that like, one of our customers has, has over like 3,500 repos, 
right. There are 200 engineers in the team and there are 3,500 repos. I mean, 
it's a, it's been, the company has been around for a long time. So of course, 
like, you know, you go through these phases. But as a security team, how do you 
even know what needs to happen to that 3,500 repos?

Like who's actually using those 3,500 repos or they are even deployed in 
production. Right. So if I go and scan everything, then I'm going to find like, 
as I said, over 200, 300,000 issues across all of these tools, then if I just 
have to go manually do one issue per. I'm looking at like years before I get to 
it.

And, and, and by that time there'll be 300,000 more issues. Right. So, so 
absolutely like, you know, combining all of these together correlating it, 
de-duplicating it. And at the same time, making sure that we can automatically 
prioritize all these things becomes like a easier priority, right. For, for a 
security team itself, like as an, as an imperative of, of how do you kind of 
manage risk and, and.

Yeah. I mean, that's, that's the fundamental problem that, that people are kind 
of facing. I mean, that's exactly the problem. That was the thesis before we 
started Zo. I mean, that is what I was facing back at Juniper as well. When I 
was when I was leading my team, right. I had three products over a hundred 
engineers and, and it, it was like a big, big issue for me.

And, and when I basically went out and talked to other engineers and some of my 
peers. In the industry and security folks it became like, yeah, it's, it's a 
problem for my team as well. And, and when I heard that over, you know, several 
times I said, okay, let's start a company and solve this problem.

[00:27:14] **Michaela:** Yeah. So another thing that I want to, you know, 
briefly talk about and you mentioned it at very, at the beginning was only 30% 
or something around this number is written in house, right? And the rest we are 
relying on more and more services. And, you know, we are all that happy that, 
you know, it's in the cloud and, you know I don't have to think about 
authentication because there are services doing it for me.

And I don't have to think about logging because there's an open source. System 
that can do it at already for me, a package that I can use. Right. And then we 
have like, luck for Jay and the vulnerabilities and so on. Right. And suddenly 
we are all facing, you know, real issues, real travels. But on the other hand, I 
mean, I have some scanners running, running for my little projects and they're 
just, you know, they're not high risk.

They're not, you know bringing in millions or something. So I don't feel that 
you know, I, I, I have a, a have a big issue. With with not updating them 
frequently or with some vulnerabilities. So I get weekly, I'm getting, you know, 
you are using some unsecure version over here. You should do something over 
here.

And it's really hard to. To keep up with that. Is that also something that you 
you think can be, can be 

[00:28:29] **Harshit:** improved? Yeah, no, that, that's a really, really good 
question. And, and definitely we need to kind of, you know and like, think more 
about, about that, right? Like at the end of the day, as, as you're saying, 
right, like you are running some of those projects and, and you are running some 
scanners and they are reporting some things to.

Do you need to go and fix them now? That's I feel like if, if, if I'm a purist 
then I would say, yes, you have to go and fix them right now. But at the same 
time, you have to kind of manage the risk of it. Like, for example, if you have 
something, what we call as RCE, which is a remote code execution, that pretty 
much means that that kind of vulnerability, if it exists in your system, then 
anybody can basically go and, and do anything in your environment.

Right. What happens is this, that there are few that come in and, and then they 
become like a big deal. Like the examples that you took of about log four J 
right. So one of the real use cases for using TRAs or for our customers was 
trying to find out where all log four J exist in their environment.

Right? Because they had today, no way to kind of figure out before Zo across all 
their services and assets and everything that they're using, how and. If I, even 
if I'm using that library or not. Right. So, so it becomes really critical to 
kind of identify what you want to kind of fix. Right. Because if the tool is 
just reporting okay.

That, okay. You have a, like a very critical severity, but let's say you only 
using it in your test environment. It's not even used in production. You're not 
shipping that software. Then probably you don't need to fix it as soon as, as 
it's it's there. Right. But at the same time, if, if, if you have something 
critical and it is internet facing, then, then you probably want to kind of fix 
it.

Right. So it's, it's not, it's one thing that the tool is giving you some 
information, but at the same time, you want to make sure that. You know, like 
you have a way to manage that risk and you define what is okay in your 
environment. Right. And that is the most important thing here because you 
cannot, and I can, I can, I can stress double there that you pretty much cannot 
fix everything that the tool is reporting to you.

There is no way you will have bandwidth to do that. Right. So then it's all 
about managing risk. And how do you kind of go about managing all.

[00:30:56] **Michaela:** So you run this survey that you already mentioned, 
right? The voice of the modern developer. What was the main finding that was 
surprising 

[00:31:04] **Harshit:** to you? So the, the key things that came out of the 
voice of the developer survey, right? Like some of the key things that were a 
little surprising for me were that one of, let me start with the first one, 
right? Like developers are, I mean, we've been talking about this, but even 
developers know about it, that they are fixing only 32% of the vulnerabilities 
that exist in the.

It today. So out of out of three vulnerabilities that are being found only one 
third is, I mean, only one is getting kind of fixed. I would say not a 
surprising factor, but, but the, but the ratio is, is, is quite surprising, 
right? I mean, we knew that we are not fixing everything, but just one third, it 
seems like quite a bit, especially these are all B2B applications or B2C 
applications.

Where, you know, it is actually generating a lot of money and revenue. The other 
thing that came out of this is a one third of the overall vulnerabilities that 
are reported by some of these scanners are also just noise. So now clearly the 
scanning companies also need to do a lot better here because if they feel that 
they're reporting false positives on that high level, right.

Because at the end of the. most scanners are just rules, right? Like they kind 
of check for patterns or check for things. And, and so if those are not really 
highly accurate or don't cover a lot of cases, then, then it becomes then it 
becomes a problem as well. So, so we see that, that, you know, developers are 
not too happy about it.

That, that, that, like, you know, there are so many vulnerabilities which are, 
which are just basically. and then the, the, the other thing was that, you know 
they found that they are actually pushing code, which is wonderful, like 42% of 
the developers push wonderful code once per month. So now this was also 
something interesting that they, they know that the code is wonderful, but they 
still are going and pushing it.

Because, because it's, it's like. it's they need to kind of go and deliver 
features at the end of the day. And they don't have enough bandwidth to kind of 
go ahead and fix some of these things as well. Right. So, so we are seeing all 
these different things pointing out to the same problem where the problem is 
massive.

There's not enough resources to fix it. And the, and, and the problem being 
massive itself is a problem in it itself. You know what I mean? Right. So it's, 
it's. It's it's, it's all coming together in such a way that, that clearly, if, 
if not mitigated or not addressed, it can really blow up to be like a major, 
major thing.

[00:33:50] **Michaela:** Yeah, I totally see that. Especially with studying 
analysis tools. Right. We have the same thing, right? So some people just turn 
them off or drastically reduce the rules. So that it's becomes fo first of all, 
manageable, but also meaningful, right? Because if you have all these false 
positives or little issues, you know, that are, you know, not that critical, it 
takes away from your attention.

Right. And so I think. Especially this prioritization and making sure that, you 
know, this is really something you should fix here. And you know, those, you 
know, because you said, well one third is only addressed, right. But one third 
is noise, right? So there's this in the middle another third, right.

Which we should actually look at, or at least way through and make sure that 
those important issues from this one third are, you know, covered or shifted 
somewhere. Yeah. I totally see. 

[00:34:42] **Harshit:** Yeah, exactly. And, and I think you, you read the 
numbers. Right? Right. Like, so, so that's, that's the, the gap here, right? 
Like, I mean and, and attackers just need one way to get in, right.

Like, I mean, they don't need one third or they don't have like too many things 
that, that they go for. Right. Like they just need one way. And so for you, it's 
like, how do you kind of mitigate it? And, and also the thing is that it's not 
that they're going to use the same. Thing year and year out. Right? Like, so 
earlier it was solar went.

Now it was lock for J now it was spring for shell and by December in Christmas, 
that would be something else. Right? Yeah. Like, so, so it's, it's, I mean, we 
definitely know that something's going to come up. So how prepared are you for 
this Christmas is essentially is, is, is the, is the question that Chi redeems 
need to ask themselves?

[00:35:33] **Michaela:** Yeah. Thank you so much. Hashi for, you know, all your 
wisdom and your insights into security. I think now is the time that you also 
tell a little bit more about Trusso it's the end of the show, right? And so 
maybe if people want to check it out you're working on this, right? You're the, 
the co-founder and CTO of this startup.

So. I think I understood quite a bit of the ideas behind of the motivations. You 
know, why you, why you are on this path, but maybe you can share a little bit of 
this path to, you know, wrap this, this episode up maybe also, how long have 
you, you know, Have you been doing this? Have you developed tr so and, and 
what's your solution, right?

What, what do you think is the right way? To do that in a, I guess software way 

[00:36:18] **Harshit:** yeah, absolutely. And, and thank you for asking that, 
so. Yeah, we started Zo about, I would say 15 months back. Right. So we are a, I 
would say a relatively new company, but at the same time, both me and my 
co-founder have like years of experience, both in engineering as, and as well as 
security.

Right? So we are not new to the space or new to the problem. The problem, as I 
said, just intensified in the last couple of years, right. With, with everything 
becoming. Right. Like, as I was saying that network, it became software, your 
infrastructure became software, your microservices, just to cough. Right.

And, and you had now a per repo earlier, everything used to be a mono repo. 
Right now you have a repo for every small little thing as well. Right. 
Everything became like, I would say a node module, right? Like you write a 
function, it becomes a node module. Right. And then nobody really knows you need 
a node module or not.

But so, so, so then dependencies really to cough, like, so a lot of these things 
exponentially scaled in the last few years. And so this problem that we talked 
about about like, how do you go ahead, like, and, and manage risk in your, in 
your environment, which is essentially looking at all the security findings that 
you have in your environment.

Right? Figuring out like what. Even software assets that you have forget the 
vulnerabilities first. Like what are software assets that you have, which we 
call as SBO or software bill of materials, right? Like what, what do you even 
have over there? How, what, what is the Different tools that you are running, 
like, do you, are you even scanning for all of these things, which are kind of 
important in your environment and then also then going and looking at, okay, 
what are those tools reporting?

Right. Combining all of this just gives you the visibility, right? So it gives 
you a pretty dashboard, but again, that is not the end, right? Like, I mean, 
that's good to know that I have something that's the first. but then how do you 
kind of go and, and like automate some of the prioritization that you need to do 
with it.

Right. So, so building in that context about like, what is important why this is 
important for me to kind of fix environment and being able to prioritize it in a 
way which is like automated right. Becomes like really, really key. And that's 
where proso comes in. And that's why we bought built proso to help you kind of 
figure out like, Here is everything that all the tools are reporting, but this 
is what I'm going to prioritize.

Right. And then just prioritizing it also doesn't solve the needle. Right? The 
key needle is that, how do you influence developers to kind of go and fix them? 
Right. So, so we've built out like all the things that are talked about, like 
leaderboards, right. Going and talking to, to engineers in the workspaces that 
they work in.

Right. Making sure that we automatically comment NPR. Sending them slack 
messages and, and making sure that, that, you know, they have the full context 
of like how something needs to get fixed. There's no, there's no need opening a 
JIRA ticket or telling them something, if there's no fix available.

Right. What are they going to do? Yeah. It is there. Right. You know, big deal. 
So, so making sure, like, you know, you make software. Security really easy for 
developers and, and having a tool that does that is essentially what, what we 
kind of say that, that that's what our vision is and that's what we are driving 
towards.

Right. And so we've kind of built out, like, I would say the initial framework 
of doing all of these things. And, and we have a lot of, I would say thought 
leaders in this space were kind of helping us as well. Like we have 26 CSOs from 
leading organizations, right? Like coin. Robin heard and, and like lemonade and, 
and a lot of other folks who are kind of coming and, and helping us build this 
thing in the right way as well.

Right? So, so the goal for us is to kind of make every software security team 
successful and, and, you know, they become like the heroes of the company and, 
and that's our, our really goal in, in, in making. Yeah, it sounds 

[00:40:12] **Michaela:** really exciting. And well I, I've been doing a lot of 
data mining right at Microsoft and, you know, back back detection, finding 
duplicate parks and so on.

And I know, you know, it's quite a tricky task, so how good are you? And I, 15 
months in is probably. Not that long. Right. So do you see initial results that 
people are really happy with? What you can do automatically, how you can group 
those things, how you can find applications, reduce that, prioritize that, and 
do that all automatically.

Is that working already? Really good. And and what do your first better USSA or 
do you use users? How far are you with this? 

[00:40:49] **Harshit:** Yeah. I mean so we are very far, I would say in, in, in 
making sure that, you know, there there's adoption of the platform itself. 
Right. So we have paying customers today. And, and they're being like, so we, we 
started with like higher end midmarket kind of where, you know, there are at 
least like a thousand plus people in the company at least like, you know, 500 
plus engineers.

So, so they have. Dedicated security team working towards resolving that. Right. 
Because as I said, we wanna make them heroes. Right. So so, so they are really 
happy with the product, right. We've what we started with was definitely like 
the visibility piece and then the automation. Right.

And now we are getting more and more. Entrenched into the developer workflows, 
right? Because every engineering team and every engineering culture is a little 
different, right? Some of our teams are customers that we work with. Everything 
is open, right. They know everything about everything. Everybody is okay in 
learning about somebody else's vulnerability.

And it's like a, I would say total open culture. There is another customer where 
everything is closed, right? Like you can only show this to this person or you 
cannot even. Know, what other services somebody else is working on. Right. So, 
so we are working through some of those workflows right now and building out 
those features.

And then the other big thing that, that we are doing now is, is also helping 
customers run some of these tools, right? Like, so for example, as I said, like, 
there are 11 tools that customers are using. , but at the end of the day, 
they're not still doing everything that they could be doing. Right.

So maybe they're not looking at go dependencies or maybe they're not looking for 
like secrets in code, or maybe they're not doing something else. Right. So there 
is always that gap in which that you have left something out because a, you 
didn't have money or B you didn't have resources. So we are helping them bridge 
that gap as well.

So, because. It's good to manage what you have, but it's also good to, or I 
would say like great to kind of actually make sure that you covered the entire 
office. Right? So now we are working with more security teams out there to kind 
of bridge the gap of what they have and what they want or where they want to be 
and, and continue to that journey.

Right. So our goal is like at the end of the day like if you ask me five years 
from down the line, what do you want drummer to be right. We want it to be like 
the, the platform that application security team goes to for all the application 
security needs. Right. So today, if you think about an equal and would be like a 
sales force, right.

For every sales engineer or every salesperson out there They have Salesforce as 
their system of record, right. That, that basically coordinates, manages 
everything to do with sales. Right. Today in security, there is something, 
something like that doesn't exist. Right? So that's what our vision is to kind 
of build that system of record and system of engagement for all of security 
folks.

And then also making sure that the developers also feel bought into it and, and 
they kind of work together with security on this. 

[00:43:54] **Michaela:** It sounds really exciting. So happy for your journey. 
I, you know, I'm getting really like, wow. I would jump in in that as well. So 
I'm going to link Zo obviously in the show notes.

So people should definitely check it out and I will also link your voice of the 
modern developer survey. And yeah, maybe some other links that you want me to 
put and yeah, I'm really happy that you have been here. Hashi today was great to 

[00:44:19] **Harshit:** talk to. 

Thank you very much. And you too. Thank you. 

[00:44:24] **Michaela:** Yeah, bye bye. I hope you enjoyed another episode of 
the soft engineering unlocked podcast.

Don't forget to subscribe. And I talked to you again in two weeks. 

[00:44:37] **Harshit:** Bye.


