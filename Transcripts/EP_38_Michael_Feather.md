---
episode: "Michael Feathers - (Legacy) code - A living organism"
permalink: /legacy-code-michael-feathers
status: publish
type: transcript
---

**Michaela:** [00:00:00] Hello and welcome to the Software Engineering Unlocked
podcast. I'm your host, Dr. McKayla and today I have the pleasure to talk to
Michael Feathers. But before I start, let me tell you about Botany.io who
sponsors today's episode. Botany is a personal asistant and coach for engineers
that helps you grow and adopt better habits. With Botany, for example, you can
level up on your code review skills. Not only does Botany remind you of open
code review, but it also allows you to ask your colleagues for feedback on how
you can improve. But code reviews are not the only area Botany can help you and
your engineering team with. Botany also enables engineering teams to improve
praise, develop better habits, and foster a more informed and collaborative
team. I really like the values that Botany is built upon. Growth over goals.
Action over analytics. Ownership over oversight. And push over pull. That means
that Botany allows engineering teams to continuously improve by focusing on the
personal growth and the individuality of each team member. If this sounds
interesting to you, please hop over to Botany.io to request access to the tool.
So, that is Botany.io. But now, back to Michael.

Michael is the author of the super popular book "Working Effectively with Legacy
Code". He's also the founder and director of  
R7K Research & Conveyance, a company that helps engineering teams with the
software and organization design.

Recently, Michael also joined Global as a chief architect. Since I have been at
university reading his amazing book, I always wanted to pick his brain. So I'm
super excited to have Michael here with me today. Michael, welcome to the show.

**Michael Feathers:** Ah, thank you very much. It's great to be here.

**Michaela:** Yeah, it's my pleasure. I'm really, really excited. Michael, you
have been probably working more than 20 years with engineers, with software
companies from all over the world. This is so, so fascinating to me. I'm super
curious about how different organizations develop software. I'm always asking
the questions. What makes teams and organization more effective than others?
What software engineering practices do we have? I'm a big fan of code reviews.
And so I want to know from your experience, are there best practices? Can you
make out best practices that really lead to success for engineering teams where
you say, well, if they follow that, right, they will be very successful versus
factors that you think they are definitely bad and lead to a lot of troubles.

**Michael Feathers:**[00:02:28] Uh yeah, it's a great question. And it's
interesting too, because like the practice space is very interesting, but I
think a lot of it really comes down to organizational culture, you know? And
it's, you know, if you have a good culture, then basically like the practices
will develop almost invariably, right. Or you'll at least be open to going in
and exploring different practices and things along those lines. I think, you
know, for the thing that I have gotten called into organizations for quite
often, you know, legacy code, the thing I kind of noticed over and over again is
that what is missing sometimes is really a very frank conversation about the
quality of the stuff that people are working on. Right. And in the worst cases,
it's kind of like uh, it's like everybody is told, you know, you must write code
and you must design this thing and create it, but nobody's really paying
attention to it. And sort of like, you know, thinking about it as being
significant, you know, quite often there's like a task focus rather than
focusing on the quality of the thing that you're producing, that kind of thing.
So I, you know, I wouldn't really know how to go and actually sort of say, what
are the best practices? I think that so many of the things that we basically do
in the industry now regarding testing and pairing and mobbing and you know, the
way that we allocate work and stuff like that, a lot of those things really kind
of help. So.

**Michaela:**: [00:03:44] Yeah. So one thing that I thought about is engineering
values versus practices, right? So I think that engineering values and
developing those as a team, and not a lot of people are talking about it.
Unfortunately I think much more people should talk about values. The engineering
values that we have. And not the practices because practices can change and they
should change. Right. They should change over time. And with technology changes
and with our, how our society changes, the practices should change and somebody
comes out and has a new idea. Right. And they try something, they fail maybe 10
times, and then suddenly they found a new thing. But the values, I think, for
example, what about our code health. Right? I wanted the quality of the code
that we are expecting how we are developing software, how we are talking about
the things I think those values are really important. Is that something that you
have more and more teams do or, you know, successful teams do.

**Michael Feathers:**[00:04:37] Yeah, definitely. I think it's yeah, it's a lot
of, it really comes down to taking the work seriously. I think, you know, in a
way, and in terms of values, it's, it's, it's funny with this too, because you
know, there are many different, like, you know many different ways we can look
at, you know, values across organizations and different frames we can use. But I
think that actually going and seeing the systems themselves as valuable is like
a rather important thing to do as well. Right. And that's a little piece that
tends to be missing at times. One things that's kind of been striking to me
across, you know, my career is basically noticing that in the very beginning
back in the 1990s, it seemed like there was this thing of kind of like, well,
we're all kind of like disposable and as engineers, you're just basically there
just to do the work and then basically go home or go bowling or whatever it is
you want to do in the evenings. Right. To going and recognizing that we can
become more whole people at work and basically valuing our own development and
valuing our communication, our relations with our coworkers. And I think that's
a great thing, but then there's also this other thing too, of like valuing the
thing that we do and looking at the things that we create as being significant
and having their own intrinsic qualities that we can kind of like, you know pay
attention to and kind of foster over time. So yeah, I think one of the things
I've been coming back to over and over again within my career is just this
notion of thinking about the systems that we create as if they were like alive
in a way. Right. And we get to care about them. Right. And it's kind of like
this way of going, like applying like this anthropomorphic frame to the things
that we're working with. And some people might say, well, that isn't like a it
isn't like a good thing or it isn't a realistic thing, but I find it very useful
to come and sort of think of them. Think of the systems we work of is basically
things that we can foster and care for. You know, I think that helps us become
better engineers.

