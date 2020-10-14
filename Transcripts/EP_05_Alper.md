# Transcript Episode 5 Alper Koc

(Intro music)

**Michaela:** [00:00:00] Hello, and welcome to the software engineering unlocked
podcast. I'm your host, Dr. Michaela, and today I have the pleasure to be talking
to Alper Kemmal Koc, who is a software engineer at a startup in Turkey called
Kuika. Kuika helps users to be more efficient in building mobile apps. It's a
low code solution so that users can build mobile apps based on already
implemented building blocks.
Alper has been there right from the start. He was the first engineer on the team,
experiencing the whole startup life cycle from working on the initial idea, and
implementing the prototype, to working with the first customers and getting his
hands dirty, helping the company succeed. So there's tons to talk about today.I'm
really happy that Alper, you're here. Welcome to the show.

**Alper:** [00:00:43] Yeah. Thank you. Thank you for having time for me.

**Michaela:** [00:00:47] Well, maybe let's start with, how did you come to work
at a startup? Why did you choose that path and what led you there?

**Alper:** [00:00:54] Well, as, as like most engineers, we, most of us like
greenfield projects. So startups usually give the chance for that. And, uh,
I have always worked in relatively smaller companies. They were either startups
or they used to be startups and they're just in the next, next phase. Kuika was,
uh, when Kuika was starting I was living in Holland. And our founder is someone
I knew already before. And he said, if I wanted to join, I said, yeah, I liked
the idea. And I always liked startups anyways. So, uh, I moved back to Turkey
for this actually in the 2015. And I've been working here since then.

**Michaela:** [00:01:31] So have you been one of the first engineers on that
project?

**Alper:** [00:01:34] Indeed, I am. I am the employee number one. I, yeah, I
have been, um, I have been doing the whole architecture and then we have been,
it was just two of us at the beginning for like a couple months.Then we hired two
more engineers and it was just four of us. We did only research and development
for, I think, almost 20 months or something. And if you were making all the
technical decisions or architectural decisions and technology choice, everything.
So I have been deeply involved since the beginning.

**Michaela:** [00:02:07] So I imagine that this friend of yours comes with this
idea to have this low code platform and then you're like fire for it. And then
you start really from scratch, understanding if it's even feasible, what you're
going to do and what your requirements are for that project.

**Alper:** [00:02:23] Yes, indeed. Our founder is much more experienced than me,
so he knows the field. He had seen this opportunity every time they are building
software projects. Most of the time you're repeating the same problems that every
software engineer is solving most of the time, and did that thing a lot of times.
So, we thought like, yeah, why don't we just wrap those up in, in some ready
components? And the engineer really focuses on the business requirements, but not
the, all the hassle around it, so they can just focus on the requirements. They
just build their user interface and you'll get the app.

**Michaela:** [00:03:02] And when you start out with this idea, how do you
decide on which technologies you should use?

**Alper:** [00:03:08] Well, I think for the first month we did a lot of research.
We looked into all the popular technologies back then, and let me put it this
way, there were two sides to the research. First of all, we were going to build
the tool that generates tools, that generates apps. So we did research on both
sides. So what should be the technology of the tool itself, of the platform
itself, and what kind of technology and apps should be producing. And, uh, on the
end product side, so what we generate, we decided to go with hybrid technologies,
for example.
So we wouldn't get into the problem of producing code for both Android and iOS. So
that was like one, one decision we made and, and the popular technology back then
was, was Ionic. But it still is. But I think it was only version one back then.
And, and we kind of did some reverse engineering. So that was, that was one fun
part of it. We didn't build our tool, we forget about it. We picked up a scenario.
We actually built a mobile app. That's, you know, nice to use, easy to build. And
from there we went back. So we, we talked like, okay, what should we do to produce
this code.

**Michaela:** [00:04:28] So you mean that first you actually produced your use
case. And then you produced a tool that would produce that use case.

**Alper:** [00:04:35] Yes, exactly. So we had the app at the beginning, like on
the, on the first month or second month that we never use, but it would be kind
of what our customers would, would want. Or what they would be aiming to build
with, with Kuika. So that kind of dictated the decisions we made.

**Michaela:** [00:04:54] And did you change some of the initial ideas that you
had on the tech stack? So did some of the technologies change over time?

