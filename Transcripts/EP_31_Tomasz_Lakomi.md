---
episode: "Transcript Episode 31 with Tomasz Łakomy"
permalink: /combatting-tech-debt-in-war-rooms
status: publish
type: transcript
---

**Michaela:**  [00:00:00] Hello, and welcome to today's software engineering unlocked
podcast. I'm your host, dr. McKayla. and today we talk to Thomasz  Łakomy.

Before I start, let me share some fantastic news.
The podcast has gotten its first sponsor. I'm excited as this means will be producing more episodes for you.
Our sponsors are  two founders, Tracy and Dom who recently reached out to me. They are building CodeSubmit, a take home
assignment platform to streamline your tech recruiting. They're already
profitable and part of the TinySeed Accelerator. The reason for coming up with CodeSummit
is because they strongly believe that take home challenges
are the most candidate friendly way of assessing developer talent and since they could not find a dedicated tool for them,they set out to build the
best experience for take home assignments for hiring managers and developers.
It's built on Git and supports 64 different languages and frameworks.Despite being a young startup, and it's built the Indy Way, they already working
with hundreds of companies.
I personally have had a chance to interact with it.It's fantastic and I
really hope you go and check out CodeSubmit. You can find it at https://codesubmit.io.
Oh, there's an offer, a free trial. Well, if you like it, please give them some love
on social media for sponsoring this episode.

Back to Thomasz. Thomasz is a
senior front end engineer at the Alix group, which is a fast-growing platform
for trading businesses.
Commercial is also an ad hack instructor. He's certified for AWS,a
speaker and blogger. I'm  happy to have Thomasz here with me, Thomasz,
welcome to the show.


**Tomasz:**   [00:01:46] Hello, everyone. I'm happy to be here.

**Michaela:**  [00:01:48] So, Thomas, maybe as a start, can you tell me a little
bit about your role at Alix group on the website?
It says it's a platform for buying and selling cars, finding housing, getting
jobs, buying, and selling household goods. But what are your team's
responsibilities? What are your tasks at this company?

**Tomasz:**   [00:02:05] Sure. So, as you've mentioned, like basically what we do at
Olin's group is,buying and selling stuff on different websites
So as you mentioned, we have cars,real estate,goods and
services. So there's obviously a lot of things going on. Thus,my team cannot be responsible for everything. The
way we work at all X group is about each team focusing on a certain area of
the business and own it competently.
My team is focused on all the jobs because not only you can bounce stuff, but also find a better hopeful job at all X.We are building solutions.Helping people find a, you know, a newer better
job in particular, we are working on something called a candidate
profile, because the idea that we have is about,you know, CVS are kind
of outdated because this concept of a CV has been around for, for ages and
we need something better.
To enable people create basically four fires at all X, but we also are
going to use the data in the profile to help locate people. I bet a job
automatically because we send them recommendations based on their profile and
also the face on the job ads that were actually, they were going through on the
other side.
So we are kind of trying to find a better job for them.

**Michaela:**  [00:03:34] Okay. So can I imagine it as like LinkedIn, but a
little bit different or is it very different?

**Tomasz:**   [00:03:41] Is this somewhat different from LinkedIn? I think LinkedIn
has this very, very focused on like white collar jobs. So, you know, white
collar, basically what I mean by that is that, you know, you work in the office,
you probably have a product to probably have a, you know, a title that is in
English and you probably spend your time in front of a computer.
And this is not the reality of like, I suppose like majority of people, because
people have different careers, people have different skill sets and whatnot. So
what we are trying to build is to have a product that is somewhat similar to
LinkedIn as a new, create a profile which you can use to find a better job,
but with a much broader focus.
We want to target basically everyone who is looking for a job in
Poland. And also help them find a better job because like not everybody is used
to, you know, searching for a job, offer online, not everybody's student
negotiating. So one of the experiments that we've had a couple of times, I go,
there's also building a platform in which the employer would have to provide a
salary because we also would like to in ideal a scenario, avoid this process of,
you know, Whenever you have to negotiate a salary, how much do you want?
How much are you willing to give me? How much do you want? And so bucket and so
forth.

**Michaela:**  [00:05:02] Yeah, for me, it's always mind blowing that, you know,
I, to be honest, I haven't known about all ex before. Right. For this
podcast, I researched on it  then went to the website and saw
this large numbers of employees that you have,same thing on
 career side. This is my idea,if they were like 16 open positions in data analysis or
data engineering, something like this,right. Then there would be like 80 positions
for engineers. Right. It's mid-blowing as l have worked as a data scientist
or like a researcher before.
Right. And sometimes struggling, like where are the companies that actually
hiring, you know, people with these skillsets and then you're stumbling across a
company that you never heard of anything like, well, this is not a small
company. It's a large corporation, right. That you're actually working for. And
so, yeah, maybe what would be interesting for me is like, well, you said my
team, right?
So my team, and then you're working with data scientists. What are other
engineers that you're working with? Right. You're a front-end engineer. So who
is on your team? You know, do you have like testers on your team? Do you have
like designers on your team and, and then you're working with data scientists.
How does the communication work like this? Can you tell me a little bit about
the structure and you know, how, how are teams collaborating at all X.

