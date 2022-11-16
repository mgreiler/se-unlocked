# Fiberplane

[00:00:00] **Michaela:** Hello and welcome to the Software Engineering Unlocked 
Podcast. I'm host, Dr. McKayla, and today I have the pleasure to talk to Micha 
Hernandez van Leuffen. He is the founder and CEO of Fiberplane. He previously was the 
founder of Wercker, a container native CI/CD platform that was acquired by 
Oracle. Micha has dedicated his career to improving the workflow of developers, so 
he and I have a lot to talk about today.

I'm really, really happy that he's here today and he's also sponsoring today's 
episode. Welcome to the show. I'm happy that you're here, Micha. 

[00:00:36] **Micha:** Thank you for having me. Excited to be on the show. 

[00:00:38] **Michaela:** Yeah, I'm really, really excited. So, Micha, I wanted 
to start really from the beginning. So you are the CEO of Fiberplane and you 
are the founder of Wercker, which you already sold.

So, can you tell me a little bit about how you actually started to this entrepreneur 
journey of yours and what brought you to the developer 
experience area. 

[00:01:03] **Micha:** Yeah, sure thing. So I have a background in computer 
science and I did my so, I'm originally from Amsterdam, but I did my thesis at 
USF.

And the topic was autonomous resource provision using software containers. This 
was all before Docker was a thing, you know, the container format that we now 
know and love. And I sort of got excited by that field of, of so containers and 
decided to start a company around it. That company was Worker, so container 
native CI/CD platform.

So we helped developers build tests and deploy their applications to the cloud. 
We went, I would say, so we went through various iterations of the platform. You 
know, eventually, you know, we started off with Lxc as a container format and 
then eventually ended up, you know, having to, to platform on Docker.

And Kubernetes. But, you know, it was quite a, quite a journey. So that company 
eventually got acquired by Oracle to bolster their cloud native strategy. And 
then, you know, spent a couple years in a Bay area as a VP of software 
development focusing on their cloud native efforts.

Tried to do a little bit of open source there as well, and then, you know, move 
back to Europe. And so sort of started thinking about what's. Did some angel 
investing. We're still doing some angel investing as well actually in the sort 
of same arena. So developer tools, infrastructure building blocks for tomorrow.

So I run a, a small precede seat fund with to other friends of mine. But then 
also started, you know, thinking about what to build next. And you know, we can 
get into that, but sort of from our experience at running work or this sort of 
large distributed. Sort of fiber plane was, was born.

[00:02:26] **Michaela:** Cool. Yeah. And so how, how was the acquisition for 
you? I, from the time I'm, you said you were studying at the university, but 
then did you write out of university, you know, start worker or maybe already 
while 

[00:02:40] **Micha:** you were Yeah. More or less studying? Yeah. Yeah, more or 
less just out of university. So it was around 20, 20 12, 20 13.

And then, you know, expanded the team. Of course we got an office in San 
Francisco and, and London. And then 2017 we got acquired by Whirlpool. Oh, 

[00:02:56] **Michaela:** very cool. Wow. Cool. So, and you were the, you were 
the founder of that and also probably cto, CEO. At, at the beginning you were 
one person shop, or was this, or have this idea and I get some funding and I 
already, you know, have a team when I'm starting out, or was it more 
bootstrapped way?

How, how was that? 

[00:03:16] **Micha:** Yeah, yeah. We both gates, both fiber plane and, and, and 
worker. We got some funding early on. Then eventually got a CTO. For worker was 
one of the co-founders of, of OpenStack. So also, you know, very early in the, 
in that sort of, mm-hmm. container and, and cloud infrastructure journey.

And then if for fiber plane, Yeah. There, there's no cto. I'm. I'm both CEO and 
cto, I guess 

[00:03:38] **Michaela:** at the same time. Yeah. Cool, cool. Can you tell me a 
little bit about fiber plane? What is fiber plane? You know, what does, what 
does it has to do with containers and with developer experience? What, what kind 
of of a product is it?

[00:03:51] **Micha:** Yeah, sure thing. So, so guess coming back to the worker 
days, right? So we, we, you know, we're running this distributed system cic cd, 
so we were also running users arbitrary code. You know, any, any sort of job 
could happen on the platform on top of Kubernetes, inside of containers. So one 
of the things that, you know, stuck with me was it was very hard to always sort 
of debug the system, like figure out what's really going on when we had some 
kind of issue.

You know, we've going back and forth between metrics, logs, traces, trying to 
figure out what is the root cause of an issue. So sort of that, that was sort of 
one thing. So we're thinking a lot about, you know, surely there must be a 
better way to, to, to help you on this, on this journey. . The other thing that 
I started thinking about a lot was sort of just challenge the assumption of the 
dashboard, mm-hmm.