**Michaela:**: [00:06:25] So, when I was preparing for this interview, I read
through the things that you write on your website on the R7K website. And this
is something that I read. I was really fascinated by it. Like. That the code is
in living organism. Right. Sort of, and, and I thought, well, this, this is
true. Right. It evolves, it changes. People come in and the levels are their
fingerprints there. Right? So coded that I write looks probably quite different
than code that you write. And even if you have engineering values around that,
and even if you have coding standards, you probably can tell, you know,
sometimes the boundaries of this is where one engineering team or engineer work.
Then this is where another engineering team works. And you also talked about
your, how actually Cultures and the organizational structure shape our code,
which is one of those laws that we have been seeing and studying for for many
years. Right. Where we see that actually. Yeah, exactly. Right. But you see that
you have the organization and the boundaries and how you structure and the
design, your organization will reflect in the architecture of the system, which
also shows that somehow it's, it's living with the organization and growing and,
you know, aging and getting to a legacy when the, also the structures of the
organization change. And it probably it's even harder to change the code per se,
when you're changing the organization. Right. So people change organizations all
the time. They're reorgs in large organization. They're reorgs all the time, but
we're not reordering the code in the same capacity. So what is your thought on
that, especially about technical debt, for example. How should we deal with
that? And how should we integrate that in our day to day work life?

**Michael Feathers:**[00:07:57] The, the main thing I keep coming back to us,
like the frame. For this, you know, it's kind of funny. We can talk about this
being like a metaphor that basically code is like biology, but I think just
about anything that kind of grows incrementally, where it's easier to add new
things than to change existing things tends to go and sort of have like these
hallmarks of organic growth in a way. Right? Like I used to say to people, like,
if you, if there's like a young tree and you kind of like kick it and it kind of
like falls over a little bit, it's kind of like, it's not going to upright
itself. It's going to basically continue to grow. You know, upward, but from the
direction you kicked it out. Right. And in much the same way that kind of thing
happens with our code is that the things that we do tend to basically leave
their mark upon the structure of the code. Sometimes in complexity theory, this
is called path dependence. It's kind of like that basically, you're dealing with
something that has a memory and basically what's possible with it depends upon
what happened previously. Right. So I think that the main thing is to kind of
like, just sort of like recognize this, recognize that that this is part of the
character of, of code itself and that we don't really ever get to go and sort of
like say I'm going to build a brand new system. Like the complete rewrite,
that's going to go and be shiny and, and perfect. You know, that's going to go
and serve. I solve all of our problems that, you know, the, the code that we
create, basically we're on a journey with it and it's going to basically take
time for it to go and react to the new situations in this environment. And those
new situations are how our organization is structured. What new features we need
within the system. And it's just going to be like this slow process of change. I
think the interesting thing with this in terms of practicality is that. It does
mean that sometimes it's easier to go and create new systems than to go and sort
of modify existing ones. And we should be a bit more proactive about doing that
sometimes. We're basically like you know, if we have particular products and an
organization think about creating new products sometimes rather than trying to
burden existing products with new features that may not quite fit for instance.
So, you know, that's, it's a rather abstract answer. I'm sorry, but it's kind of
like, you know, I think that basically this frame that we have of looking at
software in this way can help us make some of these decisions a bit better, but
they don't like sort of solve all the problems necessarily in there.

**Michaela:**: [00:10:21] I heard you say a couple of things, especially before
where you said, well, we have to take the quality of the system more seriously.
We, you know, we have to be more careful. In my experience, I see, I see several
camps, right? So there are the, really the, the engineers that, you know, they
love high quality code. They, they learned a lot about how to create high
quality code and they really do and nurture the systems quite a bit. Then you
have like some tension between business goals here because as long as it works
right, and it fits the business goal, there's like this tension and this, this
pull towards, well it's good enough. Let it be please. Don't make it nicer or
more elegant and more inspiring. Just let it work. And then you have also very
pragmatic developers that are maybe, you know, they're not, they're not into
elegant code so much. I haven't seen many of those, but they are. And I think a
lot of more people become, especially like people that are creating software
because they want to create something, right. They want to do products. So we
have like a new wave of engineers. I think, especially when I studied a lot of
people studied really for software engineering, but they were not entrepreneurs.
Are, are only a couple of them were right. And now I see there's like a huge
mass of people that are also engineers, because they want to be entrepreneurs.
They want to create products. And I think they're coming a little bit with a
different mindset into the whole you know, why are we using code and using code
and code is just a means to an end, whereby I don't know when, when I was in
university, it was not a means to an end. It was the end, right? Like, this is
why we are here. This is, it was not, it was a product focused. I had not a
single lecture about product. I had only lectures about code and what is good
code and what are good, you know development practices. And I also studied
computer science. So a lot of computer and computer systems and system
architecture and so on. But no product, right there was not all, how do we
position that product or what makes a good product, not even product management,
which probably should be there with it anyway. So I'm saying. I think there are
more people now with a more pragmatic view on software than maybe 10 years ago.
That's at least my experience. So how do we balance that? And is that a good
thing? You know, is it a bad thing? Can we even say, you know, it's good or bad?
Is it binary?