**Alper:** [00:05:01] It definitely did. At the beginning, we had this
architecture, like we had a lot of backend code. We had a lot of c# .net. And we
had a, we had a, multitier architecture. That architecture never change, but the
emphasis like the focus where most of the intellectual property lies has changed
a little bit, because we were focusing a lot on, on, on, on implementing the
business logic on the back with c# .net.
But, and that was kind of slowing us down a little bit. And, and at some point
you saw, okay, JavaScript is giving us a little bit more power and a little bit
more opportunities. So just naturally all by itself, it kind of, we kind of
switched our focus to the, to the JavaScript and front end site. That doesn't
mean we change architecture. Architecture has always been the way it is, but, um,
I mean the, the, most of the business logic that's been implemented has shifted
a little bit.

**Michaela:** [00:06:03] Okay. And so maybe to give our listeners also some idea,
how old is that startup right now?

**Alper:** [00:06:09] We started in September 2015. So, uh, in two months, it's
going to be exactly four years.

**Michaela:** [00:06:16] And how mature is it?

**Alper:** [00:06:19] Well, for the first two years we did only the research, and
on our, beginning of our second year, we released our product to our initial
customers. And it has been growing up since then. It, I think this kind of project,
it's difficult to say, it's okay, it's now mature because we are generating apps,
we're generating software and that, and the technology is changing every day. So
we always need to keep up to it. So it will probably never going to be mature. But
currently we have, I think around 15 customers, uh, we are, um, we are capable of
satisfying their needs. We have been building apps with, with the platform. Those
apps are, are live and being used in those companies right now.

**Michaela:** [00:07:08] Well, if you're developing software at a startup and it's
only you at the beginning, and then, you know, the team slowly grows, well how do
you grow in the same time, the software methodologies and the best practices and
things like that? Have you been conscious about that at the beginning, or was there
a very different attitude when you did the research, than what you have now that
you actually have customers? Was there some shift?

**Alper:** [00:07:31] Well, we have been through a lot of phases on that. And we
have been, we have been strict on that since day one. Uh, I was living in Holland
before, and I have been, I have experienced a lot of methodologies being
implemented that are, like, strictly and, and tailored to the needs of the company,
the organization.
So even from day one, the first thing we talked about, okay, what's our methodology?
How are we going to do this? Not what we are going to do it, but like, okay, what's
the point of the process and everything? Well, the first month or two, it was just
two of us, that there wasn't much, um, methodology, like, uh, rules and stuff. But
we were talking about once we grew, we said, okay, let's do, let's look into Agile.
Let's look into Scrum. Let's look into Kanban and how we can implement those. And I
think like every three, four months we changed the methodology, or we came up with
a relatively different implementation of the methodology ourselves, because our
needs changed.
At the very beginning, we were doing a lot of research, we were doing a lot of
experiments. It was not very easy to make estimations. It was not easy to make
long-term plans. Then we said, okay, here's a methodology, we are going to make
quarterly visionary goals, and we are going to do Kanban. So, you know, we will
have goals and we will define the topics, and we are going to pick those up one
by one.
After we meet those goals in the first quarter, let's say for the, for the next
quarter or the next five, six months, I don't know, we have a more clear path to
go. So we can, we could define what we are going to do. So we, we kept switching
in between depending what we need at the time. And after two years we starting
having customers, and that, that brought us to a whole new world where we had to
run projects with the customers, and some of our customers didn't know about those
methodologies, or you cannot apply some of those methods to the project management
within two organizations.
So we kind of, we kind of, um, picked, like we did some cherry picking from
different methodologies and implemented something for every project or for our own
work here within, within our, within our team.

**Michaela:** [00:10:08] So one of the things that, uh, stroke me when you
were talking about why and how you use different methodologies, you said, well
I have been in the Netherlands before. So do you think that culturally there is a
difference between the Netherlands and for example, Turkey on how much, um,
methodology-driven organizations, software organizations are?

**Alper:** [00:10:30] Uh, I think there is. I haven't worked in Germany, but what
I have been hearing from friends, like Germany, Holland, or the more, countries
that are, the more North you go, being on time, like being punctual, and being
strict about plans has more value. People appreciate that more.
But, but the more East or South you go that's, that's not, yeah well, it is still
important, but not as, not as much. That, that makes a huge difference. And I
moved to Holland and every standup meeting is so strict on the same time. Say
minutes, not one minute later, not one minute earlier, if you're late, you miss
it. Simple as that.
But, uh, it is difficult to do it that strict here, here. So, so there's definitely
a difference in culture.