So if you think about it, like a lot of the monitoring observability tools are 
modeled after the dashboard, like sort of cockpit like view of your 
infrastructure. But I'd say that those are great for the known knowns. So 
dashboard is great. You set it up in advance, you know exactly what's gonna go 
wrong.

These are the things to monitor. These are the things, you know, to keep tabs 
on. But then reality hits and you know, the thing that you're looking at, at the 
dashboard is not necessarily a thing that's. Going wrong. Right? So started 
thinking a lot about you know, what, what is a better form factor to support 
that sort of more investigative explorative debugging of your infrastructure.

And not to say that dashboards don't have their place, right? It's like still 
that sort of cockpit view of your infrastructure. I think that's a, a good thing 
to have. But for debugging, you might wanna sort of more explorative a form 
factor that also gives you actionable intelligence. I think the other thing that 
you see a lot with dashboards, like everybody's monitoring everything and now 
you get a lot of signal and a lot of inputs, but not necessarily the actionable 
intelligence to figure out what's going on.

So that's sort of the other piece where it, then the other, like, the third like 
I would say is collaboration sort of thing that stuck with. Was also like we've 
come to enjoy tools like Notion, you know, Google Docs obviously. You know, in 
the design space we got Figma where collaboration is built in from the get go 
and it is found that it was kind of odd how in the developer tools and then sort 
of specifically DevOps.

We don't really have sort of these collab collaboration not really built in. 
Right. If you think about it you know, the status quo of, of you and I debugging 
an issue is we get on, you know, we get on a. You share your screen you open 
some dashboard and we started talking over it or something.

Right. And so it's, and it's, you know, I guess sort of covid accelerated his 
thinking a bit, but you know, of everybody going remote you know, how can you 
make that experience more collaborative? 

[00:06:22] **Michaela:** Mm-hmm. . So it's in the incident space, it's in the 
monitoring space, and you want to bring more collaboration.

So how does it work? Yeah, 

[00:06:32] **Micha:** yeah, yeah, exactly. So what's your solution now? Yeah. 
Now I've explained sort of the in inception. Yeah. But yeah, but what is it? 
What is it? Right. So it's, it's it's a notebook form factor. So very much 
inspired by data science, right? Like rc, like Jupiter. Yeah, we can Jupyter 
Notebooks.

Yeah. Think of, think of that form factor. Mm-hmm. . We don't use Jupyter or 
anything like that. We've written everything from scratch. But it's a sort of, 
yeah, a notebook form factor and you know, built in with collaboration. So you 
can add, mention people like you would on Slack. You can leave, you know, 
comments or discussions and all and all that.

But where it gets interesting, we've got these things called providers, which 
are effectively plugins. So they're web assembly bundles, which we can sort of 
dive into into that as well. But they're providers that connect to your 
infrastructure, right? So we have, for instance, a provider for Elastic Search 
for your logs.

We have a provider for Prometheus for your. And it allows you to connect to 
these observability systems and kind of pull 'em together into one form, factor 
the notebook, and then, you know, start collaborating around that. Mm-hmm. . So, 
you know, imagine if Notion and Datadog would have a baby . Yeah.

That's kind what you get. Yeah. 

[00:07:41] **Michaela:** That's cool. So I can imagine that. Let's. I'm on call 
and hopefully I'm not alone. A call. You are also on call, right? Yeah, and so 
we would open a fiber plane notebook. 

[00:07:52] **Micha:** Hopefully we're in the same time zone and we don't need to 
like wake up in the middle of that. Yeah.

[00:07:57] **Michaela:** Hopefully. Yes. And then we want to understand. How the 
system is behaving. And so we are pulling in observers. These are data sources. 
Yeah. More or less. Right. And then we can do some transformation with those 
data. Data sources or 

[00:08:12] **Micha:** Yeah, yeah. That, yeah, exactly. That, that might be the 
case. The other thing that we integrate with is, for instance, PagerDuty.

So an alert goes off indeed we are on call, but an alert goes off and we have 
this PagerDuty integration. And subsequently a notebook is created for us 
already. Mm-hmm. . Okay. Maybe, maybe even with, you know, some, some charts and 
logs that are already related to the service that might be down.

Okay. So depend, So depending on the alert, obviously you're, as you know, 
you're as good as how you've instrumented your alerts. But say we've written 
some good alerts, we now have a notebook ready to go. Based off a template. So 
that's another thing that we, that we have as well, which is this template 
mechanism.

And now, you know, we're ready to, to, to go in, get in into things and start 
debugging. So we might have a checklist, you know you look at the metrics, I'll 
look at the logs, sort of this action plan. We pull in that data we start a 
discussion around it. Mm-hmm. , hopefully we come, we come to the, to the, you 
know, the root cause of, of our issue.

[00:09:11] **Michaela:** Okay. And so this discussion and this pulling in data, 
this happens all in the notebook. Can you explain me a little bit more, and also 
our listeners Exactly. When we are on this, you know, on this call now, having a 
fiber plane notebook in front of our, what do we see, right? How does that, how 
does the tool look?