**Michael Feathers:**[00:12:46] Yeah, we can, we can basically have like a very
instrumental view of code and systems and say they're there just to serve us.
Right. And that's a frame, which like you say, can basically help you out if
you're an entrepreneur. And you're just trying to get something to market very
quickly. But you know, it's a story which is, you know, just, you know, an age
old story that essentially it's like people get to market and then they discover
they can't change anything because they've created such a brittle system that
it's impossible to work with. So you're always going to have like a mix of
people they're pragmatic and people that are idealistic, I guess, the, the
important thing culturally is getting them to be able to talk to each other and
see each other's point of view and recognize that sometimes you have to be in it
for the long haul and you have to be able to make trade-offs that sometimes it's
good to be opportunistic and do something very quick and dirty and disposable.
And other times you want to go in like really invest in a particular thing,
because it's important to you. One thing that is weird about this is that I
think if we look at code as being just this mechanical thing or this thing,
which is like over there someplace, or the thing that we mess with, you know,
when in between our business conversations, which are really more important, you
know, then we we aren't paying attention to it enough to basically understand
when it can get in our way sometimes. There's a guy I know Colin Brecht who
basically started doing this thing called quality views. So it's an idea that I
had years ago and he was doing this within his organization and it's a really,
really cool tool for going in, dealing with technical debt. And I really want,
that's a great thing to go and talk about. It seems like with technical debt, we
always go and we ask like the business side for like time to go and like go back
and fix things. Right. And it's kind of like, that's always like a tough sell
and it's also kind of like people say, what am I going to get for that? Right.
But the technique around this is to go and say, let's take a look at our
systems. And kind of like make a little pictorial representation of that. Maybe
like if you have a big system, maybe it's like five boxes of things, right. And
then when we're discussing the features, we want to add to the system, we can go
and say, okay, well this particular feature touches these three boxes and this
other one touches these two boxes. And what you do is you put colors on these
boxes to indicate their level of health. Okay. And what happens is that color
gradation is going to change over time. Right. And you just basically go and use
that as a basis for conversation with the people who aren't looking at the code
all day. Right. And the neat thing about this is that without talking about
technical debt at all, it starts to become like this feeling within the system,
within the organization that, you know, the code is a real thing and it has a
particular qualities. And those things can either help us or get in the way,
depending on how healthy it happens to be. Right. So it's not uncommon to go and
do this and have somebody go and say, gee, you know, this one area of the system
is very red and it seems like every time we ask for features to touch this area,
you know, it's going to take a long time. Can we do anything about that? And
then you actually have the business going and asking for system's health.
Whereas before it would be completely invisible to them. So I think that stuff
like this is kind of like the path forward in a way is to basically sort of make
the systems are real to people within an organization. And, you know, sometimes
the choice is going to be to do something very pragmatic that might actually go
and sort of hurt things for a period of time temporarily. And you might just
need to do that for the business, but you'll at least understand what the
consequences are of longer term.

**Michaela:**: [00:16:07] Yeah. I liked that. I liked that idea a lot, because
if you think about a business and it has a building and it is in the building,
like, and the building just rots right. Buildings rot. Right. So they, they get
older. The focade is not nice anymore. The entrance is maybe not nice the floor,
right. Ceiling and so on, but people it's very visible to people and you think
like, well, it's good enough still it's good enough. But there comes a point
where you think, well, we cannot have this entrance. It's still functioning.
Right. It opens the door, but it makes some noise. Right. And it looks horrible.
So you don't want to welcome your, your people there and, you know, at one
point, there is no, you know, no way back to repair it, right? So then you have
a big disaster, but this is very visible. So I liked this idea that you
actually, you show it, you help people imagine what actually the system looks
like, right? So there's some visibility and transparency in it, which I think is
very often missing. And I think that this, this missing visibility and
transparency is also something that makes our, our lives so hard as engineers.
Right? We are in front of the computer.

**Michael Feathers:**[00:17:10] It's completely invisible to people. Right. All
they see is people looking at monitors and it's like, who, you know, they look
at us looking at monitors and they're like, "Oh, what are these people looking
at?" Right. So it's rough.

**Michaela:**: [00:17:22] And, and you also, you don't see, the work and the
quality of the work. Right. Do you see a button and one engineer can create a
button and another engineer can create a button, but you don't see what's behind
it. You know, like how is the button integrated? Is that button actually really
usable for another button? The CSS come, you know, from a class or is it just,
you know, hand drawn into in, inline style or something, right.

**Michael Feathers:**[00:17:43] I think it's almost it's beyond metaphor in a
way, is that I think it really is true that software's physical in a way, you
know, it really is. Now, when you think about object orientation, it's like
objects are meant to represent things or to basically be things that, you know,
have cohesion and coupling and can communicate with other things. You know, all
of these things live in this virtual space, but it's like they still obey some
laws of physics in a way it's kind of like modularity is like when something
grows too big to basically fit in our heads, we basically want to keep it
smaller. Right? So you can see that as being just like objects in the world.
Some things are just ungraspable because they're so huge and software can be
like that too. So we want to go and keep it smaller like that. So I think, you
know, we can use the real world as like a decent, you know, framing device for
going and understanding these things and helping us make better decisions.

**Michaela:**: [00:18:34] Yeah. So I'm interviewing and talking to a lot of
people right now, engineers, and I'm talking a lot about, you know, their values
and also the codebase health and what makes them happy, what makes them
productive. And one thing that I hear over and over again, is that you know, you
have your engineering heart, right. So good code, good quality makes you happy.
That's definitely something that I see for, for many, many people, not
everybody, but a lot of engineers, but then you have all these system
constraints and now the system is an organization, right? So you also have, you
have to fulfill your duties, you have to do what you're supposed to do, and
knowing that you're doing what you're supposed to do, it makes you also happy.
It makes you more excited. Right? So if you know that you're actually working on
something that you're not supposed to work on, it makes you unhappy. And, and
it's also risky to take on the task, right? So there's this, there's this
productivity then there's this code health and they're all some how intertwined.
Right? So people want to work on, for example, technical debt is something that
people, a lot of engineers would say. Well, it's a challenging problem. I like
to tinker with the code, like to make it nicer. I like to make it more, you
know, reusable, more maintainable and so on. But on the other hand, there is
business constraints and business needs. And my manager, you know regards me, or
also evaluates me based on the features that I'm delivering. So I actually
cannot take on technical debt. And I think you probably people will call you
when there is like, when you have a problem. Right. So it's too far. So how are
you going to change the mindset? How you're going to work with the people?