**Michaela:** [00:11:23] So it means that in Turkey, if the stand up, if the
people are a little bit late, it's normal, like five minutes later. <em>(laugh)<em>

**Alper:** [00:11:31] <em>(laugh)<em> Well, yeah, Istanbul is also one of the
biggest cities in the world, and one of the cities that there's a lot of traffic
problems, so people can be late. And yeah, also if you're a small team, yeah, you
don't want to, you don't want to miss one person and then, you know, you can't
just say, yeah, you missed today's stand up. So we wait for like five, 10 minutes,
15 minutes to get you. Yeah, you adjust to it.

**Michaela:** [00:11:56] So you're saying that, um, you looked a lot into different
methodologies. What about, for example, testing, has testing been a part of your
software engineering process from the beginning on, or is it just something that
now that you're getting customers, more relevant? What's your experience there?

**Alper:** [00:12:13] Well, to be very honest, it has, it's been a problematic 
part of our work process. We have tried, uh, different ways of testing, like. 
Let's say one person from the team is responsible for testing, but that's that's 
manual. Okay. So something is released. You want to check something that we have 
not broken the, in the graphical user interface, or we are still producing the 
same car and yeah, every person is different as, as, as, but they will.
They agree. So people are not that. So careful then thing and, and manual 
testing is when I think in the, in the past age. So we said, okay, we have to 
automate this. We have to find a different solution to that. So just like our 
methodology, our testing process has, has. Had its own phases as well. We 
haven't unfortunately done a lot of TDD, so we don't have a good test unit tests 
with, but six months through, after we started, we said, we are missing out some 
bugs.
So we have to automate this. And we came up with this idea of, uh, writing our 
own tool. We said, okay. What's the most important thing for us. Okay. We are 
producing apps. What's the most important thing we want to make sure we are 
building the same app or the same code. And we make sure that let's say be the 
liaison app to a customer.
And there's an update. Two months later, we should be losing that exact same 
code. We should be generating the exact same code. Of course also, considering 
if there are changes, of course, we need to accept those. So we wrote a tool 
that we register all the, all the apps we are working on, all the projects we 
are working with and it runs every morning or manually during the day and checks 
that we are building the exact same thing again, if it is not the executive, 
same, it gives us a warning.
We can look through the, it shows us the changes. And we can either accept it or 
we catch, we catch the bug that we haven't noticed while we were writing the 
code. It was a simple tool, but it has saved us a lot of time. And it has, it 
has caught a lot of, uh, things that we hadn't thought while we were designing 
the system did a new feature or the writing the cause.
Uh, so that has been like pretty much the main, a backbone of our, of our 
testing process. 
**Michaela:** [00:14:50] How about code reviews, for example, is that something 
that you do in a small team of four right now? How many are you at this moment? 
How many engineers 
**Alper:** [00:14:59] currently? I think we are a seven. Um, we have always done 
code reviews, maybe not very strict at some times, but we always did that.
There's also like our second insurance platform. We have, we have tried two 
methods on that. And one of them was like, okay, I will be doing the code 
reviews because, um, the structure we had most of the time, it was me and I 
found her seniors and we had either junior engineers or maybe with a couple of 
years of experience.
So we said, okay, let's, let's let the seniors do the college review. So we will 
always do the coding. And that, that works fine, but that put a lot of, um, Uh, 
obviously workload on us. And at sometimes we said, okay, everybody does the 
code review. And we had this through that each feature or each change goes 
through three people, the developer, and that person is supposed to be doing the 
development tests obviously.
And the code or the, or the, or the changes goes to the person B who does the 
code review. And the third person would be manually testing it. So we had tried 
to both methods and they both worked fine, actually. And at some point, 
obviously after a couple of years, you have some experience, you have some 
traditions of your own in the company.
So we have our own, yeah, you cannot resist notation, but we have, we have some 
rules on, on how we write the code on what are the patterns and stuff like that. 
And once, once people get used to it, most people follow. And that also works 
fine. So. So one 
**Michaela:** [00:16:44] of the things that you just mentioned was like, after 
some time you get used to, and you also explained that at the beginning, you did 
a lot of iterations and perspective.
Do you think that right now, you're still doing that enough, that you're still 
looking with the same critical eye on your processes? Um, and, and tools and 
things, how you do it, um, as at the beginning, or do you think that over time, 
there's something like, you know, you're getting very comfortable with how you 
do things and you're missing out maybe on some of the improvements.
**Alper:** [00:17:18] Well, we are still strict on it. Just like we just, like, 
we were on day one, we still do the retrospectives and, um, we still come up 
with new ideas and sometimes we also drop something that we have been doing for 
two years, because all of a sudden, it's not that. Useful anymore. So it keeps 
changing. It's still just like the day one.
And we have new new teammates who also have their own ideas or simply they can't 
adjust to the methods we have. And that that's also fine. Then, then we're just. 
For them to, if it's the most important thing, is that the whole team and every 
individual, this is a small team. So every individual's contribution is really 
important.
So if I'm person is not comfortable with, or yeah, we can't end the benefit art 
from something. We talk about it during the retrospective and we drop it or we 
change it. So we still, we still keep it writing. 
**Michaela:** [00:18:18] It sounds really important. As you say, in a small 
team, everybody should be able to provide the best work that your he can.
Is there an example that comes to your mind where you actually dropped one of 
the methods? Because of one person. And how did you address that? 
**Alper:** [00:18:35] Well, what we had, for example, what we wanted to start 
this month at the beginning of this year is there was this thing called Google 
heads, like 20% thing, you know, engineers would have 20% of their time to work 
on their own projects.
And we said, okay, let's do that. And not everybody could contribute to it, not 
the area where they have ideas. People are really happy with, with the work that 
they are cleansing to do. And they are not. Yeah. They just simply, don't like 
to come up with something new and okay. If not everybody is benefiting from 
that, and there is an imbalance in the team because we reserve some time for it 
and some people can do it.
Some people can't. Yeah, we just. Drop it. And another thing we dropped was that 
the actual culture reviews again. So, and we have a few junior, the engineers 
right now, and I start doing the code reviews like, uh, with, with all of them. 
So I said, okay, everybody is going to do. The rooms and it just didn't work out 
for some of them.
Maybe it was too early. Yeah. They, they simply didn't know what to do with it. 
So we dropped it. We will probably bring up the topic again, six months after a 
little bit more experienced, then maybe we will start doing it again. 
**Michaela:** [00:19:58] So that's really interesting. And I like that it's so 
well, so personally adjusted, but how do people address those issues?
So I imagine if I'm a junior and I'm not comfortable with doing the coach 
reviews, do you just see that those person doesn't contribute or are they 
walking up to you and tell you that they are not comfortable with it? So how 
does that actually work? 
**Alper:** [00:20:22] Yeah, one of the advantages of being a small team is.
Like we are literally sitting one meter away from each other and we don't really 
do one-on-ones. So if somebody wants to say something, yeah, we just say it out 
loud in the office right now. Right then that's, that's the kind of culture we 
want to have. And if, if some person says, yeah, I am not comfortable with doing 
this, or I don't know how to do this, we encourage them to say that one thing we 
keep telling our new team members is.
The most important thing that you should do is say. Tell us, if you can't do it, 
if you don't understand something, just say that's the most value you can add 
that I believe that are two things the engineers are hired for. One of them is 
to say no. And the second thing is to say that they can't do it.
That that's so valuable. That's really important because then we can change, 
like, okay, let's. Let's switch the person. Let's say someone else should do it. 
Or maybe you should do it with another person, like a pair program. So you ex 
you exchange your methods, you exchange your perspectives. And that also 
contributes.
So that's the kind of culture we impose. And also in the retrospectives, we do 
round Robins. So everybody has to say at least one positive thing and one 
negative thing about the last week or the last two weeks. That also encourages 
people to say things aren't loud. So nobody is running the meeting, but, uh, 
everybody is saying something about it.
**Michaela:** [00:22:02] So you said that for example, this 20% rule didn't work 
for all of the people, but it worked for some. So if you're, if your decision 
then is to drop those 20% project time, what about the people that actually like 
that idea? How do you deal with that? 
**Alper:** [00:22:20] Yeah, but they, they were free to keep working on that and 
they actually did what did one of our friends that's this one?
Funny story, actually, that we also tell our customers, it tells a lot about our 
product. We had this new team members that started at the beginning of this 
year, who was going to get married in a couple months. And, you know, I mean, 
well, in most of the countries, they, they, you know, they send out invitations 
or his family was going to send out some invitations and the family was having 
difficulties.
Okay. W what's the lift list of people that are supposed to send those 
invitations to, and who is going to give to who and which ones have we delivered 
already? And our friend here said, okay, I can, I'm working at this company that 
I can build mobile apps with now. And it's really first. So he said, can I build 
a app?
Can I use my time on that? I said, yeah, sure. And had he built this small lab 
in a couple of days and his family used it for those imitations data just said 
all the people they want to invite. So, so yeah, that person I was benefiting 
from that thing. So he kept on doing it. Yeah. I can 
**Michaela:** [00:23:34] imagine that if people can use somehow work time also 
to learn, um, that can be beneficial for both sides from this project.
He probably learned a lot about the use case of your product yourself. Right. 
Because he was sort of like the customer and could give feedback. Was that the 
reason why you decided that you can do 
**Alper:** [00:23:55] that? Exactly. Yeah. We had like two reasons. One of them 
was like, Thanks to that thing here. He did hear experience how a person or a 
company can approach for a project.
So he had to collect his requirements. You need, he had to talk to his family. 
He had to decide what he needs to make. He had, he had his own time limit, so he 
had to finish it in a certain time. So he made his own priorities and in feed. 
Considering the features and he completed that, that, so that was a lot of 
benefits to him.
Another benefit was he, he became a customer of our own product. That's 
something really important. We can keep writing, we can build this awesome tool. 
We love it. It's great. But we will really understand the value. We will really 
understand what we are doing if we are. The customer of our own product.
That's, that's the thing that, that was real nice for him. He became our 
customer. So he had a much better perspective on our tool. He had, he had a lot 
of feedback and when he was building new features, he knew what it literally 
would. Mean to, to our users. So in 
**Michaela:** [00:25:18] general customer feedback, I think is something that's 
really valuable and very, very important for, especially a startup that maybe 
even has to find some product market fit first.
How do you engage your customers? How do you communicate with them? How do you 
understand what their needs are? And if you are fulfilling that? 
**Alper:** [00:25:37] Yeah, because we are still at the beginning, we don't have 
a lot of customers. So if you don't really, they haven't. Um, we haven't had a 
need for the tool for that.
So we are talking to them one on one, we talk to our users and we get a lot of 
requests from them. We also integrated some ticketing and feature requesting 
system in that, in our tool. They can also fill in the form there. One important 
thing, though, for a startup that's really risky. You can always get a lot of 
feedback from your, from your users and they will have some feedback, especially 
if you ask for it, the more you will get.
But, but if you're building a new product and you're trying to find your way, 
you really need to think through those requests because they can also easily 
take you off your path because every customer will have their own needs and they 
will be asking. So you should be, you should be searching for patterns.
So let's see, we have this customer who is asking for a feature. Nobody else 
wants. And, and that also comes with its own cost. So there's almost like doing 
a custom development for that for the person. But if this customer B is asking 
for something that also our customers C and D kind of needs it, that's that's, 
that has a higher, so that, that has been actually a real challenge for us to 
prioritize.
I mean, first collect the user feedback first, collect the requests, then think 
them through. Then prioritize. And also actually the third important thing is to 
ask the user or ask the customer, why do you need this for, because we had this 
and that has to be a long conversation. You really need to, uh, dive deep.
The reason for that is most of the time we have seen the customer needs 
something and they are thinking, how can I implement this? And they come up with 
this solution. That's not always the correct one. And for that solution, they 
are asking for a feature. If they, they had told us the initial reason why they 
got into this loop.
Maybe they already had a, had a feature for that, or it could be a lot simpler 
or it could be maybe for everybody. So we always also try to understand what the 
user is asking for that thing, because there is usually something else lying on 
there. 
**Michaela:** [00:28:10] One of the things that for a startup also interests me 
is the deployment process.
How does that wag, is that a click of a button that deploys a new version of 
your system? Or is there more manual labor also involved who can do it? 
**Alper:** [00:28:24] But unfortunately I cannot say it's fully automated, but 
it's not a manual either. So it's kind of a mix. And then we have three stages. 
We have a testing environment and alpha environment, then a live environment.
And we deploy to our test environment every day, every night or every morning, 
like every 24 hours. And there's also the environment that we run those, our 
testing tool on. And to our alpha and live environments, we, uh, we release like 
once a week. Most of the process is automated, but it's supervised manually.
I mean, it's like kind of a script. And then one of us sits in front of the 
computer, runs a script. And, uh, just make sure everything's fine. So the test 
environment to test with part, yeah. That that's kind of a manual. I mean, like 
you click a button, right. And it gives you the results and you need to look 
through them except the differences or, and, and or if something is awkward, 
then that person raised it flag and say, okay, something is wrong in dress in 
yesterday's it changes.
So, yeah. So it's kind of a mix. 
**Michaela:** [00:29:38] You're employee number one. What were your biggest, um, 
useful resources? How did you learn? How did you grow? How did you know how to 
implement which architecture, which methodologies to use and all of that? What 
was your North star or what was your, your fuel for learning? Is it books?
Is it bought cars? Is it other people. 
**Alper:** [00:29:58] Well, I would say Google most of the time and, and yeah, 
we do have a small library of books here and, and we thought, okay, we can go 
through the books, but yeah, the books at this, we had give us more information 
for a specific technology, but just like you said, at the very beginning, the 
initial questions we had was like, okay, what should the architecture be?
And what should the technologies we should be using. So we get the first pick 
dose and then dive into the books. That, that was one thing we were lucky about 
and, and our experiences are, uh, from our previous previous jobs. And. Uh, 
software development experiences. Uh, we had been exposed to a couple of 
architectures like software oriented architectures or multi-tiered, uh, setups.
And obviously we were first talking about the things we all didn't know about, 
and that already sounded like a click. So we didn't really dive very deep into 
alternatives. We of course search through them. Like, we'd be the be Google. We 
ask our friends who have, uh, you know, software architecture experience and 
I've already, already solved it.
What we are already good at is a good click for, for this product. So. There's 
this how we started, although we didn't, she didn't spend a lot of time on that 
one thing we had to spend some time on it, though. That was the language, the 
technologies we had to pay. And for those VPs, we looked into a couple of 
alternatives.
Yeah. Back then. It was not a very difficult decision either. Yeah. Or our 
opinion was also, so the best architecture, the best technology for the product 
is the one that you are already good at. So, because, because you are skipping 
the learning, learning, learning phase. 
**Michaela:** [00:32:00] So I imagine that if you're building up this startup 
and if you're iterating and learning, there's a lot of you have to go back and 
actually redo my cleanup, um, change, you know, what you have, have seen or 
done.
But on the other hand, you have this tension of the market that you think, well, 
I have to make progress after dividend features. And, um, do you feel like have 
enough time to actually go back and redo things to rewrite or to, well, Clean up 
some mess you made in the learning phases or is that also challenging?
**Alper:** [00:32:35] Actually, that's one of the things that we first talked 
about, we already knew that one of the challenges we would have on the way was 
keeping up to date and being responsive to customer requests, new features and 
everything. So we made sure our setup is as modular as possible. It is, it has 
very few dependencies.
If I am, if I want to add a new component is as easy as possible. So we usually 
need new features. You can just plug them in. And some of them are not used as 
much. Some of them are used a lot. If it's not used a lot, sometimes you just 
look into it. Okay, nobody's using this or this is useless and, and we drop it.
So, I mean, they don't really have to change, but we removed stuff. 
**Michaela:** [00:33:26] Do you have sometimes the feeling that you have a lot 
of pressure from outside schedule pressure from your customers, or is the 
product in a way that you don't experience that? 
**Alper:** [00:33:38] It is a lot of pressure. Well, I think we had our first 
customers at, um, the end of the second year and it's almost fourth year now.
So it's literally like two equal phases of the company. The first two years was 
especially from a perspective of a software engineer. It was really fun because 
we were just in the office. We were imagining this great tool and we were 
building it and it was fun. And then we went out, we had customers and then the 
real, the real world hits us.
There were deadlines that were customers calling in our customers, usually one 
to build the first project together with us. So they buy the platform and they 
can use it, but they want to do the first project. So we also do some projects 
using our own tool that comes up with deadlines. That comes up with maintenance 
that comes with, uh, support that, that puts us some pressure.
And yeah, we were, we were rookie on that as well at the beginning. Yeah. People 
were not great on it and we kept iterating and yeah, after that, after some time 
it got better, but it was painful at the beginning and it's getting better and 
better every day 
**Michaela:** [00:34:49] in these first two years were basically doing research 
and you're building out the platform.
Did you somehow contact potential customers? Did you talk with them? Did you, 
yeah. Did you reach out to dam or did you just think you have a good idea of 
your previous experiences of what software should look like? 
**Alper:** [00:35:12] That's a real nice question. And I'm going to, to be very 
honest on that via did some talks with some potential customers.
We did talk to some people, but right now, when I, when I look back and think 
about it, I would say it was not enough that that's a dilemma for most of the, 
uh, some of the technology companies I would say, or software engineers. You 
think your tool is awesome and you build it, you lose it. Is it, the real world 
can be different sometimes.
And what I can say that the, what we build on the first two years, some of it 
never was used. It was nobody needed it in the real world. So maybe we should 
have gotten more feedback earlier and more, and from, from people from different 
fields maybe, or from different potential sectors or something like that.
So yeah, we did it, but not enough. 
**Michaela:** [00:36:07] Yeah. That's um, that's something that comes up quite a 
lot because yeah, I think it's also hard. I mean, you hear that you should. I'm 
engaged with customers or potential customers, but it's not that easy always, as 
you said, you're asking them what they want to have. And also those answers are 
not really a North star for where you should go.
Right. So it's a little bit the fussy, fussy road that you have to. 
**Alper:** [00:36:30] Yeah. And another challenge though, is. Let's say you are 
in the development phase and you want to get feedback from people and they are 
not, your customer was yes. Right? So you ask people, okay, this is what they're 
building. Do you like it?
And they say, Oh, it's great. I worked there from the back and it would solve 
all my debt and debt and debt problem. And I would build that and that, and that 
project. And those are the features I would expect from it. Most of the time 
that list chains once they are really the customers, because then the whole 
company is involved or a lot of stakeholders is involved and the real project is 
always different than an imaginary project.
So yeah, that's, that's the challenge that you can get feedback, but the real 
feedback is always going to be from the real initial customers. 
**Michaela:** [00:37:24] Well, you're saying that at the beginning, you had 
those two years that you're were building the backbone of your company, and then 
you're going out to the customer and you showed them and they like parts and 
they don't like some of the parts or they don't use those, those parts.
But how did you get the first customers and how did you acquire those, those 
feedback? Um, On the different parts. 
**Alper:** [00:37:48] First customers were difficult. The thing that we were 
lucky about is we had a good network. And, and our founder is quite experienced 
in Turkey and a lot of projects with Microsoft. So he already did some, some 
networks, so he can, he could talk to people.
He could, we could do some demos and yeah, we, yeah, I don't remember number two 
kind of convinced a couple of people, but, uh, it, it was thanks to our, our 
network. So we didn't really run commercials or anything like that. But, um, it 
was the people that, that we already knew. Okay. 
**Michaela:** [00:38:25] And I know that your company is actually funded, right?
So you got some initials seeding. How did that happen? And when did that happen? 
When did you feel. That it's right to ask for external funds. And how did that 
help you in developing your vision and 
**Alper:** [00:38:40] your company? It was around the second year or something. 
We got investment from, uh, from two people. I think you can call it seed 
investment.
Actually. It's not really a series a, but, um, we got investments from, uh, . 
Those are two big names in Turkey. Actually one of them were not as Lamar was 
the founder of. The second biggest software company in Turkey. And he sold his 
company to the first biggest one. And then there, they are building the 
enterprise ERP software and he did his exit.
Right. And Henny became an investor and it was looking it up. Yeah. And he, he 
also knew  was, was the CEO of Turkcell the biggest GSM operator in Turkey. They 
heard about us that they look into the product. They thought it was promising. 
They came in as investors. They also want to be involved on the day to day, uh, 
operations.
So they, they are like our board. And they attend all our meetings like weekly 
meetings. And they are literally in the, in the process of running the company. 
So they're not like just investors and checking on us like every six months or 
anything, and to just looking at numbers, but they also are deeply involved in 
our daily work.
**Michaela:** [00:39:56] And did that change somehow? Did you feel that that 
changes how you develop the software? Did that change your, your course or your 
North star? 
**Alper:** [00:40:04] Well, it didn't really change the, the, the, the, the 
development part. Yeah. They already trusted us and they just kept completing 
what we were doing, but it obviously helped a lot with finding customers.
Yeah. As I said are thankful to our network and it's also, it's also them. They 
are network and their names that got a lot of attention to the company. And 
yeah. When people heard that they are the masters, they were more 
**Michaela:** [00:40:28] interested. Okay. That's really interesting because I 
had another guest recently on my podcast and his experience was quite similar 
that with the funding that came also a lot of advice and a lot of knowledge, a 
lot of network as well that the company can profit from.
So it's not only the financial advantages that you get. If you have, I think the 
right investor, it probably depends really. If you have the right or the wrong 
fit. Between the investors and your company as well. 
**Alper:** [00:40:58] Yeah. Now that you say it, and I think our club that's 
actually exactly what I wanted to say.
It's not that much about the funds and money it's it's experience and 
perspective they are bringing, bring, bring in. And that, that changes a lot 
that has a very high value. 
**Michaela:** [00:41:12] And when you talked about Dom, you said day actually 
came across your company. So were you approached by the investors or was it the 
other way round that you approached investors?
**Alper:** [00:41:23] Our founder, uh, used to work with, uh, Marotta Lamar, so 
they already knew each other. So did they, they had the first contact, I guess
new, uh,  other founders. So they brought each other in, I would say, but, uh, 
yeah, our founder knew, uh, knew him that they worked together 
**Michaela:** [00:41:46] before. So when maybe one thing that's related there 
is, is what I said before is that I think there has to be a good fit between 
people, um, be it, the company and the founders and the employees and the 
investor, but also the employees themselves.
So hiring can be quite challenging for a startup. I mean, it's, I think it's a 
challenging topic per se, also for larger companies, but individual person, 
obviously on a seven team. So in person team has much more impact then on a 700 
person team. Right. So how do you make sure to hire the right people?
What's your approach there and yeah. How, how did you hire the first several, 
uh, employees that you have at your habit company? 
**Alper:** [00:42:32] You have a good point. It, it, it has been difficult. It 
has been one of the biggest challenges we had, um, because of a couple of 
things. But first of all, you are a startup and you're small.
You're just set it up. And yeah, many people want to do that. Like people, most, 
mostly engineers, like they like the big names they're working for a big company 
or some operator or something like that. And again, here comes into cultural 
thing as well. You know, in Turkey, people communicate with their parents, their 
families a lot.
So that plays a huge role when they are making such decisions. Especially if 
you're a real new graduate, for example, it's kind of difficult to explain your 
family, like you're joining this company that just started two months ago and 
it's just two of them. Yeah. They don't have a product yet. And. Yeah, that 
raises eyebrows.
So the desk difficult. So because of that, we had a smaller pool of people that 
we could attract, luckily with, we could find people, but then another challenge 
is again, also probably Turkey specific, but the average. Average time an 
employee says that the company is quite short in Turkey. So, uh, I dunno how 
that is in, in, in Europe for the States, but yeah, it's kind of also difficult 
to hold on to people.
And especially if it's software. Yeah. First three, four, five months is still 
your investment phase. You're still in, you're still investing in the person. 
You're still training them. And if they are leaving on year one, Uh, yeah, 
that's a, that's a shame because of that, we try to be very careful while hiring 
people.
One of the things that we valued the most during the interviews was the 
personality you want to make sure the person is a good fit and you want to make 
sure that the person is going to like us and is more likely to stay longer. 
**Michaela:** [00:44:41] So maybe to, to wrap everything up, what do you think 
are the next big goals that you want to achieve with Quaker right now?
What are you heading towards and what brings the next year for you? 
**Alper:** [00:44:53] Well, we have around 15 customers, but, uh, it's always 
more, the more, the better, another challenge is the tool itself is it has been 
for years, so we need to keep adding new features. And keep up with, with the 
news technology. So those are the things that are on our roadmap.
**Michaela:** [00:45:14] Yeah. Sounds reasonable. Yeah. I'm from my side. I'm 
really happy that you have been talking with me that long. Yeah. I learned a lot 
about your startup. It sounds amazing. It sounds very challenging and very 
diverse. And I think you're doing a great job. Thanks for being on my show. 
**Alper:** [00:45:30] Yeah. Thank you. Thank you for your money.
Thank 
**Michaela:** [00:45:32] you. Bye. I hope you enjoyed another episode of the sup 
engineering and luck podcast. Don't forget to subscribe. And I talked to you 
again. Bye.


