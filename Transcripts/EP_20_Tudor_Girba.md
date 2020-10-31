# Transcript Episode 20 with Tudor Girba
( intro music )
**Michaela:**: [00:00:00] Hello, and welcome to the software engineering unlocked 
podcast. I'm your host, dr. McKayla. Before we start, I want to update you a 
little bit on my current project. As you know, I'm giving code review workshops, 
and I also working with engineering teams that want to increase their 
engineering rigor and productivity.
Over the next few weeks, I'm still super busy, working with a few large 
corporations, but I'm planning on dedicating August and September posted to 
making progress on my code review book. 
Also, I started to tinker with the idea of building a 
developer tooling for some of the common problems I see, when
working with different teams. Well, If there were only more than 24 hours 
within a day, right. If I start, I will let you know. For now, if you want to 
work with me, have a look at my website: michaelagreiler.com. But now back to today's 
episode. Today, I have the peasure to talk to Tudor Girba, the CEO and co-founder 
feenk, a consultancy company.
Tudor was once an academic, but after his postdoc, he set 
out to bring his ideas to life and started working on visualizing and modeling 
complex software systems. Since 2009, Tudor works on an idea that is called 
moldable development. And with his amazing team, he developed a tool called 
glamorous toolkit.
So I'm super happy to talk with him about his entrepreneurial journey and what 
he learned along this way. Tudor, welcome to my show, 

**Tudor:**: [00:01:22] Well, thanks for having me. 

**Michaela:**: [00:01:24] Yeah, I'm really excited. So Tudor, let me know, how, how did 
you go from this PhD idea and academic idea and probably, but also then the wish to become 
a professor, and now you're working in industry, you're having a consultancy company and 
you're now developing this tool. How, how has that happened? Yeah, 