**Michael Feathers:**[00:20:00] In all fairness, people usually call me once
they recognize that they actually have a problem, you know?

**Michaela:**: [00:20:05] Yeah, it's very late, right?

**Michael Feathers:**[00:20:06] And I think that's the bigger thing too, is just
as developers, when we're working in an organization, it's a bit of work to go
and actually go and convince people that actually some investments in going
reducing technical debt gives you a payoff. Right. I think the most important
thing to go and recognize this, that like there's almost like this 80 20 rule
that basically goes and happens with code change. And I, you know, I haven't
really seen research around this, but it seems to ring true. Maybe you have, I
know you have a more of a research background, but it seems like there are hot
spots in code systems where basically there a lot of change tends to gravitate
towards them. They can shift over time. Right. So the thing is, it's kind of
like as a developer, if you're going and looking at something that's pretty
messy and then you look back and you basically see that that area had like,
thousands of commits made against it. One thing is you can pretty much count on
us, any little thing that you do to go and make things better there is probably
going to go and give you a bit of a payoff, you know, going forward because of
the fact that it's a hot area of the system that goes and gets a lot of change,
right. And I'm getting, you know, in the organization, just, you know, we should
never look at technical debt as being like this thing, which is a uniform across
an entire code base. I mean, it is in a way, but it's like in terms of the value
of technical debt, It's wildly different in different areas of the code. Some
areas are more mission critical in your code base than others are. And if you
can at least have different say, rules of engagement for the system and go and
say, you know, we know we don't have very much time, but you know what, whenever
we touch this particular part of the system, we're going to be really careful
about this. And we removed technical debt because we know that it's critical for
our business and we've changed it a lot. Just getting simple agreements about
that, going forward, give you almost like a bit of a foot in the door in your
organization to go and have this conversations about how quality impacts things.
So yeah, it's never like this thing of like, Hey, let's go install technical
debt. It's more like let's find out where it really pays off and then go and use
that as a way of going in sort of like surfacing the conversation and doing
something about it. Cause that's gonna be a smaller investment.

**Michaela:**: [00:22:04] Yeah, hotspots is definitely something that we saw in
many different empirical studies as well. Right. So that problems accumulate in
different areas more than others. And there's clusters that around that and so
on. So it is definitely rings true for me from, from this perspective as well.
And I like what you said, well, technical debt, you don't have to work on every
technical debt unit code base. Right? Some of that, it doesn't even interest you
because you're not touching it. The system runs, there's not, I think a lot of
how much it bugs you has to do with how often you're changing the parts, that
there is a lot of technical debt, right. So if you're not changing the parts who
cares, right. Probably I don't know.

**Michael Feathers:**[00:22:45] And, and really, I think, I think that's one of
the things I like in my book I talked about this a bit in terms of writing
tests, like going and breaking dependencies and writing tests for particular
areas of the system is that because there's this kind of like power loss, predo
distribution of code change that if you take the time to break dependencies
around a huge class and write tests for it, chances are, you know, you're going
to come back to that relatively soon and basically go ahead and discover that
that work has already that hard work has been done. And you're going to be able
to take the benefit of that work. Right. So it's kind of like, it's, it's weird
because like that power loss growth goes and leads to some chaos and systems,
but it would also helps us in terms of going and sort of focusing our, when we
focus our energy, we get payback for it also. So it's like a place where we get
a virtuous cycle that goes into alliance with the cycle that caused of the
problem, you know, so we can sort of leverage it to go and solve the problem as
well. Like, I'm not sure I can put words better yet, but.

**Michaela:**: [00:23:46] No, it sounds, it sounds good. Yeah. So you were
talking about testing and in your book, and this was also a good question and it
was actually asked on Twitter, right? And your book, there was this really
strong connection with legacy code and the lack of tests, for example, because
if you don't have tests, tests somehow are also a means to an end. Right? Did
they give you confidence that when you are making changes, the system is still
very similar to what work, what it was before, right? So you're not introducing
any bugs, hopefully. Right. And so the better, the better the test, the better
your confidence. And so you're, you're actually able to do changes without any
tests you don't know, like, are you messing up completely here or, you know, are
you introducing a lot of side-effects and so on? Is that still in definition
that holds true for you today? Or would you say that over time, the definition
of, you know, what legacy code is changed for you?

**Michael Feathers:**[00:24:39] Well, I think any definition like this is kind
of instrumental. I was actually the time I came up with us working with a team
and I sort of just got angry and I said, you know, people, weren't writing
tests. I'm kind of like, you know, it's kind of like, you know, this is legacy
code because it's code without tests. And I started ranting a little bit right
and a friend of mine, says, you know, you should write that down. I'm like,
okay. So I did. But the, the reason why I really was trying to press that point
is because it was like really obvious to me through my experience at that time
that there's a real strong, qualitative difference between code that has test
coverage and code that doesn't in the sense that if you don't have test
coverage, quite often, you're scared of making changes and you can be much more
conservative about how you, you know, do things you may not refactor as much.
And you know, just, you, you have like a, a greater sense of ease working in
code that has decent test coverage. And I thought that qualitative difference is
just so high that's worth going in highlighting that and basically going and
tying that into a definition of legacy code. But then, you know, there's the
thing of kind of like there's many different definitions of what legacy code is,
and, and they're all useful to some degree and that's fine, but you know, I
think for people that need to hear it, that's the one I still use just because
it's, you know it helps people go and it's, it's a definition which kind of
points to the solution, which I think is useful for us if we're trying to go and
galvanize attention towards better practice.

