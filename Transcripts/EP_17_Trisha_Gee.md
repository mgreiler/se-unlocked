# Transcript Episode 17 with Trisha Gee

**Michaela:**: [00:00:00] Hello, and welcome to the software engineering unlocked 
podcast. I'm your host, dr. McKay. And today I have the pleasure to talk to 
Trisha Gee. Trisha is the lead of the Java development advocacy team at 
JetBrains. She's an expert for Java high-performance systems and developed 
software for a variety of industries, such as finance or manufacturing.
She's also involved in open source and speaks at many different conferences. As 
I'm a huge fan of JetBrains. And I always tinkered with the idea of applying there, 
I'm super thrilled to get an insider's perspective from her on how it is to work 
there and how she experienced the hiring process. But before I welcome Trisha, I 
wanted to give you some updates on my code review workshops. Well, at the beginning of 
the Corona virus outbreak, it looked really dark for my workshops. All my 
inhouse events have been canceled and postponed. Yeah, understandably. Right? 
But the good news is that technology nowadays is so empowering. And so I can now 
say that I successfully transitioned to online remote workshops.
I've worked with quite a few people over the last weeks and I start love this new 
remote setting. In the upcoming month, I will work with over 60 engineers from companies 
around the world. So if you want to make your code reviews fast and 
effective, have a look at my workshop at  michaelagreiler.com/workshops. I will also 
link that in the description, but now let's get back to Trisha.
Trisha, thank you so much for joining my show. 

**Trisha:**: [00:01:30] It's my pleasure. Thank you for having me. 

**Michaela:**: [00:01:32] So Tricia, I'd like to know a little bit more 
about your journey. How did you actually get started in tech and what brought 
you to JetBrains? 

**Trisha:**: [00:01:41] Um, how much time do you have? (laughs)
My parents were teachers and they thought back in the eighties, they thought 
that computers were probably a good thing to be involved with. And 
although we can afford our own computers, they would borrow computers from 
school to bring back home over the summer holidays and encouraged me and my 
sister to look at programming and, and getting into computer stuff.
So quite early on probably about when I was nine or ten, I was sort of 
programming, uh, with basic on a BBC micro, I kind of forgot about computers for 
a few years up until I was about fifteen, sixteen, and trying to decide on the next 
subjects I was going to take at school. And, um, I don't remember why I decided 
to take computing, but I decided to go with mass physics and computing because, 
uh, well, computers are kind of cool and I like playing games and I, I kind of 
liked the programming side of stuff.
So, um, and it seemed a lot better than, uh, what were the other options. I was 
thinking about doing maybe chemistry or maybe some more maths. And I thought I'd 
rather go broad than deep. So I picked computing with the intention of doing 
physics at university, but then I really liked the computing side of stuff.
So I studied computer science at university instead of doing physics. And I kind 
of went from there really. I did do, um, I did a placement year, between 
second and third year at university, where I worked at Ford motor company, I'm 
actually doing programming. So that was like a major step for me to sort of 
figure out what it was really like to work in industry.
And also to sort of see how my degree did or did not map well to the sorts of 
skills that we needed to industry. Um, it was really interesting cause the 
topics I was really interested in back in 2000 where like, um, the AI side of 
stuff degree was truant, computer science and artificial intelligence. And I was 
really interested in the artificial intelligence stuff.
The, the community vision stuff. Um, I was interested in, we learnt Java at 
university, so I was interested in that, but those things weren't used at work. 
What was used at work was this stuff that I didn't like, which was the software 
engineering courses and the databases courses and the object oriented design 
stuff.
And so for my third year, when I went back, I went and refocused a lot of my 
choices on stuff that was applicable to sort of daily working as a programmer. 

**Michaela:**: [00:03:57] So you said that you're not, you didn't like the 
software engineering part of it. Has that changed over time? Do you like it more 
now? Or is that something that-- 

**Trisha:**: [00:04:04] I--

**Michaela:**: [00:04:05] stuck with you? And you're not the fond of? 

**Trisha:**: [00:04:08] I didn't get it at university when we were studying, 
bearing in mind that my, my. My parents are teachers. And so I had no real-world 
industry experience. I didn't know what office jobs were like. I didn't 
understand how businesses worked. I didn't understand any of that stuff. I knew 
how schools worked.
Cause I went to school and my parents taught at schools. So when they're doing 
like software engineering and the courses were those two main courses, I 
remember disliking intensely. One was auditorial design and the other was 
software engineering, which were coincidentally taught by the same teacher. So 
maybe there's some of that.
Um, but I didn't really understand that they were teaching us waterfall 
development. So I didn't really understand. I'm sort of a, I've been doing 
programming for like on and off for about 10 years. I kinda got the coding bit. 
I didn't understand how to do, like, requirements analysis, technical design, um, 
you know, any of the sort of waterfall type development stuff.
I didn't understand what I was doing in terms of like "What is the thing I'm 
trying to fix? How do I, what's the problem I'm trying to solve? How do I break 
it down into a technical technical specification or whatever?" I didn't really 
see the value in any of that. I'm just like, just tell me what I need to do and 
I'll code it.
Um, and I didn't see the, the value in. Things like boots diagrams and UML, 
and, and I just, I didn't get that stuff. And when I was working in industry, I 
was like, "Oh right!" Well, some of this, a lot of this is around coordination of 
teams. A lot of this is around. Um, we need to, you ask another person what 
they're requirements are, we need to write that down.
So we share that with other people. We need to have some idea of upfront design 
because it's not necessarily me who's going to be coding it. We need to share 
that amongst the team. So sort of seeing those things in motion, made it a lot 
less boring and a lot more like, right. I understand it. You know? And, and it 
turns out things like documentation, requirements gathering, prototyping, 
technical design was actually something I was actually quite good at because 
I like writing stuff down.
And I like explaining things, which is why I ended up being a developer 
advocate. So, um, Yeah. Once I knew what the purpose was and what the value was, 
then all of that stuff sort of became much more interesting and important. 