**Tomasz:**   [00:06:13] Sure. So the way we kind of work at all X or X group is,
each team is a park. We are defined, divided into something called
a park and a park is this like self-contained unit of the organization that can
ship their staff to the production.
So each park has, you know, If you need front-end engineers, you have a front
end engineer, you have buckets, engineers you'll have product managers. There's
usually an engineering manager. If there are no engineers on the team, that's
kind of all, it is also useful. Some teams have a dedicated designer, some teams
are working closely with, you know, with the designers, but they're not
necessarily in that team because some teams have like different needs when it
comes to things like design.
We also have a business analyst in our team. So again, like this is a very kind
of self contained unit. What I like about this setup is because I used to work
in the companies where we have, we had a front-end department and we had a
backend and not only was communication tricky, but also working in an actual AI
way was some somewhat difficult because as a front end engineer,getting a piece
data from the backend,would be a challenge.
Then you had to go the backend team, talk to them, but they apparently don't have
the authority for this, for this space. I have to wait for the next bit and
whatnot. Whereas in our current setup, we've worked very closely together. So we
are not working in a silo, but quite the contrary, we are working very closely
together with backend engineers, front end engineers.
All of those skill sets that are required to build amazing products. Everything
is included in that team. And I are very proud as a front end engineer of our
backend engineers, because there are actually submitting a feedback when it
comes to design and when it comes to UX solution that we build it. So this is
honestly,something that I hadn't seen before then.
Just the level of commitment to building. Uh, great products and not only, you
know, juggling Jason data, as some of buckets engineers are used to doing.

**Michaela:**  [00:08:23] Okay. Yeah. And so how many front end engineers are,
for example, in your team?

**Tomasz:**   [00:08:29] those tems, they don't have to be very large. So in my
thing currently, we have two trumpet engineers.
There's two backend engineers. We have a dedicated contact in the data science
team. So he's not technically in our team, but we are working very closely
together. We also have a dedicated designer, a product manager, business
analyst, and my engineer manager. So there's less than 10 people in total. I
like this role that each team should be large enough that a one pizza can fit
the entire theme.
And I think this is not a good metric for how large the teams should be. Yeah, I
like that.

**Michaela:**  [00:09:07] But with 10 people and one pizza, I mean, everybody
gets a little slice. Really?

**Tomasz:**   [00:09:14] Yeah.

**Michaela:**  [00:09:15] Yeah. And so one of the things that I love is code
reviews. If you have like two front end engineers, do you do code reviews
for each other?
Or do you have like the back end engineers also looking at your code? And are
you looking at the code off the back end engineers and visa versa? Or is that
like very dedicated, like for the roles?

**Tomasz:**   [00:09:35] So there there's a couple of things here. First stop. We it's
one of us. Tries to grow. So I am trying my best to kind of review
infrastructure changes.
We are using several of the framework, something bucket the engineers are eager
to take a look into what's happening on front and side, but. The the way it's
usually happens is, but my team is only a smart, small part of a way larger
organization. So we have lots of front-end engineers, backend engineers and
whatnot.
And so, because those teams are self-contained, you may have this impression
that we are working completely alone in a silo. We don't look at what we are
doing. This is usually not the case. So for instance, l am also able to
review their code and whatnot.
I believe this is quite useful because first of all, we do require two
approvals on each request. So by definition, if there are two of us, I cannot
approve my own stuff. I have to get somebody else from another team to also
approve my changes, but it also builds this culture of at least having this
vague idea of what the other teams are doing.
And if should they be uneasy, they can also contribute to the other codebases
and visa versa.

**Michaela:**  [00:10:51] Okay. Yeah, that makes sense. And so now I imagine you
write you like this one pack, and now this is a large corporation or a large
organization. So I'm thinking, well, there's your pack. And then you're
probably.
Maybe 20 other banks or even more. Right? So how do you,select the
pegs that would review your code and would it be obviously the same, you know,
like have you, do you have like two other bags that you are like, you know,
working together or do you randomly allocate people from different packs to look
at your code?

**Tomasz:**   [00:11:21] I would say it depends on the,scope of the changes,
because I am working in a pocket that is, like I said, we are building products
for four jobs. So we are helping people find a better job. There are also other
parks that are also in this kind of like job ecosystem. So there are other
solutions for instance, for recruiters.
So if something, if it might change, is. Or actually in this domain of looking
for a job. So this is like in this part of the code base, or there's this
context of, you know, the stuff that we are actually currently building if
necessary. I am probably going to ask for code review some of the members of
that team, but if I'm doing something that is more like platform related, so I'm
making kind of like core changes.
I don't know, if I'm updating a very major dependency in our code base. I am
probably going to reach out to somebody from our platform team, because a lot of
things that I especially hate as a front end engineer is Bheki for direction.
My goal is as a developer. And the question about testing in general is I
don't want the big production.

**Michaela:**  [00:12:29] So I actually read through one of your articles that
you also have mentioned on LinkedIn is one of the Africans that you are most
proud of. That's most popular, something like this, it's called a seven years as
a software developer, right? The lessons that you have learned there, and you
were talking about culture base again, right?
And so one of the things that you were saying, and I'm just, I'm now quoting you
robot him more or less, right. USA. I've personally seen people submitting code
reviews when X, right, the person wasn't in the office, or why was it a business
trip? X was a brilliant programmer, but enduring through his code reviews
process was a chore.
If you leave 15, eight pigs and comments, and there are PR of someone who is a
junior programmer, you're not proving your superiority as a developer, you are
proving that you're not a good human being. Right. And so. How do you handle
that? Like how, how do you, how do you handle unkind commons and how do you
surface that at, as a company, as a team?
You know, how do you deal with that?