[00:09:28] **Micha:** It's, it's very similar to, I would say, like a Notion 
Page or a Google Doc page. Mm-hmm. . So we've got like different, different 
headings. The other thing that we have is, so you might have a title for a 
notebook, right? You know, the billing, the billing API is now. The other thing 
that we have is sort of this, this time range.

So maybe usually when there's an issue, you know, we've seen this behavior over 
the last three hours, so we can sort of have that time range locked into place. 
So we only want to see our. For the last three hours. And that means that any 
chart that we plot or any log that we pull in will adhere to that global 
timeframe.

So that's what we see. Mm-hmm. . We have support for labels, so, you know, 
obviously big fans of Kubernetes and, and Promeus. So we, you know, labels are. 
A first class primitive on the platform. So you're able to sort of populate the 
notebook with the labels that might maybe be related to our service.

Right? So it's a US East one, which is our region. It might, you know, say 
service is the billing. It might be, you know, environment is production. And 
the status of our incident is, mm-hmm. ongoing, stuff like that. So we have, 
we've got, go ahead. 

[00:10:34] **Michaela:** Cool. Yeah. And, and so is it then from top to bottom 
we are writing and we are investigating and we are writing out down the 
questions that we have and the investigation.

Yeah, exactly. We do. 

[00:10:44] **Micha:** Yeah. Yeah. And so, so 

[00:10:45] **Michaela:** we might have, Is it an Yeah. Is it Yes, 

[00:10:48] **Micha:** we our work? Yeah. Yeah. It's sort of Exactly. And I think 
in the most ideal use case, right. And I do it most ideal scenario, you're kind 
of like writing your postmortem as you go along. That's what 

[00:10:59] **Michaela:** I, I was thinking exactly that.

Right. And then maybe next time I'm on call again and I get PagerDuty and 
something is down, it's again, billing. Can I search in the fiber plane 
notebooks to find, you know, what we did last time and then 

[00:11:13] **Micha:** Exactly. So you'll, you'll search, jump to the conclusion 
. Yeah. Yeah, exactly. Hopefully, hopefully if you, if you experience, you know, 
the same issue multiple times at some point, we'll, we'll, you know, do a little 
commit on GitHub and we, we fix our, fix our, Yeah.

Do. But yeah, indeed, so you can search Yeah. Cool. On the notebooks and see if 
you've, you know, ran into similar issues. So that's, you know, it's great for 
building up this, this system of record, right. This knowledge base of mm-hmm. . 
Mm-hmm. . Of infrastructure issues and, and incidents. And it's also great for 
onboarding, right?

If a new person joins, like, this is our process. These are some of examples 
that we've run into you know, have a look. And now you've got a sense for you 
know, how we, how we handle things and some of the issues that we've 
investigated. Yeah. Cool. One more thing on the, on the product. So the other, 
so, you know, sort of explained the, the notebook form factor.

We've got these providers, right, that pull in data. From different, different 
data sources like Elastic Search or, or Prometheus. The other thing that we have 
is a command line interface which is called fp. Mm-hmm . And apart from, you 
know, being able to create notebooks from your terminal and you know, even 
invite people from the terminal, all this sort of usual stuff that you would, 
you know, expect from interacting with an API, with, with a product like this, 
there's two other things that we do.

So one is a command called FP Run. And it allows you to, if you are typing a 
command like cube, ctl logs for a specific pod, you can pipe that the output of 
that command to a notebook. And why that is useful is of course, you know, when 
we're de debugging this issue, you and I, and you're start typing things in your 
terminal.

I have no idea what you just did. And this is a way sort of to capture that. So 
you're piping these these, these outputs from your, the stuff that you're typing 
into your into your. into the notebook. And the cool thing is, you know, in, on 
your laptop you just, you know, sort of see text, right?

Monospace output. But for certain outputs such as the cube CTL logs command, we 
actually know the structure of the data and we're actually capable of formatting 
that in the notebook in the structured manner that you can start filtering on, 
on the logs and you know, select certain columns and sort of highlight even 
certain loglines for prosperity that you say, Hey, these are the culprits, these 
are the things that you need to take into, into consideration next.

So we have this sort of command line interface companion, and the other thing 
that it does, you're actually capable of running a long, like, sort of same use 
case as it just, I mentioned, but like a long running recording, like you 
actually record your entire shell session session as you're debugging this thing 
and all the output gets piped into the notebook.

Cool. Cool. And 

[00:13:46] **Michaela:** so I have two questions for fiber plane. One. Is the 
software engineer the right person to interact with you know, fiber plane or is 
it the site reliability engineer that's really designed, you know, or the tool 
is designed 