**Michaela:**: [00:06:17] Yeah. I can totally relate to that because when I 
think back off my university and when I started, um, studying. Right. 
It was quite a different journey because it had nothing 
to do with programming, so I was doing actually art school. And so we didn't 
use computers at that time. Uh, if you wanted to write, you know, your, your 
German, uh, exercises, for example, in word, that would be a big thing, right? 
No, you had to do it on paper, with the pen! And write it down. Right? 
So they were very romantic about everything like that. 
And then I decided to go for university and study Computer 
science. And so one of the first courses that I did was actually introduction to 
programming. And so we learned Java as well. And we learned, you know, what is a 
For Loop and everything. Right? 
So at the end, I was quite okay with the syntax, writing little programs and 
things like that. And then the second term, after that already, we had what 
was called software engineering one. And what we learned were designed patterns. 
And I had no idea. This seemed to me like to totally arbitrary, you know?
Yeah. I have no idea what I should do with that. I mean, even though we, we 
implemented, for example, a compiler, right? So we were programming or doing 
stuff, but there was no connection between those design patterns, for example, 
and having the compiler. 
You just wrote the compiler in a very, you know, straight forward 
way, how you would make the classes and things like that.
But there was no connection between this course and the other course, because 
those were two different courses. And then on one hand we learned all these 
design patterns that were not applicable for the size of the software that we 
were building. Right. So these are all small programs and smaller systems and 
they are more really to understand your idea behind, for example, you know, 
what is a compiler?
How does it work? Or for example, we also had a little web server or things like 
that, right. But we never applied the design principles or design patterns 
there. And for me, this was a course that I really didn't get. Um, and it was 
really later when I was in the industry, working in industry that I understood:
"Oh, these are designed for veterans and that's why we need them."
So it was very theoretical exercise at that point. And I think that's the 
problem. So if it's so, um, detached from reality and from what you know, 
and what you're actually doing. So how can you make sense out of it? 
And there was, for me, it was this guy out there was just talking some 
jibberish, and, oh, whatever, right? (laughs)

**Trisha:**: [00:08:44] Yeah, exactly. I found that a lot. Well, I mean the 
programming or guidance. Got the program because I enjoyed the programming for 
programming's sake. Right. But, um, a lot of the things I've been thinking about 
is I understand why things are taught that way at university, but I often think 
wouldn't it be better if you, at least one of your courses was.
Let's call it legacy software development. Right? And you get given a large 
system like you're talking about not Qatar, not a pro, not a, not an exercise, 
but an existing large system. And the exercises might be something like refactor 
this in this direction or add this feature or fix this bug because one of the 
things I've come to the conclusion of in the last like 10 years or so is.
Computer science degrees are not, um, apprenticeships for programmers. It's not 
the same thing. Now you do learn a lot more on the job, of course. And the 
computer science course is not designed to teach you how to be an effective 
programmer, it's designed to give you the basics in computer science, but it would 
be nice if one of those basics was how to read existing code, 
which I have talked about before, but how to read 
code, how to, how to write tests to provoke certain types of behaviors, how to 
navigate through someone else's code, how to apply a design pattern that you're 
talking about in an existing code base. Like what does it do? How does it change 
the way it works?
What's the purpose of those things? I've often thought that it would be nice to 
inherit code in computer science courses and have some exercises around 
inherited code rather than constantly writing stuff from scratch. Cause we just 
don't do that in the real world. 

**Michaela:**: [00:10:09] Yeah, that's true. And I mean, if you're writing 
something from scratch or there's this little thing in the beginning where you 
think, Oh, this is hard, right.
But very soon it's easy and it's really fun. And you're just writing your own 
system. But it's not, it's not representative of what you have to do in a day to 
day job, as you said. And yeah, I looked at one of your talks and it was called 
"Reading code is much harder than writing code". Right. And it really reminded me 
of code reviews as well.
Right. One of my favorite topics. And so now you're saying it again and I, umm, 
so Philippe Hammonds is a professor at university of Leiden. And she does a 
lot of research on how people are learning how to program, especially kids. 
How are kids learning how to program? 
And she says the same thing. She says, "Well, they have to read a ton of things, 
right. They have to read programs and they have also to get it by heart." 
Like, for example, the, the nitty gritty of the syntax of the language, how do 
you make a loop, For Loop? For example, how do you, I have different concepts 
for, for the people to really understand the problem that they're solving and 
not thinking, Oh, you know, how was that actually in Python?
You know, when I said four, do you have like to have like some, some parenthesis 
there or not? You know, something like that, but this is everything is automatic 
and you can really focus on, on the problem at hand. And I liked that. Really a 
lot. I like this idea, but yeah, as you said, we are not really doing it that 
way.
We are doing it that, "Oh, let's drive the hell away." Good. Right. I was writing 
a main method right. At the beginning, they would say, "Oh, I forgot everything. 
Why, why it's doing or what is it?" Doing just write it down and then right 
there, you know, print and hello world and that's it. And then you saw it in 
the console, right?
And you are like, "Yes, I'm a programmer now!" And so, yeah, I totally agree that 
it would be so beneficial for people to read more code, but you also said in this 
talk, is that. People don't like to read code. Why? Why is that by 
people not liking to read code, what's what's holding us back?