**Tomasz:**   [00:13:33] So, at the beginning, I w I would like to add, but if I were
to write this part again, I would probably add some more new ones with. But that
was the, a bit of a, of a hot steak. And, you know, there were lots of comments
on Reddit, uh, regarding that part, because it seems to kind of cause a little
bit of attention, which I don't think it's necessarily for the book, because the
main point is silver.
You should be kind to other people when it comes to kind of like dealing with
that. I. I think it's not easy and you are, you are probably the best person in
the world to having better cultural views. But nevertheless, I guess my personal
idea is that you should always try to reach out to somebody when there are, for
instance, like kind of comments in photos, because there are two things that
maybe happen.
First of all, they may be, are not aware that their comments are on time. Maybe
they're just trying to be direct. Maybe they didn't have the time to kind of, I
don't know, use the word please in a sentence, which I think it should happen
anyways, but it could also be that something is actually happening in their
personal lives and there are not, or the feeling, you know, like doing code for
this today.
So that's why I'm, that could happen. But nevertheless, I would always reach out
to them and say, by the way, those are kind of like review guidelines. We are
reviewing the code. We are not agreeing with the person. So, you know, please
try to be kind and regarding like bad code, because you know, when you leave
like 50 comments on the cultural cultural view and you are very nitpicky
publishing that this code is terrible.
I like to think that everybody tries to do the job as fast as they possibly can.
Nobody is a developer. Nobody is going to go to work in the morning and says,
I'm going to write some terrible codes today. Nobody does that. So when you are
seeing something in coating you, that you are shocked, that you think is
terrible, consider that you are maybe not aware of their constraints, maybe
there's some context that you are not aware of.
Maybe there's something that should be improved. Maybe you should talk to them.
Maybe if you see a culture of yours, doesn't have any tests whatsoever, maybe
propose to fire off. And those tests together.

**Michaela:**  [00:15:59] Yeah, I like, and you also had that actually in your,
in your blog post, right? You were saying, well, go and change the channel, the
communication channel.
Right. So instead of leaving all those comments in the culture view, why not
reaching out to the person directly and asking, you know, if you can be, as you
said, Of help in a different way. Right. And I think that's really important.
So, and maybe I want to come back to one of the things that you said at the
beginning is like, well, I will definitely reach out, but do you see yourself
reaching out as the person that gets this critique?
Or is it like you're a senior engineer, right. So would you also reach out to
the person if you see they are leaving unkind comments from somebody else?

**Tomasz:**   [00:16:36] I wouldn't be much more quicker to your child if it was, if
it was somebody else for the code, because I have a feeling that. As a, as a
senior in the organization, that your job is not to only write code, but your
job is also make others more productive and also builds an environment in which
people are feeling okay to kind of express their ideas, express their concerns
and whatnot.
So if it doesn't happen for their cause like this, this thing that I've written
about in the article, it happened years ago. Uh, and it doesn't do the, have
them in my current company, which is something that I'm very happy to see. But
nevertheless, if I were to see a situation in which somebody more senior is kind
of attacking a more junior engineer in the cultural view, I would different.
You reach out to, to that reviewer saying this is not okay. This is not
something that we do, because think about it. Some people are not used to
culture. This culture is, are very public. And it doesn't make people excuse
necessarily the good that I am. You know, I've just started at this company two
weeks ago and now I have a bunch of quests with like 50 comments in it.
Maybe I'm a fraud. Maybe I shouldn't be hired through the first place. Like this
is not the kind of environment that you want to build in a software
organization.

**Michaela:**  [00:17:56] Yeah, I think you're talking about a lot of different
things here. And one is for example, that the context that you have when you're
doing code reviews, right?
So this person you were talking about, the person that's just starting, so this
person probably needs something very different in a code review than a person
that's, you know, at the stable at this company already, or have found their
place in this company and the team, for example. And, and so, yeah, you're,
you're totally right.
There are so many different things that influence that. And so when I work with,
with engineers on code reviews and they are telling me those, or, you know,
sometimes people are afraid even to, to tell that, but somehow it surfaces,
right? And they say, well, coffee views is the problem. But I really think it's
not the country is that other problems that the team culture.
So if things like this happen in contributors, then it's not the culture base.
It's the culture is surfacing that. And I think on one hand, this is even. Good
because now you can see it, right. You can see things that are happening in a
more subtle way in meetings and, you know, in work coordinations or
collaborations, you know, who reaches out to whom and how do you give, you know,
orders or things like this.
So in hierarchical organizations, Well, so I know something else that I wanted
to talk with you about and that's technical deck. And so I noted your
organization is doing something a specific year. Can you tell me a little bit,
how are you tackling technical dev and you know, how you're working on it? Do
you say well happens and we never look at it and close our eyes?
Or what are the strategies that you, that you have here?

