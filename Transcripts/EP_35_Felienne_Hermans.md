# Episode 35: How Programmers Think and Learn



**Michaela:** [00:00:00] Hello, and welcome to the soft engineering unlocked podcast. 
I'm your host, Dr. McKayla. And today I have the pleasure to talk to Felienne 
Hermans about how we can learn to program faster, better, and more easily. But 
before I start, I want to tell you a bit more about ConfigCat - today's 
sponsor of this episode.
ConfigCat is a feature flag management tool that allows you to seamless and 
effortless switch features on and off in your application through an intuitive 
user interface. Everyone on the team, independent of the tech skills, is ready to 
go within 10 minutes of training to configure the feature set that your user 
sees based on rules.
You can even start to do sophisticated A/B testing, hassle-free and 
intuitively within a few minutes. 

Super interesting for my listeners doing 
business within Europe, ConfigCat allows you to have your data distributed in 
the European Union only so you can easily stay GDPR compliant. So if you want to 
tap into the sheer possibilities of feature flag management, go have a 
look at https://configcat.com/

I tried it and I promise you're up and running within few minutes. Feature flags 
mean faster deploys with less risks. Less risks is also the generous free plan 
of ConfigCat. You can start for free today. And with each paid plan, they 
plant a tree. Cool. Right? 

But now back to Felienne. Felienne is an associate 
professor at the university of Leiden and investigate how we can best learn how 
to program Felina is also active in the developer community and organize several 
developer, meetups, and conferences.
She's a big fan of Lego and served for many years as a lego judge at local 
competitions for kids, her passionate for bringing young kids into TAFE also 
leads her to being a teacher at the high school in the Netherlands. Currently 
Felienne also writes a book called Programmer's brain explaining what happens in 
our brain when we learn to code, but also when we read and write and try to 
understand code.
So I'm super thrilled to have Felienne here with me, Felienne, welcome to my show

**Felienne:** [00:01:57] Michelle. Thanks for having me. 

**Michaela:** [00:01:59] Yeah, I'm really, really happy. It took quite some time, 
but now you're here. And I'm so curious to learn more about the Programmer's
brain, because this is an area that I'm super interested. I mean, we both 
have been doing the PhD together right.
In the same research group, but we were sitting in the same office and I was 
researching program comprehension. So how are people understanding code. And so 
this is so close to what really interests me, what really fascinates me. So I'm 
super thrilled to learn more about that. So can you tell me a little bit about 
the book, but also your research?
Because I think the book is very close to your research that you are doing at 
university of Leiden, right

**Felienne:** [00:02:38] Yeah. That's correct. And maybe we have to go 
back about what led me to write this book and what led me to, to do this 
research because initially what exactly we were doing our PhD at the same time.
And then I wasn't so interested in program comprehension. I was more interested 
in developer tools at that time, but then what happened is I started to teach. 
And then when I started to teach, I realized that, Programming is so hard. I 
think I sort of forgot because I was already programming for such a long time 
for myself, that all these parts of programming, like there is so much you have 
to get, right.
If you're making a program, you have to make a plan in your head. Like this is 
where I'm going, which requires you to understand the domain, the problem that 
you're solving. But at the same time, you also have to be like ridiculously 
precise. You have to get periods and semi-colons and brackets and everything 
has to fit at so many different levels that when I started to teach kids, it's 
like, Oh my God, this is so hard.
Why is this so hard? Why is it so hard, for example, for children to remember 
syntax? Why is it so hard for kids to remember what I was working on there? 
Sometimes I saw kids was very engaged in a problem, and then I explained 
something to them. And then a few days later it was like, Oh, I have no 
recollection of this.
And I was like, but I explained this to you, like just a few days ago, how do 
you not remember? Or I saw them very determined of, Oh, I'm making a game and a 
cat has to catch fish or something. This is what I'm doing. And then they sorta 
got sidetracked. And then you, you walk past five minutes later and it was like, 
Why aren't you making a game with a cat and it goes like, Oh yeah, that's true.
I totally forgot. He goes, I fell into some hole of a variable or a loop. So 
that just got me really, really excited to understand more about how do people 
think, how do people remember things? And of course there was so much research 
already that wasn't so connected to programming. This is relatively easy to read 
all sorts of introduction books into cognition and cognitive science.
But then I realized there wasn't really a book that explains. Beginner, 
cognitive science in the context of programming. So then I was like, I could 
write that book because now I know a lot. 

**Michaela:** [00:04:51] Oh, yeah, very good. And so I actually watched one of your 
talks. I forgot where it was, but it was really good to talk about programming 
and understanding program.
And you were also talking about kids and when I watched that, and also when I 
heard you talk right now, I'm wondering, but can we actually generalized from 
kids to adults? Right. So do we struggle the same way as kids struggle. And 
I definitely do see like this abstraction levels. Right. You have to be very 
detailed as you said, with the syntax and semi-colons, or even like tabs 
and so on.
And then you have like this, this larger vision that you have to keep in mind, 
but do we struggle in the same way or do adults have different problems also 
compared to kids?

**Felienne:** [00:05:31]  That's a great question. So in general, adults and 
kids do learn and struggle at the same level, but that is the case for Morphis 
adults.
So if, if a 10 year old is learning to program and let's say your next door 
neighbor is also learning to program, and they're not a programmer, right. Then 
they will very much struggle with the same thing. However, if you, if your 
question is about expert programmers, then they don't, then they also struggle, 
but they struggle in different ways.
So you already know Java and now you want to learn R then your struggle will be 
different than someone that doesn't know Java that is learning. Whether that's a 
kid or an adult. 

