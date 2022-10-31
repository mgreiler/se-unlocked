---
episode: "Transcript Episode 32 with Nader Dabit Ready"
permalink: /serverless-competitive-advantage
status: publish
type: transcript
---

**Michaela:** [00:00:00] Hello, and welcome to the software engineering unlocked 
podcast. I'm your host, Dr. McKayla, and today I have the pleasure to talk to 
Nader Dabit, a senior developer advocate at AWS. 
But before I start, let me tell you something about coincidence. Sometimes the 
right things come at the right time, I believe. Three weeks ago, the founders of 
CodeSubmit, a take-home assignment platform, reached out to me to sponsor the 
podcast.
They showed me the hiring tool and I was really impressed. So, we made the deal. 
But do you know what happened at the same time? I started to work with a startup 
where I need to hire a team of engineers. So, this week I used CodeSubmit to 
create a custom-made system design task. The best part - from my perspective - 
of the tool is that it natively integrates with Git, it's super intuitive, and 
it allows you to give the candidates great flexibility for choosing when to work 
on a task but at the same time, you can specify a time limit for how long they 
can actively work on it. The UI and the look and feel are so slick. And yeah, I 
will report on the candidates' experience in a bit.
But for now, if you're also in need of a take-home assignment platform to 
streamline your hiring process, please have a look at codesubmit.io.
They also offer a free trial. But now, back to Nader.
Nader is a web and mobile developer who specializes in building cross-platform 
and cloud-enabled applications.
Right now, he works at Amazon web services where he develops features in the 
client team and improves developer experiences for client side SDKs. Before he 
founded his own training company, specializing on React Native and trained 
engineers from organizations such as Microsoft, Amazon, the US Army, and many, 
many more.
If you work with technologies like AWS or serverless, you definitely came across 
his writing, his videos or even his book. So, I'm super excited to have Nader 
here with me today. 
Nader, welcome to the show. 

**Nader:** [00:02:00] Thank you. Thank you so much for the great introduction 
and thank you for having me. I'm excited to be here.

**Michaela:** [00:02:05] Yeah, I'm really happy that you're here. So Nader, 
wherever I look right, be it on Twitter, GitHub, YouTube, Dev.to, you are super 
active on all of those platforms and also you have a huge following of each of 
them. How did that start and were there also times that you were writing blog 
posts or making videos or implementing some stuff and hardly anybody saw it,
or how did you break out of the unknown?
How was that for you?

**Nader:**[00:02:32] Yeah, absolutely. So, I mean, I really started my whole 
social media and I guess outbound presence about four and a half years ago I 
think I would say. I was working at a company called SchoolStatus and 
it's a small startup here in Mississippi where I still live at the moment.
I was starting to become very active in the community 
in the sense that I was following people, I wasn't really active myself 
but I was getting to know the people in the community and I was starting to go 
to conferences and, I did run a meetup for a little bit. So, a lot of the people 
that I was really admiring were often creating blog posts and videos and stuff 
like that.
And I always wanted to kinda get into that. So, I think the first blog 
post I ever wrote was a introduction to webpack. And the reason that I wrote 
it, I was waiting to find something interesting to write about. But I 
always felt like my ideas were not interesting and that someone else knew 
something more than me, still get that feeling now; but anyway, that's a different 
subject. But basically, when I was trying to build out a webpack configuration, 
I couldn't find really good documentation on how to do it. 
So I started piecing together things that I found, and I ended up
building out my webpack configuration and building my app. And I thought, you
know what, this would be really helpful for people I think. Because if I had
found this exact writeup, it would have helped me a lot. So let me go ahead and
create that. So that was my first blog post ever. And it actually
really encouraged me to write a lot more after that, because it just
happened to do really well.
I wrote on Medium when Medium was still one of the most popular 
places, I guess, for developers right. Now I think people are, 
all over the place, but it did pretty well and it was very encouraging. And yes, 
after that, I've had posts that get like zero to a hundred views. So it's 
hit or miss. Even if you have a massive following, if you have 10 times as many
followers as I do, or if you have 10 followers, a lot of times it doesn't really
matter.  I think the content itself matters the most, and like if you're creating
something that is going to help people. Of course, having like a lot of people
to share with helps boost that at first. But I think over time it will do well
regardless if you kind of create something that is really unique and interesting
and actually is helpful.

**Michaela:** [00:04:47] Yeah. Yeah, I definitely think so. I mean one of the 
things that I, I'm learning Python since almost two years now, and I'm coming 
from a Java or a C-sharp background right. So very object oriented and just a 
different flavor and different style of thinking.
And I'm actually really having a hard time finding resources for Python that
help me grow, right. Either it's really basic and I know the syntax and know how 
to do that but I'm missing how to do the architecture of a Python application. And 
I've built large Python applications already, but I am still like oh, there must 
be better ways to do this. And so, right now, for example, I'm tinkering around 
with this idea, maybe I should write some of those resources, because I feel they 
are not there. But it's really scary to write that if there is nothing that you can 
fall back and say there is no true or wrong. Especially, I mean here we are going a 
little bit away from "Does it work or doesn't it work?" because how you structure 
applications is a little bit up to you (laugh). There's no, "This is how we have to 
do it". But how is that for you? If you're developing something or writing something 
that hasn't been done or hasn't been done in that way. I feel there's a little bit 
of risk. And for me, it holds me a little bit back to, you know feel confident 
enough that, well, I know enough of Python and I made enough applications and 
architecture that I have something to say. And I am mainly thinking about, I have 
maybe something to say for people that came from a Java background right, like this
niche of people. But how is that for you?