[00:14:03] **Micha:** for? Yeah, it's, it's, that's an excellent question. So I 
think one, one site reliability engineers, you kind of see in more larger 
organizations, right, where you start splitting up your teams.

I will say, I think at the end of the day, right, is if you're an engineer, 
you've built the service, now you need to maintain it now you need to operate it 
like it's, it's your baby, right? You need to, you probably know best how that 
system behaves than anybody else. So indeed I would say that, yeah, the target 
group is, you know, developers.

Mm-hmm. . 

[00:14:40] **Michaela:** And so the other question that I had around fiber plane 
is also. When we are on this call and we are writing in this notebook, how does 
the whole scenario look like? Are we still on a call, like, do we have Zoom or, 
you know, Google meet open, or are we really in the, in the fiber plane document 
just writing, Or are we sitting next to each other?

You know, what, what's the traditional, Is there a traditional scenario or is 
this all possible with fiber plane? How would you recommend using 

[00:15:09] **Micha:** it? Yeah, Yeah. Yeah. Not a, not a great question. Right. 
I think back in the day, it would be that, you know, we maybe sit in the same 
office and I scoot over and we start looking at a, at a screen, right?

And start typing together. Mm-hmm. . The reality is, of course, we're all doing 
remote work now, and we might not be in the same room. So I do think people will 
still use a Zoom call or a Google meet you know, as a companion to talk over 
stuff. I think, you know, people will still communicate in Slack and sort of 
start chatting back and forth.

But I think what we hope to achieve with fiber plane is like the pasting of 
screenshots, right? Well, if you take a screenshot of some kind of chart in your 
dashboard and you put it in Slack and you know, somebody yells, Oh, that's not 
the, that's not the thing that you should be looking at. You should, you know, 
like all that sort of slack glue That, you know, it's our, our goal to do away 
with that.

[00:15:59] **Michaela:** Yeah. And, and the slack blue is also very problematic 
for the search. At least I'm never able to find it again. Right. It's like is in 
the dark, super in 

[00:16:07] **Micha:** the dark area. Yeah. Super ephemeral. Yeah. Yeah. You 
can't, can't go back in time easily. And, and you know, how did we solve this 
last time? So again, like building up that system of record, I think.

[00:16:17] **Michaela:** Yeah. Very cool. And so how long are you now working on 
fiber plane already? 

[00:16:23] **Micha:** So we've been working on it for about two years now. Which 
is a, is a, is a long time. I think as a sort of, you know, one of the things 
that we've, I guess, sort of discovered along the way that we're kind of like 
building two startups at the same time, Right?

We're doing a notion or like a, a rich text, collaborative rich text editing 
experience, which is kind of like a startup on its own. Mm-hmm. . And we're 
building sort of this infrastructure product. So it's, you know, it's taken 
quite some time and, and energy to, to get the product to where it is now.

[00:16:54] **Michaela:** Yeah. And do you have already users? Is it like can 
people that listen today, can they hop on fiber plane already or. 

[00:17:02] **Micha:** It's, it's in it's been in private beta, mm-hmm. , but I 
think by the time this gets aired it's will be in public beta and people can 
sign up and take it for a spin. And, you know, we would love to get feedback on, 
on our roadmap, right?

And Okay. People can suggest what other types of providers we need to support, 
what are types of integrations we, you know, would love to, to have that 
convers. 

[00:17:23] **Michaela:** Cool. Yeah. So is there, There is the provider side. Is 
there something else that you want feedback on that you are exploring 

[00:17:30] **Micha:** maybe. . Yeah. Yeah. So we've got the providers that's one 
thing.

We've got sort of our templating stack. Mm-hmm. So curious to sort of see how 
people sort of start codifying their knowledge, right? What's, what, what kind 
of processes people have to debug their infrastructure and sort of run their 
incidents or write their postmortems. So curious to see what people come up with 
there.

Other types of integrations. Right? So we have as I said, sort of PagerDuty what 
other type of, sort of alert, alert to notebook or other types of external 
systems that we need to plug in with. I would love to get some feedback on that 
as well. Yeah, 

[00:18:04] **Michaela:** I think I had page Bailey over on the podcast.

She's from GitHub and she was she was also, they were releasing something with 
copilot and you know, For data scientists, some, some spaces here. And she also 
said like, well, we really need input from the users, right? So try it out, you 
know, tell us how it's working. I think it's so valuable, right, to see not only 
like you have your vision and obviously.

It's going one way, but then if you have your users, sometimes they take your 
product and they use it in a very different, you know, way than you anticipate 
it, which can be very informative. Right. I dunno. You have done two startups 
already. Have you seen that? And how do you react to it? Do you instrument the 
data a little bit?

How do you realize that people are using your product in a different. . Yeah. 

[00:18:50] **Micha:** So, so obviously we have metrics and analytics on sort of 
usage patterns of the, of the product. But I think, I think that data is 
excellent, right? But also qualitative data is, mm-hmm. , especially at this 
stage is probably even better, right?