**Trisha:**: [00:12:09] I mean, whole bunch of 
reasons, but one of the reasons why I came up with that talk.
Yeah, well, I was talking with my colleague. Um, and so she speaks a bunch of 
like different languages. Um, I'm constantly trying to learn Spanish because I 
live in Spain and we were talking about how, how you learn natural languages 
versus-- versus, um, programming languages. And I used to work with her when we 
were doing code view stuff, actually for the code review tool that we have at 
JetBrains, which is why it's all related.
You know, one of the reasons why people hate code reviews is cause you have to 
read other people's code and you hate other people's code. Cause you don't 
understand it because you didn't write it. And. There's a number of different 
reasons why you don't like reading other people's code. One, we just, we don't 
practice it very much.
We don't read code at university. Like you say, you get shown "this is an if 
statement" or "this is a main method", but that's all boiler plate. That's the crap 
that you don't read. That's the stuff you skip over when you're actually reading 
someone else's code. That's the stuff you want your eyes to kind of glaze over.
So we should be learning more like the here's here's a bunch of code. Like what 
do you think it does? Which when we studied English literature used our 
yearbook. And you say, what was, what were the characters feeling? What were 
they doing? What are the things in this piece? We don't many do that with code.
We have to do all the time in the day to day job. We have to go, right? What do 
we think this code is doing? How do I want to change it obviously, but when 
we're learning how to code, we don't really answer questions on "What do we 
think this code is doing?" If you're doing certification, it's always some trick 
question, like: "Given this really simple looking For Loop, what's really printed 
out at the end of it?" So, well that's dumb 'cause I'll just run it. 
So I don't really, I don't mean things like that 
because anything which is like a compiler trick or something, which you can see 
quickly by running something. I think that's dumb. What's more interesting is 
you've got big block of code. Like "what do you think this method should be 
doing?"
It's almost definitely not going to have an output and input cause it's in a 
bigger system. So like what should it be doing? So we don't like to read other 
people's code because we don't practice it enough. We don't like to meet other 
people's code. Because we didn't write it, and that makes it difficult to 
understand.
We don't like reading other people's code because we are conditioned to think 
that as developers as programmers, our outputs, our value is in output lines of 
code. So we're still not, we're not really measured that way these days. You 
don't really measure it on the amount of lines of code that you write, but 
ultimately your organization cares about whether you deliver some features, 
whether you've fixed a bug.
So we're still internally, we sort of think that our value as members of the 
team is about writing lines of code. We don't see the fact that in order to 
deliver that feature, we spent 90% of the time reading. We tend to think of that 
as a massive waste of time, because all I was doing was reading, trying to find 
the place where this bug happened, instead of writing the stuff that fixes it, 
we just, we are not valued for, for reading code for, for unassigned stuff.
We feel we're not getting our little gold stars or our tick boxes for, for doing 
the reading bit of that. So I think that's part of the thing we just don't 
recognize as an industry that although we do probably spend. I'd say 70 to 90% 
of our time reading code. We don't see that as value. We just see it as, "Oh my 
God, this code must be awful because I had to spend 90% of my time reading it 
and understanding it instead of the 10% of my time writing my new lines of code" 
instead of accepting "No, that's, that's how it is." 
Like if you wanted to, what would be a good analogy? 
If you're updating a book, let's say there's an existing, I don't know 
a Java book. And you want to add a new chapter to that book on a new feature in 
Java. You can't just write that chapter and insert it somewhere, like wedge into 
the book.
You have to read the book, figure out like what's the, what the pattern is, what 
the flow is, what the, what the structure is, find the right place to put it. 
Make sure your prose matches the prose in the book, but you can't just write 
something and chuck it in there. Yeah. That's not, that's not how things work. 

**Michaela:**: [00:15:55] So during my PhD, I worked a lot on, uh, 
code comprehension, so helping people to understand code.
And I think one of the main problems is that reading code is a little bit tricky 
because we have only one abstraction. Right? So the code is the code. There 
isn't I mean, obviously, for example, in, in an idea, you could then collapse 
the things and then it might tell that just the method names and things like 
that, but there isn't a lot of granularity there for the abstraction level that 
you have. So one of the things that I did during the PhD was, I was building 
models, especially also a visual models that help people 
understand the code and they were abstracting things. So for example, whatever 
it was, the task, there were some of the things that I just skipped, right. So I 
thought, well, based on what that person now wants to do on the intent of the 
developer, for example, you don't need that information.
And so those methods were really. Trying to help people understand code easier, 
because I think it's a very hard task, even if you're doing it very, very often, 
it doesn't, it gets easier, but there is still a level of hardness to 
it. Right. That doesn't go away. It doesn't go away. What do you think about, 
for example, comments and things like that?
I am actually quite a fan of comments. I'm also a fan of having very 
readable code. Right. So if you can express it with the code, that's the best, 
right. But I'm not opposed on, you know, having any comments there and helping 
people read to understand what's actually happening again. Did this starts from 
CSS code I'm writing right.
With, if I'm defining something, I write there, you know "what this class does, 
where does it belong? Which part of the system is it?" Because it's just making 
it so much easier. You don't have to go and figure it out yourself. Right. What 
do you think about that?