**Michaela:** [00:06:09] Okay. Yeah, I see. And so something else that, that 
I also thought 
when, when I heard you talk about all different concepts and you were saying, 
well, experts known something different than like a novice or, or struggles 
differently.
Like for example, I'm trying to learn new programming languages. Right. And so 
I, I know Java, I know C-sharp, I know Python and a little bit of JavaScript, 
but. You know, the further it goes away from the languages that I initially 
learned with her Java and object oriented programming, the more I'm struggling.
Right. So I'm struggling, I think, because I have all these preconceived ideas, 
mental models, notions of, you know, what's right and what's wrong, how to do 
that. And then sometimes I feel like, Oh this doesn't work so well now in Python,
right there, maybe this is not that I'm not meant to do it that way.
Right. And so how can, how can people that already know a language? How can they 
overcome those things are some techniques that we can employ, rigth to get 
better at learning new languages. Yeah, 

**Felienne:** [00:07:08] definitely. So one of the things that I talk about in my 
book is the concept of transfer. So transfer is you already know something about 
domain A and that helps you to learn domain B.
So if you have two languages that are very close together, let's say C# 
and Java. Then you probably experienced lots of positive transfer. Like, Oh, I 
already know this. Oh, it's exactly the same in Java. That's no issue. So 
that's positive transfer, but then you also have. Negative transfer where you 
assume that something works a certain way and then it doesn't.
And for example, if you do, Oh, object oriented programming in Java, and then 
you go to Python, then there's also object oriented programming. There's also 
classes and methods. So maybe you're like, I know this stuff. I understand what 
a method is. And then suddenly stuff, of course in Python happens as real time.
And then you're like, Whoa, everything I knew was wrong. So there you have 
negative transfer where you might assume that you know something and especially 
if you're an expert and also you think this cannot be hard. I am already an 
expert programmer, so probably Python isn't very hard. And then it's harder 
than you think.
And then of course you also run into issues of motivation where you're like. I 
will never learn this because it's so hard. So actually, if you want to improve 
on transfer, there are two techniques that people typically use and the 
techniques are called hugging and bridging. So hugging is where you try to get 
the concepts to be really close together.
An example of hugging is if you already know Java then it might be easier for 
you to solve a problem in Java. So first you solve the problem in Java and then 
you simply, it's not always simple, but simply translate your solution into, 
let's say Python, if you're learning that. So that makes it easier than 
You're trying to get the languages closer together. And with bridging you're 
deliberately looking for concepts that are the same. So you, you really set out 
like you're walking in a forest and you're like, Oh, I know that. So I 
know that tree. So with bridging your reading, you tried to walk around in 
Python and you're like, Oh, a function.
I know a function. What is, what is it that I already know about functions? 
Well, they have parameters and they might have output parameters. So are you 
really getting your prior knowledge? That's already in your long term memory? 
You're, you're fetching all the knowledge you have and with the knowledge 
close. You're trying to bridge the gap between the old and the new programming 
language. So those are concrete techniques that we know that can help. Make it 
more likely that positive transfer will happen so that you will benefit from 
existing knowledge. But of course, this is not a magic trick. So learning a new 
programming language, learning something new will always remain hard.
So my book doesn't really talk about motivation. That much, it's really more 
about the, the cognitive theoretical, cognitive side, but yeah, you also have 
to be prepared to be a beginner again. You have to accept that it, even though 
you might have been doing Java for, for 30 years by then will still be hard 
probably, and will still trip you up in unexpected way.
So I don't have better news. Like these techniques I described in my book, 
definitely help, but they're not a magic pill. It will always be hard to learn a 
new programming language. 

**Michaela:** [00:10:24] I think also for me, for example, when I'm thinking about 
Python and Java, cause this is a very concrete example that I'm experiencing 
things years now is that, you know, there are also not so many resources 
specifically for
people that, you know, have Java knowledge and want to learn pattern, right. As 
you said, because if I'm aware of that, I could actually transfer some of the 
concepts and help people. So for me, it would have mean, so when I started 
Python, right, well, the first thing was I actually started in the Django. So I 
went to the Django 
girl's website, which is wonderful. I have to look that up and put them 
right link down there in the show notes, but. And so they, they walk you through 
a complete web application and that was wonderful to get me started and, you know, 
to give me some tools. And I was also getting a lot of really quick
positive experience. Right? So I was learning a lot, but I was also making 
progress. But then from there it was really hard for me because when you 
go through a normal Python court, it was really boring. And I couldn't, I 
couldn't drag myself through it because it's like, Oh, this is a data type. And 
this is a variable and see how we assign something to a variable.
Read, this is not a good use of my time. Right. And so I think it has also a 
little bit to do with being more aware that there should be resources for people 
that have already some preconceived notions or somewhat models and help them to, 
you know, hop on to a different language. What do you think about it?