Where you can get somebody on a call and, you know, tell us about your use case. 
Tell, tell us about the problem that you're trying to solve here and how can we 
be, be helpful in like what types of integrations should we support? I think 
sort of the difference between. Worker, I would say, and, and fiber plane is 
that, you know, worker was a pretty confined piece of surface area, right?

Cic, c d the whole goal is so you either have a, you know, a green check mark 
next to your build or a red check mark next to your build. Like it either, you 
know, failed or passed. And we need to sort of do that fast for you, get, get 
that result quick. Mm-hmm. . And with fiber plane, it's a more. I think that the 
interesting thing here is like, it's a, it's a more explorative and a sort of 
rich design space, right?

It's this notebook, which already you, you know, you can start typing and text 
and images and headings and check checklists and whatnot, right? It's a very 
open form factor and design space. And then of course, with the integrations, it 
can even, you know, be richer. So I'm very curious into your point, right what 
direction people will pull the product into.

Cause you can take it into all sorts. Use cases and scenarios. Yeah, 

[00:20:05] **Michaela:** exactly. And I think as a founder also, or as the 
design team, product team, it's it's also a little bit of a balancing act, 
right? So how far, you know, let me, are we going with what the user are doing 
with our product and where are we setting some boundaries that they can't do 
everything right?

So there's also often the talk about opinionated products, right? That you can 
actually do one thing and on one thing only, and we have an opinion on, you 
know, how. Supposed to use our product. And you know, we try to, if we see 
people deviate from that, we try to put an end to it. And then there's the other 
way where you say, Well, you know, if you take fiber plane and you do X with it 
and we haven't thought about this maybe, you know, we are okay with it.

Or maybe we even support that path, right. 

[00:20:48] **Micha:** Yeah, I think, I think we're more on indeed on the, on the 
ladder, right? I think what we've sort of, we talk about this a lot internally, 
sort of everything is a building block. You know, you've, we've got the 
notebook, you've got these different cell types, you've got providers, you've 
got templates.

Mm-hmm. You've got the command line interface. So like for us, like everything 
is a building block and we, we actually want to retain that flexibility. Not be 
too prescriptive. Cause maybe you have a, a if you think about sort of the, the 
incident debugging or, or investigating your infrastructure, like you might have 
a certain process, I might have a completely different process and we need to be 
able to facilitate, you know, these different workflows.

So, you know, thus far sort of our, our thinking around the product has been 
everything is a building block. And it should be this sort of flexible form 
factor that people can pull into into different scenarios and use. I mean, 

[00:21:36] **Michaela:** we have infrastructure as code, right? And we have like 
security as code.

Maybe we have debugging as code. Maybe, you know, this is what's coming next. 
Can, can you envision that, that it's going in this direction? Because while we 
have building blocks, maybe right now it's not you know, programming language 
for debugging, but it could go a little bit into the distraction, right?

No code coding for debugging. 

[00:22:02] **Micha:** Yeah, we've actually, we've, we've had some of, of that 
sort of discussion internally as well. If you think about the templates right. 
To, to some extent that is a, you know, we use J Sonet as a, as a sort of 
language, but we sort of codified them in a certain way and you can, you could 
argue that the templates is, you know, sort of a programming language for at 
least, you know, that debugging process, right?

Yeah, exactly. Right. Yeah. And. And, and we, you can take that even further and 
make it kind of like statically typed and make it adhere to, you know, certain 
rules and maybe even have control flow. So I think that, that there's, there's a 
piece there. And then maybe, you know, obviously we have you know, some YAML 
configuration on how you set up your providers, right?

Like how to connect to your infrastructure. So there's some, you know, 
observability as code in mm-hmm. in that realm. Yeah. Yeah. I think that'll be 
an interesting part of the journey, right? Like to figure out can we, and some 
even. 

[00:22:55] **Michaela:** Yeah, in some parts should be well, don't repeat 
yourself, right?

Like, for example, pulling in these providers, configuring that, you know, I get 
the right data. This would actually be something that I'm, you know, pulling in 
again. And probably that's what your templates do, right? So you say billing, 
oh, and then check, check, check, check, check. I have, you know, all my signals 
here and they're configured in a way that it's useful.

And then for this investigation, hopefully, One at a type thing, right? So I'm 
investigating, and as we, as we talked before once I realized what's going on, 
hopefully in my postmortem I'm going to, you know, make sure that this is not 
happening again. So this code probably is not going to be reused that often.

Maybe some, you know, some ideas from it, but hopefully we won't reproduce the 
same sect completely exact thing again. 

[00:23:44] **Micha:** Yeah. Cool. Yeah, that's, that's a super great point. And 
I think coming back, sort of the early part of the conversation around 
dashboards, right? I think thus far what we've sort of experienced as, you know, 
engineers ourselves, like, I think, I think we probably had sort of a phase 
around information gathering.