**Michaela:**: [00:26:02] So on your website you also wrote what we call legacy
code is exactly what you would expect when developer turn over is faster than
code turnover. Right. So for me to seems very much it, legacy code has to do
with the loss of the knowledge about the code base. Right? So if you're, and
this sometimes has to do with the technology as well. Right? So if you think
about systems, you know, written in some languages, well, we just have really
only a few people that are still familiar with this code it's legacy code,
right. Or if you're having a code base and people leave, even it's written in
React, which is now, you know, modern and that everybody knows it. People don't
have knowledge about the code base. So it's legacy code. Is that something that
you think also rings true for you?

**Michael Feathers:**[00:26:48] You know, I kind of like somebody offered that
as like a an alternative definition is that, you know, legacy code is the
product of, you know, it's when your team turns over faster than your code turns
over. Right. That kind of thing. And I think it's important to go and basically
see that system dynamic because it really affects a lot of the decisions we make
about process and team structure and all these things going forward within our
organizations. I remember, I try to remember which tool this was so I won't
mention the name because I'll probably get it wrong, but there was like a tool
that's widespreadly used within the industry of database technology. And my
understanding is it's actually done only by two or three people. And they've
been working on it for decades and it's kind of like their life work is
basically going to supporting this particular piece of software. Right. And to
me, that's almost like the ultimate fantasy in a way. It's like, Oh, you know,
have this house that you live in, that you basically sort of like remodel,
continuously except this code. And then basically, you know, it so intimately
that you're in this space where basically it's never really legacy to you
because you're constantly able to go and improve it and add to it and stuff
along those lines. Right. And it should never be something which is too big,
where it's too big, then, you know, it's so big that a couple people can't work
on it together, you know, that you need an entire team. But it's interesting
without to go notice that that's almost like an idealistic situation of having
something that's durational, the people are going to be with it long-term, it's
relatively small and you can basically do a lot of really great practice with
it. But the thing is, it's kind of like in the typical development that happens
to these days that never really quite happens. The software tends to grow up,
grow bigger than us bigger than what will fit in like two people's heads, for
instance. Right. And beyond that people will basically leave and go to other
jobs and other people will come in and stuff like that. And it's these things
that happen, which go in, tend to go and cause you know, the, these issues that
we tend to have, and then we have to go and introduce practices like, you know,
extensive testing. You want to make sure that we can detect when something goes
wrong in this thing that we don't quite understand when we make changes to it.
Right? All these things are almost like props that we use to go and basically
deal with this fundamental mismatch between the lifetime of the team, the
lifetime of the code. And I think it's kind of a fascinating thing to go and
recognize that those tensions are inherent in what we do. And it's not that
we're bad programmers, we're just dealing with a pretty hard problem that we
have this, this lack of alignment between team and, you know, piece of code that
we're working on.

**Michaela:**: [00:29:18] Yeah, exactly. And I think it has also to do with, I
mean, there are so many factors that influence that. So for example, in our
industry, people that are, you know, five year in one company, this is like,
five years! How could you say that long? Right. Like people are turning over
really quickly also for various reasons. Very often also because they want to
level up. And because there is, or yeah, because there is a lot of opportunity
out there, right. So people can choose, pick and choose, be quite choosy. But on
the other hand, as you said, well, people are leaving and they're with them a
lot of knowledge is leaving, which I think sometimes organizations still don't
recognize the value of the, just the knowledge that people have in their head
that they accumulate. Right. Because, and we see that and you know, that I'm a
big fan of code reviews, for example. And I did a lot of research on cultural
reason. What we see for example is that the person who has seen a file at least
once this is the big zero to one, right. Has seen the file, the, the code that
you're asking them to review, at least once, then it will give much better
feedback than before. Right? So if you look for example, usefulness of feedback,
and so how many of the code review comments are useful? We see that if they
haven't seen the file before the code, before the code base, before this part of
the code base, before they give around three. Out of 10 useful code comments,
right? So only 30% of their comments is really useful to the author. But if they
have seen it, at least once it, grows from 30 to 70%. Right. So this is a big
jump, but then you only see incrementally, like until five times, then it
doesn't matter anymore. Right. So if a person has seen the code five times, then
it's plateauing the usefulness of the comments that they are giving. Right. So,
but coe reviews in general, I think it's a really, it's a good practice if it's
done right. To help that more people are familiar with the code. So for example,
if you have at least two people or three people that have seen the code base, or
know a little bit of what's going on there, they don't have to be in a, like the
author of it. But I think they are quite intimate, familiar with the code base
because of the cultural reason we see that. Knowledge really increases that we
can measure, even at the knowledge of the code base increases for teams that are
doing code reviews versus with teams that are not doing code reviews. How is
your experience with that? Is that something that you recommend that you
recognize as important and so on?