**Tomasz:**   [00:19:24] Okay. So first of all, if any of that software organization
is saying that they don't have technical depth, they're absolutely lying.
Everybody has technical that including, including us for record. So from my own
perspective, I'm very happy to be in a somewhat Greenfield project.
So we don't have a lot of tech depth. Well, mostly because we are building, you
know, completely new features and functionality on top of existing stack. Bob.
Nevertheless, we are also integrating with something that was certain, that some
of it is definitely technical debt. So there are a couple of things that we have
been doing so far.
You know, the two are just because we have to continue, we have to continue to
develop and we have to continue building, you know, experiences for our users.
We have to be able to do some of the fast and when technical debt is high
enough, you cannot do it anymore. So we having this concept of a wall. And this
is something that we did a bunch of times, and we basically about two types of
worms.
So first up we have those forums where you get together a group of engineers who
are interested in a certain area. So for instance, I don't know, we have
problems with our, this, or we have problems in our front end performance. We've
been together, a group of engineers who are interested in that, and they will be
able to help.
So they would be not like full-time visit on new features and experiences about
some part of the work versus like 50% will it be spent, you know, focusing on
fixing technical debt in order to unlock everybody. But we also had a case in
which we are functioned as the heads just stopped. And we had a, basically like
a company, maybe not necessarily a company wide, but department wide, a worm.
By this, we were not working on anything new for if I remember correctly two
weeks and we did manage to combat in massive portion of our tech debt. And my
takeaway from all of that is you have the activity plan for six executives for
my money. This is not something that happens in the meantime. This is not
because I, I work in on some teams and there was this idea about.
Each sprint, we're going to spend 20% of our time on Tecademics. This are the,
are the words, what I think works so much better is to have dedicated time and
dedicated people who are passionate about, you know, fixing technical depth in
my, in my humble opinion, the best way to address, for instance, like
performance issues is together.
For engineers who are passionate about performance and leave them alone for two
weeks, he will be very much surprised with the results.

**Michaela:**  [00:22:08] Yeah. Yeah, definitely. Then it becomes, suddenly
becomes a project, right? It's not like something that you have to fix on the
side, which is, you know, in your way and actually distracting you from
something.
And it's also an achievement. Like if you give them, this is a project then, and
it's achievement that you can achieve and it not something like, Oh, you haven't
worked on that feature. Well, I did something, you know, but because you're
always like, it like drops that you're putting, right. So you don't see them,
they are dropping and you know, like the, the fondant on a stone and it's so hot
that you don't see the drop.
Right. So you really have to have a drain that the stone somehow pulls down,
which also reminds me on automatic for examples. I had like likes the singer on
my show. And he was talking about automatic and they, what they do is they stop
feature work for, I forgot the timing, but it's, it's impressive. And they just
do technical death, right.
Just to just do everything that they didn't do before. And they also get so much
done. And it's the whole company. Everybody does this now, and this is our
number one priority. And yet he also said that it's really helping a lot because
you know, you have this focus, you have this dedication and it's not like a
distraction on the side that nobody was ready to take on.
So when I looked at your LinkedIn profile, I not only saw, you know, where
you're working at right now, but I also saw a list of things that you're doing.
Outside of work or, you know, partially at work or whatnot. Right. So you are
also an egghead instructor. And I think I remember correctly, you said like you
have 150 videos or something, is that

**Tomasz:**   [00:23:39] correct?
More than 170 at this point?

**Michaela:**  [00:23:41] Wow. 170. So how are you doing that? Like, this is
something that fascinates me and I just have to get more time and get better at
all of those, you know, recordings. Staffing things like this, but this is
definitely something that I aspire to do as well. How do you do this videos?
You know, what, what motivates you to do them? How did you become a head
instructor? And yeah. Can you tell me a little bit about that?

**Tomasz:**   [00:24:05] So, first of all, I was not aware they're recording videos
before I started in a bit as an insect or I was doing, I was trying to think on
my blog, I was doing contract talks.
And that is basically how I got noticed, because people have basically noted
that I have a way of kind of teaching people what I know and I'm passionate
about, you know, teaching basically everything that I know that that was kind of
my, one of my personal goals is just sharing as much as, as from what I know
with others, when it comes to recording over while I have that 70 videos, I
recorded one video, then I did it again.
Then I did it again. And I did that again, because this is how you get to, to
this kind of level. I was absolutely not planning on the coding. So many videos
when I started two years ago, nearly to the day two years ago. I remember at the
very beginning I had a F I had this feeling, but what am I going to record?
I have nothing to teach. Um, this is not exactly true. I think that if you have
non trigger experience as a developer with defense, they have something to teach
others. And if you are, if you have this feeling that you have definitely
nothing more to teach, well, this is a good time for you to learn something new.
And I found with myself that I learned the best by teaching. So the best way to,
for me to solidify something that I've learned related to the recency is to
write a blog post about this.

**Michaela:**  [00:25:38] And so you do it from a, from a work from, yeah. From
a book process perspective. Do you write a blog post first and then you make the
video or do you make a video first or you just make videos for things that you
think that are better covered in a video and you write a blog post for things
that you think better are covered in a blog post.