**Trisha:**: [00:17:37] Yeah. Um, so I used to be a big commenter because I'm 
because I've got terrible memory and I can never remember what, what I was doing 
in the code and when and why.
And I'm more likely to rework my own code than someone else's code. Cause I'll 
come back to it. Go, what is this piece of rubbish? And of course it'll turn 
out. This is my piece of rubbish that, you know, I wrote it. And so. Um, for 
like the first 10 years of my career, I just spent a lot of the time writing 
comments going, okay, well, it has to be this way because this didn't work.
And I tried this and that didn't really work and this piece is trying to do this 
sort of thing. Um, so I used to put loads of comments in my code as mostly 
memory AIDS. Um, when I moved to, to Elmax in London and I was working with a 
bunch of people who are eight, doing a lot of clean code B, writing a lot of 
automated tests, um, C excellent developers.
Um, D not afraid of refactoring. They said we don't write comments in our code. 
So I was like, okay, well, this is going to be a big change for me, but let's, 
let's see if I can make this work. And it turned out when I was working. Now I 
didn't write a single comment because, well, there's a few reasons. One, we 
didn't have the clean code.
It was a bit easier. We'd have really readable tests. We had tests that all 
these different levels. So you talk about different levels of abstraction. We 
had like acceptance level test right outside and almost. That's of human English 
down to unit level tests. So if you didn't really know what was happening or why 
you could always look at the tests and they were very readable.
Um, and another thing was, it was fundamental for us to work as a team. This is 
the sort of thing that it would be very difficult to remotely. Although we did 
have a couple of remote workers. We've had programs every day. So if we didn't 
know what was going on, we would always ask the pair, like, what do you think 
this is doing?
And they might have worked on it in a pair, or they might know someone who did 
it. So we would, everyone was always interoperable to ask like, You seem to know 
what this is, what does it do and why? And we also had very technical business 
analyst of like combination between the, an architect and a business analyst.
So when we were like, what is this module? What is it responsible for? What's it 
supposed to do? How's it supposed to work? We would always have them white 
boarding stuff out and saying, well, this is kind of how the system's supposed 
to work. These are how these things work together. So, um, I didn't really need 
comments because there were always people to ask about like what was happening 
and why it was happening.
And I think that's, that's part of the other reason why code is difficult to 
read because. Even even these days, there's this idea that we're all lone 
programmers and we have to sit in front of the computer and read the code on our 
own and understand it on our own. That's why we have to sort of annotate it with 
our little notes.
If we are reading, let's say, well, for star code is huge, right? So it's not a 
tiny, it's not novel. It's not easily digestible. The story with like a single 
thread. It's like a massive, uh, I don't, I like it  have like 26 volumes where 
everything isn't, it doesn't have a coherent thread and they self reference and 
you can't read all of that to find the right thing.
Um, well you can cause that's ordered, but. The, the, the code bases we're 
talking about are, it's not like reading a story. So that means you do need to 
do any sort of other human beings and saying, well, you did this bit, like, what 
does, what does that, how does it work? Why is it that way? So comments are 
useful.
I think if you are going to have to work on the code in isolation, for example, 
open source projects where, um, diff different people were working on it at 
different times, the person who's responsible for that code might not even be 
contributing anymore. They might not be available on your time zone.
That kind of thing. It's really good to annotate. Like you were saying the ways, 
the bigger picture stuff. Why is this here? What's you know, where does it 
belong? What are the, what's the reasoning? You don't comment. The what, what is 
this doing? It's a four loop. It's iterating it. Doesn't that doesn't need a 
comment.
What needs a comment of, why are we iterating? Why haven't we put this into 
different data structure that might be more effective, for example? 

**Michaela:**: [00:21:24] Yeah. So one of the things I'm giving workshops for 
code reviews, for example, and one of the exercises that I do with my 
participants is, and give them some piece of code, right.
And I give them a few minutes to look at it. It's not really large it's so one 
file, um, 

**Trisha:**: [00:21:40] a couple of 

**Michaela:**: [00:21:41] lines of code and they have to try to figure out 
what's going on and everybody sitting and to try and do the thing and to tinker. 
And then after maybe five minutes, because we, I don't want to spend a whole day 
doing that.
Right. I give them the description off the code review, and this code review 
description tells them actually what what's happening here. What's the purpose 
of that code, you know, and what changed. But it's really, really hard at the 
first minute understanding those pipelines, but then once you give them the 
explanation behind suddenly.
The questions changed completely. They understand what's happening here. Why is 
that happening? And then the question becomes very different. It's like, is that 
correct? Would I would do it in that way? And things like that. And I find it 
really fascinating because yeah, as you said, understanding code is difficult 
and if we get some guidance, the whole soft process changes.
So one of the things that I wanted to talk with you about as well is your role 
at JetBrains. So talk to me a little bit, how you started getting started at, 
uh, with computer and with, with tech, but how did you start at JetBrains? When 
did you start there and how did you get into contact with them and things like 
that?

**Trisha:**: [00:22:53] Uh, I've been here five years now, which is the longest 
I've ever worked for anyone. That's it? Massive record. And so I graduated, we 
did in 2001, so I've got like 20 years experience the first 10 years of my 
career. So I kind of stopped the story. Didn't I, when I graduated from 
university, the first 10 years of my career, I did what, what I would advise a 
lot of junior developers to do, which is like hop around from job to job.
I did like, you know, 18 months here, two years there. I did a couple of jobs 
where I was only there for three months and cut your losses fast. That's my 
advice. Get the hell out. Yeah. 

**Michaela:**: [00:23:24] You don't like it. 