**Michael Feathers:**[00:31:42] Yeah, no, I think it is. And it's, it's funny
with this too, because I kind of come, you know, at least I'm gonna become a
consultant, I really got embedded, like in the extreme programming and agile
communities. And so we had like pair programming in the very beginning and we
would basically use that as like a, a way of going and trying to go and arrive
at like continuous code review. And then more recently you have mob programming
and ensemble programming as well. And it's kind of weird about this because it
feels wrong in a way to go and have five people working on the same piece of
code at once, right. In a group. But I can't, you know, the more I reasoned
about it from first principles, I think it's actually a pretty decent thing to
do, right? If knowledge loss is one of the main things we we deal with over time
within an organization and basically making sure that everybody's involved in
the decisions and those, the code intimately, it's probably a decent investment
for an organization to make. It's a hard sell. I'm sure you know, many
organizations, but it's, it's also something which is kind of fascinating. I
think one things that's kind of funny with this. I know that like, this is like,
knowing this pod, you're kind of like asking me a bunch of questions, but with
your background in code review, the thing that I kind of noticed, and I'm
wondering if there's any research around this is that sometimes there's this
issue of like, whether people will really be forthright about their criticism of
a piece of code. And if they're not, do we basically just sort of like let
quality deteriorate because nobody really wants to step up and say, there might
be an issue here, you know, is that a thing which happens in code review that
you're.

**Michaela:**: [00:33:02] This is definitely something that happens and it
happens for various reason, right? It could happen for example, because people
know that even if they are criticizing it, the team and the organization, how
it's structured and how, you know, incentives work and all of that. Right. So
there's a lot of that behind the theme thing. It's too late. Right? So most of
the time the criticism that's not said is because it's too late. So even if I
would say it right now, we are not going to, you know, change it. We are too far
in it. Right. So this is, this is one, one part where this happens quite a bit
and it's really sad. And you know, this is also a planning issue, right? Is the
ticket to big? When are we involving people to give feedback? And so, you know,
people have worked like a month on something. And then you're, it goes higher up
and people say, well, this is from an actual perspective. It's horrible, but it
cannot even say it anymore. Right. They cannot change you're too far in. And
then obviously there are also hierarchy issues, right? So is a, is somebody
allowed to say something? Is it even heard when you're saying something? People
learn if the, code review feedback is not perceived or not received and not
changed people that also learned that this doesn't, you know, it doesn't make
sense. So this is definitely something that happens. There's also something
called, you know the priming bias. So if you see that other people already
looked through the code you're also primed for their answers. So the best thing
would be that people are looking through the code without looking how others
responded and say, well, it looks good to me, or, you know,

**Michael Feathers:**[00:34:35] Yeah. And we're talking to somebody, an
organization, a very big software development organization, and they were
saying, we know we hire great engineers. But the one thing that we kind of
noticed is that essentially we can see through the metrics that the code quality
is deteriorating, but nobody on the team knows because they're just so used to
looking at the same code all the time. They just kind of understand what's going
on with things. So the newcomer would be completely, you know, surprised by it.
So one things I kind of wonder about all the time, is like, can we basically get
new people on the team, people visiting that we'll be able to basically say,
well, you know, you're saying this is great, but I don't understand it. And then
sometimes I might be like a, like a jolt to go and say, it's like, wow. You
know, it's like, are we building a silo of understanding here that basically is
disconnected from understanding of the world. Might be a possibility with that
too, you know, to go and sort of like try to mix things up a bit to the point
where the teams don't become stale in their understanding.

**Michaela:**: [00:35:25] Then, for example, code review feedback, right? So I'm
working also a lot of very often with people or teams on how to give feedback so
that others even can, you know, receive it. And very often there is like, Oh,
but in our team, we understand when we are talking very harshly with each other
or whatnot, right. But this is also a sort of blindness, which I think is very
similar to the blindness for your code that you say, well, if you have to be
very intimate with your team and know that this is actually not a harsh comment,
but it's a joke for you. Then first of all, it's not welcoming to others. It's
not something that you want to leave on because in two years, your team is not a
team anymore than it is today. Right? So if somebody looks at this code comment
they will not understand. Right. And it's also, as you said, it's something that
you're building up where it's not conforming to what we were expecting outside.
Right. So it's really something that's very, it's a very narrow, very blind view
on your system. Right.

**Michael Feathers:**[00:36:17] Yeah. Yeah, no, it's, yeah. There's a lot of
really interesting dynamics around all this stuff. I find it really fascinating.
It's funny with Conway's law, you know, where Conway's laws, you know, saying
that the code structure is gonna end up going in, mirroring the structure of the
teams to kind of like, you know, look at that at a very deep level and go and
say the same thing is true with quality. If the code starts to be kind of messed
up at probably in the case, there's communication problems within the team, in
terms of nobody's able to go and stand up and say, there's something wrong here.
Maybe, you know, I mean, it seems like that kind of effect can occur as well.

**Michaela:**: [00:36:52] Yeah, definitely. There are lot of different issues
behind why quality deteriorates. Right. So what I also often see you and I mean,
what really breaks my heart is that if people want to, but they're just really,
they can't or they feel that they can't. Right. And this is very often from an
organizational perspective. So one question that I had for you is when you were
coming in, I think there's a lot of buy-in from a path, right? So there's a lot
of top down understanding suddenly, Oh, this is important. Whereby teams are
dealing with this bottom up, you know approach where they have to see, well, I
see this is a problem. We feel this is a problem. We don't have enough time to
do it. You know, there's a lot of deadlines and so on and they would have to
communicate up to which I often feel this is really, really hard. And if you
don't have commitment, this is also what developers say, right. If I don't have
to commitment, I just can't fix it. It doesn't matter if I find it important or
not.