**Felienne:** [00:11:50] Yeah, I think that's very true. I think there's lots of 
materials that are aimed at absolute beginners. And you never know who might 
take your course. So maybe let's just explain the variable just in case. And let's 
just explain the new, and of course it would be like a combinatorial explosion. 
If you had to have courses for like python for Java programmers and C 
for python programmers.
So I guess it's hard to develop these things. And actually I just finished a 
research study where we interviewed. High school teachers, high school, computer 
science teachers. And we asked them specifically about this and we asked them, 
Hey, do you take into account a programming language that students already know 
when they come into class?
And it is very, very hard and it's unlikely for various reasons. So sometimes 
teachers say we don't have time to specifically spend effort on this, or we 
don't really know what programming language knowledge they already have. So it's 
very hard to connect to prior knowledge because one kid might've done scratching 
in elementary school and another might've already done a bit of Python.
So it's definitely a recognizable problem with sadly, it's also a hard to fix 
problem for professional resources for professional programmers. And also for 
kids that are learning programming in school.  

**Michaela:** [00:13:04] I have one. I mean, you're definitely right at the 
high school. 
There's also one teacher, you know, and let's say 30 students or 50 students and 
so on.
But I think it's K on the internet, I think it's a similar one with, with 
all the niches. Right. So niches are now think about like, The, I mean, even 
though there are only a few, but let's think about how many people there are 
that know Java didn't want to learn Python. And I think if you think about the 
internet and if you have a big distribution, like it could be really relevant.
I mean, there's programming resources. They're like, they're really. Coming out 
like weed everywhere. Right? So many people that are jumping on this train to 
teach others to program it. I think it's maybe some niche that is unexplored 
from an entrepreneurial perspective to actually make that work.

**Felienne:** [00:13:53]  I think you're definitely right.
That as your own struggle is a very recognizable struggle for many people where 
beginner resources are too slow and boring, but then you also not quite, and 
ready enough to just start to build something after an intro, like Django girls, 
something like that hasn't prepared you enough to be a professional Python 
programmer.
So yeah, I think it might be right that there's a, like a market gap there and 
it's someone could feel. 

**Michaela:** [00:14:19] So in your book, you also talk about reading and 
understanding code. So not only learning and reading, I mean, reading is one of 
the things like 60% are a couple of studies that showed it almost 60%, over 60% 
of our daily work is on reading and understanding code.
So how can we get better at that? What are some of the concepts that are things 
that we have to learn to get better at reading and understanding code? 

**Felienne:** [00:14:44] Yeah, but I describing my book is three different types of 
reading code, because I think that as programmers, we don't really read code 
that much. And that also means we don't have good strategies for reading codes.
Like if you have to start a project and you probably know a bunch of strategies, 
like how am I starting a project? Maybe I'm starting with tests or I'm really 
doing a small, minimal viable project. You have some strategies for reading code 
sometimes. I want to use a certain library and I go to the GitHub page of the 
library and I sort of skimmed their code to see what they do because of course I 
don't have repeat me or it's outdated, or it's an understandable to me.
So you skim the codes and like, how do I do that? Why start at the talk? Like 
it's a book or do I start somewhere and looking for a main methods and then. 
Then look, what it refers to these are of course, both things that people do, 
but we don't really have good strategies. And very quickly people are like, Oh, 
code reading is hard and other people are bad at writing codes.
It will be just easier for me if I write this library from scratch, because it's 
so hard to understand codes. So the book offers a number of different strategies 
that you can use to read code. And as I said, I had distinguished three 
different types of code reading that are associated with three different 
cognitive processes.
So firstly, you have your long-term memory that has all your memories and also 
programming related memories and also syntax of programs. So sometimes you're 
reading a specific cpde. And the example I give in the book is an  
programming APL. This is sort of an oblique programming language and no body 
knows.
And if I give you an APL problem, your problem will be a long-term memory 
problem, because you don't know the keywords of APL because the keywords of APL 
are Omega and Delta. And even they have a keyword that looks like an angry face. 
It's very weird. So your problem is a long-term memory problem, which you can 
also sometimes have in Java sometimes in Java, that can be a Java built in 
methods that you don't recognize.
So that's a specific long-term memory problem. And if you're aware that, Oh, 
this code is confusing because I just don't have enough knowledge, you can 
specifically go look for that note. Another issue that you can have is a short 
term memory issue. So your short-term memory as people might be aware of is 
very, very, very small.
So you can only remember for like, let's say around five things at the same 
time. So if code forces you to remember more than five things, then your brain 
gets full and then you're just lost. So if you, for example, have a methods with 
many parameters or a function, you have to remember the function name, and then 
you have to look up in the code search.
Oh, where's the function defined. Oh. And then you have to remember the actual 
parameters and then, then define parameters. And now your brain just gets full 
and you cannot remember everything. You cannot get it in your short-term memory 
then of course, it's also very hard to understand the code. So that's a 
different type of problem.
That's also has a different type of solution. If you don't know what keywords 
you have to Google the keywords, but if you cannot remember everything, you'd 
maybe have to get a sheet of paper and write down the information that you're 
lacking. So that's really a problem of information. And then there's a third 
type of confusion and that's confusion that's related to the working memory.
So if you think of my example in the book is a basic program. If you think of a 
program that's a heavily imperative program, then maybe there are just three or 
four variables. So you can remember them and maybe it's just multiplying and 
dividing and looping. So you do know what's going on, but still the code is 
hard.
And that might be because you have a working memory problem because. And this 
happens. I often say this is when you have to use the strategy of the fingers. 
So once you take your finger on the screen and you started to reading like, Oh, 
Oh, this is this variable, this is this variable. Then it's very likely that 
you're, you have a working memory problem.
You have the information, you have the knowledge, but it's still puzzling to 
get, or what is going, going wrong. So I think once we understand these three 
different memory processes and the three different types of confusion that you 
can experience while reading code, you also see that there are three different 
solutions.
And then, you know, as we're learning a new programming language, it will 
always be hard to read code that's made by someone else or made by you a long 
time ago. It will never be very easy, but once you recognize. What type of 
confusion you're experiencing, at least you might be a little bit closer to the 
solution.

