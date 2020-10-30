# Transcript Episode 7 with Charity Majors

**Michaela:** [00:00:00] Hello and welcome to the Software Engineering Unlocked
podcast. I'm your host, Doctor McKayla and today I have the pleasure to talk to
Charity Majors. Charity is the CTO and founder of the startup called Honeycomb. 
Honeycomb helps modern development dev ops and site reliability engineering 
teams operate more efficiently, string ableing, observability and monitoring 
of their systems. Before starting her start up journey, Charity worked for 
Parse, a company that was acquired by Facebook. 
Well I'm super thrilled that I can ask her today what observability means to 
her, how she assesses engineering excellence and how she decided to start her 
own business.
Thank you Charity for being on my show. 

**Charity:** [00:00:42] Thanks for having me. 

**Michaela:** [00:00:43] Yeah, I'm really thrilled. So Charity, can you tell me
a little bit about your startup? How long does it already exist and why, 
and how did you start that company? 

**Charity:** [00:00:53] Yeah, totally. Um, we have been around for, 
it'll be four years on January 1st. And, and I started it cutting right out 
of Facebook.
Um, I was at Parse right before this mobile backend as a service. I was the 
first infrastructure engineer there. We were acquired by Facebook a couple of 
years then. And I was there from before, like pre beta till there was well over
a million apps. And I left Facebook fully intending to go be an engineering 
manager at Slack or Stripe or something.
And instead kind of settling went, I had had this experience at Parse where
, um, You know, it was, it was down all the time. We were doing all of 
these exciting things that we now have names for, like, you know, microservices
and stuff. We didn't have names for it. And we just knew that everything was 
breaking all the time and we had to do terrible rewrites, et cetera.
And I had, like, I had come, I was coming to this horrified conclusion that we 
had built a system that was basically undebuggable. By some of the best engineers 
in the world, some of the best I've ever worked with all doing the quote 
unquote, the right things. And yet it was down constantly. Like every day it was 
going down and, and, and not just, it wasn't just reliability, even if it was 
up, we just didn't understand it.
You know, like a user would write in and be like, you know, complaining that 
parcels was down or complaining about the performance or something. And it would 
take us. You know, hours, if not days to track down, was it a real problem? Was 
it, you know, for the imagining things, did they not plug their network in?
It's just about impossible to reason about, and we'd have triggered that by 
brute force. And I tried every tool out there, every monitoring metrics, 
logging, you know, APM, everything, and everything was really good at giving me 
answers to questions that I. That I knew. Right. But like, I didn't have that 
kind of problem.
What I had was problems where I had a vague report or two or three from 
unreliable narrators, or I had a suspicion, the problem is not answering 
questions. The problem is figuring out what. The question was like, by the time 
I knew what the question was, I usually knew what the answer was. Like. The 
answer usually comes before and the question is distributed systems problems.
And at some point we start to get some of our data sets flowing into this tool 
at Facebook called scuba. And that was when like, The sun started to come out 
because the time it took us to understand these complex systems problems 
dropped, just dropped like a rock, like from, you know, days to two seconds or 
minutes, you know, and like reliably.
So like predictably. So like it wasn't even an engineering problem. It was like 
a support category problem. This made a huge impression on me, obviously, you 
know, like when I was leaning Facebook, I, I suddenly realized, you know, I no 
longer knew how to engineer without this stuff that we had built. Like it 
becomes so fundamental.
So core to this, like my five senses, you know, for understanding systems and 
my, my friend, Christine, who was also a purse, she had had a different, but 
similar experience. I mean, we decided to build this. And it was only over the 
course of that first year, 2016. When we started talking to users that we 
started to realize just how much anger there was tools that you know, and these 
tools that they're great tools.
I'm not trying to shit talk them, you know, they're great tools. And when they 
started shelling out a lot of money for them, they genuinely solved their 
problems. It was, it was like magic. You know, um, that was mostly like all of 
these tools were started back in the days with the monolith and now like we've 
blown up the model.
It now, you know, it hops to network and, and so we can't use the debuggers 
anymore. And yet. The tools that we use to try and understand it and monitor it 
really hadn't changed. And there's, there was just this enormous, like we 
started talking about the things that we were doing that were different and it 
really resonated with a lot of people very quickly, which was, which was a 
surprise.

**Michaela:** [00:05:02] And so the first step with starting your company was 
actually talking to users, or did you have already a prototype? What was the 
first thing that you did. 