**Michael Feathers:**[00:37:46] I'll offer some advice that might be kind of
seen as like problematic in a way. Right. But the thing is, I think sometimes
with a good team, if you can find other people on the team that care about code
quality issues, the way that you do just form a little bit conspiracy with them.
It's kind of like, you're not going to ask for permission. You're just going to
make things better silently and just not really talk about it with the rest of
the team until they start to notice just like through osmosis, that this is a
better way of doing things, right. One of the worst things you can do as a
developer is try to lecture your other developers on the team. Right? Nobody
likes that. Right. And you know, if you have some respect already that you're
able to go in sort of like say, you know, you should really do things this way
and it works. You know, communication wise, that's great. But if you don't have
that, you know, it just doesn't go all that far. But I think, you know, the, the
main thing is the programming can be very fun and cleaning things up can be very
fun also. Right. And if, you know, you can develop that kind of culture
internally within the team. That's great. And worked with a team a long time ago
that really had this interesting thing. They did great work, but part of it was
also a feeling that every other team in the organization was a bunch of idiots.
In a way. So it's kind of like this thing of going and saying, like us versus
them and it formed like this cohesive group with them. The thing is they were
all smart enough to go and recognize that, you know, that was like not the
truth. It was just like this little story they told themselves to basically sort
of like say. Yeah. Yeah, we're doing this great thing. And it's like, who cares
if nobody else really uses it? You know, that way that we intended, it's like,
it's still okay. I think we can basically play those emotional games a little
bit to sort of like not hurt anybody, but also kind of bolster ourselves up as
we try to do things. It's funny, cause I've mentioned this a couple of times in
interviews and stuff that I really feel that I missed an opportunity with the
legacy code book to basically give it a positive frame because even though it
can be kind of treacherous to go and deal with legacy code, it can also be like,
an adventure, if you basically sort of frame it that way, you know, it can kind
of let go and say, look, you know, you're kind of like going through this crazy
jungle and you're learning things and you're picking things up and making things
better as you go. And that can be a decent way of going and motivating yourself
and people around you to go and do some cool things.

**Michaela:**: [00:39:51] I think that a lot of engineers actually like cleaning
up, right. It's like, if you have like a kitchen sink and it's, it's dirty and
then you swipe over it and it's nice. Right? And so I think a lot people also
recognize that and it's, it's a hard problem, right? It's on one hand, a hard
problem. There's a lot of architecture thinking about it. So sometimes maybe
people don't even have the possibility to be involved in such. Higher decisions
or impactful decisions. And suddenly with refactoring, all those decisions are
actually at your fingertips that you can actually change something and make it
better. And, and, you know, it's in the small, but it can have a lot of ripple
effects and all of that. Right. So to think about that, I think can be very
challenging and.

**Michael Feathers:**[00:40:32] Yeah, I think it's a cool thing too, when people
are talking about what good design is, it's kind of like, you know, if you give
anybody a blank piece of paper and tell them to design something, they can
usually do something really cool. But the real skill in design is working with
stuff that's already there, right? Because the number of constraints that you
have basically go into sort of like help you exercise your design skill in a
way, because you have to go and sort of like work around them and work with
them. At least to deeper design insight, working with things where you have,
where your environment is a bit more constrained than than you might hope it to
be.

**Michaela:**: [00:41:05] Yeah. So there were a couple of questions on Twitter
as well that I want to weave in a little bit. So I was thinking about best
practices again. So people were thinking about how can we, you know, show best
practices? I asked you that at the beginning as well about best practices. And
we talked a little bit about transparency and in my recent discussions, I'm
discussing a lot with engineers right now. We also talked about transparency and
how cool it would actually be in an organization or outside of an organization
to see, you know, what are people doing and then also seeing the impact, right?
So you can pick and choose. And there is also, this is also something that we
are lacking a little bit different transparency of best practices. Well, even if
practices, right, it doesn't have to be the best practice, but the practice.
How, how is that team doing? How is this team to doing and similar to what you
said too, when I'm working with larger organization, we also see that all
there's this division and that division and the third division. And then they
think that this division is actually doing the best. Right. And so they're
really proud of their Practices and the other are doing like really bad work.
And suddenly you see that people are working and there are constraints. Right?
So because one is like the driver division. Yeah. Which is a very different kind
of a beast. And if you're working on the website side of things right. Where you
can update things much easier, but it would be really cool to see a little bit
how are people working and how could you do that in an organization? Is there
something that you learned where organizations surface that and show what are
good practices that other teams should adopt?

**Michael Feathers:**[00:42:35] Yeah. Typically with organizations that worked
with them, I had them kind of like moving to like this show and tell mode where
like, you know, once every couple of weeks or something like that, people from
different groups will present what they've done and kind of like just make that
available for people to go and see, you know, where the other possibilities are,
you know? And it's, it really does you know, a lot of it does come down to what
you were saying earlier is that some practices might be better in certain types
of development than others. But the thing is, you know, you get to raise the
consciousness of those things and it's creating forums for those particular
things. And the cool thing with that, as you get developers real used to going
and doing a little bit more, like say public speaking, even though it's
internally within the company to go and describe, you know, the various things
that they happen to be working on and doing. Right. Yeah. I don't know. I don't
know that there's anything that's really like, you know, it's just doing that.
Sorry.

**Michaela:**: [00:43:23] Yeah, communication, right? Brown bags, for example,
that you could leverage.