**Nader:**[00:06:27] Yeah, absolutely. I mean, even today I still get that 
feeling, but I think the interesting thing about technology is that it's not
like math, where there is a right and wrong answer. A lot of times there are just
you know, there are best practices, but a lot of times you can see someone that's 
extremely successful or two people that are extremely successful.  They can both have
completely different opinions. And when you realize that it starts opening the
door for, in my opinion, to kinda have a little more confidence and be able to kind 
of put yourself out there and share your ideas. And sometimes you'll be completely wrong. 
I mean I've created posts and I've said things in the past based on what I thought was
right. And I've had experts chime in and say, "Hey, you're completely
wrong". And I think that it's not the greatest feeling when you're kind of trying to
like teach other people when something like that happens, but it's also a good
feeling because you can then go back and update you know what you wrote and have that
best practice there. And then over time we are just learning more. But I think
one of the hardest things about creating, you know anything is the fear of being
criticized. And some of that criticism could be us being afraid that we say the
wrong thing. And I think being able to kind of feel comfortable being wrong is a big
barrier to overcome to be able to be successful like if you're a quote
unquote content creator. So for me, it was hard for me to  overcome that at first.
And I think you'll still feel it, even as you become more and more comfortable, but 
it will still linger I think.

**Michaela:** [00:07:56] Yeah, I think so too. And I think it really has to do 
with this humbleness. And maybe what I try often to do is to have this learning
perspective in my writing, in my things that I create. And now I started
streaming on Twitch and it's the same thing here. I was really afraid, but I
really try to go into that with this learning angle, where I say, "Oh, I'm new
here, I really don't know what I'm doing". And this somehow lowers the barrier a
little bit for me, or at least I feel like more confident to share the things
because I set the stage for "Well, I'm not an expert here right, I'm just sharing
my story if you want to listen. And if you think I have, you know something 
interesting to say, I'm happy, but obviously, you know, feel free (laugh) to do 
something else". So you were talking about being a teacher and I think this goes
maybe a little bit back to this part of your career where you actually were a 
trainer right? So you trained engineers at large organizations and probably also 
small organizations. So many engineers for, for example, React Native. 
How, how did that happen? How did you start this company, this training company? 
And how did that actually go?

**Nader:**[00:09:07] Yes. So I did training and consulting for about year and a 
half. And I was in between you know, it happened when I ran that company in between 
where I'm now, where I was before. So I was at a startup as an engineer, today I'm a
senior developer advocate at AWS. And in between these two jobs, I was running
my own company and I actually still have that company. And I still have a little
bit of revenue coming in from contractors that kinda of, that get leads through that 
company. But it kind of happened organically I would say. The whole, you know, the 
whole training industry to me is extremely, extremely interesting. And it's changed 
a lot, I think, of course, since COVID happened because a lot of the higher priced 
trainings were like onsite trainings, where you would come and do you know, work with 
the team on site. But I do know of some companies that are actually still able to do
some pretty high value trainings remotely and still get a decent amount of money 
for those trainings. But the way that I kind of got into it was, the React Native
ecosystem is kind of what I was specializing in. And when React Native first
came out, I was one of, or my company was one of the first companies to
actually build and deploy a React Native app to the app store. And I was
fortunate enough to be on the team that built that or actually I was the main
developer behind that app. So in the first few months after React Native came
out, I was, you know learning React Native and I was all into the documentation,
but also on Stack Overflow, asking questions and also answering questions. 
And I think that whole process of getting in really early on that technology and
learning it and helping other people with it, it kind of helped lay the groundwork
for me to kind of brand myself as a specialist. And I think when you brand 
yourself as a specialist in any technology; this is kind of what I learned 
during this whole process. It's much easier to kind of grow and create a training
slash consulting company. So when I was doing all of this work with React Native, 
I built a reputation on Stack Overflow for answering questions, and I became one 
of the top people there within that tech and what ends up happening is actual
recruiters, companies, and people go on to Stack Overflow to actually find
people to work with. So I started getting contacted by a lot of different people
within the industry asking me to do consulting, just organically. And the
consulting that was coming in was actually paying a lot more than my full-time
job. I was making, you know, a very low end developer salary actually at the time, 
because I was working at a startup in Mississippi. It's nothing like a salary, 
of East or West coast, especially. So, when I started doing this consulting a little
bit, I started realizing, okay, I'm going to make a lot more money doing this
than working for the startup. So I was like, I'm going to really try to make
this thing happen. So I built a website for React Native training because I had
a couple of training gigs that came to me and I actually would take my vacation
days to go do these trainings. And they were, I would make more money in one or 
two days than I would in the entire month or two. So I was, you know, really 
wanting this to happen. And I was okay. 
So I built this website called React Native training. It was just a single page 
written with jQuery and HTML and CSS, nothing fancy. And I started just getting a 
ton of leads coming in from that and landed a really big contract. That was the 
one big contract that kind of enabled me to quit my job. So I took that contract, 
quit my job, and I did that full-time for about a year, maybe year and a half. 
And it was really exciting time in my career because I was really, that was kind 
of when I moved, I would say from being kind of unknown in the community to kind 
of being a little bit more well known just because I was able to network with so 
many people and focus a lot of my time on building, you know, relationships and 
stuff like that. So during that year, year and a half, I did nothing but training 
consulting and grew my following on Twitter and stuff like that a little bit and, 
you know, learned a lot about consulting and it was a really interesting learning
experience because I learned that there are things that I really liked about, 
about it. And there are things that I really disliked about it, but I think the 
one thing that I learned is that I didn't know what I was doing at all. And if 
I had kind of known, you know how to run a business, I would've maybe stayed 
doing it and maybe been a little happier. But by the end of that year, I was just 
kind of miserable. I had as much work as I wanted coming in, but I was overworking 
myself to the point where I was working like seven days a week, traveling all the time 
and the opportunity to work with AWS came around and I was able to kind of like 
look at it as a way to kinf of take my foot off the gas a little bit, and also learn 
new technologies and almost kind of get paid to learn those because, at AWS, I'm 
learning so much, but I'm still getting paid. Whereas when you're training and 
consulting, you're expected to be the specialist and you can't really take your
time to learn anything new that's outside of that, because then you kind of are
almost taking money out of your own pocket and it starts becoming this whole
psychological thing that messes with you. At least it did for me. So that was kind 
of my story, I guess.