**Charity:** [00:05:11] Oh, no, we had nothing. We had four slides and we didn't 
even really know what we were building. We just knew that we had had this 
experience that was really, really powerful.
And we didn't even know why. 
So 

**Michaela:** [00:05:23] you said it really started from a problem 

**Charity:** [00:05:26] problem space. Okay, 

**Michaela:** [00:05:27] cool. And so then you went and you found different 
customers or not even customer users. Right. And do you want to see if they have 
the same problem? 

**Charity:** [00:05:36] Honestly, we kind of went heads down for a year because. 
You know, I've spent my entire career career telling people, never write a 
database, just don't ever write a database.
Well, we kind of had to go and run a database, or I will, I will, I will protest 
weekly that it is a storage engine. This is a distributed storage engine, but 
like, you know, the things that we realized that were so important, high 
cardinality, these arbitrarily wide events. There's nothing out there that can 
handle it.
Right. And so we basically just for a year, we just went heads down. We started 
writing this, this, the storage engine and in parallel, Trying to figure out 
what it was we were building and why, and how to talk about it. And honestly you 
think that writing a database would be the hardest thing, and it was not trying 
to figure out how to talk about it was by far the hardest thing we ever had to 
do.
**Michaela:** [00:06:33] And so how did you figure out how to talk about that? 
**Charity:** [00:06:37] Well, after about six or seven months of freshing and, 
and like flailing and, and being unable to sleep and, and, you know, being so 
frustrated, like every term and data is so overloaded and overused. Um, it was 
July that year that I actually created major.
I, I. I happened to Google that the meaning of observability is kind of on a 
whim. And, and that's when I realized that it had this really rich pedigree that 
came from mechanical engineering, right? Like everybody is a mathematical duel 
of controllability and the extent that you can, um, you know, Observe the 
outputs of the system.
You could infer what's going on internally. Like you can understand. And that 
was when light bulb just kind of went off in my brain. I went, Oh shit, that's 
what we're talking about. That's exactly what we're trying to build. We're 
trying to build a tool that will let you understand any state that the system 
has gotten itself into.
Even if you've never seen it before, it's never happened before. You don't have 
to predict it in advance. You don't have to see it before to parametric. You 
should be able to. Understand what's happening inside this complex system. Um, 
and, and, and that, that was when I started to realize why that was so 
important.
**Michaela:** [00:07:52] Yeah. So one of the things that you talk a lot about on 
your blog as well is that you want to make the on call experience better. And 
that being on call should be, you know, it shouldn't be a drag. It should be 
something that's, that's fun. Maybe even, um, 
**Charity:** [00:08:10] it should be. 
**Michaela:** [00:08:11] How do you think that we can get to such a state?
And why do you think it isn't for, for many of the people, why is on call and a 
little bit in anxiety, introducing experience right now? 
**Charity:** [00:08:23] Yeah. Well, it's really scary because you feel like 
you're on your own and anything could happen, you know? And so like, I, I, I 
increasingly think of these systems that we're building is being very they're 
sociotechnical systems.
Right? You can't look at it. Just the technology. You can't look at just the 
people like there either. There's a lot of back and forth and interplay there 
and on-call has gotten a lot scarier, right? Because you are encountering so 
many different new problems. You can't just like get trained on it. And after 
six months of doing it just.
You're trained. It's cool. You know how to respond to everything that happens. 
If there's a, runbook like, there's no, runbooks where we're going. Right? Like 
the time that you spend on a runbook is largely wasted too, because like, you 
know, you don't see the same things break over and over again because right.
Fix them. But there's just as many weird little, you know, ways that it can 
break like left for you to discover. I guarantee you so like, Problems have 
gotten way more complex and open-ended, system's gotten bigger as such that no 
one person can fit a model of the end of their head. And just reason about it.
Like you used to just be able to close your eyes and imagine the request 
entering, you know, at the edge. And you can just visualize it. Boom, boom, 
boom, boom. When it comes out, right? Oh, you can't do that anymore for most 
systems. And if you try, you'll be shooting yourself in the foot because you'll 
have an inaccurate cash of the data in your head and you really need to.
Kind of give up and put this in a tool where everyone has equal access to it and 
it is more or less up to date. So like systems are getting harder, more complex. 
Uh you're you know, less and less of it. Um, and, and the stakes are going up, 
right? So it's like a perfect storm. And in ops we have such. A well deserved 
reputation for masochism for a 50 payment on ourselves and like the, the martyr 
complex and, you know, it's, it's deserved and like I'm over 30 now.
I don't want to get woken up in the middle of the night either. Like, I'm sorry, 
I'm done with that. 
**Michaela:** [00:10:26] So what do you think, can we do about that? What can we 
do to make it better? 
**Charity:** [00:10:32] I feel like the first day is putting software engineers 
on call or at least in a position of ownership over their code. Because as it's 
getting harder and harder to operate software, um, it's getting harder to 
operate it unless you notice supposed to do right.
Unless you built it or unless you're. Updating it, and, and there's this 
beautiful virtuous feedback loop that gets created when the person who has that 
original intent in their heads is writing the code, you know, deploying this 
system, watching it, seeing how it performs. Well, real users are using it in 
production and fixing the problems that they see.
But if you break that up so that the person who's writing the code, just kind 
of. Hits, you know, merged a master and walks away and doesn't, and doesn't 
follow it all the way out to production. Ooh, person, who's trying to debug it. 
Doesn't have that original intent. It's just bad. You know, like there are so 
many pathologies that have come out of this whole, like breaking up this 
virtuous feedback loop and we're just starting, we're just starting to build it 
back up again and put people like in a position to see all the way through its 
life cycle.
**Michaela:** [00:11:46] Yeah. So I, I noted you aim and also measure 
productivity and high performance by the ability of a team to write code and 
ship it. Right? The, the time that actually, you know, passes from writing the 
piece of code that it's actually in production. That's also one of those 
measurements. That's a very good indicator for well, for high performing teams.
Right? One of the things that I thought about is how do you think that, for 
example, QA departments or manual testing. How does that fit into this dev ops 
life cycle? Where we, you know, we write the code and we ship it. When is the 
right time that, you know, manual testing takes place when our QA departments or 
are they actually all obsolete?
Right. 
**Charity:** [00:12:33] Yeah, they're not obsolete any more than, you know, 
people are always proclaiming that, you know, QA is dead or ops is dead and any 
we've still got software and it still breaks a lot. So I guarantee you, like, 
there's still a need for us, but these are becoming niche specialties. Right? 
Um, the, the general software engineer is expected to know how to write tests 
and.
They're increasingly in, in, in my view, um, we like, it's like the first wave 
of DevOps was very much about yelling at off people to learn, to write code and 
like message received, you know? Yes. We all write code now, but like the second 
wave of DevOps is, is still in its early stages. And it's really about, okay.
Software engineers, like you're a turn. Now it's time for you to learn, to build 
operable services and learn what it means to operate your software and learn how 
to build software. That is maintainable build software that doesn't wake you up 
all the time, build software, that's resilient, build software that is, you 
know, self-healing build software that is understandable and well instrument it 
and all these things.
And we're very early on in, in that. And, and, and like SRS, um, ops people like 
myself are increasingly force multipliers who know how to build systems really 
well. Right. And, and we can help you own your software. And I think the same is 
true of QA, um, where, you know, they're experts in testing. There's a lot of 
stuff.
There's a lot of depth there that the average sufferer in New York just has no 
clue even exists. And so for systems that have super higher quality needs, um, 
you know, Testers can come in and consult with engineers to help them, um, test 
better, um, as for, yeah, for the stuff like, you know, manual testing and so 
forth.
Um, I feel pretty strongly that it can't be allowed to bring up this virtuous 
cycle and there are a lot of ways to get code into production fast, um, without 
necessarily, you know, Turning it on for all users, you know, there's feature 
flags, there's, you know, progressive deployments. There's, you know, there are 
lots of ways to do this, that don't.
Add that don't break that up and make it so that you can't actually like 
completely, uh, I don't think that most people we'll have started really fixing 
the organizations, but, but they're going to have to, because the companies 
that, that do, um, move a lot faster, experiment a lot faster, make better 
progress and they will.
Out-compete the people who don't. I 
**Michaela:** [00:15:07] find it really interesting. You said I also would see 
that as staging areas, right? You would have maybe staging areas and then before 
it goes to production, or as you said, you have like switches that you only turn 
the cold on for, you know, a subgroup of your users. How would you, as an expert 
in that field define what would be an optimal way to do that?
Is there an optimum 
**Charity:** [00:15:28] way for me to staging? I tell people. Do you really need 
staging? Can you turn it off? Like really? And I'm not actually that much of a 
radical, I'm not an abolitionist. I'm not saying everyone should get rid of 
teaching, but a lot of people who have staging areas don't really need them.
And there's a real cost to keeping staging areas around. It is really hard to 
keep them in sync. Honestly, you can't keep them in sync any, and you probably 
shouldn't try. Um, It can be a huge black hole for engineering time, especially 
now that we have distributed systems where like, what are we going to spin up a 
copy of Facebook to test Facebook every time?
No, they're not. And so, because it's not the same environment with the same, 
you know, load patterns, um, the lessons that you learned from running things 
and staging, you're always going to be wrong. They might be useful to a limited 
degree where that stops, you know, it was always up for debate. I, I feel like 
right now, people are just starting to realize how much they have been over 
committing so many cycles to staging environments and fake environments and 
therefore starving production of.
The engineering cycles needed to, they do things like the guardrails build 
things. So that the thing that you do default, the easy thing is the fastest 
thing is the most convenient thing. And it's the obvious thing. So that it's 
actually hard to do the wrong thing. The disastrous thing, the terrible thing 
that will, you know, all your data to me, like the definition of it, the senior 
engineer is someone who's intuition.
And instincts I trust, right? The senior engineer is like, I have a really bad 
feeling about this. I will stop and we'll figure out why. Right. You only get 
that kind of intuition and instinct by spending a lot of time in production. You 
do not get it by spending time in staging. And in fact, you learn like your 
internal, like machine learning brain, um, Learning on staging environments 
learns the wrong Corpus of data.
It learns the wrong instincts about what's going to be slow versus fast. What's 
going to be hard to do. What's going to be easy to do it. It incorrectly learns 
that things are okay when they're not at scale. Uh, and it's just. It's it's, 
it's a net negative, honestly, it's, it's not useless. There are uses for it, 
but it's, it has a lot of costs that people don't really factor in.
So 
**Michaela:** [00:17:58] how much of this advice do you think is specific to a 
business or, you know, the size of the company? 
**Charity:** [00:18:03] Everything is specific. 
**Michaela:** [00:18:05] And do you think that something can be generalized from 
that? 
**Charity:** [00:18:09] There's something that can we generalize it's this, 
every single company, every company has in common is we have a limited number of 
engineering cycles, right?
Even if even very large companies have a limited number of hours in the day 
engineering cycles. And a lot of times the argument will get made, Oh, we don't 
have time to do this in production. It seems extra teams, you know, and. I, I 
argue, I have never seen a company that shouldn't move some of those cycles that 
are being spent on falsified environment staging and reallocate them to project.
Like every company I know is under invested in, including mine has underinvested 
in their deploy process, giving it to interns, giving it to people who are, you 
know, just kind of hacking shit together, you know, or clone something off, get 
them. No, no, no, this is good enough. You know, when that's the most important 
software in your company and.
Every engineer should be able to deploy. Uh, and yet, you know, play code is 
isn't it unloved? It is unmaintained. It is nobody. I don't know if anybody 
who's built a really, Oh, I know of one. Facebook has a really nice built system 
actually. Um, but you know, for people that are complaining that they don't have 
the time energy takes in the cycles away from stage, you can give them to prod 
and that can absolutely be generalized.
Okay. 
**Michaela:** [00:19:24] And so you said even your, your own company, 
**Charity:** [00:19:27] um, has, 
**Michaela:** [00:19:29] you know, it doesn't give as much love to that area as 
it should be. Why is that? What do you think? Why are people not investing? 
**Charity:** [00:19:36] Because we have seven engineers, we have seven 
engineers. And for the past year we've been like in, you know, hardcore sales 
enablement mode, trying to raise money, trying to get past this hump.
And that means that we have to think very, very, you know, Critically about what 
we're going to spend our time on and anything that is not for the, for the past 
six months, you know, anything that was not contributing towards getting new 
customers, onboarding customers faster. Um, got deprioritized now that we have 
gotten past the fundraising, we are starting to go back and pay down some of 
that tech debt we accrued.
Yeah. 
**Michaela:** [00:20:12] Yeah. So one of the things that I read on your blog, 
where you said rules actually inhibit the development of good judgment. And I 
think that says a lot about your team culture and your mentality. So, um, how 
would it look in, in your company? What policies, what rules do you have, or you 
don't have any policies or rules, how much, you know, how much empowerment have 
your engineers and things like 
**Charity:** [00:20:38] that?
Aye. No rules can, can be, you know, constraints can fuel creativity, but like 
the kind of rules I had in mind were like, you know, no deploys on Fridays. 
Well, that doesn't teach you why it's important or how to use your good 
judgment. It just tells you don't deploy on Fridays. And any other time is fine.
Right? When in fact the more, the more subtle approach that I would like people 
to take is anytime you're. Thinking of merging to master use your judgment. Is 
it seven o'clock at night? Is anyone else around? Are you okay to walk out the 
door? If so, I don't care if it's Friday or Tuesday, like don't merge because 
you know, what's going to get automatically deployed.
I have a higher bar for merging things on Friday than I do for emerging things 
on Thursday. Right. Um, and I feel like I'm encouraging people to. Exercise this 
judgment and building incentives so that they feel the impact of the mistakes 
that they make. Yeah. That's nature's teacher and it's how you build good, 
thoughtful, careful engineers.
**Michaela:** [00:21:50] So you have been at Facebook and now you are 
**Charity:** [00:21:54] leading 
**Michaela:** [00:21:55] that, uh, small startup. What's the main differences 
that you see, especially for the development of software. Right? 
**Charity:** [00:22:03] Well, One of the reasons that I like small companies is 
because they run in a very human scale. Right. I love seeing everybody's face.
They're just very special to me. And I love seeing their faces makes me happy to 
be around them. I know them, you know, I can tell them having a bad day. Um, and 
it's, it's, it's very personal. Um, and at Facebook it was just like, you know, 
I. I was there for three years and I still be walking down the hallway and 
recognizing almost nobody and yeah.
You know, Facebook. Yeah. The only place in my entire career, the only time that 
I've ever like walked into a meeting room and had people like, look me up and 
down and go. How technical are you F again, I was just like, fuck you. Like, I'm 
here, you're representing a developer tool. I'm the only person from my country.
Just give me the benefit of the doubt. You know, let's just assume just Roundup. 
Shall we? I just, it was really annoying. Yeah. 
**Michaela:** [00:23:01] Yeah. That's strange. 
**Charity:** [00:23:02] It's not strange at all. It's Silicon Valley. I've 
gravitated towards smaller companies. So I've always, you know, people know who 
I am pretty quickly. Yeah. I'm not particularly shy or quiet.
Um, and so I just never, I've never had to deal with that anonymity. 
**Michaela:** [00:23:19] I think it's better on the smaller companies because 
people know who you are and know what you know, and you don't have to, you know, 
prove that all the time you 
**Charity:** [00:23:27] can't a hundred percent generalized here. People have 
had bad experiences at small companies where, you know, they're surrounded 
peoples that they don't like, and it's very.
You know, personal and I can't get away from them and it's terrible. Right. But 
I've had really good experiences honestly, in my career. So that's true for me. 
Another like, um, another big difference as far as developing software, you 
know, at the big companies, like. You know, Netflix, Facebook, Google, or 
there's a ginormous submerged like iceberg of tools you rely on every day 
without even knowing that they are.
And like, anytime you have the thought, it's something that maybe should be 
better. Somebody's already built it, or there's a team for that. And like, all 
you really have to do is stay in your lane and just churn out little chunks of 
things, which. You know, half the time your project gets canceled before it ever 
goes live.
And that's just kind of, you just kind of learned to not get too emotionally 
attached to your work at a big company, because there are always these forces 
going on way above your head, above your pay grade, and you have no visibility 
into them. And sometimes you just hand down edicts that just totally screw you.
And you just, you just have to not be too mad about it. Right. Whereas with, you 
know, with a tiny startup like ours, like. Everyone is very into everyone, 
chooses their own work. You know, we set priorities for the company. We talk 
about what's, you know, there's a lot of, you know, interdependency, but there's 
a lot of autonomy.
And we really, you know, we rely on everyone's creative brains coming to work 
and helping us figure problems out from scratch. And I find that a much more. It 
shit's a lot more rewarding in terms of the type of work. 
**Michaela:** [00:25:08] Yeah. So one of the things that you wrote about blog as 
well is it's one of the blog posts that I, that really resonated with me was the 
engineering management to credential them or the letter.
And then you write about the pitfalls. A developer can get themselves into when 
they pursue a management career. And reflected at least, right? So that they are 
actually drifting away from the technical expertise and they still have to, you 
know, get to know their social skills or up their game in the, in that area.
And that after sometimes they are somehow in a space where it's hard to navigate 
away from that. Now that you are delete. Off your company. Well, now you're in a 
CTO, but at one point you were the CEO as well. Do you feel that you are also in 
the management position or are you very technical as well? And how do you keep 
that balance?
**Charity:** [00:26:02] You know, I spent six months bootstrapping the 
infrastructure and like building the first version of everything. And then since 
then, The biggest problems have all been not engineering problems. Yeah. They've 
been honestly, there there's technical aspects to them. Like there's like trying 
to figure out, but it's a lot of, it's just like trying to figure out how to 
explain or convince or convey or break down or, or customer, you know, advice or 
like how to, you know, how roll the red carpet right up to a team's front door 
so that it, so that they don't have to do a lot of work to try and.
Figure out how to incorporate us. Cause we have kind of done that work for them. 
You know, I really do think that. Not every senior engineer, but most, every 
senior engineer should try management. Um, doesn't mean you have to manage , but 
you know, management is just a collection of skills and experiences and, you 
know, you can pick up some of them, like you can get, you can get an intern, you 
can get, you know, you can do some project management, you can do some product 
planning you can do, you know, and, and I really think that.
If you're on, if you're on the fence, you should try management, give it two 
years because the skills you take back, even if it's not for you longterm, like 
doing that for a couple of years, putting down what you're good at is very 
humbling. It really forces because you to enter that beginner brain space again, 
which is very healthy and, and, and having the experience of, you know, figuring 
out how to.
Make it a small herd of humans, I'll go in the direction that you, you want them 
to, or that they need to, like, it's learning how to inspire people and how to 
motivate people and how to think about and communicate with the people around 
you. And it will absolutely make you a better engineer. It'll make you better at 
anything you do if you are better at people.
So I'm a big fan of just like. Demystifying that, you know, making it clear that 
it's not a promotion and if it's not a promotion, if it's just a career change, 
then it's not a demotion. If you want to go back to being an engineer after 
that. Right. I think it's a very healthy way of looking at it. I think that 
hierarchies are mostly poisonous and it should be inverted or are left to die.
Um, so I, I do like thinking of it as a support role and a communication role, 
but I think that there is no such thing as a great. Senior technologist does not 
have these skills. 
**Michaela:** [00:28:30] Yeah. So I interviewed life singer from automatic or 
recently, and automatic doesn't have, for example, the management roles as 
promotions.
So it's, it's just, as you said, it's a different career track. Right. And I 
liked that very much in life said exactly the same. So if you don't like it, you 
can just switch back. Yeah, it doesn't matter. And then people choose that that 
are really good at it. 
**Charity:** [00:28:53] Ego doesn't have to get wrapped up on it. Yeah, exactly.
Yeah. And then you get people managing, not because they get more money, they 
get more respect, they get more power. Those are not the people you want 
managing teams. Right? You want the people managing teams who, whose hearts are 
really in it and who really get joy out of helping other succeed. And I'll be 
honest.
That's not me. Not really, you know, but, but I know that yeah. Now, and I don't 
regret it and, and it's, and it's been wonderful to learn those skills. And, you 
know, I learned more about myself, learn more about those around me, and now I 
can choose whether or not it's worth it to me to, you know, work in a managerial 
role versus a technical role.
**Michaela:** [00:29:34] Yeah. So one of the things I wanted to discuss with you 
as well is the tech stack and the processes that you have at your company. Can 
you tell me a little bit, what tech stack do you use for honeycomb to develop 
honeycomb? And also if you do code reviews, if you do testing. 
**Charity:** [00:29:51] Yeah. Um, we're, we're a big Golang shop.
Um, we use going for all of our backend services and the distributed column 
store that he wrote. Um, we use a lot of react on the front end. We have lines, 
we have integration libraries for. Um, you know, Ruby buys on pretty much all 
the main languages that you would suspect. Uh, we run an AWS. We, I use RDS for 
our SQL stuff, which is where we store the user data.
Um, when events come in, they get dropped into the API, obviously, which is 
pretty dumb, thin layer. It takes a minute and it. Drops them into Kafka and 
Kafka, um, you know, offers us, delivers them to the right partitions and 
distributes them correctly. Uh, but also keeps, you know, a backlog of a few 
days. So if anything dropped or deleted or whatever we could is.
Play it off the coffee queue, which is really nice. We use lbs extensively. We 
are microservices ish shop. We use circle CEI for running continuous 
integrations. We absolutely do code reviews. Yeah. But we're, but we're not so 
much, you know, some places you have to like, you know, kind of get a lot of 
permission before you build anything.
We're much more of a, you know, Oh, you feel inspired, cool. You know, go about 
it, come, you know, and we'll talk through it. We value communication very 
highly. Um, in fact, our engineering interviews, uh, the meat and potatoes of 
the engineering part of the interview is, you know, we give you a piece of code 
the night before your interview to take home and, you know, spend an hour or two 
on it, just extending it and improving it.
Um, but that's not the interview and you're not supposed to finish because we 
don't care how perfect your code is. It's not about that. We want you to bring 
it in the next, stay and speak like 30, 40 minutes, just talking through it with 
a couple of your peers, like, and just telling us like why you made the 
decisions that you made, you know, what, what you kind of have earmarked is left 
to do, um, what are the trade offs between this versus that choice?
You know, because we figure that. Anybody who can talk through the problem can 
definitely solve it. And reverse is not necessarily true. There are a lot of 
great engineers out there who do not value and prioritize communication that we 
do the way that we do. Uh, and, and it's just, we don't think less of them.
It's just, it's not the way that we've chosen to build our team because we 
believe that to build high performing teams. Um, it's incredibly important that 
you be able to talk to each other and learn from your mistakes. 
**Michaela:** [00:32:25] And how does that work at honeycomb are you're all in 
the same office? Are you all located or is there other distributed people?
Remote people? 
**Charity:** [00:32:35] Yeah. We're about a 25 to 30% distributed. And I, I 
suspect that this is a year where that goes up to about 50%. 
**Michaela:** [00:32:43] And do you measure somehow, um, several aspects of your 
code base? Do you have some metrics that you, you know, did you pay attention to 
code coverage, for example, or technical depth metrics or things like that?
**Charity:** [00:32:56] You know, the metrics that we pay attention to are like, 
how often are they getting alerted outside of work hours? And how often are they 
getting woken up? Cause we have an engineering on call rotation that includes 
everyone. And it's very, very important to us that, you know, We aim for no more 
than like 100 or a week outside of business hours.
And people shouldn't get woken up more than like once a year. Cause it's it's 
it's it's so it's so expensive for you in terms of your burnout, your 
motivation, your energy, and your ability to be a human being. 
**Michaela:** [00:33:31] So one of the things that I ask on Twitter is what 
people would like to ask me to ask you. And I had a really great question.
And that question was, what do you think about managing incident communication 
publicly versus only internally? 
**Charity:** [00:33:47] Oh, I'm a big fan of doing it publicly. And it's funny 
because I've really advocated transparency at every job I've been at because 
engineers love to hear the nitty gritty details. It builds trust.
Like it doesn't, you know, and I, my managers would always be like, no, if we 
say this, they're going to think that we're stupid. We don't know what we're 
doing and all this stuff. So we're going to make up something. It sounds 
obfuscated. I'm like, that does not earn you trust with engineers. That does not 
mean you trust it all.
It's the opposite, right? And all of us have had the experience of doing dumb 
things. It's not gonna, they're not gonna think less of us. They're going to 
think less of us if, if it's a mystery to them. Um, so finally I have my own 
company, so there's nobody telling me I can't do it. So we, we have like every 
time that we have had an outage, we've done a postmortem.
And in fact, um, You know, a couple of times ago, we actually took all of the, 
you know, the event, analytical data from the outage and we imported it into the 
dataset that's. Now, if you go to honeycomb.io/play, so anyone can, you know, we 
did some modification of the details, like app names, but anyone can slice and 
dice and look at.
How we debugged this problem and see if you can debug it faster or better than 
we did. Right. Uh, I, I'm a huge believer in transparency. I think that if you 
get started that way, um, there's no, you know, shock. Like I think if, if 
you're trying to switch midstream, people can sometimes be surprised, but why 
lie?
Like, it's just, it's better for everyone if we can learn from each other's 
mistakes. 
**Michaela:** [00:35:18] So that's the technical aspect, right? I'm also a 
little bit, uh, Engaged in the startup scene and, um, in the open startups as 
well. So what do you think about sharing, for example, revenue and things like 
that? Are you doing that with honeycomb and what do you think about 
that?
**Charity:** [00:35:38] No, we do it informally, um, to, you know, use yours. We 
haven't posted it anywhere. That's a little bit, that's a little bit more, you 
know, it's kinda like it's kind of like salaries, right? Like it needs to be 
done. Well, or it will screw you. Like nobody wants to be your first customer, 
you know, big customer are always going to kind of argue and go, are you really 
going to be around?
Yeah. You know, and so you get into this chicken or the egg thing where, where 
you can't get any, because you don't have any and. And revenue stuff is, is 
also, it really doesn't tell the full story, right? It doesn't tell the full 
context. And if, if everyone shared all this detail, it would be demystified and 
it would be fine.
But if you're the only one sharing this detail, then it becomes a competitive 
disadvantage because your competitors will use it too. You know? To crush you. 
Um, so, you know, and I'm, I'm not like a transparency zealot, um, you know, 
there are lots of things. I, I really do. I celebrate people's individual right 
to privacy.
Right. There are plenty of things that I wouldn't go around saying just because 
I'm like that deserves to be private, but I do feel like a default of leaning 
towards. Openness is the easier way in the long run because foster the right 
kind of humility and an openness to, to critique. Like I do. I see the 
organizations and people suffer when they, when they are trying to pretend that 
there's something other than they are, because they feel like something bad will 
happen, you know?
And I just feel like it's easier if you, if you just make a practice of being 
**Michaela:** [00:37:22] forthright. So one of the things that you mentioned at 
the beginning is that you actually got funding for honeycomb. How did that go? 
How did you find your investors? How did you approach them? Was this a long 
process? You know, how, how do we go about that?
**Charity:** [00:37:36] You mean the most recent round or the first one or 
**Michaela:** [00:37:39] whatever? Maybe the first one is the most interesting 
one. And then I am also interested in the recent one. Yes. 
**Charity:** [00:37:45] Honestly, it kind of makes me angry. Um, It's when I'm 
leaving Facebook is the first, only time in my life. Did I have had investors 
just basically pursuing me saying, would you like some money to do something 
I've never really had a pedigree?
You know, I didn't go to MIT. I didn't go to Google. I don't like that 
companies. Um, and so it kind of makes me grit my teeth that, you know, I wasn't 
a better engineer coming out of Facebook. I wasn't better at anything really. 
Um, except for navigating big company bureaucracies. Um, so it irritates me that 
that is what gave me the nod that people are just like, Oh, maybe you would like 
millions of dollars now.
You know, I think it's really unfair and unwise. Um, but I also felt like, well, 
this is never going to happen again. So I kind of have a moral obligation to 
take the money and do something with it, you know, but, but we had nothing we 
had. Three sides and it was all bullshit. Right. Um, and, and then wait, we did, 
you know, uh, another, an extension round and that time, you know, we were out 
of money, so we had to raise, but.
We had had to spend that first year and a half writing a storage engine, not 
talking to users and working on the UI and UX and all this stuff. So, you know, 
like in a lot of ways it feels like even though we're coming on four years, it's 
more like we're at the 18 month Mark as a company because of, you know, that 
protracted early period of, of, you know, preparation.
Um, so, you know, we, we raised money, um, and. I think that, you know, we 
raised from a couple of financial investors and they were our Creek guys. I 
think that they thought that we were going to be a different company than we 
are. And to be fair, we probably thought that too, like I think that there was 
an expectation that it would be much more like a drop in replacement for 
unstructured logs.
Just like here, you can put it in, you've got an elk stack and we'll do it 
faster and easier and better. Right. And. Boy did that, not turn out to be who 
we are. Uh, so, you know, I. This, this most recent round, um, is the round 
where I feel like it all finally kind of came together. We know who we are, we 
know who our customers are.
We know how we're trying to change the world. We know it's a tenure journey. You 
know, it's much like CIC D you know, we're, we're, we're at square one. Uh, but 
we figured out where square one is. Um, and I'm really happy with the investor. 
We got this round because he used to be a director of engineering at Netflix.
He. You know, there, there are videos of him out there giving talks about 
observability at velocity cough. You know, he really, anytime that you've been 
around as a company for four years, and you haven't like reached like meteoric 
growth, you know, everybody's excuses or reasons start to sound the same. And I 
remember telling Christina a year ago, I'm like, if we raise this round, It's 
going to be from an investor who has an engineering background, because there 
are the only ones who are really equipped to understand why the things that 
we're saying about the world are true inevitable.
Um, so that it doesn't just celebrate. Like we're making excuses. It took a long 
time. It took a long time to create that awareness, you know, cause people have 
been told for years that high Cardinals, it was impossible and that. This is the 
best you get. And, and it took a long time for, for us to like kind of show the 
distance between where, where we are and where we could be as an industry.
**Michaela:** [00:41:25] Yeah, I think it's great that you feel that you're 
finally out where you belong and that the market, and also your tooling is ready 
for the next generation of observability and monitoring of systems. So charity, 
I think we are at the end of the show, it was such a pleasure to talk to you. 
Thank you for being, 
**Charity:** [00:41:44] Oh, this has been delightful.
Thank you so much. 
**Michaela:** [00:41:46] Yeah. Thank you. Bye bye. 
**Charity:** [00:41:48] My pleasure. Bye. 
**Michaela:** [00:41:51] I hope you enjoyed another episode of the sup 
engineering unlocked podcast. Don't forget to subscribe. And I talk to you again 
in two weeks. 
**Charity:** [00:42:01] Bye.