**Michaela:** [00:19:20] Yeah. what would be one solution? Let's say, for example, 
if I have the processing problem, right? So that my processing power is not high 
enough. What can I do? 

**Felienne:** [00:19:32] Yeah, that's a great question. So some of the techniques I 
described in the book is for example, making a state stable. So I know this 
sounds really silly and a bit like you're back in school, but it really works.
If you make a table on paper or you can also do it in a spreadsheet, doesn't 
really matter. You make a list of all the variables that are in the program, and 
then you write them, let's say you're doing a loop. So on the first iteration of 
the loop, what are all the values of the variables? And then on the next 
iteration of the loop, what are all the values of the variables?
And that can give you so many information. For example, that might be something 
that acts as a counter that's that goes up. And sometimes these things are so 
disguised that there's no for i in range five, it's very hard to see which is 
going up and which is going down and which of the variables are doing list 
axes.
And sometimes before you can make such a state table, it's going to be really 
nice to visualize the dependencies in the codes. And for that, I really like to 
make a screenshot of codes and print it out as a PDF. Or you can also put it on 
your iPad. And I just link, I circle all the variables and I draw links between 
all the variables.
Okay. This variable where does it go? This variable, where does it go? And then 
once you have sort of a mental model of what is connected to once you can step 
through the coast and really make a table of what are the values, and that can 
be really helpful in understanding what is going on. 

**Michaela:** [00:20:50] For me, it sounds very much like debugging, 
like how I debug code.
Right. And there was actually, I forgot how it was called years ago. But when I 
was working at the university of Victoria with Margaret and story there, they 
had like a tool that helped you explore different programs. Right. And so the 
idea was that, well, if I want to understand how this program works, Then I 
think it was driver or something like this.
This was the research tool that they developed. And so this driver was helping 
you step-by-step goes through to code, right? So you were actually running the 
code in order to understand the code and a little bit like debugging, but that 
it had more output. Right. And you went under, you're looking for problem or 
dining, the, the bag that you're have right now, but really understanding the 
culture you were executing.
It. Something else that came to my mind is like, Uh, tests, I think tests very 
often help with that, right? So you have like a test method and it tells you a 
little bit how, you know, it tells you because it testing something in a small 
unit of how it works and then you could actually run the task and you can also 
do step-by-step debug.
That has, so this is what I'm doing. For example, quite often, if I'm not 
understanding something or want to get familiar again with them, code part of 
the system or code base that I'm not familiar anymore. What do you think about 
this instead of, you know, having your finger in some paper, really using the 
tools that we have in our IDE, for example, debuggers and so on.

**Felienne:** [00:22:14] 
Yeah. So those are definitely great tools that you can use and often they can be 
used in combination with each other. So a debugger can also give the most 
recent value of a variable, but often case the debuggers don't show all the 
previous value. So you don't get this nice table of relationships. So if you 
have the debugger, you can definitely use it to, to make all the effort, to 
understand all of our values of one iteration.
And then you do another iteration and you still write it down. So I think these, 
these task and tools, nicely compliment each other and also for our 
tests. Yeah. You might be curious, Oh, what happens if this list is empty, you 
can do this mentally. But if there is a test that allows you to run the code 
with, let's say no customers or something, no one is locked in what happens 
then?
Yeah. Then the tests can really help you also build the mental model. So the 
reason that my book mainly describes matters that you can do on paper rather 
than on the computer is because I thought, okay, Debuggers and testing. This is 
what people already know. These are tools. Am I book aimed at professional 
programmers, they will use  tests,debuggers.
They will use a developer. So these are tools that they're familiar with. So 
here and there, of course, in the book we refer to that, but the book was really 
mainly meant to give people new strategies that they haven't tried out. And, and 
of course, like, If you have a actual toolbox with tools, sometimes a hammer and 
a nail is better.
And sometimes a screw and a screwdriver is better. If you, if you have large 
vocabulary of tools, then as a professional, you can decide which tool makes 
sense and watch which context.  

**Michaela:** [00:23:45] And so one of the topics, my favorite topic is 
code reviews. And 
so here, we also have to understand, read code, right? And give suggestions also 
really understand not only what the code does, but also is the code correct on 
so many different levels.
Again, we are assessing the code and definitely in a good understanding of 
what's going on here is the first step. And. I find that a lot of people are 
struggling with that. Right. And so there are several, several issues to that. 
One is that very often code review tools that we have nowadays. Yeah. Tooling 
that allows you to do the code reviews, do not show you the whole code.
Right. So do you touch, so you snippets for example, this is really a difficult 
thing, right. But then also it's code, maybe that you are unfamiliar with, maybe 
you don't know the code base. What are your ideas about code reviews and how can 
we make them. You know, better, how can we decrease the cognitive load and how 
can we get the most out of it?