**Michaela:** [00:14:14] Okay. Yeah. That sounds really interesting. And so, you 
were saying some of the things that you really liked and some of the things that
you did not like so much. So what are some of the things that you thought you're
not doing so well or that you didn't like so much? I mean you were touching a 
little bit on it with this you know overworking and chasing a little bit the money
probably as well right. But what are the things that you think if you would do it 
again, that you would have to you know, level up as a businessman, maybe.

**Nader:**[00:14:45] Yeah, I think that the number one thing I did not
do well was scaled the business and the number of leads coming in. 
I think that when I first started, I had no idea around the demand that there 
was for that type of work. And how, if you kind of positioned yourself 
the right way that you can funnel almost all of the leads for people looking for 
a certain thing, because, with SEO and a combination of, 
writing, I read a book called "React Native in Action",
I was able to kind of get a lot of leads for this, specialty. But I 
ended up, I could only work so much and I didn't really know 
how to hire people and do stuff. I did work with a couple of 
contractors, but I didn't do it right. I ended up not really 
having anyone that, that I could consistently rely on.
So I ended up turning away a lot of business and, I was also not that 
good at managing the different contracts that I had. So, I would do a 
training. I would do it. I would, I would also take on some hourly 
consulting and then sometimes one of those consulting contracts would just 
completely drop.
They would be finished and they wouldn't need me anymore. And then I would have 
a massive spike in income and then my income would go down a lot and that 
would kind of stress me out. But I think the main thing that I 
learned was that I needed to be more organized. I need to learn how to work 
better with people.
And I need to learn how to keep up with my paperwork better because I made a lot 
of money, but I didn't pay my taxes. So the next year, I didn't spend it, 
I still had it, but the next year I had a big tax 
bill. So a lot of the money that I thought I'd made, I actually ended up owing
in taxes.
And, if I'd actually maybe expensed my stuff better too. I understand now 
that I could have written a lot of things off that I didn't write off. So 
all types of stuff, I think you could probably look at every mistake in the book 
that someone could possibly make and I probably made that, made those mistakes.

**Michaela:** [00:16:39] Yeah. And, you know, I started my own consultancy and 
training businesses. It's also why I'm so interested in this. A year ago I went
full-time, I did a little bit before also, as you did, but I was still employed
at Microsoft. But a year ago, I quit my job and, started doing this training and
consulting business full-time and I was also really afraid. I'm telling this
story quite often, I was like "Oh, I can't do it". I have to do it MBA first to
actually do it. But then I don't have the time to do that. So I just do it. And
I'm struggling with really similar things.  I'm struggling with sales because I
don't want to do sales.  I don't know how to do sales. So there's really a lot
of procrastination going on. So everybody that finds me just finds me through
organic stuff. So recommendations maybe, word of mouth, my blog and things like
this, but I've never really reached out to anybody and tried to sell them my
services. And then the accounting part as well, I have no idea about it. So I
see a lot of similarities and I think a lot of engineers that are thinking
about, making this start maybe have the same struggle. And yeah, it's really
interesting. I think in one point I have grown in the last year, I've got
better, but I also make hundreds of mistakes in all regards to the business
aspects and everything. Every mistake that you can do probably I also made. And
so then AWS came along and they wanted to work with work with you. They also
were getting to know you through your social presence and your presence on Stack
Overflow, or how did that connection happen here?

**Nader:**[00:18:19] So I think the first connection happened on Twitter.
I kind of connected or just met with someone based on a tweet that had gone out
that they were kind of engaging with another company. And it was having to do
with mobile development. And I was like, "Oh, I wanna, I want to do this thing,
but do it with React Native" because you know, that was my thing.  And somehow,
we ended up DM-ing each other and meeting, and then a few months later I was
going to be in Seattle, doing a training at Amazon anyway. So the guy that
reached out to me worked at AWS. So I was like, "Hey, I'm going to be in town"
And he was like, "Okay, there's meetups or come hang out".  So I decided to go
to there, to the meetup. And I hung out with them at the meetup. And I met who
is now my manager. And they were telling me about the project that I'm working
on now. And they were saying that they were building out some React Native
prototype, and it's going to be open source and "Hey, why don't you check it
out?".  So I was like, "Okay, cool". So I went back home. A few days later, I
checked it out and I worked with the engineer on that team remotely and kind of
just contributed their open source for free really, but also learning the
technology out there that they were going to be building out.  So during that
process of helping them I ended up adding, a pretty decent feature, I think, to
what they were building out. And based on that relationship, they then reached
out to me a few weeks later and they're like, "Hey, we're hiring for this
position and we think you'd be a good fit".  And I actually was almost a hundred
percent against it.  I told my wife about it, I was like, "Yeah, this is cool,
but I'm working for myself and it's a little less money". Believe it or not, it
was a lot of money, but it was less money that I was making. And I was like,
"Yeah, I don't think I'm going to take it".  And they were like "Look, just fly
out to Seattle, have an interview. We want to tell you more, we think you'll
like it". So I gave it some thought and I started weighing everything and I was
thinking how it would be nice to actually be not held accountable for myself, to
be able to have weekends off all the things that I weren't doing and not have to
rely on myself for a little bit. So I was like, "Okay, let me go out there". So
I flew out to Seattle and I met with the team and the things that they were
working on were extremely, extremely interesting to me and really was a perfect
fit for where I think I wanted my career to go anyway, because I was really
focusing on front-end and mobile development, but I didn't know a lot about
back-end development and the things that they were building were exactly for
people like me that were new to cloud computing.  And they just were really,
really interesting to me. So the opportunity to actually be on this team and a
lot of the people that I met were just really, really smart and I'm always drawn
to work with those types of people. So I was like, "Okay, cool". So they gave me
the offer and the offer was good.  So I was like, "You know what, let's just do
this". So I took the job and it's actually been probably one of the better
decisions I've ever made. I think.