**Michael Feathers:**[00:43:25] Yeah, I think, you know, nothing. I would go and
add to that too. Is that even though transparency like that as a good, I think
it's one of those things where it has to be discretionary rather than we're
completely transparent all the time. Right. Within an organization. I think one
things that's kind of cool is that when you have. Different groups of people
within an organization working on different things, they can incubate something
and basically not worry about somebody going in saying, well, maybe that's not a
good idea. It's like, no, we're going to try this for a while. And we're going
to go and see what works with that. Then basically go and give you results once
we feel more comfortable with that. And then you get like the enhanced, you get
enhanced psychological safety within that cloister in a way because you don't,
you know, everybody's kind of got the buy-in and the relationship with each
other. And that's just a natural part of being human, right. To be able to come
and sort of like, you know, grow things in a safe environment and then present
them out into the world a little bit. But you know, a lot of this really comes
down to leadership really within your organization. Can you basically go and
sort of like, make it, you know, okay for things to be, not to be okay. Not be
okay sometimes. Right. And just sort of like, make people feel safe to go and
communicate back and forth, then, you know, do the things they need to do. So,
yeah. Culture again, you know, I think I said.

**Michaela:**: [00:44:35] That's true. Yeah. I, this really resonates a lot with
me. So maybe the last question that I want to ask you, and it's a little bit
connected to the Twitter. Things is about testing. So I made a study, actually.
I think it's. I dunno how many years ago? A couple of years, eight years, 10
years, 10 years time flies. And I was looking at unit tests versus integration
tests and system tests. And at that time, people were all over unit tests, like
unit tests, you know, is, is the bullet that brings you joy and happiness. And
I, I feel that this shifted a lot over the last year. So right now people are
more into integration, testing, more into systems testing. What's your thought
about that? And especially in connection with legacy code, are we still because
legacy code, I think a lot of things were still unit tests, right? So we are
connecting, having unit tests and having tests in general around the system to
make changes. Has that shifted as well? What do you think about system tests?

**Michael Feathers:**[00:45:28] Yeah, I think, I think it's shifted a lot with
service orientation, right? When we're doing like microservices and stuff along
those lines. There's like a, you know, We talked about like code being alive,
right? There's this great talk from Alan Kay at OOPSLA, basically in the 1990s
where he basically goes and draws a parallel between code and biology. And he
talks about, you know, his original conception of object orientation being kind
of like cells communicating with each other through messages, by chemical
messages. And it's kind of funny because when you send messages from one cell to
another via chemicals, it's asynchronous and it made me kind of realize it's
kind of like, you know, Well, we wanted OOP to be is kind of what services are
in a way it's like you can send a synchronous messages notifications across
these services and they can be really very well decoupled from each other.
Right. So basically going and testing things at a service level is a very decent
thing to be able to do. The unit testing thing was really very pragmatic when it
comes down to, if you're making a change to a particular piece of code, you want
to be able to go and get close to it. And if you can basically go and write
tests, like at the class level around it, then you're in a situation where you
can go and get immediate feedback about what you're happened to be doing. And so
it's like this way of going and sort of like building. You know, building like
this assurance as you basically go and make changes that you really are doing
the right thing. So unit, it seems like units in object orientation tend to
align around classes or aggregates of classes. And so I tend to see those as
being a unit in a way and that wrong. And it's really all about going and making
it possible to go and get that feedback and, and build, you know a
knowledge-base through tests that basically can go and find out very quickly by
running whether things are working or not. One of the things I've been kind of
throwing around is as a frame recently as that essentially test determined where
your unit in a way that if you can basically go and get an area of code and it's
easy to go and basically test it, then that's a decent, decent definition of
unit as you can ever get. And for you, a unit might be a service where it might
be a class, but it's the point at which the testing comes to difficult that you
basically know that you've got a modularity boundary, that isn't all that great.
And it's just, you know, like a way of going and looking at things in that
realm. So yeah, I don't, I don't really, I think as long as people go and
understand that tests and modularity kind of work together in a very interesting
way. It doesn't matter to me whether you call it unit tests or systems tests the
test will give you feedback about your modularity and that's a cool thing to
know.

**Michaela:**: [00:47:53] Yeah. Yeah. Like the, like the frame. So well, Michael
I think we are at the end of this show, I'm really happy that I could pick your
brains for so long. Is there something that you wanted to let my listeners know
before we are ending? And I will definitely link a couple of things down there
in the show notes, but is there something that you, you know, that you'll want
to end the show with?

Michael Feathers: [00:48:13] Yeah, I guess just basically going and saying that
we're all part of one, we are part of the system as humans working in software
development, and we need to basically take the systems that we work on
seriously. And, you know, I think that seriousness for us means kind of like
looking at them as entities that have their own qualities and we can make them
better. You know, the thing about this that I think it's kind of fascinating is
that if we are going from job to job and place to place, and these systems
remain behind, you know, it's good for us to go and actually exercise enough
care that we leave the place, leave the system better for the next people,
because you know, that's just what empathy is all about.

**Michaela:**: [00:48:53] Yeah. So you show your empathy through your code,
right? In the quality that you leave for the people that have to deal with it.

**Michael Feathers:**[00:49:0] Like, I did this tweet like a couple of years
ago. It's like code is the way you treat your coworkers. Right. And it's kind of
like, it's true. It really is. So...

**Michaela:**: [00:49:08] Yeah. Yeah. I like that end note. Thank you so much.
Um, was a very inspiring talk. Thank you so much for taking the time.

**Michael Feathers:**[00:49:15] Excellent. Thanks.

**Michaela:**: [00:49:16] Okay. Bye.

**McKayla:** [00:49:17] I hope you enjoyed another episode of Software
Engineering Unlocked podcast. Don't forget to subscribe and I'll talk to you
again in two weeks. Bye.