**Felienne:** [00:24:40] Yeah. So I do think that the three different forms of 
confusion that I described in my book can also be helpful in code reviews. So 
what I really hope is that people won't just read the book individually, but 
also like you can buy one copy and read it with your whole team, because I think 
the different forms of confusion give vocabulary.
If you are in a code review, I've of course, often people will say, Hey, I find 
this code confusing, and that's sort of fair. If you find the code confusing, 
then, then that's what you think that that is not an unfair comment, but there's 
not as helpful for the person that has written the code. Okay. You find it 
confusing.
Why? And then in my experience, people find it really hard to vocalize. Why code 
is confusing. And if you have these three different modes and at least you can 
say, Oh, this code is confusing because I don't know these keywords. And that's 
mostly the author's fault that you don't know a certain keyword or certain 
language constructs in Python.
And for example, list comprehensions, you might just not be aware of lists, list 
comprehension for job if you're coming from Java. So that's not really 
problem of the author does that's more a problem of the reader that the reader 
can fix by just learning a content. So once they can vocalize this goes and 
confusing because, Hey, I don't understand what that, that list thing is doing.
Then the solution can be I explained that to my teammates and then the code is 
no longer confusing without a change to the code. Whereas if a certain piece of 
code requires lots of processing power that maybe as an author, you can change 
it. And we have some, some techniques in the book book as well, but people might 
already be familiar with techniques like giving stuff better names, 
refactoring a large piece of code into different steps.
So if the issue is processing power, then there might be something that the 
author could do or once to do that is going to make the code better. So I think 
these different modes of confusion and just the notion of cognitive load that 
sometimes your brain takes lots of processing power because it lacks certain 
understanding.
I think that might also smooth go code reviews. It it's really, the book is not, 
man's only to be. Help for the individual programmer, but also very much meant 
to set a common vocabulary. Like if more programmers would know the difference 
between working memory, short-term memory and long-term memory, then I guess they 
could also understand their own confusion, better understand why other 
people find their code, which they think is so beautifully documented.
And so well-structured. It might still be very confusing. If you bring me a 
fantastic poem in German, then I will never see the beauty. I know some words. 
It's not that I don't understand any German. I can like order a coffee or 
something and you might be totally crazy about this. Look how fantastic it is.
And I will never join you. And that's most of the Bowen's problem. That's just 
because I don't know enough words and grammatical structures to really see 
what's there. So I think that that difference might help people also have more 
smoother code reviews. 

**Michaela:** [00:27:43] Yeah, I think a common vocabulary, not only about, you 
know, the processing power, but in general, like also shared engineering values 
are really, really important.
Right? And this brings me to readable code because maybe I'm a junior or maybe 
I'm unfamiliar with this framework or with this API writer, as you said, I'm 
having some lack of knowledge here, and this is why it's confusing, but it 
could also be that the code itself is, as you said it a little bit unreadable 
and so on.
And I think it's really important that teams develop their own or as a team, 
right get coherent engineering value. What is readable code for us? What is, 
what are we valuing like high quality means for us? Isn't that right? So, and 
I'm working with this startup right now. We building their engineering team.
And so one of the first thing that we worked on is our engineering value. So 
whenever we are hiring and when we are getting new team members that we are all 
on board and this is a living document, right? So we change it. And you know, 
when somebody is coming in, we can reflect on those engineering's values again, 
and things like what is high quality code?
What means that our code is good, tested or testable, you know, maintainable and 
so on. And I think this is really important for contribution as well. And, and, 
and also for understanding the code of others, because it helps us to see, and 
this is something I read the first two parts of your book that are already 
available on the website.
And so what I really found interesting was that readable code
for example, that has design patterns or follows 
design patterns. And it has to do, and not, I have to explain it. I will explain 
it. And you can then, correct? 

**Felienne:** [00:29:19] Yeah. It's really great to hear what other people take away 
if you're writing.

**Michaela:** [00:29:23] So please go. Yes, it's hard because it's had one readable 
code, right. Or code it's easier process is code. It follows the same patterns 
if, and only if the person that reads this knows design patterns, because then 
they're taking those patterns, these parts of the code from their long-term 
memory. So this frees up short-term memory and frees up processing power.
So they can actually understand the code quicker. But what I also took away from 
them that it does that well, design patterns, okay. remember everything that 
we know right. So that we can recognize whenever we have as it. Is it team, if 
you have a good structure and we know this is where, you know, those files are 
right or we are structuring our classes in that way, all of that is very similar 
concept.
I think we can transfer in generalized that from the design patterns and go away 
and say, well, if we know where to put those artifacts, And, uh, people can 
expect something. They will also overtime, you know, be better in understanding 
and processing our code. So this is what I took away and I thought this is 
really great.
I will put that into my code review workshops because I think it's really helpful. 
And this is also where I think. Coherence there, the power of a coherent code 
base comes from, right. So there'll be coherent coding practices, coding 
style, because this really frees our memory, freeze our processing 
power so that we can re try to understand, okay, what is this or isn't doing and 
not, you know, we're going to find different methods and variables and so on.