**Michaela:** [00:21:17] Yeah, it sounds really cool. And so when you were 
flying you in for this interview, was this more like a persuasion interview
where they try to convince you that you should start, or did you have until,
after even writing, some major contributions in open source and your presence
and the trainings, did you still have to prove yourself in the interview
process?  Or how did that, go?

**Nader:**[00:21:41] Yeah, it was a real interview process, but I also
got to see the office and meet a few of the people on the team. And there was
the typical five-step Amazon interview and there was a technical interview and I
didn't do that good on the technical interview from what I understand, but I did
do really well on all the other ones.  And I did well enough, I guess, for them
to throw the dice on me, but I did have the regular interview process. Yeah.

**Michaela:** [00:22:05] Okay. Yeah, this is really stunning for me. If they 
really want a person and then they still send them through this, well, probably
very consolidated process.  Right. So nobody can go around it. Okay. So yeah,
what's really interesting to me as well is, if you could tell me a little bit
about serverless because this is your specialty, I understand. And you thought
this is super interesting to you because you were not familiar with the backend
so much.  You were really focusing on the front end. And so you said it's
technology that enables you or front end developers to actually ride full-stack
applications. And this is also what I read some of your blog posts for this
interview today, to be ready. And this is also what I read in this blog post
about full stack serverless, right?  Where you have, we have actually the
infrastructure as code and you have the backend actually as services that people
can just consume. But if you have to explain it, what is serverless, who can use
it and why is it so powerful?

**Nader:**[00:23:11] Yeah, so serverless and, and, you know, the early days I 
think was just basically the idea of functions as a service.
And I think it's kind of grown now to be more of like a philosophy around how 
you build infrastructure and how you build services. And I think if you asked 
me. Like today with the definition of serverless is I would say it kind of 
encompasses a couple of things. Uh, one is like not managing your own 
infrastructure.
Two is paying for the compute time versus the compute power, and basically being 
able to rely on someone else for the infrastructure to always be running. And 
also the last thing is the ability to scale up and down without having to also 
manage that, that functionality yourself. So basically buying into.
Services and anything, any API APIs and things like that that are built and 
maintained by someone else, but that are still configurable enough for you to 
actually get the work done that you need for, for your app or your, you know, 
your company. So I think that what you're basically, the thing that's really 
interesting to me is like, You know, I talk about serverless a lot, but I think 
what you're seeing in the whole cloud computing industry is that a lot of the 
things that were considered cloud are kind of moving to be more into the 
serverless paradigm.
So, so even if you look at kind of re-invent happened this week, there were a 
lot more, you know, things that were, that were released that kind of enhanced 
serverless. So for instance, Services like that, like Amazon, Aurora, they, 
which is basically a Postgres or an RDS relational database service, they're 
making that serverless.
So in, instead of having to kind of like scale up and scale this down yourself, 
you can just, you know, have an instance and everything scales up and down for 
you. So I think the idea of being able to kind of have a lot more. You know, 
powerful services on the backend that you don't have to deal with yourself, that 
you can just kind of buy into whenever you need them and focus on mainly the 
business logic that kind of differentiates what you're building from everyone 
else.
And when you kind of are able to focus less time on things that can be 
abstracted away, you're able to iterate faster. You're able to, to. Do things 
like experimentation, which will also set you set you apart, because let's say 
you want to build out a new feature and you have two options. Either build 
everything from scratch, and it might take you four weeks or take advantage of 
some managed services.
And it's going to take you one week, the companies and the teams that are using 
the things that are more. That gives you more velocity. I think our fairing 
better. And also the, if you, if you think about the engineering cost that goes 
behind it, building things from scratch versus paying for something, you know, 
the usage is there.
It just makes a lot more sense. I think for a lot of companies in my neck and 
might not make sense for like a billion dollar company, you know, but if you're 
a startup or even like, you know, a 10 or 20 million revenue company, Being able 
to kind of experiment without having to pay for it until you hit some type of 
scale is actually, it just makes a lot of sense, you know, especially as 
engineering costs continues to go up because developer costs is going up.
So any way to kind of cut costs down by having less developers is always a good 
thing. 

**Michaela:** [00:26:22] Yeah. I have so many thoughts to this topic, right? So 
one, one of them is I. I see such a connection with the no-code movement and at 
the same time, right. I also see such a connection to this problem that we are 
having or facing, or maybe it's not a problem.
Just that evolution that we are having in technology, that technology becomes 
more and more complex. Right. Uh, and we were talking about this being an 
expert. He said, well, I was an expert. I was specializing in react native 
nowadays, you cannot be an expert in everything anymore. Right. So you have two 
bigger paddles and say, well, I know, I know, react native really well, or I 
know view really well, or, you know, I know Python really well or maybe tie it 
in with some frameworks, but it's very, I mean, there are.
I don't know any buddy anymore, right. That has several frameworks. And then 
even, you know, have technologies and, you know, uh Coopernetics and whatnot, 
right. That you have this knowledge for everything. And so I think serverless 
here, it becomes also really powerful because you have some parts. That are 
developed by somebody that is specializing or knows exactly their stuff, right.
Their technologies what's needed for, for example, the service that you're, that 
you need. And you can somehow outsource that. Then you can concentrate on the 
important stuff that you have to develop and also train your people internally 
so that they have enough knowledge to really, you know, build a scalable 
maintainable solution.
What are your thoughts here? 