**Tudor:**: [00:01:48] so. Yeah, I did my PhD and postdoc and around 2009, I 
have this idea that we might be doing something wrong when it comes to how 
developers read code. I think when like this, I was writing a paper and like in 
this field, most papers start with this sentence that developers spend most of 
the time reading code, but then they realize that one of the oldest references 
in this space beats back to around 1979. So my question was, what did we do for 30 years? 
Is it possible that the way we are researching, the way we are looking at this 
problem is fundamentally wrong?. And so that's when first I created this 
method, which is called humane assessment and it starts from the 
idea that I looked at, why developers read code and developers read code, 
because they want to understand enough to make the decision.
So they don't read code like you would read, I don't know, a Harry Potter book or, 
um, or a textbook in physics. It's, you're reading really differently. You're 
reading it with the, or most of the time developers read it with the specific 
intent of figuring out what to do next. And that's called decision-making.
Now, given that developers spend most of their time doing that, then perhaps we 
should stop looking at software engineering as being primarily at the 
construction business and moral decision making business. And, you know, when 
you, when you're changing your perspective from how you look at the problems you 
uncover complete new areas that have not really properly been explored.
So what's humane assessment was at the beginning, was a systematic method for 
technical decision making, and essentially nowadays we would say that every 
single development problem includes a tiny data science problem inside. And the 
way you tackle data science problems is by creating, not by reading, but by 
creating tools through which you extract the information that you want for your 
decision making out of data and everything around systems is data including 
source code and log files and configuration files and everything 
else. So... why should it not be applicable to take all the lessons from data 
science and then apply them to the software development. Now, of course, 10 
years ago, this was not so obvious data science was not a big thing at the time, 
but in the meantime it is.
So this is where it all started. It started from that idea. And now the only 
problem here is that these tools, they all start from the problem, not from the 
data. So you like, you cannot construct the tool when you don't know what tool 
you're going to need before you'd have the question. And now on the other hand 
in software, software it's the most contextual thing we've ever created this as 
human species.
And as a consequence, we cannot predict the specific problems people were 
having. We can predict classes of problems, but not specific problems. And as a 
consequence, um, we can't give them clicking thoughts, because clicking tools bake the 
problem in the button, in the thing you click on and they're, they're too rigid 
and they solve somebody else's problem, not your problem. 
That's why people fall back to the most manual possible way of 
doing things, which is reading because reading is highly malleable. You can, you 
can apply it to anything. The only problem with it is it's horribly slow and 
it's highly inaccurate. And so that, that has to be, that has to be completely 
changed.
And the fascinating thing is. So I basically went around over the last decade. I 
probably talked with, I don't know, perhaps more than 5,000 developers, more 
than 3,000, just over the last few years. And I asked them, do you agree that you 
spent this 50% of more of your time reading code and they say yes.
And then I asked them, so when was the last time you talked about how you read 
code? So not about the code that you read, but about how you do the reading. And 
it turns out this is not a subject of conversation. It's like, it's very, very, 
like very often received like awkward. Like this is a strange question, but it 
shouldn't be a strange question because 50% or more means this is the single 
largest expense, which is nothing larger than that.
Right. And we are spending the largest chunk of our budget on one single 
activity about which nobody talks that doesn't make any business sense. You 
know, every time you're going to, if you, if you want to optimize performance of 
a system, you're going to look and find the largest expense, the largest 
place, which consumes whatever resources and, and that has never been optimized 
because that's Probably where you can gain the largest increase. 
And that's what good reading is in software development. 
Nobody talks about it. It's the largest expense. People are still looking 
for finding, you know, the significant advances  
in productivity and we think that this is the one. 
So I spent the last 10 years studying or researching this one and building various 
kinds of solutions for this space.
And along the way, I didn't do it alone. So I'm blessed to work with an 
amazing team. I've seen it's quite a long time and many of them are researchers 
and we think of risk. Like we are a consulting company thing, but we are 
organizing internally as a research lab. So essentially everyone can do 
whatever they want to do, and we are building something together and, 
because you see, when we set up to, to reinvent a thing that was obvious
for a long time, but has never changed for a long time. And to change that, 
like, there is no charter territory there. It's not like we are applying formula 
because this is a new thing. Like we don't know, we didn't know at the beginning 
how it would look like we just had the good idea. We had the experiments 
for it, but we didn't really know how this would work out.
Would it be practical? Is it scalable to all sorts of different problems? Will 
it work for many languages? and so on. So in that space, you don't know, like we 
don't follow a plan. So it's much more interesting to discover and create 
something new. And that case a tub down follow the plan. Proach is not, is not 
suitable.
And we also think that in fact, software it's almost never in that situation, 
we think the software is created not implemented. And so perhaps we should look 
at software the way we creating software slightly differently, too.  
**Michaela:**: [00:08:36] Yeah, I like this perspective also on, you know, 
nobody actually talks about one of those aspects that we are spending so much 
time on.
So I'm, I'm dedicating my time to looking at code reviewing and activity of code 
reviewing, which, you know, a part, a large part of it is again, reading code 
and I looked at that because when I was looking at Microsoft, I saw 
that, you know, engineers also spent a significant amount of time on code 
review, but nobody, as you said, nobody talks really about how are we doing 
that
You know, it's like, it's supposed to, we know it, right. So we are opening up 
the coat, the editor or whatever, and we're looking at reading code and that's 
it. Right. So how hard can it be? And I think it's a very, very similar problem. 
So I love that you're looking at that as well. And so you said it's human 
assessment method, right?
So you're started, I'm imagining, like you're doing your PhD. I don't know how 
practical it was, but a lot of time you're having like little prototypes, maybe 
some theories, and then you're getting, and having this assessment method, which 
is, it's not really a tool. How did you bridge this gap from, you know, from 
this, well, it's now a theory, it's a methodology and now I'm developing a tool, 
but you also hinted a little bit to it, but I'm not sure.
As you said, like I developed many different smaller methods or tools. So what 
happened on this exploration a way within this 10 years?
**Tudor:**: [00:10:02]  Right. Okay. So first, just about the tiny bit of 
other code reading part. So just to see how far do we go not exploring 
something. So by the way, the reason I very much am very happy that I'm on
this podcast today is exactly because there are not that many places today, 
which talk about what do people do when they already have a system. So this is 
one of those highly recommended. And anyway, so that's why I'm happy to be here. 
But just to say, like, how far does it, you know, like these, these implicitness 
go, where do people read code?
Cause you just said it, right. It's an editor. Editor. It was, I mean, it was not 
a tool that was meant for this. We happen to pram that activity on top of it. We 
can talk about that one, but, but the nature of our tools, the nature of our 
tools highly influenced the way we think about the nature of the problem, 
especially in the digital space.
And this goes all the way from Marshall McLuhan and is his theory on 
how the medium is the message and how the doors that we create together end up 
shaping the way we think. So. Yeah. That's why we are thinking that now we are 
very much convinced that the tools in software engineering, there are not 
just some nice to have optimizations.
But they are essential. And then we should be very careful with the 
characteristics of the tools that we expose ourselves to, because they're going 
to shape the way we are going to think about our systems. But coming back to 
your, coming back to your, to your questions, how do we. Yeah. How did we come 
about building the tool?
So during my PhD, in fact, I started to work. I, you know, so I did my PhD at 
the university of Bern with two professors. Once they found a cousin or Spanish 
stress, and this was a group that was highly into software engineering and where 
there was a culture of creating infrastructures. So one of them, the 
infrastructure that we created or the largest one was called moose.
The project is still active and with moosetechnology.org. And that's probably 
one of the largest software analysis platforms that there was, it started in 
1996 and it's still going on, probably supported about a hundred PhD or 
something like that. And I was, I basically was the main architect of that one 
for about 15 years or something.
So it all at all times when, whenever we were writing a paper, we always had a 
tool that supported that paper. And that was integrated into a larger 
platform that we were. Creating basically at the same time. So the idea that, so 
this, this intertwining between an idea and the tool, I was lucky enough to be 
exposed to it during the PhD.
I would very much encourage any, anyone doing software engineering research to, 
to incorporate this in their research. And so the more difficult let's say the 
more difficult part was generalizing the little things that you see, 'Cause 
whenever you're doing research, if you're taking one problem at a time, usually, 
and even if it's an ambitious research, it's still bounded by 
funding or the things that are still attainable, you know, during the research 
research environment where engineering is still not yet seen as a major 
or as a meaningful contribution to research.
So the bigger leap was taking going from there to having this idea 
that, okay... What if the way we're doing the development is 
fundamentally flawed because we haven't looked at the path of 50% of the problem 
for the last 50 years, not systematically and specifically not an industry that 
was the bigger leap.
And so going from the practical things to, to the method was what I found 
more challenging or yeah. Or the formulating a larger thesis. So what happened 
basically was that in order for us to, you know, in a research environment, you 
really don't have a lot of engineering effort. So we had to build this Meta 
tooling.
And we found that by building these meta tools allowed us to basically create 
papers faster because we could just say, Oh, let's tackle that problem. Let's 
tackle that problem. But if I can already build on top of things that already 
exist, I can do the experiments much faster. So, and then I started to do 
some consulting during my postdoc, and then I realized that
Because I thought you look, we're building all these interesting tools and 
visualizations and others like that. And so let's go in and industry and see 
what kind of things they need. And the original idea was what kind of a magic 
button do I do? We provide the industry, so that they, you know, their life 
becomes instantaneously better.
And then we took the first problem. And then the second problem, then a third 
problem. And the only repeatable thing was that it wasn't repeatable. The only 
repeatable thing was that we always have to tweak our tools to be, to have any 
chance of being meaningful. And so that's basically what led to originally 
the humane assessment and now we have generalized it because over the 
last 10 years we created this new project, which is called glamorous toolkit. 
And yes, now we are close. 
We already  shipped the first version about six years ago. And with that, we, 
we validated that indeed we can fundamentally affect how we read code or 
how we understand our systems and the way we do it is we literally create for 
every single individual problem in development.
We don't just create the code. We don't just create the tests and the code. We 
create the code, the test and the tool with which we read the code, review the 
code, and that can apply. It is applicable to how do I view an object, like from 
a single individual object and it is economically viable. That was a difficult 
thing.
So how do you make this whole thing economically viable so that you reconstruct 
tools for every single individual development problem? And so now knowing 
half that. So, and then once we knew that this is possible, then we set up to 
create what we now call glamorous toolkit. And this is still an alpha version 
pose to be a better version, like you said, and this is based on a complete new 
graphical stack, a whole new set of engines it's available for analyzing, or if 
you can, it can literally be applied to many different situations, 
the both from a static analysis perspective, but also nowadays also
for development purposes. 
**Michaela:**: [00:17:01] Yeah. So I, I actually know, uh, the research group 
very well that you worked on. And I think I read a couple of papers or had, you 
know, similar, you know, relatable ideas where I referenced your work and things 
like that.
So I was also very fortunate to be in a group that build tools as part of the 
research. Right. And so I, I totally understand this perspective, but what I 
found and maybe that's the bigger picture that you were talking 
about. So I was also, you know, working on this little problem over there and 
this problem over there, and even though they are connected, it wouldn't be 
something that I would say, well, this is now a toolkit, a whole toolkit.
Right. So what I would like to understand a little bit more is how did you 
go from, you know, having those different little experiments this 
little tools that are helping to having this, this universal idea of, you know, 
this is how we should do it. And I mean, 10 years is a long time. Right.
So I guess there were probably parts where you went in one direction and thought 
this is the right one. You had to backtrack and, you know, take a different path 
and things like that. So how did you, how did you plan that? Or was it very 
exploratory the whole way through?. 
**Tudor:**: [00:18:20] Oh, definitely exploratory. I don't know how people can 
plan that.
They can probably say it in retrospect that it made perfect sense, but in our
case, it was not like that. So it was, it became immediately 
apparent that there is merit to the thesis, that there is merit to this idea 
that through custom tools we can affect how people reason about systems. And 
originally the first use case is the first set of use cases was this idea of 
software assessment.
So not about how people write the code, we were not talking about that. We just 
about how do you, you know, simple problems, not simple problems, but problems
Like how do you, uh, do agile architecture? How do you steer agile architecture? 
Cause like, everybody talks about it, but like, how you do it in 
practice.
And, and then there were things, even simple things like this, like very often I 
go to conferences and, uh, I ask, I get to talk with lots of architects and I 
asked them, so do you raise your hand if you have a picture about your system 
and everybody raises their hand because you know, that's what an architect does.
And then I asked them, so keep your hand up. If you can bet your salary, that 
the picture is one of the presenters accurate and everybody puts their hand 
down. And so, and so the reason we create those pictures is because we want to 
make decisions, but when the picture is not real, what chances did the 
decisions?
What chances do we have to make the right decisions? So these, this was the set 
of problems that we basically focus on for the first, I don't know, six, seven, 
eight years. And that's one that's where like, this is where it consulting. They 
happened. And then, uh, actually, yeah, I took a job cause I realized, Hmm.
As a consultant, I can just come in and then say something, but I don't have to 
live with the consequences of my actions. So then I said, well, in order 
to validate these diseases, I should take a job in the crappiest system that I 
can find around, like around my area. So I did it. I, and I, I led the 
development team there for three and a half years.
And my main purpose was this was like a terrible piece of technology, like 
really, really bad, 20 years old, but there's not the, not the agent is the 
problem, but like, Just a pile of things put on top of each other. And my main 
purpose there was to my main metric for my team was how many, how many smiles 
does the team emit per day?
You see? Because like, if unhappy, unhappy developers are not likely to create 
happy solutions. So, and a lot of, I mean, development is supposed to be 
the most. The coolest job on the planet. It's super highly paid. There is no 
dangers involved. It's super flexible. Like, I mean, just think of this during 
this time now.
Right? Like there were so many people in the world that got upset with all the, 
with all the disruption in the economy and, and developers probably are the 
least. The least effective group of them. They can still continue to create value, 
they can still continue to generate income. And it's really, really comfortable.
Like if you, if you look at it in comparison with everything else, so we should 
be the happiest group of people. And yet we are not, developers are not happy. 
Uh, they don't smile on a daily basis and they definitely don't smile the, 
every, anytime they hear the word legacy and that's a terrible thing, you know, 
that that's just doesn't, it doesn't fit right.
I mean, so something must be really, really wrong. And so, anyway, that 
was my measure. How many times the developers smile in the presence of that by 
all objective measures, crappy piece of code. And I, and we could do that. We 
could literally smile on a daily basis. And still get that system to continue to 
live and then generate value.
So, anyway, so that was one of the, that, and then afterwards, we started the 
company and to maybe make this idea a little bit more accessible to 
everyone, because whenever you're doing research, you have your own results, You 
can disseminate them into research papers, but then who's going to 
read those 
is if you want to effect reality, you have to make it real. And so we 
created fake as a vehicle to create that reality, that's the 
reason. 
**Michaela:**: [00:22:47] So what reminds me your whole tool and your 
perspective reminds me of the talk that I had with Jerry D major about 
observability. So her company is providing a software that helps you understand 
runtime systems, right?
And so instead of, you know, monitoring your observing, and also your, it has a 
lot to do with visualizing data and, you know, Helping people to understand 
what's actually going on before there is something going terribly wrong. Have 
you looked into observability a little bit? And do you think it's somehow 
related?
I mean, it's, yours is more in the creation of the software and there is the 
runtime behavior, or are there overlaps between the two areas?
**Tudor:**: [00:23:29] Yeah, we have looked at it. And nowadays we,
we created the concept of multiple development, which is about how do we embed 
all these lessons about how do we reason about the system and not having a side 
problem, but have it, the first problem that development focuses on.
So it's not something that is side it's good to have, but it's the first thing 
we don't start from the editor because ideally you should edit after you 
understand, not before. So once you, when you turn this whole workflow upside 
down, then observability is one part of this. So, yeah, it is an 
important thing,it has an economical value to just focus on that
and insert it into the way currently developers work.
But from our perspective, multiple 
development or observability is just one thing that you would not naturally do 
when you practice moldable development. It's not just about static thing.
It's not about dynamic thing. We look at the system as a whole. Everything about 
your system is data. Your API is a data source stories, data, your logs are 
data. Everything is data, and every data is handleable through tools and a tool 
must match the question, not to the problem. And that's exactly what they have 
found from through their observability, from there, from just looking at the 
wrong times.
And whenever you need to reason about how the system works. Yes, you have the 
question you might not necessarily know. You might not necessarily know the 
question upfront, but you do want to have the probes inside the classes of 
questions you will know. So there's this combination between that we can predict 
classes.
So then you can create the infrastructure for being prepared for a class of 
problem, but you don't know the specific problem and that you probably want to. 
And that's something that you have to adapt after you have the question. So 
anyway, that's the relationship; there is indeed a 
significant overlap and those two problems, they came from different from 
different perspectives.

