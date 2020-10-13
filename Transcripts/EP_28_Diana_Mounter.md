# Transcript Episode 29 with Diana Mounter

**Michaela:** [00:00:00] Hello, and welcome to the software engineering unlocked 
podcast. 
I'm your host, dr. McKayla. And today I have the pleasure to talk to Diana 
Mounter. 

But before I start, I wanted to update you on what's happening in my 
life. This is the, I have the last one code review workshop for this year, where I still 
have a few spots left.
So if you want to make code reviews is super power. Now is the time I will 
resume the workshops in January prior to break, right? Yeah. The reason for that 
is that I'm finally working on the code review tool. I always wanted to work on, 
remember when I said I want to do it and there's just no time. Well, I made time 
for it.
The tool is a code review analytics tool currently focusing on GitHub data and 
it helps engineering teams too. Okay. Understand their strengths and bottlenecks 
for the code review practice. 
Right now, it is in the MVP state, but I'm already working with one 
rate company that wants to understand the different cultural practices followed 
by various team and organizations.
There's no official side or anything, but I'm interested in the code review 
analytics tool. Send me an email at michaela@michaelagreiler.com. 
I will link my email in the show notes, 
but now let's get back to Deanna. Yeah. Anna is the director of design 
infrastructure at the tap Vienna travels, divert and lift in many different 
countries, even continents.
She started as a print designer and spend some time in the government before she 
got into bed. And design now she leads the design systems at guitar. Well, look, 
I'm Deanna on my show. I'm really thrilled that you're here. 

**Diana:** [00:01:41] Thank you for having me. 

**Michaela:** [00:01:43] Yeah, sure. Well, yeah, I've never talked to their director 
of design infrastructure.
Can you tell me a little bit, what's your day to day work look like and what are 
your responsibilities? 

**Diana:** [00:01:56] Yeah, so my day to day is, you know, it's a, it's a fair 
amount of meetings, but I would say that. A lot of the work that I do is T is 
like to help shape projects, help develop roadmaps and strategy, and also people 
management.
So I think one of the things that we do at get hobbies in the design org is that 
design leads tend to also be like experienced in, in what that might seize do. 
So they have a lot of input into the design, but also people manages. Would you 
like me to tap into what design infrastructure is? 

**Michaela:** [00:02:32] Yes, please.

**Diana:** [00:02:34] Yes. Yeah. So I, it might not be the most commonly used like a 
title, I guess. So design infrastructure, I think is. A good way for me to 
describe a bit more about what we do. I think design systems are a big part of 
it. I would almost say that design systems are sort of an output of, of what the 
design infrastructure team does.
So we have a get hub. It might be different a bit in different places, but it 
get hub. A team has like kind of two for, I guess, areas. One is the design 
system itself. And the other is how the design system is used in the core 
experience of get hub. So we do a lot of work on the actual sort of like 
infrastructure of, of GitHub in terms of.
The actual like design and the user experience of get hub.com. Another way I 
feel like is, is maybe a tangible way to sort of describe designing 
infrastructure is actually to sort of comparison. It's a sort of real world in 
the real world, they just described like Amad structure and in terms of hard 
infrastructure and stuff.
And it's very much sort of works for like what we do too. So our, like how the 
infrastructure, like UI components and we have a couple of different 
implementations of those it's tooling, such as like LinkedIn's unit tests, that 
sort of thing. And then like release distribution. Like how do we like 
distribute the actual components to different websites as well as github.com and 
then the sort of stuffed infrastructure is, is the citizens.
Processes and stuff that we have to do to maintain the health of, of the design 
system. So that will be things like we have, like a first responder rotation, 
office hours, a contributor group, onboarding processes, reviews, that type of 
thing. 