**Nader:**[00:27:52] Yeah, I think it makes a lot of sense in that comparison. I 
mean, what, what essentially serverless is, is just another obstruction, you 
know, on top of things that we've been doing. And it's kind of just a name that 
people are throwing out there and it actually works in my opinion, people 
criticize calling this or that serverless.
But I think when you start thinking of it less as like a thing and more of like 
a philosophy, the serverless philosophy, or maybe even kind of. A variance of 
serverless. So you can be more or less serverless. So if your, if your 
infrastructure is completely managed, then you're completely serverless. But if 
you use maybe servers that you need certain things that you have to deal with 
yourself, then you're less serverless.
I think, you know, What you're seeing is a lot of companies that, like I 
mentioned earlier are having to deal with constraints like monetary constraints. 
Like they don't have a ton of money. So when you're working with a serverless, 
you're able to iterate faster, have less engineers and, and. Come to market 
faster and just be able to build quicker.
So you're able to, to do that with less money. And also when you're having to 
compete with other companies that are maybe in the same space as you, you have 
this idea of opportunity costs. So being able to come to market quicker, 
serverless kind of allows up and, and things like that. 

**Michaela:** [00:29:08] So, if you would allow, let's say we are really 
starting from scratch here, right?
We are a young company. We have like an idea often of a service of business that 
we want to develop. We want to develop our MVP. How does serverless shape our 
architecture of this MVP? How would we go about, you know, understanding what 
should be, you know, a service, what should we, you know, Keep in-house can we 
just, you know, outsource everything.
I mean, some of the things that come to my mind definitely is authentication, 
which is complex. And we could somehow, you know, get that out of the door, but 
what are other things, the examples that we would get in and how would we even 
tackle this problem of development? MVP, if you want to use serverless 

**Nader:**[00:29:49] technologies.
Yeah, I think authentication is actually like a really great example because if 
you think about it, when you're working with something from scratch, you're, 
you're then competing essentially against these services that are also out 
there. So we have with something like OD zero or Octa or Amazon Cognito, you 
have teams of people, specialized engineers that have spent years.
Focusing on the single problem cares the single problem area. And they've spent 
all this time tackling all these edge cases. Do you think that your team can 
build something that will compete with them? And if so, maybe there, there is a 
situations like that because maybe you have some really, you know, specific.
Thing that's happening in your system that, that doesn't maybe work well with 
these, but for the most part, when you look at it like that, you can kind of buy 
all of this expertise, like as a service. And also it's usually more secure when 
you're thinking of things like that. But the way I would look at like a new app.
Is, you know, I would kind of typically say, okay, let's list out all of the 
functionality that we need. And then we take that functionality and we kind of 
say, okay, how can we make this happen with managed services or with several of 
our functions as a service with some type of database backends. And we'll take 
all of those features and we'll plug those all there.
And if there's anything left over, then that's kind of where you would. Then 
manage that yourself. And I think like by your it's essentially a server-less 
first approach. So anything that can be serverless, try to make it serverless, 
try to fit that into either managed service or build it using functions as a 
service with some type of database persistence layer, and then whatever's left 
over then that would be what you end up managing yourself.
And I think that's kind of a good, a good way to go about it. 

**Michaela:** [00:31:32] And so if we are having those services, let's say for 
example, altercation is, I think it's a really good example, but on the other 
hand is like maybe overused example. Can you give me one other example of what 
we could, what we could, for example, use it as a serverless 

**Nader:**[00:31:47] service.
Absolutely. I think a really big one is the, well there's two really big ones. 
Actually. I think storage is, is, I mean, Amazon S3 is just massively, massively 
used and adopted, and that is a service. It's just a place that you can drop a 
video. It's like a file service almost right. You can drop videos, you can drop 
images, PDFs, and you can retrieve them.
And it's a lot faster and a lot more efficient, a lot more secure than making 
these in turning these files into binary and trying to store them in your 
database. Right. And then there's all of these. Security systems that are built 
around it, that kind of make it. Make it even more secure than something that 
most people could build.
So I think storage file stores with S3 and other similar services, you know, 
outside of AWS are good, a good, you know, a good example. And then the other 
are API services. So the two biggest ones that AWS are Amazon API gateway and 
AWS app sync, but there's others, you know, think of all these other managed 
services like Sera.
Like, you know, I there's a million of them. I can't really like, I guess 
Firebase could even be kind of considered that, right? These are like API slash 
data services where you have like an API layer that is managed by someone else. 
But all of the traffic coming in to that API layer can then be redirected 
wherever you'd like it to be.
So this request goes to this database. This request goes to this function. This 
request goes to the CC two instance, whatever, and the API services managed for 
you. And the only thing you're dealing with is actually the business logic. 
Yeah. 

**Michaela:** [00:33:15] And so how would you, how would you implement that? 
Would you just implemented directly or would you have like a abstraction layer 
in between so that you actually can change services or, or, you know, serverless 
functions or something like that?

