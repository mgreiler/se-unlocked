---
episode: "Transcript Episode 69 Michael Lynch"
permalink: /coding-practices-maang
status: publish
type: transcript
---

[00:00:00] **Michaela:** Hello, and welcome to the Software Engineering Unlocked 
Podcast. I'm your host, Dr. McKayla, and today I have the pleasure to talk to 
Michael Lynch, a senior software engineer and entrepreneur. But before I start, 
let me tell you a little bit about my latest project: [awesomecodereviews.com](https://www.awesomecodereviews.com/). 
Yeah. All my work on code Reviews has now its own dedicated 
home at  [awesomecodereviews.com](https://www.awesomecodereviews.com/) you will 
find articles about code reviews, best practices, code reviews, 
checklists, news about the latest research on code reviews, and of course 
workshops and courses I offer around this topic. So please hop over to 
[awesomecodereviews.com](https://www.awesomecodereviews.com/) and check out my latest work. 

But now back to Michael. Michael is 
a software engineer and entrepreneur.

He has launched several businesses after leaving Google in 2018. Interestingly, 
it's not a software business that was his huge success, but rather a hardware, 
or let's say a combination of hardware and software business that brought his 
real success. It's called Tiny Pilot. Today I want to talk with him about his 
experience writing software for Google, Microsoft, and now for himself, at tinypilot.

And, well, you probably know Michael as well because he manages to write, write 
articles, blog posts that frequently rank number one on Hacker News. This means 
that they're reaching thousands oh hundred thousands of people and they read 
what Michael writes. So I'm really super thrilled to have him here with me 
today.

Michael, welcome to the. 

[00:01:28] **Michael:** Yeah. Thank you for having me. 

[00:01:29] **Michaela:** Yeah. I'm a big fan of yours and I'm following your 
writing, but not only on Hacker News, but also on your blog in general, and you 
know, what you tell us about your journey as an entrepreneur. Yeah. I have been 
here from, no, maybe not from the Superstar, but sort of from the start, I think 
2018.

2019, something like this. Yeah. Yeah. And one of the articles that I obviously 
love from you is about code. Right. Mm-hmm. . So you have this article that 
tests doing code reviews like a human or . Yeah. Something along those lines. 
Right. So in your career as a software engineer, what, what are your thoughts on 
code reviews and what are your main well tips or recommendations that you give 
to people about code 

[00:02:13] **Michael:** reviews?

Sure, yeah. Code reviews are probably my favorite part of my career as a 
software engineer, and I feel like it's one of the best ways to learn as a 
software developer because you're, you're just getting this detailed feedback 
from a teammate, and so I think that's incredibly valuable and I think a lot of 
organizations underinvest in that.

and I, I, everywhere I've worked, I've tried to invest a lot in code reviews. 

[00:02:41] **Michaela:** Yeah. I think that some people really love them and 
some people really hate them, and then there is a lot of in between. Right. Can 
you understand why some people don't like them? Why they think code reviews are, 
you know, a bottleneck?

Yeah, a, I think, 

[00:02:56] **Michael:** I think if you don't like code reviews, it's probably 
something wrong with your organization like, in, in the vast majority of cases 
where I hear people don't like code reviews, it's because the organization runs 
them badly. Like they use them. They like allow senior software engineers to 
like beat up junior engineers through code reviews.

And that's to me definitely not the point of code reviews. Like code reviews 
should be. , like a shared sense of ownership. Like how do we make this code the 
best it can not like? Mm-hmm. , I'm gonna show you how much smarter I am and 
like force you into submission until you make your code look like mine. So a lot 
of the stories I hear from people who hate curve reviews, it's like something is 
wrong with their organization and they think like they're experiencing it 
through code reviews.

But the problem is actually something else that's kind of broken about the 
culture at the organiz. . Yeah. That's also something 

[00:03:50] **Michaela:** that I often see and I say it's just surfacing through 
code reviews. Right, right. So the activity or you know, these power struggles, 
they are just Right. You know, coming up and, and I think also, you know, 
there's this part of, you know, beating up or power struggles or, yeah.

But there's also, I think also this slow. And this bottleneck and this, mm-hmm. 
. This is also organizational and it's just surfacing in code reviews, right? 
People work in silos, they work very isolated. They're not really working as a 
team. Right? And then you tell them, so now you use code reviews, , Uhhuh, , and 
obviously it's not working right?

Because you're not used to show your code. You are not used to have small, you 
know, small units of work. Right? So you are working on that thing for three. 
Stressed out to show it to somebody that you're not really familiar with and 
you're normally not working with. Right? Yeah, exactly. Then you throw the code 
over the wall.

It's so much that they can't really say something about it . Right, right. But 
it's also, it's not really contribute. It's something organizational that's, 

[00:04:51] **Michael:** you know. Exactly. Yeah. Yeah. And I think, think about 
that impact. Yeah. Like I, I agree. I think better quota e practices, when I 
hear people say, oh, it slows me down.

Like, I think Yeah. If you're, if you're coming from a practice where like you. 
You know, 5,000 lines of code and then show it to somebody and you don't expect 
any feedback. It's gonna be slower. But I think long term, you're gonna save 
time just because they're gonna forcing somebody to, to. , show it to another 
person and make sure it makes sense to another person is gonna save time in the 
long run to make sure the code is maintainable.

And I think a lot of the problems were like, okay, I've written 3000 lines of 
code and now it's gonna take the person two weeks to review it. And I mean, like 
they can't effectively review a 3000 line change list. But even if you're saying 
like, oh, it's, it's so slow because like I used to be able to just check in and 
now I have to wait a day before every change list.

I think that's fixable. Like I think you. Learn to write in smaller units, and 
then the person, you can create a culture on the team that code reviews are high 
priority, so you don't let them sit for a day. You, you try to get to them with 
within a few minutes or hours. So it's not this long bottleneck, incentivizing 
per the person to wait until they have a, a big chunk of code to send it to you.

[00:06:06] **Michaela:** Yeah. And I think incentives and rewards and all of 
that are in many organizations, really centered around, you know, having 
features ready. Yeah. Without review, . Right. Right. And then we just require 
them to review code, but we are not really rewarding people for it, or you know, 
we don't. Right. , we don't value it as much.

Right. We expect it. Yeah, exactly. But on the other hand, we are not investing 
in it, so, right. You know, people, what, what are, what should people do? They 
are torn apart between, you know what? I'm actually evaluated for writing 
features and having code shipped. Right. And then there's this code review where 
there is no time allocated for it.

And then they are, they're experiencing problems with that. 

[00:06:47] **Michael:** Yeah. Yeah. And I think it has to come from the 
organization to realize, . Yeah. Like you, you're maybe gonna pay a short term 
penalty, but long term it's gonna be, it's gonna be worth the investment that 
you put in, in the short term. Yeah. 

[00:07:01] **Michaela:** So you wrote code at Microsoft very long time ago, 
right?

Yep. Yep. And then at Google. And now with your own business as well, right? So 
you, yes. I know that you're also having developers that are working with you. 
Yeah. So how did the code practice change in all those different settings? 

[00:07:18] **Michael:** Yeah. I mean, the biggest difference between Microsoft 
and Google was the tooling.

When I was at Microsoft, it was in 2007 to 2010, and we didn't have like really 
any tooling around code reviews. You would just send a diff over email to 
somebody and then they would respond writing the line numbers that they wanted 
to to talk about just in another email. So, . When I got to Google, it was a few 
years later and they had much better tooling.

I think that that Microsoft now has better tooling. I think Mikaela, you 
actually worked on that. Yeah, yeah, 

[00:07:52] **Michaela:** yeah. True. Yeah. So I was there 2012, 2018, 14, and we 
had already code, code flow and it was a code tool and was quite good. 

[00:08:02] **Michael:** Yeah. Yeah. But in terms of the culture, I think Google 
was a little bit better in terms of, Rewarding code of view and thinking that 
it's something worthy of investment.

But I, I also think it varied a lot from team to team and from person to person. 
Mm-hmm. , like, I think some people would just, at either organization would 
just kind of rubber stamp it. And it's funny because there was one of the 
developers that I worked with at Microsoft, I was my friend Matthew, and he. . 
I, I thought of it as he taught me a lot about code review and then like, I 
talked to him, we were like, you know, 10 years into our career and I was like, 
yeah, you taught me a lot about code reviews.

And he is like, no, you taught me a lot of it. Like, I thought I learned 
everything about code reviews from you. Yeah. And so it, it is funny, like, I 
think it's, it's hard to separate like how much of it is just me. Like trying to 
do code reviews the way that I want at different organizations and, and thinking 
that the organization is, is feeding it to me.

But I think code reviews for me have always been something that appeals to me a 
lot. Just like even, even in college when I would have to do like peer reviews 
on somebody's essays and in a writing class, I would get really into it and 
wanna write a lot of feedback. And so I think that's just my personality, like 
wanting.

to think a lot about somebody else's work and mm-hmm. give them feedback. 
Mm-hmm. and so code of reviews are a great tool for that. 

[00:09:23] **Michaela:** Yeah. I remember when I was at Microsoft and I was 
writing my first feature and it was actually for the code flow tool, so for the 
code review tool mm-hmm. , and I was writing, you know, a feature and I know 
that I had to ship this code, right?

Mm-hmm. , and I was so grateful. I could actually have it reviewed before, 
right? Mm-hmm. . So I was actually, I mean, I was learning a lot because I, I 
wasn't sure like, are the practices now that I, you know, that I come with, are 
they what they people here do as well? Right. And, you know, is that actually 
correct, how I did it and so on, right.

Yeah. And I didn't get, I mean, I got a couple of comments that definitely 
helped, but in the end it was quite okay and it was also a good feeling to know, 
okay, that's what I, what I did right, is actually you. I fit right in let's 
that how I'm doing it right. And maybe tweak here and then tweak there. Right.

And so for me it was a very positive experience and a very Yeah, definitely a, a 
little bit of a, a reassuring experience. Right? Yeah. So if I would have 
shifted that, I would probably very, that's probably my personality, but I would 
very, quite a long time of, you know, I shifted. Yes. But, you know, nobody has 
seen it.

Maybe they're not happy with us. Right. You know what I did? , but because you 
have this feedback mechanism and you just said, you know, maybe here a little 
bit different, but here you did very well or something. Yeah. I knew that what 
I'm actually providing and what I'm doing, especially at the beginning, what was 
good, right?

Yeah. And so this was very 

[00:10:48] **Michael:** helpful for me. Yeah. I feel like that is such a great 
benefit of code of views, that it's great for percolating practices across the 
team and the good practices that somebody discovers manage to make their way 
across the team because they'll, they'll spread that in coder views.

the, the good practices kind of have a way of bubbling up to the top. Yeah. And 

[00:11:08] **Michaela:** so now it's a little bit different, right? Because now 
you are writing codes together with developers that are, you know, in your 
company. Yeah. But they're also, I guess, contractors probably, right? Yeah. And 
so how is that, did that change a little bit how you give feedback or how you 
use the tool, you know, as, as, as helping your business and, and your code 
base?

[00:11:30] **Michael:** Yeah, I think it. . It's been interesting because I'm 
the person hiring, I can, I can influence the, the code review culture a lot 
more than I could on other teams. Like I think I, I generally was pretty good at 
influencing culture of coder reviews on the teams at Google and Microsoft. But 
with this, it's like I'm picking people that sort of align with my views on 
writing code anyway.

Mm-hmm. . And so the, the company, like, it was interesting going from. Like 
just me as a developer to having another contractor to then having two 
contractors. And then I, I was trying to spend less time writing code and more 
time on management just because, like as a hardware company, there's so many 
moving parts and I realized like, okay, I'm still reviewing everybody's code.

Maybe it's, I should just have the developers' review each other's code. And I 
was like, well, are they gonna have the same standards that I do? Like, are they 
gonna review it as rigorously because like, they don't like. Part of it is like, 
I am long-term maintaining this code, and for contractors they might not feel a 
sense of ownership because like contractor, it's, you're less bound to the 
company than if you're an employee and much, certainly much less bound than if 
you're the owner and founder.

Mm-hmm. . But I found that like after we had been doing code reviews for 
probably six months where I was doing all the reviews, and then once I started 
having. the contractors review each other's code. It was exactly the same as if 
I had been reviewing the code like I was. I would sort of like peer over their 
shoulder and make sure they're, they're not missing big things that I would've 
mentioned, but I found like I would look at their reviews and I'm like, this is 
exactly what I would say.

And often they would find more things to improve than I would've I would 
noticed. So that was a really big surprise and I, I think that's sort of speaks 
to how well code of use can kind of. Become a foundation of the coding culture. 
Like once you establish a culture around code of views, it, it sort of 
propagates itself and keeps those practices running.

[00:13:31] **Michaela:** Yeah. And I think also, not only about code reviews, 
right, as a practice, but also on the values that you have on your code, right? 
Mm-hmm. , how should a code base look like? How much, how much quality, let's 
call it quality, but how much Yeah. You know, coding standards do we actually 
require from our Yeah.

Apply or require, exactly. Right. And, and I mean, I'm working with a lot of 
different teams. teams that have, I would say, lower standards and they are 
quite a few companies, right. That have lower status that don't Yeah. You know, 
it, it's really still a big discussion if , if it's important or not to have, 
you know, readability or if it's important or not, how we name things or that, 
that things are consistent throughout the code base.

Right, right. Not every company, or also not every engineer would agree that 
this. important. Yeah. And so I think Covis are a great tool to communicate that 
as well. Right. Or, or a poor tool to communicate that if you, you know, if you, 
if you can't agree on. The, the quality, quality of your software, right? So 
then everything, every comment becomes through as nagging, right?

Why are you even talking about 

[00:14:41] **Michael:** this ? Right. Well, I think that's a thing that's been 
interesting too, as, as a bootstrapper, like the timelines are very different. 
Like code that I wrote at Microsoft, like I worked on the Windows team and that 
code is gonna exist. 15 years, like people have to maintain. I worked on Windows 
eight and Windows 10, like that's, that lifetime is probably 10 or 20 years that 
somebody has to maintain that code.

So there's a really big payoff to making sure that it's maintainable and 
especially because it's, it's also like kind of hard and expensive to ship 
patches to software like Windows. Whereas with software that I right now, like 
especially with a lot of my businesses that ended up not panning out. , I sort 
of like am used to just writing in the style of, of Microsoft and Google, 
assuming that the code is gonna be around for 10 years.

And then I read Rob Wallings book, start Small, stay Small. And he was saying 
that like a lot of engineers have this fear of technical debt because they know 
that. Managers generally, like will never let them pay down technical debt. 
They'll say like, oh yeah, we'll, we'll accrue and peck technical debt and then 
we'll pay it down later.

And then that never happens because there's just a push for a feature and he is 
saying, but if you're like, so you're naturally gonna have that fear as a 
founder. But if you're the founder, you do control when to pay down technical 
debt. And so you can do like a shoddy job on something that's still experimental 
and ship it.

And then once it causes problems, you can then go back and say, okay, like this 
is something I wanna maintain for a while. I'm gonna do. I'm gonna redo it. 
Maybe like with more code reviews. And so I think as a founder with an indie 
business, you do have a lot of decisions. And that that's hard. Like it's hard 
to, to give somebody a code and say like, okay, drop your standards for this 
code review because this is just experimental code.

Yeah. But I think there is room for like, it doesn't have to be, not all code 
has to be of highest quality, highest maintainability. Like, and I think that's 
an important thing to recognize as a founder. Like you have to, it's all 
engineering like you. what things you wanna invest in, what the payoff you 
expect it to be.

Yeah, yeah. 

[00:16:43] **Michaela:** True. And I think what you're discussing here, right, 
is now it's the conflict that you have within yourself as an engineer. Yeah. And 
as a founder. Right. But it's actually the broader conflict that we also 
experience in other companies where we are the engineering team and then there 
is the ceo, right.

Or you know, the product manager or something. Right. And they are striving. 
Going to market and you know, is it? Yeah. But, but the good thing is if you're 
the same person, it's easier for you to judge whether or not Yeah, exactly. You 
know when to make the call, right? Yeah. To make the call too. Right. You know?

A little bit more like, let's say faster code . Right, right. For the beginning 
or some prototype codes or something like this. And when to say, well, now we 
really have to improve what we, what we have. Yeah, definitely. On the other 
hand, I also had a quite a few founders also that I talked that were discussing 
that, you know, we started off with this business and then we were getting uses 
that we didn't expect mm-hmm.

and we were always, you know, always on the edge to breaking and we always 
broke. Right? For every, right, for, for every. Step in growth that we did, 
right? Let's say thousand. It broke because it was made for 10. Right. And all 
are accessing our system. And then 10,000 it broke again because it wasn't made.

Made for that. Right. And so they're running behind gross wheel, which I think 
is a good problem to have . Yeah, exactly. Like as long as you manage. Right? 

[00:18:05] **Michael:** Yeah. I think those are often fixable. Like you can 
invest more in, in fixing the bottlenecks, whereas I. people overinvest in 
things expecting it to scale to like 10 nines of re reliability for their like, 
startup that has two users and yeah.

Oh, it's gotta be on Kubernetes and it's gotta scale to like end different 
servers and five different backends. And so I think, yeah, like, especially if 
you're a bootstrap founder, I think it's, it's important to learn the lessons of 
just like investing as little as possible to get up and running and then finding 
out where the, the bottlenecks and breaks.

We could even start with no code. . 

[00:18:43] **Michaela:** Yeah, yeah. Start, right? Like I always find it really 
hard, but it would be an an option, right? Like . Yeah. Yeah. You know what I 
was thinking of? Now that you have a hardware business, how is that? Because 
it's not easy to ship batches, right? So if they have tiny pilot and they have 
some, probably some firmware that you're writing or, or what kind of are you 
writing there?

And then if you want to ship a new version, 

[00:19:08] **Michael:** yeah. Are you going to do. Yeah, that was, I mean, this 
is, this is a great example of what we were just talking about, of building like 
the simple thing and then waiting until it breaks. So, yeah, I didn't know how 
to do that. Like I, I never built any kind of hardware before where like I have 
to, Ship updates to users.

So originally the way I got code onto, so maybe I should introduce Tiny Pilot, 
is um, it's a little device that you can plug into computers or servers, and it 
lets you control the, the computer remotely through your browser. So it, it 
emulates a mouse and keyboard and it captures the input. And so I, I built it 
using the Raspberry Pie, the little single board computers.

So I'd never really done any engineering on top of the raspberry pie before for 
a consumer product. And so when I first shipped it, like I had no idea if 
anybody was gonna buy it. And so the way that when I was developing the 
prototype, I used a tool called Ansible that does, it's usually for like 
configuration management for servers, where it just creates an SSH connection, 
then moves some code over to the.

I was like, okay, that, that's fine. I'll use that. And so when it came time to 
like it's open source, so when it came time to explain to users how they can 
install it on their raspberry pies, I was like, okay, I just got, I'll create 
like a really simple bash script that bootstraps a little Ansible environment 
and, and uses Ansible to install.

the software to itself, which is very unusual. Like nobody does that and for 
good reason, which I, I later found out , but I didn't know any other way to, 
like, I, I also like had no, the, the typical way you install software on Linux 
is using like app to get or something, but my software, like, because it had to 
change the kernel a little bit.

App get was kind of hard to do, but Ansible worked and so I did that and then 
like I found that, okay, now that users have that they want to interact through 
the web interface, they have to like my instructions for how to update, were 
still to like create as an SSH connection, then update which users didn't wanna 
do.

So then we had to iterate on that and then like, Now we're, we're to the point 
where like the Ansible installations take like 10 minutes and now we're trying 
to figure out like, okay, like let's back up a little bit and figure out how to 
do this through like the more standard tools. But we lasted for, for two years.

Like looking back, maybe it's something we should have invested more in to do 
it. like right the, the first time, cuz it is a little bit hard to unwind. But 
yeah, it's, it's hard to predict those things. Like I, my friend David Toth, 
who, who's another indie founder one, he's really helped me think about like 
what things you should invest in because it's like you can overinvest in 
anything and he, the way he's found to choose what to invest in is like things 
that you can't undo later.

Mm-hmm. , so like, Something, you know, like the color scheme is probably the 
easiest thing to change. Like if, if you have a, a web app and you say like, oh, 
I don't like this color scheme anymore. It's very simple a week later to totally 
redo the color scheme. But something like a choice of database that's pretty 
hard to change if you like, are use a no Squi database is your backend, and then 
later on you realize that you actually want like a sequel base backend, then 
that's a really difficult decision to change.

So you have to. Budget more, more time to think about those investments, the 
things that are like gonna be really hard to change later. . Mm-hmm. . Mm-hmm. . 

[00:22:23] **Michaela:** And I can imagine, right, that a tiny pilot, the first 
users, right, the more the curious people, right? And also the fish saving 
people, right? So you can also burden them a little bit with some tingling and 
so on.

So that's probably what I think, right? But right now that it's getting more 
widely used, I guess there are more users. You want to get a bigger user. People 
also that want black and play. Right. The easier. Exactly. Yeah. Install, 
installment and so on. Is that something that you now try to provide more for?

Did you see how the customers that you attract change over time? Maybe that's my 
question. 

[00:22:59] **Michael:** Yeah, definitely. And I mean, it, it wasn't, I think. , 
I think it was the, yeah, like changing the, the way that we presented the 
product and changing the way it worked was a good way of going upmarket. And cuz 
at the beginning it was like, I launched on Hacker News and a lot of people 
that, that bought it, a lot of them could have built it themselves.

Like I didn't have any. Anything special at that point, it was just like, I can 
sell you a kit of all the things that you need to build it, and I'm giving you, 
the software is free anyway. So I think a lot of those people just bought it to 
support me. And then like, as it went, I, I offered more like custom case and 
then like, um, Had it more like custom built so that it was more of a plug and 
play solution.

And then I think as I did that more businesses rather than like home hobbyists 
started to become interested because it's like they want, they want, like, I 
think the hobbyists love to tinker and like, don't mind like, oh, I have to ssh 
and run from the command line. And I think the businesses are just like, I want 
something that, I like the idea of something that I don't have to, I don't wanna 
tinker with it.

I just want it to work. Yeah. So yeah, we've over a time we've, we've tried to 
make it. More for the people that like don't care about tinkering while still 
making it friendly to people that like want that extra power. 

[00:24:13] **Michaela:** Yeah. And so did you see that the kind of support 
requests that you're getting are different now?

Do businesses send more support requests or less support requests, or is that 
all the 

[00:24:24] **Michael:** same? Businesses tend to, it's, I think a lot of people 
observe this, that like the more the business spends, the less support they 
request, which is like the opposite of what you would expect. Like you'd expect, 
yeah. Oh, they're spending 10,000 dollar with us.

They're gonna like expect a lot. But usually if, if they're spending 10,000 dollar, 
it's. a very small amount to them, and they have people on staff that like can 
figure things out. Whereas it's, it's the business that are like very budget 
conscious where they're like, we spent 350 dollar on your project, like your product

And that's a huge deal for us. So we expect the moon. And so like they, they 
tend to be more demanding and like mm-hmm. want a little more direct support. 
But yeah, like that's, that's been a whole other journey of just figuring out 
ways. Manage customer support, because at the beginning it was just like all the 
customer support was like, just email me.

Like, I'll, I'll respond to any support quest. And then that very quickly became 
like, I was spending four hours a day just responding to emails and most of them 
were like the same email. Yeah. So I, I've had to figure out ways to make that 
scale better. . 

[00:25:26] **Michaela:** So how did you do that? What, what, what's your, 

[00:25:28] **Michael:** what's your way?

So there are a lot of things. So the first thing I did was to add a support 
forum and that was, that was a big help cuz I was seeing like, okay, a lot of 
these questions are repeating. Actually, I think the first thing I did was add 
an faq cuz mm-hmm , it was, it was much easier to say like, okay, instead of 
like rewriting this answer every time, I'll just write it once really well on, 
on my website and then point people to that article and then it would, it would 
let people.

Solve their own problems if they ran into something. And then the next thing I 
did was add a support forum where, because the problem with, with doing it over 
emails, it's siloed. So like you answer the question once and then nobody else 
can see that answer. But on the forum, it, it tends to force everything out into 
the open.

So like, if. , if somebody else runs into the same issue later on, it doesn't 
cost you extra because they can easily search and find the, the same solution. 
Before then I started adding local staff that handle the fulfillment, so they 
ship out orders and everything. Mm-hmm. and then I realized like, wait, they 
could be answering these emails too.

Like I, I had. For a long time thought like, oh, like a lot of these emails are 
technical, like, and the, the fulfillment staff, you know, they don't have 
experience with Lins, they're not gonna be able to answer these questions. And I 
realized like, probably like half of their requests have nothing to do with, 
with tech support.

It's just like, Hey, I didn't get my tracking number. Or like, hey, like, you 
know, I'm. I need to update my address or something like that. So very easy for, 
for somebody without a technical background to solve. And then the last step was 
adding somebody who does have Len experience. So I hired a support engineer 
earlier this year.

And so that's like all those things together have made it so that like I end up 
only participating in maybe like, 10% of support requests. So it's, most things 
are, are pretty easy for, for the staff to handle. And then we're always trying 
to make it like, keep things scaling. So like if, if there's like a.

A consistent issue that users run into. They have to read the F faq. Like we try 
to make it so, okay. Like how can we change the product so they don't have to a 
add that? Mm-hmm. , one of the like interesting ones was we would, at the 
beginning we would get a lot of questions like, oh, does this it tiny pilot 
captures H D M I output?

And we'd get a lot of requests like, oh, what do I do if I have v g output? And 
so we'd say, oh, like. Use a VGA to H D M I adapter like we've tested this one, 
it's fine. And then I realized like we could just sell that. Like we just have 
like a checkbox in the order saying like Add a VGA to H D M I. Adaptor.

Yeah. And so then like that made those questions go away. And like a lot of 
those, the customers now just will buy that from us. So yeah, we try to like 
figure out ways, like how can we change the product, how can we change the 
website so that users don't have this question in the first. Yeah. 

[00:28:04] **Michaela:** Yeah. So coming back to the software on Tiny Pilot, 
yeah.

You talked about code reviews, and the code reviews that now that you actually 
use code reviews, you were able to have them on the same standard as you were 
expecting, but also that you probably, maybe not for tiny pilot, but for your 
first. Attempts in, in different, you know, products and, and SaaS businesses or 
whatnot.

Right? Yeah. What you're trying out as a, as a founder, as a indie founder, you 
have different kind of standards on quality. Yeah. What about unit testing? Do 
you have unit tests for tiny pilot? Do you have unit tests for your other 
projects? Are you always necessary? Do you have system task integration tasks?

What do you think about testing? 

[00:28:44] **Michael:** I love testing. I'm a huge fan of unit testing, and so 
for, for most code that I write, I have unit tests. The exception is like I, I'm 
not very good at writing unit tests for front end codes, so like stuff that has 
to interact with the, like I, I know there are ways of doing it, of like loading 
components of your page and unit testing that in isolation.

I've never learned how to do that and I also like, it hasn't ever come up as 
like something. Mrs. Bugs, but generally with, with almost all of my projects, 
I'll write unit tests because I feel like they pay for themselves so quickly. 
Like, especially when it's, it's something that like you have to parse user 
input or something.

I feel like. , it's so much easier, like once you have the unit tests in place, 
it's so much easier to just keep running your unit tests than to keep having to 
manually test things. So I, I tend to write a lot of unit tests, even for things 
that I don't expect to last very long. I'll typically write end-to-end tests 
using Cyprus.

Cyprus is a tool for browser automation and it's pretty easy to just, I, I have 
this standard set up that I use where I run it under Docker, and so as long as I 
can run my app under Docker, I can run. Cypress in one Docker container in my 
app and another, and then they, they just talk to each other and it works pretty 
well.

So I, I tend to write a lot of uni test, actually, ironically, tiny Pilot is the 
place where I probably have the, the least test coverage because the tooling is 
pretty hard. It requires, cuz if you think about what tiny pilot does, like it 
has to run. on to, it requires like special functionality in the Linux kernel 
that mm-hmm.

is only available on certain hardware, and so Raspberry Pie is one of those. So 
it has to change the kernel so that it can emulate a keyboard and mouse, which, 
so you can't really do that. Like if you just throw that on GitHub actions or 
Circle ci, like you can't test that functionality because you can't modify those 
kernels.

and then your, your test. The, like, the real functionality is like, if I type 
this key, does it show up on the remote system? Mm-hmm. and that's very 
difficult to, like, you, you'd have to like have a very complicated test setup 
to, to test that functionality. It's doable and like, I've thought about ways 
of, of doing that, but we don't have end-to-end tests and the, the end-to-end 
tests that we have now are like, for a long time it was just, I, I had a long 
Google.

Explaining like how to test every single feature that I would do before every 
release. So it would take me like about a, a full day to, to test a release. And 
then I handed that over to the fulfillment staff that they handle that We do 
have uni tests, so for the. The web backend is written in flask, and so that 
part is very like just testing the, the rest endpoints and a lot of the low 
level code that's very easy to unit test.

So we have pretty good unit test coverage there, but the, we don't have 
end-to-end tests and that's, that's something that like is, I'm kind of ashamed 
of and always think like, oh, like maybe we should take, if we took probably two 
or three months, We could get uni end-to-end tests up and running, but it's 
like, do we really wanna take a feature freeze just to, to get to that point And 
Yeah, it's hard.

I know, I, I love testing, so it's, it pains me that we don't have end end test 
coverage for that. But I don't, I, I don't think it's worth the investment yet. 
. Yeah. 

[00:31:56] **Michaela:** So for me, tests are, regressions are the, the, the 
reason why I, yeah. Have tests, right? So yeah, the confidence that forgettable 
me, right? Going back to the code that I wrote, I don't know, a week ago, or 
it's, let's say half a year ago, right?

Like this is like somebody else wrote it, , right? And then needing to remember, 
you know, does it have a side effect? Maybe something else, you know, like 
collapses now. So is that something that, do you feel that you. Tiny pilot to be 
tested just because you wanted to be tested and it's your standard, or would it 
really help you with that?

Like that you say, well, my confidence is, you know, now increased because 

[00:32:36] **Michael:** I have, uh, test. Yeah, definitely. Because there are 
like, there have been bugs where there, there's some subtle regression where 
like this dialogue now doesn't pop up because we changed something in the, the 
front end and. doing, having those tests be manual, like does give me that 
confidence, like the same confidence that I would have if they were automated 
tests.

Mm-hmm. , but it's still like, it's, it's very costly. It still costs a human. 
30 minutes to, to run those tests. And then I, I review those tests to make 
sure, like I don't see anything that looks odd in the, in the test output. So, 
mm-hmm. , I'm, I'm still getting the same confidence and like, that definitely 
is important to me to have the confidence that we're not shipping something out 
to users that's just like completely broken.

And, and even with those tests, there's been, we've, we've discovered gaps in 
the test where we do ship something. Some combination of functionality doesn't 
work and we're like, oh, that, that was embarrassing. And then we update our, 
our test plans so that we make sure that we always include that in the future.

But yeah, it like, as the test plan gets longer and longer, I, I'm more and more 
interested in automating it or at least automating some of it. Yeah. But like 
the, the problem with something like this is like the big investment is just 
getting the test set up. Like just getting to the point where you can write your 
first.

And then once you have, yeah, because probably then it's 

[00:33:52] **Michaela:** straightforward, right? If you 

[00:33:53] **Michael:** have that. Yeah, exactly. If it works. Yeah. Yeah, 

[00:33:56] **Michaela:** yeah. I was, I was doing dynamic and static analysis 
and was, you know, working with the eclipse ecosystem and things like that. And 
also they're, you know, the, the system tests and so on, they were not, That's 
straightforward because I was also, yeah, changing the system internally and so 
on.

So I have a little bit an idea of how, how difficult, not completely, because 
it's not hardware then, but it was still, it was still not straightforward. 
Right. It was not that you just could use J Unit and you know, it just drive 
out. Yeah, exactly. You know, runs out of the box or something. . So how, how do 
you think about this?

Do, do you think about it? Okay, now we are spending like half a day every week 
and then you calculate how many days that is and weight it up with how much you 
estimate that it'll take to write that, that test, you know, the 

[00:34:41] **Michael:** test runner. Yeah, I mean, I think the biggest 
bottleneck I think of the software in terms of.

Of feature velocity. Like I wanna be able, like I want us to have maintainable 
code and like code that the developers enjoy working on. Like, I don't want it 
to be a pile of hacks, but I also want like, I think part of that, like you 
can't just make beautiful code. Like you can't just refactor forever. Like I 
think users and also developers expect to like continue shipping features.

And so it's a question of like, okay, how much developer bandwidth are we losing 
to. Tests because like if we had automated tests, we could just run them on 
every commit and find out very, very quickly if we broke something. Whereas like 
if it has to go to a tester and then the tester re reports back, we can only 
afford to do that like,

You know, it just logistically, it's hard to do that more than like once every 
few weeks. And so there's a, yeah, a long turnaround where it's like, okay, this 
broke. What was what? Change broke it, and so it would cause analysis. Oh my 
goodness. Yeah. Yeah. So like that, that happens infrequently enough that.

it's, it hasn't. Mm-hmm. been a, a strong push for us to like, automate 
everything, but I think like, as the, as the, we add more features, it's, it 
necessar necessarily makes it more complicated to test and then that pushes us 
more in the direction of like, okay, like when, what, when can we start 
automating some of those testing so that we're not relying on a human to 
manually run through all the features?

Yeah. , 

[00:36:09] **Michaela:** I wanted to ask you about another topic, and that's in 
Introspectives, right? So Sure. Intro inspections, because I know that you're 
writing this. I, I'm subscribed. Subscribed to your newsletter, right? Mm-hmm. . 
So every month I get sort of a tiny pilot, this and that, right? So I, I always 
can follow what, what happened to you, but you don't also doing that on a weekly 
basis.

Right. And on a monthly basis, and then animal and so on. Right. I looked at the 
weekly ones, and they're even ratings here. So you're rating yourself, you know, 
how well you did in an area and so on. Yeah. So why you do that? What is that? 
Actually, maybe you explain it a little bit. What It is better than I did right 
now.

Sure. And then, and, and then why are you doing it? 

[00:36:48] **Michael:** Yeah. I got the idea from this tool at, at Google called 
snippets. So that was, it wasn't universally used, but it was just, A very 
simple tool was just like a markdown field where at the end of the week you 
could write down what you did that week, and then the following Tuesday, it 
would get emailed to all of your teammates and then anybody could, could 
subscribe to your snippets if they just wanted to see what you're up to.

So sometimes, like a partner team would subscribe to your snippets, just like as 
a, an easy way to get updates on what was going on. A lot of the value was also 
just the. Two or three years. I was working for a manager who was in California 
when I was in New York. And so like he didn't have a lot of natural insight into 
what I was doing, and so the weekly snippets helped him understand what I was 
working on each week and then, Previous companies, like our status meeting would 
be like, I would have to explain like what I had been doing since our last 
status meeting, whereas this was like, they already knew everything I was doing 
cuz they'd been reading my snippets and I thought that was such a great tool.

It was also good at, at promotion time when you had to like go back and review 
all your accomplishments for the year and figure out like, okay, like what's, 
what am I gonna use as evidence? For the promotion team. And it was funny 
because I, I switched managers and then I found out that my new manager wasn't 
even reading my snippets.

And my reaction was like, oh, then like, what? Why am I even writing these? And 
then like two weeks later I was like, oh, I like, they're good for me. And so I 
just ended up. Writing them anyway, even though my manager wasn't reading them. 
And then when I quit Google, like the first week after Google, I just kept, I 
opened a Google Doc and just started writing them for myself.

And yeah, I, I just find it very, it's, I. , it's very easy, like especially for 
a developer to end a week feeling like, oh my gosh, I didn't get anything done. 
Like if you spent the whole week like trying to debug a, a difficult bug in your 
app, you're just like, oh, I, I, nothing happened. I spent the whole week doing 
that and I would often feel that way, and then I would go back and like when I 
write my snippets I'll.

or I, I call them what got done. I would look like, look at my, what code? I, I 
checked in to GitHub. I would look at my outgoing and incoming emails. I would 
look at my calendar, and so it forces me to kind of take a, a more objective 
view on what I did for the week, and I'd be like, oh, wow. Like, so there would 
be weeks where I feel like I got nothing done.

I'd just spent the entire week debugging this one thing, and then I was like, 
wait, that was actually just the last two days on like Monday and Tuesday. 
Mm-hmm. , I shipped this big feature. It was so, it feels like so far long ago 
that I've forgotten it, but like, forcing yourself to go back and review it, 
it's very satisfying.

It like, makes me feel like, oh, like even weeks where I feel like I didn't get 
a lot done. It's because I'm, I'm seeing it through this, like very down on my 
self perspective, but if I look at the facts, I realize I actually got a lot 
done. . Yeah. 

[00:39:32] **Michaela:** Yeah. And, and there's this one part right, where you, 
it's a memory or age right?

Where you see actually, oh yeah. All of those things got actually done. And I 
mean, I, I really have a hard time with to do lists. Yeah. Because I always do 
things and then Right. I can't write them, so I. Normally, you know how , how my 
day starts. I open up my to-do app. Mm-hmm. , I write down five things that I 
have to do while I'm doing this.

I'm thinking about something they really have to do instead of writing down that 
I have to do that I do it. And then when I haven't done it, I'm, I don't add it 
to the, to, to-do list anymore. Right. And so, yeah. Uh, and while I'm writing 
my to-do list, I do all the things that are really important. And then I have 
five things still on this thing that I have done right?

They're like, this is so frustrating, . Right? And so I like this that you, that 
you change it, right? You write about what you have done instead of what you 
have to. , but what about the evaluation of it? Or evaluation, right? Where you 
think about, you know, could I have done that better? Or you know, was it, was 
I, yeah, what I expected?

Because you're also doing that, right? So you're, 

[00:40:35] **Michael:** yeah. Yeah. I find that helpful as well. So in my 
monthly retrospectives i'll at the. At the end of each retrospective, I'll set 
goals for the following month. So I'll usually publish my retrospective in the 
first few days of the month, and I'll say like, okay, at the end of this month, 
these are the three things that I wanna achieve.

And espe, I think, I think especially as an indie founder, it's easy to kind of 
like lose sight of the, the high level goals. And like, you can, you can think 
at the beginning of the month, like, okay, I wanna ship this thing. But then you 
get so into like, oh, I, I really wanna polish the ui, so I spend. A week on 
that without really thinking about whether that contributes to my larger goal 
and then like the month ends.

And if you're not thinking about like, did I hit my goals, you can just think 
like, oh, okay, like I didn't ship the feature, whatever. Like, you maybe don't 
even like take a breath to think about whether you, you met your goals because 
you didn't set them to begin with. And so I find that like, If you're a founder, 
there's so many possibilities.

I think that's the thing that a lot of people miss if they have never worked 
outside of like a standard employment situation. Like if, if you're in charge of 
deciding what to do, like there's infinite possibilities. You can invest more in 
marketing. You invest more in engineering, you can invest more in hiring.

And so like there's so many things you could do. And if you don't set specific 
things that you're trying to achieve, like you could go down the rabbit hole on 
something. doesn't matter. Like you can mm-hmm. , you can spend a month 
polishing your website and like the website, if you really sat down and thought 
about it beforehand, like you would probably realize that like the website 
probably isn't the thing that's preventing you from, from gaining new users or 
gaining new customers.

And so I think like having these, these goals and then like thinking about at 
the end of the month, like, okay, like. Did I hit these goals and then like, if 
I didn't, did I have good reasons or did, did I just get distracted and like 
forget about my goals or like what, I think it's helpful to just take time to 
evaluate like, why didn't I meet this goal?

Yeah. And like, what can I do in the future to, to help me ma like achieve my 
goals better? 

[00:42:36] **Michaela:** And do you think about these goals and more activity 
driven or more output or outcome driven? So do you think about. Or I want, you 
know, 10% growth of tiny pilot users. Or do you think about Oh, I want to make 
that 

[00:42:50] **Michael:** feature?

Yeah, I try to balance it cuz it's hard. Like I, I do sometimes set goals of 
like, I want to reach this, this number in revenue. Um, because yeah, like you 
don't have full control. Like, you can work as hard as you want and like 
sometimes you can't. , there are other circumstances that prevent you from 
getting to 70 K in revenue for the month or, or whatever it is.

So I think if it's all goals that are driven by that, like you, you don't 
ultimately control. That's very difficult. And so I try to balance it with like, 
certain things are like entirely within my control. Like I know if I focus, I 
can do those things. Like it doesn't depend on the response from external 
factors.

Yeah, I 

[00:43:30] **Michaela:** think probably you also have like, maybe it's. This is 
my goal, right? The goal is to have 10% more users and then the activities that 
somehow, okay, because I want this goal, I'm going to do X or Y, right? Right. 
So let's say the next three months, I'm trying to implement two new features 
because I think this will give me, you know, those 10% of users, right?

And then you can look at did it actually, let's say we are managing to do this 
to features and we don't have the 10% of more users we can think. Well, maybe we 
should have the, you know, purchase flow optimized or something. Right, right. 
So next time we have maybe the same goal, but the different activities to, 

[00:44:08] **Michael:** to reach that.

Right, right. Yeah. Yeah. Yeah. And I think that's, that is the, the other thing 
that's useful for like the high level goals, cuz if your goal is like, I wanna 
add this feature, and then it turns out that like adding the feature takes three 
times as long as you expected. It isn't, it probably isn't worth pursuing that 
goal if like your real goal is, You know, increased growth by 10% or like get 
another, like double your user base by the end of the year.

Like your goal isn't like, yeah, your, your goal is like the, ultimately the 
growth and not like the, the low level things you want to do to get there, 
because yeah, it could turn out that it's more expensive than you thought, or 
not as effective as you thought. Yeah, exactly. 

[00:44:47] **Michaela:** So I want to come some to something back and probably 
my last question for you, and this was when we were talking about code reviews 
and you were talking about culture and you said, I'm pretty good at influencing 
culture.

Yeah, so I want to know how, how are you good in influencing culture? How did 
you influence culture at Microsoft or Google? I mean, these are large 
organizations and, and yeah, I would say pretty hard to influence, right? I 
mean, probably a little bit on your team, but how do you, how do you go about 
influencing culture there?

If you see, well, you know, cultures could be improved or done differently, how 
do you do that on a. 

[00:45:25] **Michael:** Yeah, it's, it's something I didn't realize I was good 
at until like pretty, maybe like 10 or 15 years into my career, but I, I think I 
was kind of doing it accidentally. So the first thing I think is important to do 
when you join a, so I'm, I'm good at influencing culture, like on my team.

I'm not good at like influencing the C of Google to do what I want, but I, I, I 
think I was. , I was historically pretty good at like getting people to invest 
more in code maintenance stuff, like getting people to invest more in code 
reviews and testability and maintainability and stuff. So the way I found that's 
effective to do that is when you join a new team, it took me a, a long time to 
realize this, but the first thing you should do is shut up and just listen to 
other people and just kind of find out like what the dynamics of the team are.

Problems people are having. Cuz if you come in with a lot of opinions and you're 
saying like, oh you do code reviews like this, like I think you should be doing 
'em like this. You're now like the annoying one that's like, thinks they can 
boss everybody around without really proving themselves. So I think like the 
first thing you have to do is just.

kind of figure out the dynamics of the team and like understand who has, who has 
influence on the team, like what the pain points are that people feel. Because 
if you're somebody who's like a code review zealot, but everybody on the team 
like really hates code reviews, then your first battle probably shouldn't be 
code reviews.

Mm-hmm. . And then I think the next thing that's important to do is do something 
like make a contribution to the team in the domain of, of things that you care 
about. Is sort of like indisputably valuable. And so one of the things that I 
would often do when starting on a new team is to write new hire documentation.

So I'd say like, Hey, I'm like ramping up. Like is it okay if I write 
documentation just. Outlining all the things that a new team member has to do. 
And like, it's pretty hard to say no to that. Like, why you, you expect to hire 
more people? So like that's obviously a good thing. And also like when you join 
a team, people don't really expect you to do that much cuz it's like, oh yeah, 
they're, they're still ramping up.

And so like, if they see that you're spending time writing the ramp up 
documentation, that's very valuable. And it's like, okay, like this is a person. 
Like isn't invested in helping the team mm-hmm. , they're gonna do things more 
valuable. And then after that, like I think a few months in, you can start to to 
think about like, okay, like what are, what's like a low risk thing that I can 
contribute?

So like, Redoing the code. Like if there's no code of reviews and you're like, 
everybody has to do code of reviews, like that's a pretty big risk. So you 
probably don't wanna start with that, but something like, oh, we don't have 
continuous integration. Like, let's add continuous integration. Cuz that's like, 
there's not a lot of ways that that, I mean there are ways that can go badly, 
but like usually it has a, a really high amount of value and like people are 
gonna see that.

Mm-hmm. . And so I think like during this process, you, I dunno if you've ever 
heard the term social currency, but it's like, , you're making yourself valuable 
to the team and like making it like, so that you seem like a credible person, so 
that later on when you're recommending things that are more risky, that people 
are gonna have more trust in you cuz you have this track record of delivering 
things that have been valuable to the team.

Yeah. And then I think like a, a few months in when you, you've had this track 
record of like, okay, you've had like a few small bets or like a, a few low, low 
risk things benefited the team, then you can start pushing something that's like 
a little bit more controversial. So a, a thing that I. often do it.

Google is push teams to do design reviews because like a lot of teams didn't 
take design. They would, they would take code reviews very seriously, but they 
didn't take design reviews very seriously. And I think there's a lot more bang 
for your buck in reviewing design documents. And so, but everybody hates design 
documents, so that like that's a thing you need a lot of social currency to push 
for.

And I think with that it's like very important. Take time together. Everybody's 
feedback and say like, okay, like what should, like, it's not, you just decided 
something and you're pushing it on your team to influence culture. It's like, 
what? What do we all collectively want out of this process? Like what?

What value do we expect to get from it? What do we have to invest to, to get 
that value? And then I think it's also important to like, keep the team 
involved. So like, okay, here's the, I've, I've written this process, like how 
do people feel about this? And then like, once you've been doing it for a few 
months to like schedule another review.

Like, okay, we've been doing design reviews, like how do people feel like it's 
going? Like what, what are the things that we can improve in that process? 
Mm-hmm. . So those are things like, I've, I've found that are, are very useful 
for getting credibility and like being able to influence the. . 

[00:49:44] **Michaela:** Yeah. And, and so when I listen to what you explained 
is there's the social aspect, right?

That you're Yeah. Getting credibility, that you are getting points with your, 
with your team, that they're trusting you. Yeah. But also it seemed to me that 
you were talking about things first that you can do, right? So it's on your 
shoulders. Right? And then when you actually ask them also to contribute, 
because you can't, you know, you, you can be the only person that sets up the C 
I C D probably, right?

So that's exactly. , that's your extra hours that you're maybe putting on. But 
then if you want them to review the sign documents, right, it's, it's not you. 
Right? It's, it's not useful if it's only you. So you have to ask others. Is 
that also this gradual thing that first I'm investing my time and then I'm 
thinking more of, can I ask others to contribute time as well to 

[00:50:27] **Michael:** something?

Yeah, definitely. That's a great point. Yeah. Like, I think. as you're like 
accruing social currency. Like part of that is being able to get people to, to 
take time themselves because Yeah, like with, with new hire document or ci, it's 
like, okay, sure you can do that. Like, it costs me nothing and like, yeah, it 
doesn't really seem like there's a downside.

And then yeah, things like, oh, we should change our code of views, or we should 
change our design reviews. Then it's like, okay, well now you're asking me to do 
something. Like, do, do you, do you have credibility? Do you have credit on the 
team where like, I wanna take this risk with. . Yeah. And then 

[00:51:00] **Michaela:** also I wonder if, if I say, well, let's say I'm writing 
this new hire document.

Okay, maybe this is something that you really, you already have to go through 
it, so it's really hard to say no. Yeah. But maybe for C I C D I can see that 
people say, oh, you know, rather or not, do it, focus on this. Yeah. Are you 
done doing that outside in your own time or do you, do you ask for permissions 
to do it on your, you know, work time?

Do you want people to see that as a positive contribution to, to, to your, you 
know, to your career or to your performance? Yeah. 

[00:51:31] **Michael:** I, I think when I get re like early on when I get 
resistance, I try to figure out okay, like what's, I don't wanna like battle on 
something early on, so I try to figure out like, okay, like you don't like ci.

Like is there something else? Like maybe reducing our alerts. Like is that 
something that you think would be vi like, is that mm-hmm. worth me investing 
time into. Yeah, like I think you could also set it up like try to do it anyway 
and like show this like you normally 

[00:51:55] **Michaela:** you are looking for buy-in, right? So even though 
you're investing your time, you're looking for buy-in, right?

So you're asking around and seeing if people are seeing that as valuable as 
well, right? Yeah, 

[00:52:05] **Michael:** definitely. 

[00:52:06] **Michaela:** Yeah. Yeah, yeah. Cool. So Michael, I had really good 
time talking to you. Thank you so much for sharing it. A lot of fun. Yeah. 
Sharing all your insights about testing code reviews. Yeah. Also 
entrepreneurship a little bit.

I will obviously link all your cool stuff, but is there something else that you 
think are is important for my 

[00:52:26] **Michael:** listeners? No, you can follow me. My blog is mt lynch.io 
and I'm on Twitter at Deliberate Coder. Very 

[00:52:33] **Michaela:** cool. Yeah. I will link everything in the show notes. 
Thank you so much, Michael, for being on my show.

Thanks, Mikayla. Yeah, thank you. Bye. This was another episode of the Software 
Engineering Unlocked Podcast. If you enjoyed the episode, please help me spread 
the word about the podcast. Send the episode to a friend via email, Twitter, 
LinkedIn. Well, whatever messaging system you use, or give it a positive review 
on your favorite podcasting platforms such as Spotify or it.

This would mean really a lot to me. So thank you for listening. Don't forget to 
subscribe and I will talk to you in two weeks. Bye.