**Tomasz:**   [00:25:59] That's a good question. What I basically do when I want to
share something with others. I mostly tried to think, what would it be useful to
me? Because some concepts of amazingly well explained as a blog post, because,
because you can search through it and whatnot, some topics are better when it
comes to, to a video.
So for instance, if I were to, I have a book post on my, on my screen right now,
uh, I was watching this amazing talk about coconut cookies, tokens, and API is
kind of this in depth, dive into, into those topics. And that was doing some
notes and basically turned them into blog posts that I published yesterday.
So this is, this is good. This works great as a blog post, because I have video
of me doing this content is no better than the conference topic that I've just
watched. But if I were to try to explain something that is a bit more visual. So
how do you do something in AWS console? Then the video works somewhat better
than this.

**Michaela:**  [00:26:56] Yeah. Yeah. And so you just said AWS, so I noted your
are AWS certified. What do you do there? How did you know, was it a requirement
from your job, or why did you set out to do that certification? And I also
started, you're going to the next level from AWS certified and yeah. What
motivates you to do that?

**Tomasz:**   [00:27:18] So there are two things here. So first of all, all ex has
been. Largely. I mean, all it's basically on the books, we have migrated
everything to AWS. I think like two years ago, my team we are working with ,
which is based in AWS. So we have API gateways, we have Lambda functions. We are
using dynamo DB, a storage SQS.
So there's lots of different diverse services. And I've joined today, a company
as a front end engineer, and I am still a front-end engineer, but when I joined,
I had. No idea about data. I, it was completely agreed in that area. So after a
while, my manager and encouraged me to learn more about this, because the idea
was, if you want to be able to contribute more, if you want to be able to
contribute to the technical discussions that you have to act detector decisions,
you should probably know what is going on.
And getting certified is a. It's a good way to accomplish that for two reasons,
because there's this texture system over there. And in order to become a
certified, because there are, there's basically a list of topics that you have
to be knowledgeable in, in order to pass the exam. Right? So we have the sector
idea of what do I need to learn as opposed to, I'm going to learn everything,
because this is not viable with AWS and psycho.
You have some sort of a proof that you have at least vaguely. Vague idea of what
you are talking about when it comes to us. And like I said, in 10 days from now,
I am going to pass my another example. So this is the AWS developer and I sure
hope I'm going to pass it because this episode is going to be live.

**Michaela:**  [00:29:03] Yeah, it could be. Yeah. So yeah. And well, one of
the, the, the question that comes to my mind, you said, well, when I joined
Alex, I was a front end engineer. I'm still a front end engineer, but at that
point, I didn't know, AWS. I guess in their job posting, I don't know. Maybe you
reacted to that or I don't know how you were hired or how you were, you know,
getting, getting the information that there is this description.
Maybe they, they said you should know AWS, or it's preferred that, you know,
it's something like this. And how do you, you know, how do you communicate that?
Can you tell me a little bit about your hiring experience? You know, and you
know, what questions were you asked? How was that process going? And, yeah, that
would be interesting.
So

**Tomasz:**   [00:29:48] the fun thing is that I've joined two and a half years ago.
And I haven't been in that I've joined a somewhat different company because we
are, you know, changing and growing quite rapidly. So, I mean, I can talk about
the process that we have today because I am also kind of involved in the hiring
process because I'm interviewing somebody basically every week.
But nevertheless, when it comes back to AWS for us plus Fanta, We absolutely do
not expect trans engineers to have AWS experience. I wanted to do. There was
something new I wanted to grow. This is why I am interested in investing in that
area. Nevertheless, I do a command to keep your eyes open. Like we don't
explicitly expect, expect the best experience, but I've never done that because
it is useful.
But when it comes to hiring process itself, we have a bunch of interviews. And
our hiring process. So from my kind of technical perspective, we have two types
of interviews. So there was a strictly technical interview in which we are
talking about somebodies experiences. We are also kind of diving into some
topics when it comes to JavaScript to react and whatnot.
And we also have a second interview, which is a system design interview. So the
idea is that we give you a problem. And architectural problem. And B basically
have this conversation about how would you solve that problem? What kind of
technologies would you use? How would you use them? How would you test that?
How would you monitor monitor VAT? And then so it's actually one of my favorites
because he had get to learn how other people are thinking about building
software and, you know, Charlotte architectures and this just, I learned as much
as, as they do on those interviews.

**Michaela:**  [00:31:36] And so now you are at the company.
Do you have like a career ladder there? Do you have like some, you know, when I
was working at Microsoft, there was like this really set in stone, things that
you have to accomplish to get to the next level, you know, what should be your,
you know, skills technically, you know, professionally and so on. How does that
work at all X.

**Tomasz:**   [00:31:57] So we do have a, we have a career lover that is by I'm Ching
at the end into somewhat like a tree. So there's junior there's mid-level slash
Aguilar engineer there, senior engineer and after a senior engineer. So
basically where I am there's this change is going to branch out. So there's a
manager stuff and there's an individual contributor path.
So in the manual, just powerful can become an engineering manager afterwards.
You can become a head or director of engineering after work, probably a CTO or
something. I'm not even thinking about this level right now on the individual
contributor path. We have fleet engineers and principal engineers, and.
Chief engineers if I remember correctly. So basically what we want to do is to
avoid this problem that I saw at my very first company where you had senior
developers who are promoted to engineer managers, not only not because they had,
they had manager skills. But you had to promote the subway. That that was the
UNBC option.
And some engineers are terrible managers because managers managing people. It's
a completely different job than, you know, being a casino software engineer.