**Felienne:** [00:30:54] Yeah, I think that's a great takeaway. And if you like 
that, part of it will be lots of more in the book and the rest of the book that 
we can talk about now already a little bit. So the process that you're 
describing here in these schools chunking, and that means that if you group 
similar information together, then rather than remembering it as similar 
information, then you can remember it as one go. 
For example, if I re if I asked you to remember cats, dog donkey, 
that's a lot easier to remember than salt, roof, microphone, because those words 
have nothing to do with each other. Only they're in my view right now, as are 
easier to remember three things that are similar and three things that have 
nothing to do with each other.
Because with the first one you think, Oh, these are all animals. You might 
already anticipate if I say get it. And the next thing could be dog. The same 
story we need for code. So if you look at code that has, let's say the 
Singleton pattern and look at the code and you can just say, Oh, this has a 
Singleton pattern and you can remember, Oh, and the Singleton is this one thing, 
like a token, for example, that can only be given out once.
Whereas if the code is sort of all over the place and it doesn't specifically 
use a design pattern, then you cannot add one go  memory. You have to remember 
individual lines or variables or class names. And remember your short term 
memory is really limited. So if two or three or four things are in there, then 
it's full.
And as you exactly said, it frees up some mental space. If you can just. Say 
shingles and pattern token, and you have two things in your brain. Whereas if 
you have to remember, Oh, one variable is creative. Oh, if you try to 
instantiate it again, you get an error. Then you have to remember many different 
things at the same time.
And, and you're right. That, that, that really goes beyond design patterns. Some 
other examples that we have later in the book are for example, about variable 
names. There's, there's a really nice new paper that came out that talks about 
the concept of name molds. Like how do you form a name? Let's say you have to 
make a name for the maximum value.
What do you use? Do you say maximum value or max value? Or value max or value 
maximum or maximum of values. There are so many different ways in which you can 
do this. And this paper that I described in my book describes an experiment in 
which they asked people to just came up with names for such a situation.
And you see, indeed developers are all over the place, but if you teach them to 
use a specific tree step technique, then they get a lot better at making the 
same type of names. And then your code gets easier because if you're looking for 
a valid variable, then you know what to look for. If it's always maximum and 
then the entity, you know, there's all the maximums will be in the beginning.
You have to look for the entities in the end or the other way around. It seems 
like there's not a big difference between different molds, but code gets really 
confusing if different people use different molds. So again, also variable molds 
are not naming name. Molds are another example of, if you make it easy for 
people to protest code, then they will process it with ease.
But if you make it hard by having max value, but then interest maximum. It just 
gets harder and it's, it's unnecessary complexity. We also talk about that in 
the book, you just said cognitive load. You have the difference between 
intrinsic cognitive load and extraneous cognitive load. So intrinsic cognitive 
load is this problem is hard.
It's really hard to do this and this SSL algorithm or something, but extraneous 
cognitive load is like having maximum interest and Value maximum just for no 
good reason, mixing up different name molds is going to add to your cognitive 
load, but it's not gonna help you in any way. It's just like extra low, extra 
fluff that you have to process.
So I think that's also another concept in which chunking that we described in 
the book. Okay. Or at, at many different level at a quite high level of design 
pattern, but also it's a really low level of choosing a variable name. 

**Michaela:** [00:34:56] Yeah. And I think what's really valuable here is that we 
have some way where we take that a little bit out of this.
Oh, this is objective. I can do whatever I want. Right. So readability, I mean 
the whole readability area sometimes gets very, very loaded because there 
are some people that inderstand that it matters. And then there are a lot of 
people that hold against it and say, well, it doesn't matter because it's 
objective.
Right. Whatever I want, I can do. It's the same for the compiler

**Felienne:** [00:35:26] Yeah. Or even that they might argue that my 
method is better because whereas it doesn't really matter even. 

**Michaela:** [00:35:36] Yeah, exactly. 
Right.  And so I think having more research in that area and really 
understanding, give us a better understanding of, you know, Where is some merit 
to making it more coherent and making it more, you know, easier and where 
there's really, it doesn't matter.
Right. So I think that's really good.

**Felienne:** [00:35:53]  And, and the happy news is that other research 
also shows, which I think is really nice is once you choose a specific way of 
doing stuff, then people tend to stick with it. So people aren't as, and you 
know, Oh, I know better than, than you might think.
So if your team has a way of choosing variable name, for example, it's likely 
that people new to the code base without you really saying, Oh, welcome to our 
code base. This is how we do names that people will just pick it up like 
automatically if you're, if you are deliberate about it. But of course, if you 
are all over the place and people don't have any methods to click to, so then 
yeah.
Then they will just do whatever, whatever they feel is better. So a little 
investments might actually results in a more consistent code base that keeps 
going without any efforts. Yeah.  

**Michaela:** [00:36:42] And I think, I mean, everybody will be happy 
because choosing name is 
hard and annoying and I hate it. Like every time, like I love programming, but 
then choosing my names from my variables, my methods it's like, Oh, what should 
I pick?

**Felienne:** [00:36:59] it's just low effort for you while, right. 

**Michaela:** [00:37:01] Exactly. It's like a pattern. It's like an algorithm that 
you can take and you can just generate your methods and your names out of it. 
And I think that would be that's great. 

**Felienne:** [00:37:10] Yeah. That's really cool. Yeah. So that's chapter a chapter 
nine of the book probably comes out.
So you have to wait a little bits before that comes out. You know, what, what 

**Michaela:** [00:37:20] I'm waiting for for the chapter about complex code. Can you 
explain what is complex code and how can we better get better in maybe not 
writing complex reading complex code?