**Michaela:** [00:04:24] Okay. And so if I'm thinking I'm a software engineer now at 
GitHub, how do I connect to design infrastructure?
So I'm actually getting UI components from you that I can then reuse or just, 
you know, you sort of out of the box. That's how I would imagine it, but I'm not 
sure if, if that's the correct. Understanding. 
**Diana:** [00:04:46] Yeah. That that's the happy path for sure. Like that's what we 
hope the experience will be. So I think, you know, I'm working on the front end.
Yeah. Get herb is likely to interact with the design system, which is called 
primer on github.com. That's probably the two main ways that people would 
interact with that system. Um, in terms of like the actual code implementation. 
One is his primacy assess, which is really where we started with the design 
system.
And the other way is through our component architecture in get hub.com, which is 
called few components. So that's a rails implementation of components, similar 
to what you might use with in like a react implementation. And so at the moment, 
yeah, the reason why you might sort of interact with both is because we're in a 
sort of like transition.
Phase of moving to towards components, but we've still got a lot of work to do. 
Another way that engineers would interact with the system is they're building in 
react. We used to have a react component implementation, also a documentation. 
So how to like guidelines on how to implement and, and then, yeah, probably code 
review in NPR.
It's like we review a lot of this sort of. Sort of PRS that tension UI 
implementation, basically. 
**Michaela:** [00:06:11] Okay. And so from, from an organizational point of view, 
the hierarchy and how divisions are located, is it that, you know, you have like 
design infrastructure is their own thing where, you know, I imagine a lot of 
designers and, you know, sit and create those infrastructures and processes.
And on the other hand, you have like the engineering teams and then. The 
engineering teams just interact with the infrastructure or is it more that in 
the engineering teams, they are also designers and they connect to the, to the 
design infrastructure team. 
**Diana:** [00:06:45] Yeah, that's it. That's a great question. So on my team, I 
have both designers and engineers, and so the engineers tend to work on the, the 
actual UI components in our different implementations on like things like the 
tooling, like lenses and unit tests, like.
I mentioned earlier, they, they managing cut their releases. It's the engineers 
that are more often working in. On the actual github.com products, then they'll 
also update the different versions of, of our primary packages and like test 
that and make sure that's working. We do a lot of updates.com itself, so like a 
lot of refactoring and bringing the front end and the design forward.
Design our team is like pot is the product design. So yeah, we have like a ton 
of designers on the team T summit. Some of them are more technical. Some of them 
are working more on the visual side of things. And, um, so we're part of the 
product design team and product designers tend to work in. And squats with PMs 
and, and engineers in the engineering org.
So it's kind of like a sort of a matrix set up, really. So we're our own org. We 
also work with a lot of other product teams, basically. 
**Michaela:** [00:08:06] Very cool. And so, well, one of my favorite topics called 
reviews. So for example, let's imagine we have to improve the code review 
experience for who and how. Would designers be part of that.
Right. So, yeah. So would it be like one product team that would say, well, 
let's, you know, redesigned, for example, that experience on that one page, 
let's say per request page. Right. So, um, and we go through data and then you 
have some designers, as you said, in the team, in a squad that would redesign 
really how it looks like people would implement it.
Like the engineers would implement it. And then the buttons, the components we 
will really pull out from infrastructure. Is that right? Is that how I would 
imagine it, or how would that work? 
**Diana:** [00:08:54] That's, I'm fairly close to, I think how we work, I'll add a 
little bit more fidelity to that. So, I mean, I think that it's often easy to 
think of design is sort of, you know, pushing pixels, but really designers are 
thinking about the sort of end to end flow.
What's the customer experience also in working with PM and engineering. 
Leadership to, to think about like the business sort of impact as well. And some 
of, some of our designers work on things that, you know, don't really have that 
UI. So we have design is working on and her boss cl GitHub CLI for example, it 
used to be called hub.
So I, I was using the outdated name there. But yeah, we have get hub CLI, which 
is like, Oh, tech spec based, but it's still like stuff to design there. It's 
still yeah. Experience. You're still sort of thinking about the flows, the user 
experience and, and interior, like how that interfaces. So I think, you know, 
and designers have a big role to play in that overall experience, working 
alongside, um, engineering and product.
When they are, they're often like using the system, but also influencing the 
system. So yes, you, you, you mentioned like, will they grab the like buttons 
and stuff? We, we have a lot of content and components in our system. And I give 
her a lot of the sort of foundational way, but we also have an, you know, 
honestly still working on building up, like how will these pieces connect 
together?
In fact, we actually just did a six or seven weeks of a, like a whole org sort 
of, I, I want to say hat quake, but it was, it was several weeks. So it was more 
like a hack month, really, of all, a lot of, most of product design and design 
system. And engineers like working on some of our, like UX debt together.
And so product designers, you need that using the system a lot of the time, but 
they're also breaking it. They're finding the places where it doesn't cover and 
you pattern that they need for their feature. And so there, we really want to 
work really closely with product designers so that we get that feedback about 
what, what the system needs to cover, how to evolve it.
And so it's really great to have those contributions from, from product 
designers and engineers working outside the team as well. So. Yeah, 
**Michaela:** [00:11:24] and it sounds really amazing. One question has popped in my 
head when you were talking about, you know, having all these engineers, you have 
the product designers, maybe product managers, you have a lot of internal.
People that are also your customers, right. You could have is a product that 
most of the engineers or all engineers and most of the employees of GitHub will 
even work with, right. That they will experience that they will use. So somehow 
you're your own. Uh, you sandwich is very handy because you can, can use that 
knowledge to evolve the product in the right direction, but you also get her 
information from outside.
And how do you do that? Like, do you do user studies, do you ask really larger? 
Do you have studies with larger numbers participants? They are, that are coming 
from outside that you ask, you know, how to improve the system, or how does that 
work? How does that process work? 
**Diana:** [00:12:19] Yeah. Yeah. So you, right. It's kind of great to like, be able 
to use, get hub, to build, get hub.
Our team is like, Kind of particularly fortunate because of the fact, then we 
also married an open source design system. We get to use a lot of the features 
of get hub, but also like experience it in a way similar to some of our 
customers. But it's also important to realize that when the way that get hubby's 
is get him, it's not necessarily like how every customer uses get hub.
And so it's, we have to be careful to not fall into that trap that. If it works 
for us, that it works for everybody. That's definitely not true all the time. 
And so, yeah, it's really important for us to talk to customers to understand 
that. And so, yes, we have a customer research team. We also, which is like, you 
know, if we want to do usability testing interviews, the studies, those are the 
people that we will work with.
A lot of PMs and designers do some, some of that interviewing and, and, and sort 
of learning from customers that themselves. We also have other ways to interact 
with our customers and get feedback. So we have a feature preview feature, which 
allows us to, to make available certain features to customers and they can opt 
in to try them out.
And that's something our team has definitely made use of in the past and with 
some of our like big overall. So it was really a really great way. To get 
feedback week. Cause then we can look at both data, like look at how the metrics 
are tracking. Um, like for example, I really basic signalize is people that are 
opted in like they Oh doubt.
Right. Is really, and that's a signal that it's not working so well, but it also 
allows us to get like direct, written feedback from customers. We also have a, 
like a maintain is great that we can have like discussions with. And then 
sometimes we'll like, If there's particular individuals or groups or companies 
you want to talk to, then we might reach out more directly to them.
**Michaela:** [00:14:22] Yeah. One of the things that you. Talk or passionate about 
is inclusive design. So what is exactly inclusive design and, well, I think a 
little bit, it plays into what you just talked about. So how, how, how do you 
make sure at GitHub that, you know, your design doesn't leave out large parts or 
even small parts of, of, you know, the, your user base.
**Diana:** [00:14:46] Yeah, good question. I think that's a good question. Lots of 
times though, because they were all kinda questions. I think the best way that I 
can think of to describe why I like the framing of inclusive design, is it, is 
it just helps you think about. I think, how do we include everybody into this 
experience and to get help, wants to be, you know, a home for all developers?
How, how are we going to do that? If we're not trying to think about, like, how 
do we make this an inclusive and accessible system for everyone to use? Oh, a 
lot of the time we talk about accessibility, which is incredibly important. And 
I see that as a sort of subsection of, of inclusive design, but I think it's 
easy to sort of quickly sort of think about compliance and boxes that you need 
to check off rather than sort of sort of thinking how can I make this a great 
experience for anyone?
And so. Yeah, inclusive design is I think, honestly, something that we have to 
continually work at a can be how we offer that experience can be influenced by 
many things. One of the things that we really sort of tangible, sort of simple 
examples, even if it's not simple to implement is thinking about Kolomiets.
If you've been on the Twitters or I've seen some of my other talks, like we know 
that get, get her abusers would really, really like dark mode, for example. And 
there are accessibility the reasons for why people might want that. And then 
that's just like, this is a preferred experience to me. And so thinking about 
like, how do we offer something like doc mites and like other sort of color 
modes or, or like, Choices for how a user experiences yeah.
Get help. Like the actual sort of UI design is a way that we can is one way that 
we can make that experience more inclusive and to people is incredibly hard and 
it gets as good and harder and harder since they've been at get hub to build an 
experience that works for everybody. We've got open source maintainers.
We've got people. Learning to code. We've got an enterprises, we've got people 
using it, sort of, you know, dead, it's a utility, it's a critical part of their 
workflow. And then people that are using it to sort of, you know, for 
creativity, they've got an idea and they're sort of, sort of starting yeah. A 
project on get hub to sort of explore that idea and.
And test it out and maybe share with if he friends or coworkers. And so I think 
that we increasingly have to think about how do we, where do we, where is it 
important for us to give customers the more about the actual, like sort of core 
experiences get hub? And I say, I think inclusive design is a really important 
part of that.
**Michaela:** [00:17:36] Yeah. Somehow I can see how, if we start thinking about 
that we come into this or we could fall into this trap of, you know, a hundred 
different decides, right? So one, one person is a power user and they want all 
the possibilities right there. And, and use every feature that could have has 
available. And then we have maybe somebody that's occasionally on GitHub.
And so, uh, what I hear very often, and I'm, I'm not very deep into design, but 
is that you have a very simple or very simplistic design at the beginning. It 
should be very simple. There shouldn't be a lot of options. And then people 
start to dig deeper. I'm not sure if that's really the best, the best advice.
How are you approaching that? What's your philosophy behind that, right? Like if 
you want to have, yeah. Novice people work with GitHub and also advanced people 
have all the power with the features that are available, but without, you know, 
overwhelming somebody that isn't very often on GitHub or not using everything.
**Diana:** [00:18:39] Yeah, it, I mean, I'm not, I don't think that there's like a 
three step process to sort of figuring that out. It's, it's a thing that we, 
that is challenging and that we have to keep working at. I think the, some of 
the things that we discuss and, and, and try and think about is how can we make 
everyone feel like experts and make everyone feel like power.
It uses, I couldn't give you like, here's the X XYZ of how you. Exactly do that. 
Cause it's very dependent on like each feature, but that's a conversation we 
have. It's like, how can we make everyone feel like experts? We really don't 
want people to feel like that, you know, they're not smart enough to use, like 
get hubs UI because they can't find where things are.
And I think, you know, we've got, we have scaled the product and we've added 
more features and we have made that experience more difficult in places than it 
should be. So that's definitely something that we. We are working on right now. 
**Michaela:** [00:19:37] I really like this idea of making everybody feel like an 
expert, because there are so many different ways.
These are so many questions. I met so many goals that you could have, right. 
Making a person feel happy or, you know, satisfied or, but. Having them feel 
like an expert and really like that independent of their experience level. I 
think this is something that can be, you know, you know, stuff or designing your 
system.
And the question that you could ask yourself. I mean, if you achieve it, this is 
another question, but I think it's a very good, it's a very good goal to have a 
really like that. 
**Diana:** [00:20:08] Yeah. Yeah. And I think it's like thinking about not having 
anything, be a barrier to like core interactions and like having those power 
features that think that is a bonus almost to the experience.
Like it's an add on it's it's not necessarily. You have to spend like 10 hours 
learning how to navigate to a pull request in I'll just use, get hub. It's like, 
we want not based sort of cool workplace to be very obvious and easy to follow, 
but then as people like, you know, if you're using GitHub day in, day out and 
building that muscle memory, how can we like, you know, I guess.
Find the opportunities there for the people that are using all the time to sort 
of like build on top of that experience. Like make it quick. I have to decent 
things like am let them customize certain things in a way that like enables them 
to sort of really mold get her to, to that flow. Yeah. Like the, the, sorry, I 
was just thinking like, There's a, it's like that you're a sort of keyboard, 
right?
Your computer keyboard. Like you want like people to be able to, you know, the 
letters are in and type it, but it's customizations you can do on top of that to 
really. So that around you experience, maybe you want to, I'm in a more 
comfortable position that you want different sort of like types of keyboard 
keys, because you, that works better for the, for the way that you are using 
your computer.
If you're typing a lot, you want some delight in there. So you want some colors 
because will make you feel happy, but maybe you're like mapping different keys 
to operations that you want to do, like really frequently. I think those are the 
sort of like, Things that you want to make an add on and not get in the way of 
the core experience.
If that makes sense. 
**Michaela:** [00:22:00] Yeah. Yeah, definitely. And I mean, one of the things that 
came to my mind when you, he said, well, make everybody feel like an expert, and 
this is really a tiny thing, but it's one of the first things that if you go to 
GitHub and you want to clone a project, you have to get bash command right 
there.
Every time you're clicking on that. You have it right there and it's somehow not 
intrusive, right? It's not like, Oh, you think I have seen that hundreds of 
time? How can, it's more, it's subtle, but it's there. You don't have to look it 
up. I mean, even if you're cloning a system quite often, if I do it, I don't 
know, second month I might look at it.
Right. I might look it up just to be sure that I'm doing the right thing. Uh, 
but here I know it's, it's there. I don't have to go anywhere. Right. So there's 
a little bit reminder. Yeah. So this is one thing that came to my mind. Well, we 
talked a lot about design systems already without really introducing it.
And yeah, I have a lot of my listeners and myself, we are engineers. Uh, so can 
you explain it a little bit? What are design systems and you know, how do we use 
them? Why do we need them? And yeah. 
**Diana:** [00:23:10] Yeah. Um, gay question again. Um, so I would type that like a 
lot of engineers who are working on the front end interact with design systems 
or have, have some awareness, but basically a design system is, you know, 
essentially.
Thanks sense of sort of rules and, and principles like codifying code in design. 
So like the implementation of our system exists in a few different forms, right? 
So it's it's components. And for us, we have, you know, a few different 
implementations. It's also on the design side. It's also those components 
existing in designing tools for designers to work with.
Yeah. And then the connector is really the, the sort of API of the system, 
right? It's the bridge, it's a design language that you're hopefully developing 
to make it easier for designers and engineers to have conversations about. And 
the UI. So that they can say, I want a three column grid and you know what that 
looks like, where I want the primary button.
And they, they knew what that is in both design and code. So I, uh, I like I 
would go is really to provide that sort of cohesive design language so that 
people can represent the brand and the product UI in a consistent way. But it's 
also about efficiency. So we see, you know, in the past we've seen people 
reinventing the wheel in design and code.
Like we don't want someone. The really simple example is like, we don't want. 
Yeah. Someone to, to waste time, we redesigning our primary button and recoding 
it. Right. But that's, we want them to be thinking about the feature and the, 
the, the flow and the, the core experience. So whenever we can find that we can 
solve like a problem once that can be reused many times, that's like something 
that might end up in the, in the design system.
I think like over time, we, with those sort of very basic building blocks that 
those are now we're sort of thinking. At a bigger scale, like how do you, like 
many, the components fit together? What are the sort of longer form like 
interaction patterns and like what sort of like onboarding experience, for 
example.
And so it really, yeah, there's a, you know, systems are kind of like, Assistant 
a system of systems. There's like many parts to it. There's a rambling answer. 
But did that, did that cover it? 
**Michaela:** [00:25:44] Yeah. Yeah. And well, especially from the last part, what I 
got is that, so how you started having all these little individual units, right?
Each button is a unit. Each input field is a unit, and then you say, well, it's 
actually not only the input. It's how it looks. And, and you package it and so 
somebody can take it and use it somewhere else. And it's the same, it's the same 
thing. And then you say, well, not only the input in the button is something, 
but a beach is something.
So somehow you have like this little system, then you have a larger system, 
which is a, is it. It's a page and then you have the system of systems as you're 
sad Valley, it's not a page, but it's a page flow. Right. So it's, that's what I 
understood when you say, well, how is the onboarding experience, right. So 
you're thinking really about when do we want to have the user, uh, see message, 
for example, do we have, you do have to click three buttons or, you know, goes 
through three pages or something like that.
And so, so it gets more and more. On one hand complex, but on the other hand, a 
little bit more mature. Is that, is that what you experienced at GetApp over the 
time? 
**Diana:** [00:26:50] Yeah, I think it's largely to do with scale. So saying, yeah, 
it, you know, you have to start somewhere, so hopefully it does get more mature 
you as you grey the system, but as get hub has.
Introduce more features as the team sizes grind. We've had scale the system with 
it. We started off with a very we'll make like utility first, a very functional 
sort of system. That was lots of small building blocks with a lot of 
flexibility. And now we need to sort of have more constraints and sort of larger 
pieces of the system sort of plugged together and a lot less variation.
So that means we're sort of choosing to reduce some flexibility in places where 
the, the, the value of flexibility doesn't really pay off, if that makes sense. 
**Michaela:** [00:27:41] And so. One of my question that comes to my mind. If you're 
talking about something like that is how does technical debt of for example, 
legacy code, right?
How does that, is that something that's also a problem for design systems for 
designers that you say, well, you know, now we want to have a fresh logo. We, we 
rethought what people actually want or how, you know, how to the UI should look 
like, but now we have this system and it's in so many places. How do you.
How do you change that over time? How do we evolve a design system when you work 
with older parts of the system? 
**Diana:** [00:28:18] Yeah, a lot of refactoring, but I think, I think like, like at 
the point of a system is to be built from enabling change, um, in my mind. And 
so it's actually, once you have some part of a system it's easier to make bigger 
changes than having no system at all.
An example that of that is a couple of years ago. Probably like three years ago 
now I worked on introducing a color system to get ahead of where we didn't 
really have one. We had a very small handful of, of variables, like sass 
variables. And we had over 2000 like hex values that were just like not 
connected in any way.
And so now that we have some system that yeah, enables us to do, we have a 
system of variables we have now, it's more like we have a handful of, of. Of 
values that are outside the system. The majority of the UI is using the system 
variables that makes it easier for us to do more work on that system. So now 
that we're introducing something like working on something like doc mode and 
building another layer of abstraction that is far easier than starting with 
nothing at all.
But yes, it does mean like making updates to the API of the system. And so that 
does mean like breaking changes at times. And so what we have to do is we have 
to do like an amount of a fair amount of record back to work, but we also 
prioritize that in, in a few different ways. With like visual refreshes, for 
example, we'll prioritize that around all like most visible core components.
Like when I call primary buttons, most highly visited, like iconic sort of parts 
of our UI. So like on most highly visited pages, like the repo. Iconic parts of 
the UI, like the contributions graph, the lots of sort of, we lived in looking 
at things like, what did the snippets of get hub UI that people share on 
Twitter, for example, to help us like, get a sense of that priority.
Because if we try to be like, Oh, we have to do it. We think all in one go, 
we're like, we're not going to enable ourselves to sort of like iterate and 
incrementally progress for you, this stuff. And like learn from it along the 
way. So another way that we tackle sort of these risk factors is like, you know, 
we do look for shortcuts while I was training.
You know, I think systems teams generally trying to. Fill it for the long term, 
they're looking at things very holistically, whereas feature teams that are 
working towards sort of different goals and timelines, we still also look for 
shortcuts like shortcuts and like interim fixes that we can do. And the metaphor 
I can think of is things like codeine.
Um, so we just did like a update to our icon system. And while we actually. 
Well, that's a really reflected an updated, like the, the, the instances of, of 
those icons in get her.com. There were a ton of cases where we made our best 
guess and just match the older iPhone to any icon. And because we had done that 
in combination with spending a lot more time, like fine combing fine-tooth 
combing through like our client pots of UI big Mo like highly visited pages.
Yeah. Then we have more confidence that the, we already have the UI changes are 
going to look good. They're going to, it's gonna. That it's going to be not very 
highly visible bugs and they, because we do things like trying to iterate and 
ship this internally and gradually ship this to customers, we'll pick up the 
sort of dark corners that we've missed and they sort of smaller UI bugs along 
the way.
So even with like visual refreshes and we still are able to like prioritize and 
break things up incrementally. 
**Michaela:** [00:32:13] Yeah. That's really cool. So. You're talking a lot about 
refactoring. And 
**Diana:** [00:32:17] when I hear 
**Michaela:** [00:32:18] I'm thinking about tests, that's the first thing that I was 
thinking about, like the safety net that you have with regression paths so that, 
you know, you're not, you know, screwing something up.
And, and another thing that comes to my mind is code reviews. Right. Or having 
other people look at the changes that you're introducing, if they're not 
breaking anything. So how is that for designers? Do you have a software 
engineering? Practices like that. I heard you saying something about code 
reviews, but it seems like more, you're looking at the code reviews of others, 
but how does that work for, for designers or if you're changing your design 
systems, do you have like contributes or do you have like tests that you're, 
that you ran regression tests, automated tests and yeah.
How would that look like for a refactoring of all of those iconic pages? I 
imagined this is like high risk thing. So you don't want to break anything here. 
**Diana:** [00:33:10] Yeah. I mean, honestly, like I think we're finding some gaps 
in that we want to build more testing infrastructure so that we have a higher 
level of confidence in that some of that testing can be a bit less manual.
I listened to your. I think you had, was it ? Yeah, so I, that was really, that 
was really interesting to listen to you. And, um, you know, yes, we, we were 
trying to find the places that we do have tests. Like we have, it's easier for 
us. It's not too difficult for us to have sort of like unit testing and stuff on 
our actual component libraries.
But when you get to like, get hub.com. Being able to have tests to like seeing 
that sort of visual regression is, is something that I think there is room for 
improvement for, I get hub. They still like a fair amount of sort of. Manual 
element to that work. And that's, you know, definitely a concern when we're 
doing sort of invisible changes or changes that should be invisible like that.
The user shouldn't notice it's really our sort of the infrastructure behind the 
scenes. And so, yeah, we do do a lot of code review that we do have lenses. Does 
that help us like spot, I guess, deviations from the system that like help us 
go. Okay. There's a potential for rescue. This could bubble down and effect have 
unintentional, like side effects.
But we do, we do have like, like a bunch of, like, we have a lot of like CIA 
checks and stuff that help us like catch things, help us catch things like 
accessibility issues. We have vessels. So you get maps into sort of the local 
development environment too. So you can, you can run fences and. Run some 
accessibility, tooling and wiring liquid development to try and catch some of 
those bugs.
But yeah, we also have like in person or async like design reviews too. And so 
just like, like odd team mates to talk about code as well. And when we can, we 
like to sit in when it makes sense to, I really love this kind of approach of 
like, Really driven, um, development. So like design needs the API before you 
start.
So they're like really building it. So, cause that's sort of like the interface 
that people are going to use. And I feel like that's a good way to sort of walk 
people through the experience of this sort of. UI component changes. And in 
design, what we want people to do is also walk through what's the customer 
experience going to be of this change.
And so I think, you know, designers have to be, you know, it's helpful if they 
get sort of storytellers really is like helping the audience that they're 
talking to you, which might be like other PMs leadership or their engineering 
managers, and get a sense of the experience that a customer might have. So, 
yeah, we have like regular design reviews code code review, like, like actually 
three of the products, but also we do meet in person to talk through stuff as 
well.
**Michaela:** [00:36:11] Very interesting. Very interesting. I love to hear you 
explain that to me. What about feature flags? I think probably with the user 
base of GitHub, it's, it's really nice and very practical to use feature flags 
and see, you know, how. How people behave. You know, you, you talked also a 
little bit about metrics.
Like if you're rolling out a feature and you see, like, people are opting out 
one of the metrics, so are you using features, flags a lot? And what are some of 
the other metrics that you are, for example, getting there probably depends on 
the under feature, but what are some of those common metrics that really are 
insightful to help you understand whether or not there are some problems with, 
with the design, with the, with the feature.
**Diana:** [00:36:53] Yeah, so we, yes, we definitely use feature flags a lot. Yeah. 
Like that's most of them development and.com is done behind a feature flag 
because that gives us a level of safety because it enables us to roll, roll that 
back and be very intentional about who we're adding into that feature folks. So 
some, sometimes PE teams are just using that with their teams as a way to sort 
of work behind that feature together.
Um, and then sometimes we also use the feature preview function that I mentioned 
earlier, which actually gives a way to, like, for your customers to like opt 
themselves into that same feature flag, basically. 
**Michaela:** [00:37:33] What are some of the, you know, what are some of the probes 
that you're actually placing throughout your work too, to get some feedback?
**Diana:** [00:37:42] Yeah. So we have a, we use feature flags more for, yeah. 
Rolling out like a feature rather than something like an experiment. So we do 
have a slightly different approach, even though I might be using some of that 
same tooling, if we want to do an AB test. And so we have a data scientist, I 
get her that week.
If we want to like, compare like a design to another design. So. If it's in a 
conversion flow or something really important, like for example, we have a 
sponsor's feature. We wouldn't want to negatively impact sponsorships. We 
wouldn't want, we wouldn't want to reduce that metric. So individual like 
feature teams and, and, and then we put, you know, we do have like a set of core 
metrics that we.
Um, watch very carefully. And so if I'm walking on it, my team is working on 
something that you like might bump into one of those features, then I'm likely 
to then be having conversations with that PM and discussing with them, like, 
what are the metrics that we need to measure here or watch for? Do we need to, 
is it going to be talking to data science?
Do we want to run an AB test before we do anything? Or is it just something that 
we want to. Track and make sure we're capturing metrics for, as we slowly roll 
this out or in case we do need to roll it back. So yeah, it depends on the 
feature, but yeah, we, it would be a collaboration with, with products and with 
data science, depending on what type of thing we would, we would changing 
basically.
**Michaela:** [00:39:24] Okay. Yeah. So maybe I want to switch a little bit the 
gears. Talk about a different topic, which I'm really interested in. Um, and 
that would be your experience in a, in a very remote first organization. Right? 
So I have worked as an ICU, individual contributor in remotely workplaces, but 
I've never worked there as a manager.
And I, I somehow feel, or imagine it quite tricky to be a manager and people 
manager in a remote set up. How do you experience that and how do you. How do 
you get the opinion of everybody and how do you connect with people? What's 
what's the new secret? 
**Diana:** [00:40:06] I said, if I have a secret, I think it's a thing that is 
challenging.
I think GitHub is fortunate to have been like a remote distributed company from, 
from the beginning. And so. I F you know, for me, it has been a pretty great 
experienced, like this was my first like full time remote role. Yeah. When I 
worked at, at, we did have team members that were remote. Yeah. The core design 
team were mostly in one place.
I wasn't the roommate person. So this was like really my first experience of 
that. And it, it was, it definitely took a bit of getting used to, and I'm, I'm 
not sure, sure. That there are things that are necessarily like harder being a 
people manage it, being remote than there are just like being a manager is just 
hard and being remote.
It's just hard. And like the sort of. The crossover of those two worlds can 
maybe, yeah. Exacerbate some things. I, you know, I think the hard thing is 
always like building connections for me. One of the practical challenges is 
being mindful of that different time zones. And, and trying to, if I do want 
FaceTime, you know, there's sometimes that it's just not.
Really possible to get every it's not really possible right now for me to get 
like every single member of my team, unless someone is great working in very 
undesirable and hours. So what we're trying, you know, what we try to do? I 
have. They smallest sort of meetings and connections that have the async 
communication and Slack.
And we also do racing design reviews. So we use, like, we have discussions that 
we use fig, which is, is pretty helpful for us and works well for us because it 
means that. If people are in the same time zone, they can jump in, in the same 
tool and be in connect because you can jump on the web. Right. And so you can 
like be in the same tool together, which is fantastic for designers because they 
can like move things around together.
But on the async side, they can email each other comments and chat about stuff 
later. So, yeah, it's just, it's really just being mindful of different. Ways of 
working, keeping, making sure that we keep working really hard at the, the async 
communication, not relying on, on, on, in person meetings all the time and being 
too biased T to like one particular time.
But yeah, it's definitely, definitely challenging. I can't help, but point out. 
That it's been even more challenging and then than usual. And so sometimes it's 
just been helpful to have casual hanging out time, like social time for people. 
We've, we've either just like jumping on a call and just like hanging out or 
having a silly game to play.
You know, we did like a demo day, a couple of weeks ago, and it was just super 
fun. Like there was people that were in Europe that stayed up. Like we started 
it in Europe time to get through the, and to go all the way through like the U S 
time so that people could do. You know, some stuff in person, but watch 
definitely knew, but didn't want to, but some people were so excited that they 
stayed up till like 1:00 AM, so they could like be through the whole thing.
It was like a conference. And that was just great. Cause it was like a way to 
like, have everyone together really celebrate the work that we're doing. So I 
think finding the opportunities for like a bit more human connection, it has 
been a bit more important because we don't, we're not able to sort of meet in 
person at the moment.
**Michaela:** [00:43:48] Yeah. I actually see a lot of the things that you stress 
here for remote work is something that's a very good mindset to have also for 
your design systems, right. For the inclusive design. And so you have, I'm 
thinking about time zone, thinking about other people's experiences that maybe 
they have like dinner now, or they have kids at home and it's lunchtime and 
things like that.
So, yeah, I think this is probably something that makes you very strong also on 
the, on that, not that part. Well, yeah, thank you so much for, for being on my 
podcast, being on my show. It was really fantastic to talk with you. I could go 
on and on, but you have to, we have to stop at one point. So thank you so much 
and yeah.
Have a good day. Enjoy your day and hope to talk to you soon again. 
**Diana:** [00:44:34] Yeah. Thank you so much. So I really enjoyed it and yeah, I 
could keep going. So thank you very much for having me on the show. 
**Michaela:** [00:44:43] Yeah. Wonderful. Okay. Bye bye. 
**Diana:** [00:44:45] Bye. Bye. 
**Michaela:** [00:44:47] I hope you enjoyed another episode after sup engineering 
unlocked podcast.
Don't forget to subscribe and I talk to you again in two. 
**Diana:** [00:44:57] Bye.