**Michaela:**  [00:33:18] And so where do you want to go? Like you're now in
this, you know, one step before, so when you're branching out, which direction
will you go, where are you going to the management route?
Or will you go into the lead engineer?

**Tomasz:**   [00:33:29] I would have to go into the lead engineer out because I'm the
kind of person who likes to make, make an impact in the organization, but mostly
from like a technical perspective and mostly from the perspective of. How do we
that software, how do we think about fountain?
How do we think about, you know, quality and whatnot? Because like all the
components we have more than once to do as, as all companies we would like to
improve and having, you know, people and having more people in those kinds of
like leadership, technical leadership roles helps us can kind of drill the
picture of where we would actually be in, I dunno, two years in charge of this
and whatnot.
I am not entirely sure whether I would be the best manager alive. Definitely not
a remote manager. Maybe if this wasn't no, the year of 2020, where everybody's
working remotely, that would be probably a different story. But as of as welfare
right now, I am gearing towards the reef engineers

**Michaela:**  [00:34:29] posh. And so one of the things that when I hear you
talking, right, it feels like you're very involved in the decisions that are
made about, you know, for example, well, how do we tackle technical debt?
Right. Do we do this war rooms? Are people involved in those discussions about,
you know, how do we actually. Build our culture internally. How do we, and
especially obviously also, uh, engineering, right? What role does caudry we have
for us? Is that something that you feel that you can actively change or is it
something that others are thinking about and your are adopting it?

**Tomasz:**   [00:35:03] So we have, we have a couple of confining values and two of
them are my favorites. So the first one is be open. And the second one is to
take ownership. And I imagined the thing that the, because most kind of like
senior engineers in our organization, like we have this strong sense of
ownership. So we are not building something in a bad way because I don't know
somebody from higher above telling us, do we want to build the best experiences
that we, that we possibly can.
And if we feel like we should improve in some area, So for instance, well, I
don't know, imagine that we were not doing cultivars at all. And I thought we
have a group of engineers who are saying, we want to do code reviews and we get
to kind of influence our, you know, technical directors are very open to
communication too, to discussion.
So it's not like there are no them all kinds of people. There are very, you
know, kind of eager and to not only do discuss, but also to listen to our
feedback. And to improve and also grow, grow on each other. We also have this
process of kind of like a request for comments documents. So if you, as an
engineer, if you feel like somebody, something is not 100%, okay.
Like there are some processes that could be improved. You can always, I document
ask other for feedback. And maybe like this document has become basically the,
the way we do bad things from now on at all life.

**Michaela:**  [00:36:40] Yeah. So one of the things that I know is your area is
somehow testing. And I know that you, I mean, I asked that question today on
Twitter.
You know, what people want me to ask you? And testing was one of the things and
they said, well, yeah, you're doing testing. If your skills are not really good.
Yeah, exactly. Yeah. Can you tell me a little bit more about your philosophy
here and.

**Tomasz:**   [00:37:05] So my philosophy when it comes to testing is that I want to
sleep better at night. I don't want to worry about my changes back in
production. I am not brave enough to push major features to productions that
they don't have pets basically.
So when it comes to that, I struggled with believe that something that is not
tested, it's not done. And this tweet that you are referring to is from my
colleague of mine. Right. And we have this internal job that's tests. So down
development, because if you build a feature and you guys did the test, it is
twice the work.
Right. But imagine that you are building a house. You could probably, you know,
build it's pasta, which, you know, having cheaper materials, maybe those were
wait, maybe you shouldn't wait this long for the concrete in order to, to finish
like whatever the concrete is doing. If you know what I mean, maybe it is a
better idea to have solid foundations on how we build software and then to kind
of improve upon them.
Because my own impression after working here for two and half year is about. We
are building websites and experiences, fall shoots. Number of people, all that's
in Poland is in top 10, most visited websites in this country. My mom is using
goal X. I do the gets the break production. Um, some like, you know, obvious
mistakes because production incidents will happen always.
But I have a feeling that as engineers, we kind of get to choose what kind of
productions incidents are not going to happen at all, because we've managed to.
Test and make sure that I don't know, it is not possible for our login page to
be empty.

**Michaela:**  [00:38:51] Yeah. And I also think, I mean, Slowing down. I think
it's a, it's a little bit a wrong perception because you're not only writing
code.
Right. So there's this task that you're writing code, but an actually code lives
on. Right. So, and you wanted to have it live on for a long time. And so if you
think like this is the first investment that you're making, and then based on
this investment, you're profiting from it. Right. But by your profit thing, you
actually have to maintain.
The code. And so if you're, as you said, if you're building a better foundation
and if you are adding tasks right in, you know, your foundation is actually good
in the long run, you will have less iteration on, you know, maintaining that
thing to improve it, to fix things that are broken or wrong. And so I think in
the end, it amortize it itself over time.
Very, very quickly. Yeah. So yeah, I definitely think that's true. So one of the
things that you also mentioned was product driven mindset. What is a product
driven mindset and you know, how can we get that?