**Trisha:**: [00:23:25] Yeah. Yeah. Get out because it's, you know, you can 
always, there's always ways to justify that sort of thing.
A, you can always say I didn't like it, or you can always say it's a contract. 
It was just a three month contract, you know? Yeah. Don't be afraid of, of 
getting out, particularly for women, if it's a toxic environment, get out 
straight away. Yeah. So for the next, for the first 10 years, I kind of moved 
around from jobs, job, always doing Java programming, largely like Java and web 
stuff.
So there was usually a web front end to it, which sometimes I was involved in, 
sometimes I wasn't. Um, then I started working at this company. I just mentioned 
Elmax in London. Where for the first time I'd been reading a lot, I'd read 
about, um, extreme programming. I'd read about agile. I'd read it. I did my 
scrum master certification.
I read a bunch of stuff by Joel. Spolsky like I had this idea of how software 
development, so it should be, and it worked for a lot of places where it was not 
really like that. I mean, I worked for consultancy, which was really good where 
I worked at a couple of different banks in London. That was interesting.
Cause that's where I saw. So does the computing power being used for real stuff 
rather than some of the rubbish time seen before. But when I was working, that 
was a totally different ball game where that people would doing the stuff that 
I'd read about. They were doing extreme programming, they were doing pair 
programming, they were doing retrospectives.
They would doing continuous delivery before. Like they finally was literally 
writing the continuous delivery book while he was my boss at Elmax. The book 
hadn't even been written and we were already doing it. And so all of this stuff 
was, was really mindblowing. And I learned more in the first year there, I let 
more than the previous 10 years or put together.
And at that point I kind of, so I worked there for four years and. My last year, 
I was kind of recent last two years. Really? I was responsible for doing sort of 
their developer advocacy type stuff, because, because why? Because I read a lot. 
I was, I was interested in blogs. I was interested in writing blogs.
I'd been to Q con London. At one of my previous jobs, I liked this idea of 
conferences. I was kind of involved in the Java, the London Java user group. So 
I was kind of involved with people who are part of the bigger community who are 
going to conferences. And, um, you know, as part of the job of user group, you 
were seeing presentations and meeting a wider range of people.
And I thought this is something that I want to be involved in. Um, Elma, 
interesting stuff. I want to, you know, enough about what's happening there. 
That I can talk about it externally. It's great for us to recruit people. This 
is a great place to work. So I was very comfortable going out and talking about 
what we were doing and saying, come and work for us because I really got a lot 
out of working for them and we really needed to, and our team.
So the last sort of couple of years, yeah, I was involved in setting up, um, or 
getting everyone started. Well, I knew everyone wanted. Doing some technical 
blogs, getting like an aggregator for our blogs so that we had like the Mike's 
blogs, adding people who wanted to present from inside Elmax into different 
conferences and presenting, and then sort of organizing the people who did that, 
organizing their schedules and doing a bit of admin stuff really around that 
applying for you can apply to.
To win awards. I didn't even realize this is how it works. Like they don't just 
hand out like prizes, you know, you can submit yourself for various awards in 
the industry like yourself personally, or your organization or the code you've 
written. And so I was doing a lot of that. Yeah, I know. Right. So we are 
consultant a piece of our software, which is very good for us because it gives 
visibility over the, some of the amazing code that we're writing.
So I submitted that to a bunch of like awards and said, look, this is kind of 
cool. Like maybe we should win an award. And then, um, I ended up co-presenting 
at job one with our CTO. I'm talking about this open source piece of software. 
And as part of that journey towards the end of it, I'm like, this is what I want 
to do.
And at the time I was sort of spending one day a week, doing developer advocacy 
four days a week, doing full time, pair programming and developing and stuff. 
And. And I was like, I'm not satisfied just doing the development anymore. I 
want to do more presenting. I want to, I want to invest more of my actual day 
job doing the stuff I was doing, my blog posts at weekends and things like that.
This is like, I was single and I didn't have kids. It was a lot easier to do it. 
So, yeah. So I left and I went to go and work for Mongo DB, where they offered 
me a role, which was like 50% engineering and 50% advocacy. So that I thought 
that was the right blend because I didn't want to move away from the engineering 
particularly.
Being a woman in technology. The first question people ask you, I'll call you a 
real developer. Yes. I'm a real developer. So, you know, I really wanted to make 
sure that I could answer that question truthfully. Yes. I am developing stuff on 
the Mongo DB job driver. Um, but over the course of that, um, one year talking 
about the Mongo DB Java driver conferences, and then I realized that my real 
skill with it is, is showing people how to, how to code stuff.
Like I I'm, I'm a. I'm a good developer. I'm a solid developer. I really, my 
four years working at Elmax. I got to know intelligent idea very well. And I 
realize, um, I'd spent 10 years working as like an ordinary developer using my 
IDE in a very ordinary way as in not really using it very much. Um, and so I was 
demoing how to build Mongo DB applications, using intelligent idea and sort of 
showing things like.
Code completion and like templates and all these things that I learned to Elmax 
um, when I was paired programming with people and over the course of that year, 
then, um, how to use the boss of JetBrains developer advocacy. He kind of came 
to me. Well, actually I asked him questions about how to do developer advocacy 
in a, in an effective way.
And then he said at the end of that conversation, he's like, yeah, Do you want 
to come and work for us? I was like, well, it seems a bit rude because I'm 
trying to get ideas from you about how to be an effective advocate at Mongo DB. 
And so over, like over the course of the next six months, Mongo Debbie's 
direction went in a particular way.
I mean, they are a database company. They have very few Java developers. My 
specialty was like coding, Java app. Occasions inside the IDE using a Mongo DB 
backend, but it really, they, they carried on going in a particular direction 
and I saw that my career needed to go in a slightly different direction. So, um, 
you know, it was like an amicable Orica breakup, really.
Um, and so he said, come and work for us. And so I, I went to go and work for 
them. 

**Michaela:**: [00:29:25] And so how did the hiring process really work? I'm 
very, very afraid of hiring processes and, you know, approving myself, even 
though I went through several walls, also, these really large. Large 
organization hiring like they do at Microsoft, but I really don't like it.
So how was that for JetBrains? 

**Trisha:**: [00:29:44] How did you experience that? I, I already had, I had 15 
years experienced by this point in time, I was sort of, I was famous cause I've 
been speaking at conferences. I had a blog and, but it was it's the first job 
I've ever not had an interview for. So I was literally headhunted for that role.
I said to Hattie in November. Yeah. Okay. I'll I'll yes. I'd like to come and 
work for you. He's like great. Here's your contract. You're starting again. I 
love that. Yeah. I love that. The first time. So I had a lot of jobs in London, 
like I said, I've, I've moved around a lot and I was quite involved in the 
London, Java community.
And even with all his, that I'd been using my equipment agents for, for all of 
my roles before then I'd have to go through a formal process for all of my other 
jobs. But no, that was the first one. Why there basically, because my, I had a 
pool folio by then, I'd already been giving demos on intelligent idea at 
conferences I'd already.
Blogged about how to do stuff. So 

**Michaela:**: [00:30:39] that's also a direct show off of what you're going to 
do there. Right? It's not something that's a byproduct, but it's, it's your 
work, right? So you're actually, you see what you, they are hiring you for. 
Right. 