**Felienne:** [00:37:30]  Yeah. So the, the chapter about 
complex code goes, it has a number of techniques that come from natural language 
reading because often of course we say, Oh, programming is like math, or I like 
mathematics, but new research last year, a paper was 
published in nature, which is like one of the top journals for researchers 
that says that's actually how well you can program is very much correlated with 
how well you can do natural language and less so correlated with your 
mathematical ability. Which of course, if you think about it, it makes all the 
sense in the world.
It's a programming language and 70% or something of tokens in a program 
will be natural language because you have key words are variable. So there are 
some sense students. So that led me to the idea that's expressed most, most of 
my research that, Hey, maybe we can learn from how natural language, thus stuff.
So maybe you remember that if you were in, when you were in high school, you had 
to look at non-fiction texts. Very often for, for German or English or Dutch. 
And they ask you a question like, Hey, here's a newspaper article. What are the 
five biggest, most important lines? Or, Hey, here's a newspaper article first.
Don't read it. Just look at the paper, look at the images, or just look at the 
structure. Look at the headlines now, or look at it for three minutes and, and 
see what you still remember or write the summary. These are all well established 
ways to deal with non fiction texts and all these strategies can also be 
applied to code.
So these strategies, these are, these are the exercises we have in the book 
where we ask you to look at codes for two seconds or a minute or something, just 
look at the code glance at it. And what is the first thing you see? What have 
you learned from just glancing at the codes? So that is a way that you can deal 
with, with complex codes.
Look at the code for five minutes and try your best to write a summary. And of 
course what you take away says a lot about your prior knowledge. Hey, if I have 
to, I don't really know R. So if I had to look as an R program, probably I 
will take away something different than if I look at the Python program.
So it tells you something about your own level of ability, but clearly it also 
tells you something about the code. So these are all techniques that you can 
try. As I said, it's just filling a toolbox that you can try to help you read 
more complex codes and it will always be hard. But if you, if your only strategy 
is read the codes. Oh, I don't understand. Oh, read it again. Then, then you're not 
really going to advance. So all these techniques we know that really support 
nonfiction, reading of texts are probably also likely in different 
situation to help you with reading cope. 

**Michaela:** [00:40:14] Wow. I'm so looking forward to that, like I was reading 
your book by using a screen reader, 

**Felienne:** [00:40:22] so cool.

**Michaela:** [00:40:24] And it was really cool. Like I was reading like the screen 
reader, wasn't reading the book and I was reading at the same time and I 
actually. Experimented a little bit with two different screen readers. Like one 
was really highlighting the, the sentences and the words, which was very 
different for me to process the, the book because I was reading at the same 
time, the same thing that she said.
And so it somehow hit my brain, like in two ways and then the other, but this 
was a very annoying screen reader, which also read a lot of other things. So 
then I switched. And here I really had to find it. So what I did and was like 
just glancing over the parts and was listening to it and could also take notes 
and everything, but I felt that very my attention and what I could take 
out of it was really enhanced.
So I will, I will continue doing that anyway. So I'm really looking forward to, 
to read more of your book. One thing that I wanted to ask you maybe as the last 
question is a little bit about the process of writing your book, but I'm also 
writing a book and I probably have a very different process that you have, but 
how are you doing it?
How do you come up with the chapters? How do you come up with these different 
exercises? How do you know what the readers really want to know? 

**Felienne:** [00:41:35] Yeah, I think I sorta cheated advance because I was already 
giving a course at Leiden. You have programming. And 
I've been, I gave this course already four times to different groups of students 
and the book is sort of my lecture notes.
So the exercises are things I have tried out I was in class with. Students and 
the storyline is more or less the storyline that I use in the course. So clearly 
that helps a lot because I already had this storyline and I had already read all 
those papers because I discussed them in class with students.
So, so that was like the beginning of the process was I had a plan, of course. 
The book turned out really different from the lecture notes for various reasons. 
Because once you start writing stuff on paper, you also have to be precise in a 
really different way. So in lecture, I can just say, Oh, it's more or less this, 
and you can read the paper.
That's your homework. I know for you, you have to be really pretty. You have 
to really understand as a diff if you're coughing a paper in a book, You have to 
understand as a different level, like what exactly was the experiment. In class
You can say, Oh, for example, I have this part of how's camel case, a snake 
case.
You can just say, Oh, camel case is better for comprehension, but snake case is 
quicker. That's the result of the paper. That's, that's exactly what it says. 
Well, of course in this book, you have to say, Oh, how many people participated 
in this study and exactly what was there. So, and then you start diving in 
deeper and then it makes you reflect at a different level.
So clearly many changes were made, but my, my biggest process was cheating by 
giving a course of activity, the same topics for a bunch of years, and then 
writing everything down in detail. 

**Michaela:** [00:43:11] And so really last question now, not a last question, but 
one more. Why did you choose to go with a publisher and not self publish your 
book?
Like nowadays everybody's self-publishes books, right? 