**Tomasz:**   [00:39:53] Sure. So the way I think about it is my job is not to push
tickets in JIRA for 'em to do to them. My job is to build products, assault.
The way I think about it is as an engineer, I think that the best part of our
ability by people who have this great understanding of what exactly are they
building, and this is sometimes referred to as business context. So I don't
know, I am not adding this form to make my manager happy. I am adding this form
so that our users can either know their bank accounts number to the account.
But when you go one level above and think about what kinds of problems am I
trying to solve then actually you are building better products because it's not
about the form. The form is the way we address an actual problem that our users
have their actual needs. So as an engineer in my team, okay, why are we adding
this form in the first place?
Maybe we could do it in some other way. Maybe we could get this data from this
other, I know microservice that already has this data. Maybe we'll go to talk to
that people. And this product driven mindset means that you don't necessarily
think about the structure of building in terms of, again, JIRA tickets you think
about, okay, this is the problem that we are trying to solve.
How can we do that with maybe without even writing any code at all? Because some
problems can be solved. By, I dunno, an email. I have a, I have a, this example
that I often give, that we had this idea that we wanted to ask our users
feedback on a certain feature. This feature was not used by many people, so we
want them to kind of have a survey inside of this page, but then we decided that
we are going to send an email to them because it took us 10 minutes and we get
the, exactly the same kind of feedback that we had.
If we were to build a form or survey.

**Michaela:**  [00:41:48] Yeah. And so what came to my mind when you were
talking about this, is that I think. I mean, they're definitely engineers that
don't want, or don't care so much about the product. And I, again, think it's
not the engineer themselves. I think it's the culture in the company, right?
That at one point you give it up maybe and just say, well, yeah, it doesn't
actually met him. What I think. So we just do what we are asked to because
that's what we are incentivized for that, you know, that's what our incentive
structure is all about. And, and I don't, I cannot change anything. Right. Even
if I think this is not.
The right step for the product. But I also think that sometimes there's like
this business driven mindset, right? So there are like those two things that are
a little bit competing with each other, right? So there's this product driven
mindset, which I think is maybe easier to adopt as an engineer because we like
to create, and we maybe are even taught about, you know, how to think about the
users and how, but then what's a little bit, even further away from an engineer.
Is this business driven mindset, right? So. Let's say a large corporation,
right. And they wanted, they have like a tool and it's for code reviews. And so
you have all these great ideas as engineers, how to improve this cult review
tool. But there's this business aspect, which says, well, we are much bigger
than contributes, right?
We are doing so much more. So right now we don't have to make the best product
for code reviews. And so somehow this idea about, you know, making the best
product com becomes a little bit diluted by, you know, the business goals that
you have as well, which are not always the product goals. I don't know if this
has makes sense to you if you feel that as well, but this is something that I
feel it's.
Very often, very challenging and very de-motivating can also be very
demotivating because I think, you know, there's, it's easy to fall in love with
your product, right? It's a little bit harder to fall in love with business
goal.

**Tomasz:**   [00:43:43] Exactly. I know, I know definitively what you mean, uh,
because I, I can give you an example.
So we are on running apps on all X. Every large website is running ads. We are
no exception and. Engineers are, you know, we, we don't like that. We don't
like, you know, having other Sonos creeps that are loaded on our beautiful,
beautifully crafted pages with Google ads or whatever. And then we get, you
know, get informed that by the way, this is paying X percent of your salary
guide because, you know, we are not putting those apps for, because we want to,
right.
We are putting those ads because they help us, you know, our business and, you
know, earn more money for the business. And I completely agree with you, but
sometimes it is difficult to kind of figure it out. Why we should do a certain
thing. And I think it's always important both in programming product and
business, to try to figure out what do we optimize for a given moment, right?
So are we optimizing for growth in our user base? Are we optimizing for the best
possible product or are we optimizing for the greatest revenue? Because doing
all of those at the same time is actually impossible.

**Michaela:**  [00:44:59] Yeah. Yeah, yeah, definitely. Yeah. I find it always
quite challenging, especially like all those, even though, you know, it, it's
not pleasant.
Right. So even though, you know, okay. To add some now paying part of my salary,
it's still not a pleasant feeling like, Oh, the performance goes down. That's
horrible. Can we block it? Where's the ad blocker, right? Yeah, exactly. Right.
Yeah. Yeah. Very cool. So, well, I think we actually reached the end of our
session today of the interview.
Is this something that you want to share with my listeners that we haven't
touched on that you think would be important or something that you want to tell
them? Some advice that you want to give them on their way?

**Tomasz:**   [00:45:43] Um, okay. So I had this, I had this fault like yesterday,
because I'm not sure whether you are listening.
You know, you listen, if you're a student or if you're younger than me,
apologies, I've thrown them the 30 this year. And this is a major moment for me.
But I was thinking today about when I was studying at the university, I have a
master's degree in electronics and telecommunications. How somewhat this degree
is to my career.
If you are studying for, in a computer science degree, you were probably going
to become a developer and some of those skills are going to be useful. But
nevertheless, I w I wanted to kind of express this idea that if you are in
college, if you are, if you basically should have chosen our own pager for, for
a set and you have ended up.
I have this strong feeling that as you know, your university is basically not
kind of like a defining point of your life. I am standing to name like most of
the names of my professors from the university, not to mention the, kind of the
content of the class that they taught. I am a JavaScript developer and I didn't
write a single line of Java script doing my inner negativity.
So this was something that I would love to hear.