**Michaela:**: [00:25:36] Yeah, sounds really interesting. So I saw on your website 
and there's like a little bit, the timeline that I'm in 2015, I think was 
created. Right? So this was somehow when you started your consultancy company 
and you actually co-founded it with your wife. How does that come about? Is 
she also a software engineer?
She's a researcher. How, how did you decide on, you know, creating your own 
company with your partner?
**Tudor:**: [00:26:01] Yes. So she's not a software engineer, she 
has an MBA. And so she comes from an economical and marketing perspective and I 
think would have probably not existed if you were not for her. And because, you 
know, I don't know, like creating something is not necessarily a synonym with 
making it or with running a company or so, so without
that push. Yeah, we probably would have not started. So she made it 
possible. And so then we started, 
**Michaela:**: [00:26:40] so somehow you are doing your postdoc at that time. I 
don't know exactly the timeframe. And then she drags you out of this research 
idea environment then says you have too much to give to the world.
Let's start a company. 
**Tudor:**: [00:26:54] No. So I finished my postdoc in 2009 and then did 
consulting and then was leading this development in this other company. And then 
the jump was to stop that relying you're on a more secure income and then 
go and take a leap. That was the, that was the push. 
**Michaela:**: [00:27:16] Okay. So because when I started, so I did my PhD and 
then I went to Microsoft and now that I'm self employed, for me this was, I 
mean, probably still is a big deal.
Right? It's a very different mindset. It's a very different, it's also 
different, the skills that you have to have, a different perspective also. A lot 
of things. So when I was doing my PhD, A lot of things are about understanding, 
but not, not voicing your opinion so much. Right. You're just voicing data and 
analysis results that you're seeing.
And then even though you have this data, right, you're still like very, you're 
trying to be very neutral. Like not interpret too much right there. Yeah. Maybe 
one part is also how papers are structured. Right. Do you have, like, you have 
the introduction, some surrounding, then you have the experimenting, then you have 
like just the data and then you have it small part of interpretation and don't 
lean yourself to buy it made out of the window.
And I feel that I feel actually this is somehow it lost a little bit because 
there's so much knowledge and so much wisdom. I call it wisdom in the academic 
community. But we are trained not to voice it, not to say it, you know, don't 
say what you know now, now you're saying, well, everything, I saw everything 
that the data says, and then there is my gut feeling, you know, and
first we tried to rationalize and go away and don't be biased by whatever 
gut feeling you have, even though it's not possible.
Right. But we train ourselves to be, you. Very far from that, at least this is 
my experience. And so now I try to go the other way around too. You say, well, I 
learned so much, I saw so much and now what is my opinion on that? You know, 
and really try to develop this opinion and stake in it. It's an opinion 
that, you know, based on what I saw and what I heard, this is what I think.
And then new data can invalidate that again, you know? So it's not something 
that you develop and then it's like made out of stone and it cannot move any 
more. But I think it's important to have one. And so I see that this is somehow 
something that I'm, that I have to work on actively work on to, to be better at, 
because industry needs it.
They need people with opinions and who better to have opinions that people that 
saw a lot and learned a lot and under, yeah. Investigated a lot. What do you 
think about this? 
**Tudor:**: [00:29:40] Yeah, I definitely agree. At the same time. 
We also have to, like, we, it's very important to have opinions. But at the same 
time, it is important to not become religious about them.
Um, and this is a hard, it's a hard thing to, to navigate, 
especially when you have a vested interest for your idea to be right. So when I, 
when you're like, we have a company and it is so the validity of the company, 
and then the fact that the company can run depends on whether or not, we can 
convince customers that our ideas are right.
But if the ideas are not right and then like, it's a contradiction, right? 
So, and it's a fragile line to travel. And one
thing that we always look at is. We're looking to we're a consulting company. So 
we, that means that we earn money by going into real life projects, or maybe 
people have legacy systems that they don't know what to do with them.
They need to make strategies, decisions. How do they migrate this? How do they 
split it into whatever microservices or so, which is. Not often a useful thing, 
but, or, and if, once they do make that decision migrating from some mainframe 
to some new language, and once they do make the decision, how do they 
navigate that, that time when they still have to construct new features, but 
they still have to fundamentally perform deep structural surgery.
So that's one of those kinds of scenarios. And. So, what is interesting there 
for us from our perspective is that we created the company such that every 
single commercial project we take on, also acts as a validation for our thesis. So 
we only, we would try to pretty much, we are only adding value through the 
tools that we built.
And there's two reasons for that. One is that the tools. So we think
that we creating these tools because we want to be much faster than the team 
that has created the system in the first place. So we want to be faster at 
giving them advice about their own system. Then the team that actually created 
the system.
And, but on the other hand, this also acts as a validation. So we are saying 
that software assessment or this idea of multiple development is pervasive. It 
is applicable in every single situation about software development. And the only 
way to validate that is to put yourself in ridiculous positions and then, see how it 
applies there.
Cause there's no other, I don't think there's any other way. 
**Michaela:**: [00:32:32] I think it's the best way 
**Tudor:**: [00:32:33] to validate. And so what this means now is that we 
literally see, we were, we look at our consulting is pretty much being applied 
research. Because it has this, well, do all the parts. I'm the one who 
we have to print immediate value.
On the other hand, we always look at how did we instantiate whatever we wanted 
to, or whatever concepts we had. So that specific case. And how did 
that, that specific case influence the overall theory and when it became stable 
enough, that's when then we say, okay, now we have, we start to have something.
So, but there is a tension there. Because we were very likely biased 
cause that, so we are saying now multiple development is a new way of 
programming. I really believe that now. Although I shiver every time I say 
that because it's a big claim and then the validation is still highly biased 
because we are pretty much the main per people that have validated it.
So until it's going to be validated by many other people, any other, the 
contexts of that claim will still just be just the claim. But now at least we 
are confident. This is like that. And we will, we are hoping to see if
others may be will, will invalidate it, or maybe they will do something else 
with it.
But anyway, just wanted to say that there's a tension between this. I do think 
that people should have opinions. I do think that people should go and try them 
because after engineering is an empirical science and, and there is no, I don't 
think there's a one the way to get feedback without seeing it in 
practice.
But at the same time, we have to be careful, maybe not to get too stuck 
with it. If something else comes along. 
**Michaela:**: [00:34:18] Yeah, sure, sure. I think there are, there are a 
couple of things. So that came to my mind when you were talking, the first one 
is there's this sayin and it's as strong opinions loosely held, right?
Which I, I think off quite often. And, but also your way that you're describing 
is exactly it resonates so much with me because when I moved from academia to 
Microsoft, for example, one of the things that make me really happy is that 
there was this so what question in the room? Right? So this was the first thing 
that they ask.
So what, you know, First, it was like, Oh, I can visualize this data in that 
way. Or I can, you know, look at this system with this wonderful graph. Right. 
But there's huge. And you know, you cannot look parse it instead. The only 
question is, so what, so what, so what are we, you know, are we saving time with 
that?
I be saving money with that. Are we making people happier? You know, what is 
the impact that you have. And the other way around is, so now that I'm, I think 
it's even a step further, or maybe it's also, you know, just growing, you know, 
it's, it's having this opinion. When people ask you about something that you are 
not a hundred percent sure.
Maybe that's the thing that makes me very are made me very, very uncomfortable 
for a long time. Right. People ask me, so should I do a or B. And I know that 
I don't have the answer for it. Right. But I also know there is no other person 
that has the answer and maybe I know the most about it in the whole room or, you 
know, in, in whatever in the team now.
So actually it's my responsibility to say something about it. I cannot just say, 
you know, I don't know, even though I don't have the full data, we never, you 
know, know everything. So. Even though we don't have every, you know, thing 
answered. And also I'm writing a book now, right. I'm writing a book about Cody 
Rees and then writing it together with a very good friend of mine and a 
wonderful researcher.
And we are also, we are trying to, you know, provide answers and we have a lot 
of data in there, you know, research to back that up. But there are holes 
everywhere right there. And it's like, so should we say nothing about it? And 
now we should say something because we have a lot of knowledge. That's also very 
valuable, but we should make probably make it clear that, you know, there is 
research that says A and there's receptor since B, and this is our 
interpretation.
So I think again, if you didn't make an interpretation, um, and you clearly 
stated as that, and this becomes really, really valuable, even though it's not 
the truth, right. It's, it's just, it's your interpretation at that point. And 
it can change with, with new information that comes along. Anyway, I rambled too 
much, but it's interesting.
It's an interesting conversation with you. And so, because we are, we are 
running a little bit out of time. One of the things that I want to ask you is, 
so now you have this tool, right? And it's actually open source and people can 
download it. Right. You can play around with it. Is that not true? And so what, 
what, what's your, what's your
Idea about this tool. And then also from a, from a company perspective, from a 
business perspective, how, how does that, you know, open source tool fuel your 
company and why you're doing that? 
**Tudor:**: [00:37:34] So our business is a consult is consulting or that's our 
main business, bootstrapping and we're self-funded, which means 
that.
Our goal is to aim and build things for the long run without necessarily 
being concerned with whether or not it does well on the market. We're targeting 
an idea we're targeting to build a completely different kind of an experience. 
That will lead people to think differently. And, uh, so there's, this duality 
gives us that a little bit that space.
So we're making the tool free and open source because of two reasons. 
First is, uh, wishing that we want people to experiment with what multiple 
development means as, as immediately as possible without friction. And the 
second one is that moldable development is applicable at all levels of 
abstractions, including at how the tool is created.
And so the tool itself is a case study for how moldable development was made or 
works in practice. And it's a significant case study. And we think that I shouldn't 
have access to everything on their stack. There shouldn't be no black box for a 
developer. It's enough to developers create black boxes that they put 
out in the, in the open.
And I think that's wrong too. So at least this one should not be such a black 
box and then people should not be afraid the thinker with their own tools just 
because of licenses differently. So that's the premise. Oh, why 
we're doing that. 
**Michaela:**: [00:39:10] And so that it's actually because of that, very often 
people start with a consultancy business.
And as you said, based on what they see in practice, they get a very good idea 
of, you know, what is evaluable tool idea, for example. And then they very often 
transition away from this consultancy company into a product company. That's not 
what you have in mind right now. So you would still like to stay as a 
consultancy company?.
**Tudor:**: [00:39:35] 
So we do have that in mind. It's just not going to be the, the idea that it's 
the product, but this ID is free and it is free and open source 
under an MIT license. So anybody can do what they want with it. But there are so 
many, we are dislocating. I mean, 50% of the software development budget 
is a huge economical value.
If we can improve on that. And we think we can improve on that. Maybe to an 
order up to an order of magnitude. If we can improve on that, like this, there's 
a huge amount of value that is being left in the open, and then the people can 
make other, there are other kinds of, there are other kinds of things 
that people can sell on top of that, if that's the, if that's the concern.
So yeah, this is how we, this is how we are seeing it, we think that 
there's going to be a lot of opportunities on top. Created on top of it. Like if 
you think of, for example, just look at the way we look at multiple development. 
Like it's like this first we have code. Then we had tests as code. Then we have 
infrastructure as code.
Now we're going to have tools as code each one of those, each one of those 
steps, their Cisco infrastructure has created whole new economies on top of 
them. That's what we think this is where we think the value is. 
**Michaela:**: [00:40:57] And that sounds very cool. Cool. So I have one last 
question for you. It's about code review, because I know that you're doing code 
reviews a little bit different in your organization, and you're also thinking 
about them a little bit different.
It's again, you're not reading the code, but instead, what are you doing? 
**Tudor:**: [00:41:16] So again, there are two reasons to read code. One is to learn. And the 
other one is to say, is it good or bad or make a decision about it. The learning 
part, whenever you were learning whenever they were learning the new language or 
so reading is a very appropriate tool when we need to make a decision about the 
code or when we want to say this code
Corresponds to my wishes about that though. Let's say that it fulfills the 
conventions that we have about the code. That's not a reading problem. That's a 
testing problem. It's a regression problem. And regression should never be the 
job of a human, none of in after development, at least. It should be the job of 
a machine.
So just like if we, if I can say what the rule is, if I can formulate a 
principle, let's say this one should not talk to that one. All my services would 
have this kind of policy in place of various kinds of things. It's bounded 
contexts. Like this call should not goes, you know, across bounded context, 
except that through the, in public interfaces, things like that, all of these 
things, these are immediately transferable into it
Tasks. There's just not a functional test, but it's a structural test, but it's 
nevertheless, it's a test. So we do code reviews, like for us code reviews are 
very much like exploratory testing. You you'll learn what kind of things you 
want about the system, but as soon as you know it, you're transformative.
You give, you make it the job of the system to carry it, to carry that role 
forward. 
**Michaela:**: [00:42:50] Yeah, I like that. Well, it triggered so many 
different questions, which I now will not ask. I will ask him maybe a different 
time, because I think this is, I could dig into so many things. Yeah, you just 
said, but. It was, it was really wonderful to talk to you.
It was super interesting to hear, and I'm definitely gonna check out your tool. 
Can you give us some, some website where we can find it, or I will also link to 
it down below that the people can, can go and yeah. Play around with it, develop 
it right. Hands it to change it and see it for themselves. 
**Tudor:**: [00:43:29] So the the tool is called glamorous toolkit or 
the, the environment.
So, and then you can find this at gtoolkit.com. And our company is called Fenk, F 
E N k.com. And we have conversations on different platforms. We are most active 
on Twitter and LinkedIn. Um, so on, especially on Twitter, we post very often on 
a daily basis, usually little snippets on, on how the either a problem problem 
was solved through a custom tool or how the tool looks like inside.
So like our Twitter feed is also a list of kind of case studies and you 
can find us at F E N K com fenk com on Twitter. And you can also contact me at, 
on Twitter at GIRBA. 
**Michaela:**: [00:44:20] Yeah, cool. I will link everything down below. Thank 
you so much for talking with me today and sharing so much interesting 
information.
**Tudor:**: [00:44:29] Thank you for your time. It was wonderful. And thank you 
for the podcast. 
**Michaela:**: [00:44:34] Thank you. Okay, 
**Tudor:**: [00:44:35] bye. Bye. Bye. 
**Michaela:**: [00:44:38] I hope you enjoyed another episode after suf 
engineering unlocked podcast. Don't forget to subscribe. And I talk to you 
again in two weeks.
**Michaela:**: [00:44:49] Bye.
( outro music )