**Felienne:** [00:43:26] So, yeah, I think there's a variety of reasons. Firstly, it 
just looks, I think, better on your resume to have a published book. I think by 
promotion committee will be more impressed by me having a privileged book on my 
name, especially by like an established author in your field.
That's going to be stronger than. Hey, I put a PDF on the internet. Uh, so, so 
that, that's definitely one reason. And another reason is also that, of course I 
pay most of what I make through the publisher and that is not left for me, but 
it is worth it, I think, in terms of making the book better. So I go to editors, 
both the development editor and also a technical editor does that, that was 
representing the goal audience and it's technical, 
the first development at a editor 
like, Oh, this is I, I wrote a scientific lecture notes, right. 
Oh, this is way too theoretical. And you have to really dress up the theory with 
this sugar coated layer because it's for professionals. And of course, first I was 
like, yeah, And of course a professional can read a little bit about science, 
but yeah, you have to make it relevant for, for the daily practitioner 
or they won't read it.
So those two editors just really make the book a little better, even though the 
process was less fun because just writing a PDF, I'm putting it on lymphoma. It 
is easy. So I was as well. And a few times of course, this like this, I'm sure 
it's like this for your book as well. Sometimes you're like, Oh, this is going 
well.
And then you're like, Oh, I will never finish this. So the process was harder 
because I had to really rethink, okay, well, why is it valuable for people to 
know this? And of course, it's really different if students, they enter your 
lecture hall at Piccolo now of course they will move, leave in the middle of 
lecture.
That's very unlikely. So you can first builds up all the theory. And then the 
last 10 minutes, talk about why this is relevant because they aren't, they are 
in your, in your power. They're not leaving. Whereas of course, in the book I 
realized after I failed a few chapters that you get  to do 17 pages of theory, 
and then explain why it's relevant.
That just that structure of those aren't work for practitioners. And I don't 
think I would have really made that realization myself. Without the development 
editor are really used to selling books to practitioners. And then finally, also 
in terms of marketing, of course, then it really, it really helps. Of course I 
track my sales and I have a link, like my own link and a link from the 
publisher.
And you do see that. They are reaching an audience that I'm not reaching and 
they are bringing sales, which is not only nice because you know, it would be 
nice if I make a bit of money out of the book. But also of course, what I want 
is that people know this little bit of cognitive science because I really truly 
believe that it's just going to make them better and happier programmers.
So that's another reason that I, even though I have quite a following on social 
media, You do see that, that the publisher is better able to sell books through, 
to my target audience and than I will be myself. So, so those were, those were 
my reasons. 

**Michaela:** [00:46:28] Yeah, I think there are valid reasons or things that are 
also going through my head.
I haven't made the decision yet. I'm also writing the book together with our 
better fertility. So it's a collaborative decision and you're always like, Oh, 
let's do it this way. Oh, let's do it the other way. But I think we still have 
some time to decide what you're going to do and it's hard. 

**Felienne:** [00:46:45] And in any case, I would 
definitely recommend to, to, to ask for feedback.
Very early. If I, if I can give you you and other people in the audience, maybe 
that are considering writing a book. And my first reader was the technical 
development editor of the publisher, which was helpful because she 
slayed everything. As I said, because I had much too much theory in the 
beginning, but.
In retrospect that they didn't have to be the case. Right. You know, most of my 
friends are programmers, so I couldn't have asked other people for a little bit 
of feedback that I, that I trust and like loads on the entire group, of course, 
but just some examples. And do they make sense? And what do you think of this 
order?
I definitely made the mistake. That's maybe common to people that are experts in 
something. I was like, I wrote a PhD thesis. I know how to write a book. It 
wasn't, it wasn't the same. So I thought I knew how to do it then, then I 
didn't. So if you go with self publishing or with a publisher, doesn't matter, 
but definitely reach out to all your friends and followers on Twitter for some 
dress reading, then it will be nicer than waiting until the ends and then having 
to overhaul everything.

**Michaela:** [00:47:53] Yeah. I think that are great. Last words for this 
episode. I I'm so happy that you have been on my show. Felienne talking 
with me about all these ideas on how to learn program, how to understand code. I 
would love to talk again. Maybe I'm inviting you again to deep dive into some 
other areas and yeah.
Um, maybe something, maybe one last thing that you want to tell my listeners. 
And then I let you go.

**Felienne:** [00:48:16]  Yeah. I think I said it a bunch of 
times, but I'll say it again, like learning something new is really, really 
hard. So cut yourself a bit of slack. Like even if you know everything about 
Java. Python will still be hard.
And even if you're an expert Python programmer, reading a Python program that 
you've never seen before by someone else, it will always be hard. So remember 
that you are an expert in one thing, but you're still a beginner in something 
else. So take time and patience and use the tools you have and specifically 
reach out for tools because don't make the mistake.
Maybe like I did with my book, thinking on this will be easy because I did it 
once. Every new beginning is still hard and that's okay. That's like the way it 
is, you will get smarter than you already are. The only thing you can still 
learn is new knowledge in a different field. 

**Michaela:** [00:49:10] Yeah. Thank you so much. So thank you for Felienne
for being on my show.
Thank you so much. 

**Felienne:** [00:49:14] Yeah, it was really nice to be on the show. Thanks for 
inviting me. Bye bye. Bye. 

**Michaela:** [00:49:20] Before you go, let me tell you that my code review 
workshops are starting again. So if you want to transform your code review 
practices from bottleneck to superpower, check out my 
training at https://www.awesomecodereviews.com
So, thank you for listening to another episode of the software engineering unlocked 
podcast. Don't forget to subscribe and I talk to you again in two weeks. 
Bye. 