**Trisha:**: [00:30:51] It's a very different thing from, from programming. The 
programming interviews are.
100% broken and I can rant about this for a long time. If you really want 
programming interviews are very, very difficult. It's difficult to set and 
difficult to answer because we really don't know what makes a good programmer. 
And we really don't know how to measure that. And we really don't know how to 
demonstrate our value as a programmer.
One of the values I have as a programmer is asking stupid questions. Like, why 
is it. Doing that. Right. But I can't ask that in an interview because you 
haven't given me an application enterprise application and ask me to fix a 
problem. So you can't see what my superpower is. My other superpower is 
documenting code that no one else understands because I'm really good at that.
And I like that, but that doesn't come up in interview either. And no one 
thinks, right. Let's go find a developer who can document code that no one else 
understands, right? People think I need you to write lines of code. This is why 
interviews are fundamentally broken. Anyway, what, what you're getting from real 
technical interviews, what you're really getting is it's more like dating.
How does this company work? What, who are the people in this company? What sorts 
of things do they value? And who am I as an, as a developer? What sorts of 
things do I care about? Like, am I attest first hand? Person or their test first 
type of organization. Do I want to be able to pair occasionally, do I need to be 
able to ask questions?
Because sometimes I don't know what I'm doing or do I want you to just leave me 
alone to do my own thing? So really technical interviews should be more like a 
date. Like, what is your style? What is my style? Are we going to get on quite 
well? But we haven't really recognized that. For, for advocacy, it's much, much 
easier because we can demonstrate exactly what we do.
Like you say, it truly reflects what we do. How do you had seen me presenting a 
Java zone? He knew what I was capable of. He knew he'd seen two different types 
of at least two different types of my presence. One is a very opinion based 
where I stand up and walk around, like the reading code one that you were 
talking about and the other is the live demo where it like live demos are.
Really difficult and, um, lots and lots of work. Um, but I really liked it 
because this again was my way of saying yes, I am a real programmer watch me 
code. Um, but he'd seen me driving the IDE. He knew that I knew how to use 
intelligent idea. He knew that I knew how to demonstrate that to other people. 
So like he didn't need to interview me.

**Michaela:**: [00:33:04] What I really find interesting is that you repeatedly 
sad that. You are trying to prove that you're belonging somehow where you are. 
Right. And I have the same feeling. I mean, I'm, I'm in technology in 15 years 
and. I have the constant feeding still now. Right? Like I did my bachelor's in 
computer science.
I did my master's in computer science. I have a PhD in software engineering and 

**Trisha:**: [00:33:28] still am like, yes, 

**Michaela:**: [00:33:30] I know what I'm talking about. I can program. And I'm 
still like, learning like a maniac right now. For example, I'm refreshing my 
Java script knowledge. Right. I'm learning a new language. I'm learning now, 
Peyton, because I feel like with Java and teashop, I'm outdated.
Right. And I want. I have this feeling that I have to prove that I belong over 
and over and over again on one hand, it's it's 

**Trisha:**: [00:33:51] a little bit tiresome, I feel, but on the other hand it 
also keeps 

**Michaela:**: [00:33:54] you sharp, but yeah, I find it really interesting that 
you are also expressing that a little bit. When, when you're talking about how, 
how you behaved over the last 20 

**Trisha:**: [00:34:04] years, I feel over the last five years, certainly since 
I've been at JetBrains.
A lot of that feeling has gone away in a good way. And part of that is because 
I've been presenting at conferences now for seven years. Um, having a little bit 
of famous, quite helpful, because you don't have to prove yourself when people 
come up and say, Oh, you're Trisha, gee, I saw you talking about, but I 
don't have to start with I'm Tricia.
I am a real programmer, right? Yeah. So I built up that portfolio is a public 
portfolio. So that, that does help. I do a bunch of screencasts now as well on 
YouTube. And, and so I'm showing how to, how to demo the IDE, but also I've had 
an opportunity, particularly now, as a developer advocate, I've spoken to way 
more developers than you do when you're working inside a small team.
So when you're working inside a team, like you. You have to prove yourself when 
you join a team, this is true of anybody. It doesn't matter what color you are 
or what race you are or what gender you are. When you join a team, you are 
having a, again, it's like a dating thing. You're getting to know them.
They're getting to know you. You want to, you want to start with your best self 
and say, look, I'm good at all these things, you know, you want to prove 
yourself when you joined the team that's normal. Then once you get into that 
position, they should accept you and you should feel comfortable being part of 
that team.
But. You're you've only had to do it to like half a dozen people or 20 people 
maybe or whatever. Um, and every time you move on to a new team, you have to do 
the same thing again and again, as a developer advocate, I get to speak to way 
more developers now. So I just, at the conferences, you speak to like 20 people 
at one conference and.
You no longer feel the need to be like, Hey, I'm Tricia, I'm a real programmer. 
You just can't start off with, like I know by now I know I'm a real program, 
right? I've spoken to a lot of you. I know what your problems are. Not all of 
them, obviously, but I've heard, you know, a lot of people saying, I don't know 
how to do this thing.
And I'm like, Oh, I know that. Well, what about this stuff? And I'm like, Oh, I 
know the answer to that. Or how do you think about that? And I'm like, Oh, I 
don't know anything about that. But I do know someone who does know that thing, 
or I do know which words to Google to find that out. So having spoken to lots of 
people are having much better idea of what my strengths and weaknesses are.
It makes me much more comfortable with, with being me. Like I no longer feel the 
urge to go into if I go into, um, A big technical conference, maybe, you know? 
Well, there's one that I know well, and I don't need to prove myself, but if 
there's one, let's say I go into JavaScript conference, I'll be much more 
uncomfortable because I don't know anything about JavaScript.
But I do know that I know a lot about Java. I do know about technical 
presentation skills. I do know a lot about our IDs and I'm comfortable now with 
what I know and what I don't know. And that gives me that, you know, people come 
up to me and go, Oh, well, that's a really stupid way to write a JavaScript 
statement.
I'm like, yeah. Okay. If you tell me that's true. I don't know anything about 
JavaScript. If someone comes up to me and says, that's a stupid way to do that 
thing in Java, I'm like, well, you've got your way. I've got my way, whatever. 