**Nader:**[00:33:29] I think like when you're buying into these types of things, 
then you're, you, you are somewhat, you know, tied into or locked into those. So 
I think it, it's kind of, you know, when people are typically building in this 
way, they are, I guess, weighing the different trade-offs that they have. So I 
think when you're, when you're doing something like this, you're some somewhat 
tied into that, to that system.
So for instance, I think a lot of. New customers are using stuff, or they're at 
least evaluating stuff like graph QL with app sync, because a lot of the apps 
that are modern or basically, you know, interacting with a bunch of different 
clients. So you don't just have a web app. Now you typically have a web app and 
mobile app, right.
But you don't want to build separate end points for each one of those different 
apps. So using graph QL, you can have a single endpoint and for, you know, your 
mobile devices, you might want to fetch a lot less data for. For you to have 
better performance, but on your, your web app, you, you know, you can assume 
that they have a better connection and more power.
So you might fetch more data plus to have a larger screen with graph QL, you can 
just have like the single entry point and be able to just ask for exactly the 
data you need and things like that. So, 

**Michaela:** [00:34:41] Yeah. And it makes sense. Yeah. And so you you're 
writing books like you don't have like one book you have, like at least two, 
maybe you have more, I dunno, but the two that I have seen, how are you going 
about that?
And especially if now staying with whichever and for example, full stack 
serverless, right? How, how do you go from idea to have this finished book and 

**Nader:**[00:35:04] yeah. So I have two books. One is a react native and action 
from Manning publications. And the other is full stock serverless from a 
Raleigh. And I think that it was the first book was probably the most 
challenging thing I've ever done.
You know, really, I would say my career as far as like a long-term project, it 
took over a year and a half to write that book because a couple of reasons one 
is. The publisher. I was working with the editor that I had within that 
publisher changed like three or four times. And every time a new editor would 
come in, it took a while for them to get up and running and then they would go 
through my book and then they would give me all these changes and then I'll make 
the changes and then react native changes a lot.
So there would be, then I would have to go back and make more changes. And then 
a new editor. It was just, it was kind of a mess, but it was mainly because of 
the rapidly changing technology that is react native. So. But that process kind 
of was really, you know, it was really, it taught me a lot. Yeah. I think 
because when you're doing something for that long and you know, you stick with 
it and you finally finish it, it feels really good.
And then my next book with, with a Raleigh publications was a lot easier because 
I was able to actually write it a lot faster and get it out there. And then also 
they have a way for me to update it using, uh, get. Which is, you know, what 
would I'm very familiar with? So anytime something changes, we create a new 
version.
We, and we have it ready to publish. But I think that, I think that, you know, 
when you have an idea for a book, there are just so many options now to publish, 
right? You can go with one of these publishers like I did, or you can self 
publish. And I think there's trade-offs to each. I think the reason that I chose 
to write my first book with react native was because I was not really known at 
all.
And I wanted to kind of have a book. And have it published by a known publisher 
because that would give me a little more credibility. And I think that those are 
the types of questions and trade-offs people have to consider. I mean, once you 
get a lot of credibility, you can self publish a lot easier. I think because 
people already know you, but if you're kind of brand new to the community and 
people don't really know you, it's, it is a nice way to earn trust when you're 
working with one of these nine publishers.
But it's just a lot of, uh, A lot of work long long-term, you know, writing, 
but, but a lot of people, you know, find it very fulfilling and you know, 
people, people are putting out some really interesting books lately out there 
I've seen. 

**Michaela:** [00:37:23] Yeah. And why did you choose for the second one? I 
mean, you had already a follower in your were known.
Why did you choose to go again with a publisher? 

**Nader:**[00:37:32] So a Raleigh publications is, you know, a Raleigh is kind 
of what I learned almost like if I read any technical book learning what I know 
now, I would say about 80% of them were a Raleigh. So having the opportunity to 
actually write one was just a really cool opportunity.
And I just wanted to do it mainly because. I have so much respect for a Raleigh 
and I've actually heard a lot of good things about the writing process. So I 
just did it because I thought, I thought that was really cool. It also, it kind 
of feel like the reach that it would get might be a little better with the whole 
platform that they own.
So, yeah, but it could have gone either way. I think for my second book. 

**Michaela:** [00:38:11] Yeah, I can, I can see that. And so did it help, did 
the editor help in the whole process? Did you feel that it actually a better 
book because you had like an editor that was working with you on the book? Yeah, 

**Nader:**[00:38:23] the editing process was really, really seamless and it was 
cool because I was writing, you know, putting my, my pages in, get hub or a good 
provider, like get up.
So anytime that they would make changes, I could just run a good poll and pull 
down the updates. And most of the time they were doing really tedious stuff that 
I didn't really want to do anyway, like grammatical errors and formatting, which 
was really nice. And they did, they did a lot of that. It was pretty painless.

**Michaela:** [00:38:48] Yeah, that's really cool. So one thing that is still in 
my, on my mind is, um, we talked a little bit about when you have like 
serverless and I'm thinking is a little bit like the no-code movement as well, 
right? Where you have like this abstraction layer and you were also saying, well 
authentication, right.
People know so much about authentication. So if you want to do. A similar 
service, how much would that even cost you to, to replicate, right. To do, to 
maintain and everything. So, and one thing that you also said is like code is 
liability, which is, I really think this is so on point as well, but what's 
actually different.
Is it, is it actually the same? It's the no code movement also serverless or is 
that something else and what makes it different from the serverless movement? 

**Nader:**[00:39:35] Yeah, that's a good point. I think they all kind of start 
overlapping, you know, here and there. I think that the, the, the no-code 
movement is really interesting, but I, I would say that you could kind of 
compare several lists in my opinion, closer to like the low code movement or 
like the low code tooling, because what serverless does is it kind of gets rid 
of automated things that you're doing a lot of times.
So for instance, I mentioned the API layer, you know, you have. Oh with back-end 
developers. A lot of times their role is to do a lot of things, but one of those 
things is often to just create API end points and those API end points like 
interact with some database. And I think what you're seeing with a lot of these 
managed backend providers is that they're kind of doing.
You know, that worked for you so you can kind of all flow down and then you can 
give the back end developers more important stuff to do, but with the no code 
movement, you know, I think that when no code succeeds at something, it kind of, 
it just crushes everything. And it just does really well. But, but, but it's 
hard to do certain things with the no code.
So for instance, before we had Wix and before we had these types of tools, you 
know, people that didn't know how to code. There was pretty much no way for them 
to create a website. Now they can do that. But I think for someone to go from 
creating like a marketing website to creating like an app that actually has big 
core business logic, that step seems to be a lot harder to do.
And I think that's where serverless and no-code shine because they automate a 
way, a lot of the tedious stuff and they allow you to kind of just get to the 
core business logic that is kind of differentiating what you want to do versus 
everyone else. 