Like all these dashboards are great for information gathering, but now with 
Kubernetes and containers and microservices like the, the, the number. Services 
that we're running and the complexity has increased. So I think, I think there's 
sort of an opportunity for more exactly what you're describing. So it's more 
about action, right?

Mm-hmm. , what? What are we doing? We want to have the information, we want 
actionable intelligence that informs us what to do. 

[00:24:20] **Michaela:** Yeah, yeah, exactly. Because now I'm looking at this 
dashboard and I'm seeing the signals. But then everything else is outside of, 
you know, this realm, right? So what actions do I take?

Do I go, go to the console? Do I restart that service? You know, or, you know, 
whatever I'm doing. And, and it's also vanishing, right? So I'm doing it, but 
then. Who can see it, What I did. Right? Yeah, exactly. And so now we are 
capturing this, which is very nice, and then we can learn from it Right. 
Postmortems as well.

Yeah. So I looked a little bit through your blog and and, and your Twitter, and 
you were also talking about blameless postmortems. So how do you think about 
psychological safety? How should people. In an organization look at on call and 
incident management to really make it sure that we are ending the blame game.

Right. You probably have some thoughts about that as well, because you're 
working in this area. 

[00:25:19] **Micha:** Yeah. I, I think it's important to, and you like not have 
put any blame on any person. Right. It, it is a, and I guess sort of, you know, 
that's also why we're building this product. It is a collaborative process to 
debug an issue or resolve an incident.

Like, and what you want to achieve is to put the entire team in the best 
possible position to solve the issue at hand and and, you know, a support 
structure around it. So, you know, coming back to the product, like being able 
to, to open discussions. Point people in the, in the, in the right direction.

[00:25:52] **Michaela:** So maybe also if it's easier to find a problem to root 
cause it, and, you know, incidents become no issue or at least a lesser issue. 
So maybe the blame game is not that important. Can, can we say it that way? 

[00:26:08] **Micha:** I think so. Yeah. Yeah, yeah. If, if, you know, if the 
process becomes repeatable and we codify that and we collaborate on it and we 
build up that, again, that system of record and knowledge base I think that, you 
know, puts us in a safer position to, to solve the next one.

That's 

[00:26:25] **Michaela:** true. Yeah. Another thing that I was thinking of when I 
looked through, you know, fiber plane and what it does is KS engineering and I 
thought like what KS engineering is where you try to prevent not only the 
knowns, but also the unknowns, right? So really think about, you know, what, 
what could go wrong and then, you know, make a fallback so that your system is 
reliable.

Or, you know, if this database goes down that not the whole system goes down, 
but only a part of it and so on. Do you think that KS engineers can act. Source 
or, you know, use those notebooks that you're creating as input for knowing, you 
know, what we should actually look at and, Yeah. 

[00:27:02] **Micha:** Well, I think it, well, one thing I think it'd be a great 
provider yeah.

integrating with, with, with, you know, one or many of the, the chaos 
engineering services out there. I think it's a great way to train your team, 
right? You, we plug in some K engineering provider. The, the provider 
communicates with your infrastructure and such, pulling out wires from from, you 
know, your, your system.

And then now go ahead and start, you know, debugging this issue and mm-hmm. and 
you know, use different templates and you can, you know, sort of trial all sorts 
of different issues. I think it'd be super fun. Yeah. 

[00:27:37] **Michaela:** Yeah. So Micha, one thing that I also saw is that some 
of your of fiber plane is open source.

So what's your vision for open sourcing that are, you know, are some parts being 
open source? Can people help with the building fiber plane? 

[00:27:51] **Micha:** Yeah, great question. So right now what we've open sourced 
is a project called fp bind Gen. So this is actually of SDK bindings, generat. 
For how you would create full stack web assembly plugins.

So this is what we use to build our own elastic search and our Prometheus 
plugins. So we've, we've open sourced that. It's on GitHub we've already got 
some, quite some feedback on it. So, but would love some more. And then going 
forward we'll be open sourcing sort of our templating stack the proxy.

Which sort of sets which you install inside your cluster and sort of sets up the 
secure connections between the providers and your infrastructure and then the 
fabric plane managed service. And then the command line interface that I 
mentioned will also be open source. So expect more to hear from us on the open 
source front.

[00:28:36] **Michaela:** Yeah, Cool. I think that's so important, especially for 
developer tooling, that people can also really get it into their hands and then 
help, you know, shape the, or make the best product for their, for their 
environments that they have. I think this is such a success strategy. 

[00:28:50] **Micha:** Yeah, exactly. And you know, we, as I said, we would love 
to get feedback on the, on the providers and the, the plugin model, but maybe 
even, you know, once we open source the the, the provider stack would be great 
if people maybe come up with crazy ideas.