**Michaela:**: [00:36:48] Yeah. I think maybe it has also a little bit to do 
with growing pain. Right?
So every time you're moving, you're changing something. You're shaking things 
up. You are in new territory and you have to somehow prove it also to yourself. 
Then, you know, you. You know what you're talking about. Right. So I think, for 
example, for me leaving Microsoft meant also leaving sort of some of the 
Microsoft technologies behind.
And now I'm, I'm looking at, for example, the startup scenes and different, you 
know, it's, it's, it's actually my tech Pablo that I'm right now in, and it's a 
lot of JavaScript, a lot of react that's going on there. Right. And I'm like, I 
have no idea about react and it really bugs me. It's like, Oh my God, something 
is missing.
I cannot, you know, I don't know what people are talking about. So now it's on 
my list that I have to learn that. And, um, and I think it has to do with this 
growing pain that you are changing, that you are doing something you, as you 
said, like you're doing. Your thing 

**Trisha:**: [00:37:43] already for 

**Michaela:**: [00:37:43] quite some time. So you're settled and you're knowing 
that, you know, the things and, um, 

**Trisha:**: [00:37:48] yeah.
And I think part of that as well is that one of the, one of my sweet spots. So 
one of the things that I've been, um, have made my area is the new, new upcoming 
bits of Java. So I know if I'm like right on that straight away, There's just 
almost no one knows that stuff. Cause it's brand new. The only people who know, 
who know it better than me are people who read way more than me or the Oracle 
developers themselves.
So that's also a benefit. Whereas if I'm going into something like, um, like 
spring is a problem for me, for example, I don't really know the spring, spring 
framework very well. I've used it a bunch, but I know there are lots of people 
out there who use it all the time and they use it in their way. So yeah, like if 
I was going to be, when I was doing my spring demo last year, Had a certain 
element of, I've either got to read like everything to, to get to know this 
really well.
Or I've got to put myself into that mindset, the sort of beginner's mindset of, 
okay, this seems to be the most effective way to do this. It appears to work 
like, but there are plenty of other ways to do stuff. 

**Michaela:**: [00:38:46] Yeah, yeah. Yeah. That's true. 

**Trisha:**: [00:38:48] So one 

**Michaela:**: [00:38:49] of the things that I wanted to talk with you about is 
the development processes at JetBrains.
Chad finds is definitely one of the companies that I always think about I'm 
applying and working there. So if I applied there, how would, you know, how 
would the development process look like? What, you know, what would I do? Would 
I write code what I have, you know, a test environment. We have testers there, 
you know, how does that all work?

**Trisha:**: [00:39:14] Um, so Japanese, I don't know if a JetBrains is unique, 
but JetBrains is, is a very interesting sort of organization in that it's very 
developer driven. The people who started the organization were developers and 
they created an IDE for them as developers. So everything, everyone from the 
bottom up is, is basically a developer.
Um, it's interesting for me because, um, I've worked one of what to large 
organizations, they're all quite command and control. So you kind of, you, you 
know, there's like a hierarchy to navigate, to, to, to ask questions or to, to 
feed stuff back Japanese doesn't really work like that. It's more like, um, It's 
more like a network.
It's more like a sort of ecosystem. We've got a thousand over a thousand people 
work at JetBrains. Um, but really everyone's still any like two levels away from 
the CEO is really flat. Like my boss is Hattie and Hattie is he reports directly 
to the CEO. 

**Michaela:**: [00:40:04] Yeah. 

**Trisha:**: [00:40:04] Yeah. And, and my team is like 20 well. So now I'm, I'm 
a team lead of, of the Java advocacy team.
So I Malheur reports to me. So we have like a tiny team. Um, but the, the 
developer advocacy team has like 20 people who report effectively to sort Patty 
who has his boss and. The same to some extent with the other developers. So I 
think there's something like 300 developers on intelligent idea, but I don't 
think, I don't think that's like in some sort of really strict hierarchy.
And I kind of know it's not in a strict hierarchy because the way I interact 
with the, with the developers, cause I don't develop on intelligent. 
Specifically myself, is that I'm usually doing a video or a blog post on like, 
what are the new features unintelligent I did? And the way I like to approach 
those is not like, here's, here's the button, click this, do this.
It's like, okay, what is this feature? How would it help me as a developer to 
get to do the thing I'm trying to, trying to do? Like, I don't really care about 
what the feature looks like. I care about what I want to use it for. I'm always 
trying to come up with these videos and blogs to say, let's say we have this 
sort of problem.
This is the feature that will help you fix that problem. But often when I'm 
doing those, I have to, to figure out what the feature is, how it works and what 
sorts of problems it solves. And in order to do that, I usually speak to the 
individual developer who created that feature. Like, I don't, I don't have like 
a single point of contact.
And when I'm asking them, like, why did you develop this? They're like, well, it 
just, it was a problem I had, so that's okay. Or it seemed like a good idea at 
the time, you know? So a lot of, a lot of the organization, they, um, the 
developers. They are dog food in the product because they write intelligent idea 
and they're using intelligent data to intelligent data.
And they're using Kotlin in intelligent idea to write intelligent idea. So 
Kotlin and, and intelligent idea, or kind of, um, there's got the symbiotic 
relationship because the developers are like, Oh, wouldn't it be nice if we had 
an inspection, which showed us when the code looks like. This. So that's why the 
IDE particularly for, for Java, cause they're intelligent, their code base is 
still has a good chunk of Java as well as some and stuff.
You know, the intelligent idea, Java features are always just expanding 
ridiculously because our developers go, Oh, this would make my life easier. And 
that really helps to really helps with our users because they're like, Oh, that 
makes my life easier too. But so, yeah, so we do a lot of dog food. It seems to 
me there's a certain level of the developers can kind of more or less pick what 
they want to work on this year.
We've actually got a roadmap. So we have a product roadmap and the plan is to 
kind of try and do features, which go towards that product roadmap. But I think 
this is the first year I've ever seen a product roadmap. Usually it's much more 
if it's, if it exists, it's much more informal. So the development organization 
is, is very, um, It's kind of where I think a lot of developers would like to 
work.
It's kind of like, we just kind of trust you to get on with your job and just, 
just do it. Yeah. And they're, so they're all like they're all coat. Well, a lot 
of them, most of the intelligent idea develop because our in st. Petersburg 
where we have a big office, we have a bunch in Munich as well, where we have our 
European development office, but then all of the developer advocates, all of 
ours, there's like 20 of us.
We're all remote. And we will work. So I'm working from the South of Spain. 
Yeah. Malice, India had, he's actually had, he's only about two hours away in 
Malaga, but we have never, ever met up in Spain ever in the Lake seven years 
known him. And we always meet in like London or Amsterdam or New York or so, or 
some Petersburg or Munich as it.
Yeah. There's people in the States, people in the UK. 