**Michaela:**  [00:47:03] Yeah. And I also think that there's always a point to
change, right? I mean, if you look at my, if you look at my path, there was a
big. A big turning point that people would probably say, well, that's the big
turning point, right? There's when I finished art school and I went on to do
computer science.
Right. And I didn't have an idea about computers. And so maybe that was, it
seems like this is a turning point, a huge turning point, but actually it's not,
it wasn't really like this huge turning point. When I started from computer
science to software engineering, right. When I made this switch was again, It
was probably the same turning point, right.
When I then went to, you know, do for my first job was again, a very different,
you know, experience when I worked as a researcher and actually over the years,
you know, things really. They get less, less important and still, you know,
every time you do something new, it's again, it feels like, Oh my God, can I do
that?
Right. It feels like, Oh, this is what I, so when I stopped my research position
and people were telling me, you're completely crazy that you do that, right. Who
would give up this position? And it felt crazy. And it felt like, Oh my God, you
know, like what now? And now it's. One year later. Right. And I feel like, well,
it completely changed again.
And so I think it's always, when we are in this situation, we feel like, Oh,
this is now so important, right. This is such a defining moment for my life. But
actually we can always change. I mean, even if you don't have a computer.
Science degree or no university degree, you can actually really change. And
it's, it's a lot about imposter syndrome.
Also, maybe getting over, you know, yourself and you know, your, your feelings
or your thoughts in your head that tell you you're not good at that, or because
you don't know it. Right. You don't know it. And I started my business. My first
intention was I have to do an MBA, right. To be prepared. Let's do an MBA
because somehow, you know, this gives you some security that you know what
you're doing, but I felt like, well, this takes way too long and too much money.
Right. I don't have it. So I have to just figure it out myself. And I think
every step that you're doing, even if you're not, let's say you are, you know,
in the fast food industry. And now you think I want to become also a JavaScript
engineer or developer. It feels really unreal and impossible right now, but
really this small steps that I think maybe just brings me back to what you said
about your videos.
Right. I made one video and another video and another video. Right. And then you
look back and it's like it's two years later. It's probably another overnight
success, right? You're not waking up, you know, watching one YouTube video,
writing your first website, and then the next day you are, you know, you
accomplished your dream, but if you, every day, you know, work on that, I think.
Yeah. And don't let you know whatever happens right now. Define you. I think we
are giving too much, much, too much weight to what's in the now. Right. Which is
important on one hand. But. You know it. Yeah. It, it, it becomes less and less
important over the years. So I totally agree.

**Tomasz:**   [00:50:08] Yeah. Uh, also, I was still supposed to tell this story
because this was requested on Twitter.
And I think it plays very nicely to what we just talked about. I went skydiving
for the very first time this year, because as I mentioned, I've done 30, my wife
decided to, to attempt, you know, connect me, therefore she booked out a
skydiving session. Luckily I did get the parachute. So that was actually
excellent.
But the reason why I'm mentioning this is that it was absolutely scary, but the
scariest moment was the night before. I was unable to see if I was in the lane,
in my bed. I was going through the sky dive over and over in my head, even
though I had absolutely no idea wasn't going to do. I, you know, I watched a
video on YouTube.
So I have this vague idea of, you know, I'm going to get into an airplane. We're
going to fly up and then they're not going to jump out of a freaking moving
airplane. But when I actually got there to the airport, Then I realized that,
you know, some other people are also doing this and there are not dying,
therefore I am going to be okay.
So I think this is a huge, important life lesson for me is about this curious
moment. When you are trying to make a huge impact, a huge change is a guide
before you make them. Because as soon as you get to work, as soon as you
actually get started, it becomes. So much easier. It doesn't mean that it is
going to be easy, but it is going to be easier.
And with each kind of like additional challenge that you overcome, like those
things have a good chance of getting easier. But going back to my access videos,
I struggled a lot because they, my very first like five or 10 videos, that was a
hustle. And honestly it took me, I don't know, the next three hours to record a
two minute video.
That was a disaster. I thought I am so much better than this, but it took me, it
took me awhile. So you have to, basically, I would recommend that, you know, you
should always try to kind of keep him put away and go out of your comfort zone.
And every once in a while, if you feel it feels like it, uh, I think, you know,
it is a good idea.

**Michaela:**  [00:52:21] Yeah, I think so too. Yeah. That's, that's definitely,
that's definitely true. So, well, I think that's a perfect ending. Thank you so
much, Thomas, for being on my show and spending the time with me and telling me
so much about, you know, how it is to be a software engineer at your company.
And yeah. Thank you so much.

**Tomasz:**   [00:52:40] Thank you very much for having me.

**Michaela:**  [00:52:42] Yeah, it was my pleasure. Okay. Bye-bye

I hope you
enjoyed another episode of the software engineering unlocked podcast, but before
I let you go, let me tell you that this week black Friday, I have some special,
really amazing discounts on my code review workshops. So if you ever think of
the idea of booking one.
I think now is the time. So hop over to https://awesomecodereviews.com. And I hope to
see you in two weeks for another episode of the software engineering unlocked
podcast. Bye.