Right? You can think of any type of provider that you could surface data inside 
of, inside of the notebook. Yeah. Doesn't need to be observability or like 
monitoring data. Like could be. Yeah. 

[00:29:14] **Michaela:** Cool. Yeah, I'm super excited. What, you know, what 
will come out of that. Yeah. So I want to come back a little bit to your 
founding story because I know a lot of people are interested in developer tools 
and, you know, and, and Startup founding as well.

And you did it twice already, right? And maybe several more times in your life, 
I dunno. But right now we know of two instances. Yeah. There, there. So, and and 
also for fiber plane, you already got funding, right? Several million dollars. 
And so how do you do. How do you do it out of Europe is also some of my 
questions that I have because I think it's a little bit a different game here in 
Europe than it's in Silicon Valley.

Yeah. It doesn't look like, you know, opportunities around the corner 
everywhere. I, I have been studying in the Netherlands, so I know that actually 
Netherlands is really a good place, I think for, for tech startups and, you 
know, also a little bit out of the universities I saw there like You know, you 
get a little bit of help and, and, and funding and things like this, but still, 
I would assume it's harder than in Silicon Valley.

So how did you make it work? How did you get funding? You also said that worker 
had some funding at the beginning. Yeah. 

[00:30:26] **Micha:** Yeah. It's a good question. Well, how did we do the second 
time around, to be honest, Because it's the second time. Yeah. It was a bit 
easier. I mean, it's never, It's, Yeah. Yeah. It's obviously, you know, never as 
easy.

But it was definitely easier. I do think in Europe, if I also compare it to the 
worker days to where we are now, Like I do think the funding climate and sort of 
the, the, the, the thinking around startups has improved a lot, right? There's 
there's more funding out there, there's more feess. I think more importantly 
though, what we've seen is that now.

Sort of the European unicorns have exited or gone ipo. And we have actually more 
operators inside of Europe that have experience in either founding a startup are 
able to sort of start doing angel investing or have worked at multiple startups 
and we have just more operating experience you know, versus honestly like 
bankers, right?

That That, you know, help you out or are, are investing in you? So actually the, 
the, the funds that funder does were Crane Venture Partners which is actually a 
seed fund out of London that's actually focused on developer tools and 
infrastructure. So I would highly recommend, you know, talking to them.

If you're thinking about, you know, building a developer tool company and you 
need some funding, of course my own fund is also focused on developer tool. So 
shameless plug there on MP Hard Ventures. You can just Google that and find me. 
And then we have North Zone, which is a, you know, very like multi-stage fund.

Also out of, well actually quite different geographies and Notion Capital out of 
out of London as well. Okay. We've got some have several micro VCs, several 
things. Yeah. We have somebody funded West Coast Alana Anderson was doing with 
base case capitals investing in a lot of infrastructure and enterprise startups 
and Max Cloud from System one in Berlin.

Is another one. So yeah, we have a good crew of, you know, a diff different 
experience and sort of different stage type of funding as well. 

[00:32:19] **Michaela:** Yeah. This was my next question that I had for you. 
It's probably not only about the money, you said experience, right? It's also 
about the knowledge that people have, right.

How to do things. Probably, yeah. The people that they know, right? So that they 
can Yeah. To be Yeah, exactly. Can consider the right people have the right 
network and so. 

[00:32:36] **Micha:** Yeah, I think, I think the most, yeah, it's is, is 
introductions, but it's also. You know, if you, if you think about the, the 
funds that actually do developer tools, right?

So they, in their portfolio, they, they've seen, you know, startups trying over 
and over to tackle some kind of go to market issue or trying to build an open 
source, mm-hmm. company, right? So they have some, some pattern matching and 
some, some knowledge about, you know, what to do and what, what not to do.

Of course, it's all advice, but it's good to sort of have some people in your 
corner that have at least seen this, these types of companies being built. Over 
and over again. Right. That's, and then, and then other VCs have more experience 
in, you know, more, more like how to build up or scale up a sales organization 
and thinking about how to run a SaaS company.

So yeah. Different experience from different, different funds. 

[00:33:20] **Michaela:** And so now you listed quite a lot of different 
investors. Do you reach out to each one of them or do you have like a whole 
group meeting and they're all in there and you ask them for advice? , how does 
it 

[00:33:33] **Micha:** Yeah. No, it's, it's sort of one on one chats, right?

Either over, over chat or, you know, we meet up for coffee or, or or breakfast, 
mm-hmm. . But yeah, we try to do that on a, on a regular cadence. And then of 
course, when, you know, something exciting happens, such as our launch know, we 
try to group them together and get them all on the same page around the same 
time.

Or of course if an issue arises, Right, which could also be the case. Yeah. And 
then sort of all hands on deck and everybody in the same room or zoom. 

[00:34:01] **Michaela:** And what about your biggest struggle on your, on your 
entrepreneurial journey, maybe now with fiber plane or maybe with Worker? Did 
you ever think that, you know, worker, when you started it, did you think that 
somebody is going to buy this and.