**Michaela:**: [00:43:26] So, yeah. Traveling a lot as 

**Trisha:**: [00:43:27] well. Well, not right now. 

**Michaela:**: [00:43:30] Yeah. That's what I wanted to ask you about. What are 
you doing right now? What does an develop an advocate do during a pandemic? 

**Trisha:**: [00:43:37] Oh, so yeah, this, this is. There's one good side of 
this, which is that I'm working on a lot of content.
I'm doing a lot of blog posts and videos. So I don't really have a boss who 
tells me what to do. I have like an internal customer who gives me suggestions 
on things she'd like, and she's always sort of saying, well, we need these 
videos. And she's been saying for like three years, we need these 42 videos.
And I'm like, yeah, I guess I'm averaging about three years. It's gonna take 
awhile to get around to doing them. And in the last like three weeks or so, I've 
done three videos already and then way more videos. More blog posts. I'd already 
cut down my travel a bit. This year. I'd only committed to six events.
Um, and usually do sort of eight to 12 events. Something like that. To be 
honest, I'm really happy. I'm not traveling this year. I just really, I just, I 
think I really liked the travel. I really liked the conferences I worked 
remotely and, uh, and I live in Spain where I don't really get out very much. To 
people in Spanish, out here very much so I like conferences cause I get to go 
out and connect with human beings and do stuff.
But my kids are two and four now. Um, one of them is at school and I just really 
don't need to be jetting off every two weeks or so to spend four days. I'm not, 
I don't spend four days conference. He spent like a day getting there. Day, 
prepping a day, give it like an hour, giving the presentation another day, doing 
whatever else.
And then another day getting back and you just you're like, I just gave an hour 
long presentation. It just seems like a massive waste of my time. So I will be 
doing some more virtual events, more webinars, but honestly, I'm just really 
looking forward to doing more writing and more video stuff right now.

**Michaela:**: [00:45:06] Yeah. Yeah. I can't imagine. And I can totally relate. 
My kids are also two and four as a yeah. You're talking about okay, Trisha. 
So thank you so much for, for being on my show today, we talked about so many 
things. Is there something that we haven't covered that you would like to, you 
know, Let my listeners know, or you know, that you want to throw out.

**Trisha:**: [00:45:25] So, yeah, hiring and other Java developer advocate. Um, 
if anyone is interested in playing, I didn't actually talk that much about 
developer advocacy hiring process. So I got hired. But without a process because 
I was already well known. Our hiring process is we, well, first you have to 
apply. If you don't apply, we can't interview you and you will be interviewed by 
me and an HR person.
You will usually have to submit a, uh, as an example, post, it could be 
something you've already written. If you already have blog posts and example, 
screencast or video, if you've already got one, that's great too. I mostly want 
to look for evidence that you can use intelligent idea and you know, what the 
IDE is for.
And it's not just a text highlighter, you understand, using the keyboard to 
navigate you understand life templates, shortcuts, all of those sorts of things. 
Yeah. Yeah. And then, uh, and then mostly the most important thing for me is 
probably gonna be team fit because Matt and I, we work quite well together and 
I'm just looking for a third person, like I'm nominally in charge of the team, 
but I just really want as the three of us, whoever we are.
To work well together to gel well, to be able to compliment each other in our 
skills. So for example, I'm not looking for someone who's an expert in, in Java, 
in like cutting edge Java stuff, because me and Matt have both got that. Like we 
both are on top of the new versions of Java and I'm not looking for someone 
who's necessarily.
Going to be a very experienced developer advocate because I've got some 
experience. I've got plenty of experience. Matt has got some experience. We can 
help teach a lot of that stuff. I am looking for someone with complimentary 
skills. For example, I know nothing about AWS or cloud or DACA or any of that 
stuff.
And I would really love someone who understood that stuff. 

**Michaela:**: [00:47:06] If somebody wants to apply, they should drive an email 
directly to you or go to JetBrains, uh, slash and jobs, and then apply there. Or 
how 

**Trisha:**: [00:47:16] I'm just having a look at this. You'll probably hear me 
typing. I think it's JetBrains. Yeah. Dre jetbrains.com/careers.
Careers. Okay. Um, and there, you should be able to look for a developer 
advocacy role. They are sometimes listed as being, as having an office location, 
but they're not, they're fully remote. I think the office location might be just 
literally, um, you know, like a, a thing. The system makes you put in that. So 
developer advocacy roles are they're fully remote.
Ideally we'd like someone in North America because we don't have someone 
covering that geography and time zone. But, um, yeah, it's a fully remote 
position. 

**Michaela:**: [00:47:51] Okay. Okay, cool. Very cool. So thank you so much for 
taking the time to talk with me. I hope you enjoy the rest of the day and, um, 
thank you so much, 

**Trisha:**: [00:48:00] Tricia.
Thank you. It's my pleasure. Bye 

**Michaela:**: [00:48:03] bye. Bye. Hey, if you enjoyed my show, it would mean 
the world to me. If you become a Petron, you can find all information on 
se-unlocked.com/patron. I have some exclusive perks for you. Another awesome way 
to support the show is by helping me spread the word, you can send the episode 
to a friend or share it on Twitter, Facebook, LinkedIn.
Well, thank you so much for listening to the soft engineering and luck podcast. 
Don't forget to subscribe. And I talked to you in two weeks. Bye.