**Michaela:** [00:41:10] Yeah. I, I, it's definitely the, also like the 
granularity, right?
So with the serverless, you have like really smaller building blocks that you 
black in together. And as you say, it's, it's actually not no code because you 
definitely have to code and it's not even low code. Right. It's probably a, it's 
really cool. 

**Nader:**[00:41:28] I don't know. 

**Michaela:** [00:41:30] Yeah. I don't know where to distinction near comes and 
what is actually called.
Right. A lot of things, even Exley is somehow coding. Right? Yeah. And, and 
yeah, this is how I see it. Right. It's like it's this and weeks and all of that 
are really like these large things, but they're like smaller services. Now we 
have like Sopier for example, or, you know, like where you can have this 
automation off.
Of processes. And I think people are really doing, I, I'm not really too much 
into this no-code movement because I think if you can code, this is maybe the 
default that you do, but I try to, I try to get a little bit into it because I 
feel that I don't want to replicate everything right. And spend my time.
Doing things that I could actually take out of the box. So this is why I'm 
really interested in this no-code. And I also think that serverless is really, 
really interesting because you can save yourself so much time and even, I mean, 
I'm, I'm a solopreneur, right? So it means that every time I'm touching 
something, I really have to think, well, how I'm going to spend my time and how 
I'm going to scale.
And so I think those things can really, can really help here. Yeah. So one of 
the question that comes to my mind, and especially if I watch some of your 
YouTube videos is I feel also the complexity right now with serverless and those 
technologies in general, with our ever evolving technology of base comes a 
little bit from programming to configuration, right?
So like you have to open up your call online, right. And you're. Just installing 
something and I'm sure I hit enter and they will come in ARR and I'm like, Oh my 
God, what I'm going to do? Something is wrong. So I actually struggled quite a 
bit with setting up my environments and all of that. I feel it much easier to 
open up, you know, like it's just a very plain editor and start writing code.
So I feel that a lot of this complexity that we first had in, in writing code is 
now in configuring your environment, knowing how to, you know, install and 
having systems talk to each other. How do you see that? 

**Nader:**[00:43:35] Yeah, I think, I think it's a super interesting topic. And 
I think it's one of the things that we take for granted as developers, as we 
start getting more experienced than we're doing this longer, because a lot of 
the things that these obstructions start doing for us were things that we kind 
of understood anyway, but we're just kind of happy that we don't have to do it 
anymore, but a lot of times.
Those things, you know, need to be tweaked, or you have to kind of understand 
that those things are happening. And then when a new developer comes in, someone 
that's just starting, then they run into these issues and they don't understand 
like why they're running into them. And a lot of times it's because there has 
been something that's obstructed away from them that they don't really see or 
there's nuance.
And that there's so much nuance that, that is there. As you become more familiar 
with how the computers. W, you know, work, the command line works, whatever your 
environment that you're working in works and yeah. And, and, and all of these 
configurations are kind of like, you know, where those things can open up to 
give you an idea of like, what's going, hang on.
And then, and then when you start thinking about, and this is slightly during 
off, so I'm sorry. But when you start thinking about what we were talking about 
earlier with cloud computing and serverless. What you're also seeing is kind of 
the ability to provision infrastructure based on infrastructure as code, which 
is essentially kind of like configuration and.
I think what's really going to be happening over the next few years is that 
people are going to be building a lot more powerful tools on top of 
infrastructure as code and abstracting that away. So I think the tools are going 
to be things like, like seek command line interfaces, but also GUI. So user 
interfaces that allow you to kind of create an infrastructure as code under the 
hood.
One of the really interesting ones that is out there it's called Stackery. They, 
they allow you to kind of. Drag and drop. And then under the hood, they're 
basically creating infrastructure for you. And then the amplify CLI, which we 
work on does the same thing. And then there's a CDK, which kind of does the same 
thing, but it all, yeah, it all comes down to like configuration and when 
you're, and when, and if you're a new developer coming into it and you're using 
the tools like we create, and you don't really know what's going on under there, 
there's only a certain point that you can get to before you need to kind of 
understand what is happening.
So I think there's a big trade off there. Like, yes, it's great for us. For new 
developers, but it's also kind of like a possible area where they can, they can, 
you know, hurt themselves or, or they can just be limited because they're going 
to run into some issue. And they're not going to know why that issue is there.
Whereas someone like us that's been doing it for longer. It may take it for 
granted, unfortunately. 

**Michaela:** [00:46:05] Yeah. I mean, for me, it's always like, uh, back early 
days when I did my bachelor's right. It was, it was databases. You had to 
install like a database and you have to really make sure that everything runs. 
And it was like, Oh my God, this that gonna explode.
And it's, it's like a black box, right? So obviously you can figure out, but it 
takes a lot of time. And, and now I have the same feeling here. Every time I'm 
using a new tool or a new API or something that comes out of the box and that's 
actually a black box, I always feel like, Oh, is that. Is that going to work 
now?
And if it does, I'm like, wow, this was amazing. Often it doesn't. Right. And, 
and as you said, and it's really hard, I think to travel shoot, especially if 
you're new to it, because it's a black box. And so how, how should I know what's 
going on here right now? So, yeah, there's definitely a trade-off and I I'm 
really excited about what you were saying about these tools that we'll build.
On top of that. So how do you envision that will be, will that be extensions of 
the IDE or will that be something separate? You're talking about the AWS CLI, 
right. So this is probably separate from, from the IDE, but could it be also 
part of it or how do you think, which direction will that all go? 