This is going to be huge. 

[00:34:16] **Micha:** Yeah. Yeah. I think, I think the ambition was always 
there. Mm-hmm. . And, but, and, and sort of that drive to just make better 
developer tools. I think that sort of, that, you know, that's been true for all 
the companies or all too. Yeah, that's, 

[00:34:30] **Michaela:** Yeah. And what 

[00:34:32] **Micha:** I struggle. Yeah. Yeah. So I think, I think as I think for 
fiber plane now, it's not necessarily a struggle, it's just the real, which this 
mission of this flexible form factor, just the fact that we're doing sort of two 
startups at the same time has been sort of mm-hmm. An interesting thing to to 
build now, right? You're doing this rich, collaborative, rich tech editor and 
trying to build this infrastructure oriented company, and I think that's been 
yeah, just an interesting experience with building out a team.

You know, the technology and the product that we. 

[00:35:01] **Michaela:** Yeah. Yeah. So maybe can you tell me a little bit more 
about again, if people want to hop over to Fiber plane now and try it out how 
does that work? Do you have to, you know is there a sign up? Is there a waiting 
list? I mean, you said probably when this airs there is a public beat, but still 
do you have to, you know, what do you have to reach out to you, you give me a 
demo or I just fill in my credentials and I'm off to 

go.

[00:35:25] **Micha:** you can just sign, sign up with Google and then you're off 
to the races. And then of course, if you want a demo and sort of get some more, 
more more help or onboarding we're happy to help you and get on a call and walk 
you through it. But yeah. Okay, cool. Try playing com. Is there 

[00:35:40] **Michaela:** also a, Yeah, is there a video or something that we can 
look 

[00:35:44] **Micha:** at?

Yes. The, the website and there's a video. 

[00:35:50] **Michaela:** Okay. I will link that so that people can go Yeah. And 
it will explain everything to them. Right. What about pricing? Whatever pricing? 
Yeah. You have already some idea around pricing. Yeah. 

[00:36:01] **Micha:** We've got some ideas on how to charge, but I think right 
now for us, it's important to get the product market fit, mm-hmm.

and as such, you know, get, get the feedback. From these companies and these 
teams using the product. So we'll introduce pricing at a later stage. So for now 
it's, it's free to use, mm-hmm. . And you just give us your time and your 
feedback, and then Yeah, we're grateful. 

[00:36:20] **Michaela:** Yeah. And what about my data?

Is it safe with you? Like, do you have some visibility into my data or do I send 
it over to 

[00:36:29] **Micha:** you? Yeah, so we actually so the way the, the providers 
work the plugins, so they actually get activated through a proxy. So we install 
a proxy inside of your cluster. The proxy sets up a secure bidirectional tunnel 
from your infrastructure to the fiber plane managed service.

And then we do, for that specific query, we do store the data that's related to 
that query. So of a result, we do store that in the notebook. And yeah, we 
probably will come up with sort of more enterprisey ideas around how to self 
host 

[00:36:59] **Michaela:** it, Right? Or something 

[00:37:01] **Micha:** as an example. Yeah, yeah, yeah. But again, we'd love to 
get some feedback on that.

[00:37:07] **Michaela:** How that works. Right? Yeah. Okay, cool. So yeah, that 
sounds really good. I think you, at least my questions, , you could answer them 
all, but maybe my listeners have questions and then they can send them to you. I 
think you will be, Yeah. Quite happy, right? 

[00:37:22] **Micha:** A hundred percent. At mes on Twitter, m i e s and at 
fiber, playing on Twitter, fiber playing.com.

Sign up, take it for spin, shoot us a message. Yeah, sounds. 

[00:37:33] **Michaela:** Yeah. Yeah, it sounds super interesting. I hope that a 
lot of my listeners will do that, and I will link everything in my show notes 
that we, you know, talked about your, your Twitter handle and everything so that 
people can reach you. And I hope you get a lot of questions and people give it a 
spin and give it a try and send you their use cases,

And yeah. I hope you all the best with your product. Thank you so much for being 
on my show today Micha. And yeah. Thank you. Bye. 

[00:37:59] **Micha:** Thank. Thank you for having me. 

[00:38:01] **Michaela:** Yeah, it was really great. Bye bye 

[00:38:04] **Micha:** bye. 

[00:38:06] **Michaela:** This was another episode of the Software Engineering 
Unlocked Podcast. If you enjoyed the episode, please help me spread the word 
about the podcast.

Send episode to a friend via email, Twitter, LinkedIn. Well, whatever messaging 
system you use, or give it a positive review on your favorite podcasting 
platform such as Spotify or iTune. This would mean really a lot to me. So thank 
you for listening. Don't forget to subscribe and I will talk to you in two 
weeks.

Bye.