**Nader:**[00:47:22] So I think they just actually based on some very recent 
experience, because we just released actually something on my team this week 
that kind of gave us a very good idea around what people like.
But I mean, what, when, when you go, for instance, you log into something like 
Azure or GCP or AWS and you start creating. Things in the console, you're 
basically provisioning infrastructure, but you're having to do it, you know, in 
this, this user interface. But you're only really able to kind of like do one 
thing, right?
If you want to kind of replicate that there is no way to do that. And when 
you're thinking about like real-world production systems, you typically have 
different environments and you have built processes and you have testing and all 
this other stuff. So you typically need some way to kind of automate that.
And that's kind of like, you know, where infrastructure is code comes, but when 
you're like a new developer or even an experienced developer, you start looking 
at some of the older ways of writing infrastructure's code. If you're using AWS, 
the one that you might think of as confirmation, just to create something pretty 
basic, it's just a lot of boiler plate and there's a lot of.
You know, knowledge that you have to have to kind of make that happen too, 
because you have to know which keys in which values do what, and you have to 
kind of know what options there are. And just for a single service, it might 
take you dozens or even hundreds of lines of code with a lot of things. So 
that's just one thing.
Imagine putting, you know, Five or 10 things together, or a hundred things 
together, which you know, is not uncommon. So what basically all these newer 
tools are kind of doing is they're kind of, they're, they're giving a way to 
kind of go back and forth. So before you either had the option to do in, in, in 
the console, but it was harder to replicate or you could do it in this.
Configuration file, which was hard to get started with. But what if there was a 
visual way to do it that then export that into a configuration file that you 
could then run in some CICB process or just hand off to a new developer and have 
them copy it. I think that's where we're headed. And that's what the amplified 
CLI does.
That's what kind of, what CDK? Well, I wouldn't say that's what CDK does. CDK is 
just another way to kind of do this where you can write TypeScript or Python, 
but I think in the future, what we're going to basically see. Is these graphical 
user interfaces that create infrastructures code that can export, you can modify 
them and then redeploy them.
And then they create that create the infrastructure. So you have kind of this 
back and forth going on and it, and it will, it will vastly lower the barrier to 
entry for people to, for cloud computing, because it will allow them to build 
out these real world production systems without having to know a million things, 
you know, 

**Michaela:** [00:49:58] Yeah.
Yeah, I can see that. So actually I took a lot of time from you already, and I 
think this brings us somehow also to the end of this interview. Is there 
something that you think you want to give my listeners on the way, especially if 
they are interested in serverless, for example, or cloud computing, mobile 
development.

**Nader:**[00:50:20] Um, there are a lot of things I would probably like to 
plug. So let me think about this for a second. I mean, if you're interested, you 
know, in, in cloud computing in general, I would definitely just recommend 
checking out all of the different options that are out there. There's AWS, but 
there's also Google and there's the Azure and they all kind of have their own, 
you know, Communities and they're all pretty cool.
I would probably, you know, I would just encourage to find different people 
within all of those communities and follow them and just look at the stuff that 
they're putting out like creators, you know, people making videos and stuff. I 
don't want to plug anyone in particular because I'm kind of a big fan of a lot 
of different things.
And it's hard for me to just pick one or the other. But I would say, even though 
I work for AWS, I encourage people to look at, look at everything that's out 
there and find what is, you know, Not only interesting to them, but kind of 
what's easy for them or what makes sense to them because I think they all are 
done a little differently and some click better for others than, than others.

**Michaela:** [00:51:20] Yeah. Yeah. Maybe I have a little follow up question 
when you're saying it that way. Do you think that you can let go back to this 
example that I had, we are building our MVP or are we designing our system? Can 
we take servers from here and from there and from over here, or should you stick 
with one provider with one company that's providing those services to 

**Nader:**[00:51:41] you?
I just always say pick the best tool for the job, whatever that is. So for you, 
if that's all with a single cloud provider, then that's great. If, if you want 
to kind of expand and do multiple cloud providers, then if that makes sense for 
you, then do that. I think I'll always, and this is slightly against the 
messaging.
I think that you, that you hear a lot of Toms from cloud companies where they 
kind of say, you know, Multicloud is what they call it. And they say like, don't 
do it, but I'm just kind of the type of person that says do the best tool for 
the job. There's there's someone that I follow. His name is Joe Emison and he's 
actually built and sold multiple companies using serverless technologies is I 
think he's on his third company, right?
Wildly successful, super smart. Um, he, he uses AWS, but he also uses other 
cloud providers for different things that, that, that are done really well, 
that, that you can't really find within AWS. So I'll say find the best tool for 
the job, whatever that is. So that's kind of my take on that. Okay. 

**Michaela:** [00:52:40] Yeah. Thank you so much.
Now there for being on my show, it was really a pleasure to talk with you about 
all these different topics and, and hear you talking about so many things that 
you experienced from, you know, being an entrepreneur, to working at AWS and 
author and blogger tutor, everything. Thank you so much for being here.

**Nader:**[00:52:59] Thank you, Michela. It was really, really nice to be here. 
I appreciate you having me on 

**Michaela:** [00:53:03] thank you so much. Okay. Bye. Bye. I hope you enjoyed 
another episode of the self engineering unlocked podcast. Don't forget to 
subscribe. And I talk to you again in two weeks. 

**Nader:**[00:53:17] Bye.


