# Transcript Episode 29 with Kent C. Dodds

**Michaela:** [00:00:00] Hello, welcome to the software engineering unlocked 
podcast. I'm your host, dr. McKayla. And today I have the pleasure to talk to 
Ken, C. Dodds - once again. 
Kent is a software engineer and teacher. Before he 
started this training business he worked for PayPal. He's a major open source 
contributor, and also the creator of the widely used open source testing library.
Code that he writes is used by millions of people around the world. And he also 
teaches thousands of engineers, how to test their Java script systems and how to 
work with React. 

Yes, Kent already joined me for an expert talk about 
testing, but after talking about over an hour, we still had many things to 
discuss. 

But, before I started, If you enjoy the show, it would mean the world to me, 
if you leave a review on Apple podcasts - or any other podcasting platform of 
your choice. 

You can also help me, by telling your friends about this podcast 
or sharing the episode on Twitter. 

As I want to spend even more time making great 
new episodes for you, I decided to open the podcast up for sponsorship.
I will be very selective, but if you think you might be a good sponsor fit for 
this show, have a look at the website: se-unlocked.com. Right at the top, there's a 
sponsorship page. I will also link it in the show notes. 
But now let's get back to Kent. Kent, welcome to my show. 


**Kent:** [00:01:19] I'm super thrilled to be back here.
Thank you so much for having me again. 


**Michaela:** [00:01:25] So last time we talked about integration versus unit 
testing and you stress that well with the tools that we have nowadays 
integration testing is actually what gives us more bang for our buck. I don't 
want to repeat our conversation. I will link to previous
episode in the show notes. But I wanted to dig a little bit deeper, especially 
when we are talking about integration and system tests, the concept of mocks 
comes up quite a bit. So mocking actually means that you create a fake version 
of your service, of your method, of your unit, right? That you somehow replaces 
the real one so that you can test faster or, you know, more quickly without, you 
know, spinning up another system and things like that.
But yeah. If you're thinking about that, what do you think about somehow? We are 
still not testing the real system, which was one of the things that you said is 
really powerful for integration testing, right? That you are, that you are 
having the whole system there. And you're not just one isolated thing.
So if you're writing a lot of those marks, somehow we are again, creating a very 
artificial environment environment. What do you think about that? And how do 
you, you know, what do you say in your courses about marks? What should people 
do. 

**Kent:** [00:02:36] Yeah, that's a great question. Mocks is a big subject and 
first I'll, I'll preface it by saying that there is a place for mocks, but the 
reason I preface that is because when I'm about to say is going to make people 
think that I don't think we should do mocks.
So, uh, if like the, the reasons that you mentioned for why, um, people want to 
mock it so that they can write tests faster and various other things like that. 
But that's actually not the reason that we test, right? Like the, the reason 
that we're trying to. That we write tests is to get confidence. And so anything 
that we do to reduce the amount of confidence that we get is actually making a 
trade-off on our purpose for writing the test in the first place.
Now there are reasons to do that, but I think it's important to recognize that 
mocks are the antithesis of what we're trying to accomplish. And it actually 
makes it like. From a purely, like full philosophical standpoint, you shouldn't 
mock anything because it's the, it allows you to do the opposite of what you're 
trying to do when you're testing, which is reduce the similarity between your 
environment and the environment that your users are running your code in.
And so that's something to keep in mind is that when you're mocking, you're 
making trade offs here that take you further and further away from your goal. 
That said there are reasons to mock. And my favorite example is let's say that 
you're an e-commerce platform and you want to verify that people can add items 
to their cart, remove them from the cart.
You see the total, you know, the cost. And let's say that your e-commerce 
platform is for people to buy boats. And so this is like tens of thousands of 
dollars of product that you're adding and removing from your cart. And then you 
want to make sure that the checkout process works. Okay. So to do the checkout 
process, you need to give some credit card information, and then you hit 
checkout.
And then all of a sudden, every single time you run these tests, your credit 
card bill goes way up because you're buying all these boats. So that wouldn't be 
a very scalable solution, right? You don't actually want to charge your credit 
card just to verify that your checkout process works. And so that right there is 
a place where you need to slip in some fake.
Environment and the surfaces that you might be using, like Stripe, they have a 
test environments that you can hit that will say, like do everything except, you 
know, give me a test environment. That's really a mock it's a mock that's 
provided to you by your provider, but it is a mock it's not actually, what's 
going to happen in the real world.
But if you did exactly what happens in the real world, then. Like, that's not 
practical. And so monks are really there as kind of a stopgap mechanism to 
enable you to test certain things that would be impractical to test otherwise. 
And so we do make this, this trade-off, and that's not the only example.
There, there. Various other reasons where mocks can be useful and we can dive in 
deeper to that. And in particular, when we're talking about the different levels 
of testing, like we talked last time, but I think the main takeaway is mocks 
poke holes in reality. And when you poke a hole in reality, then you lose a 
certain amount of confidence.
It's like poking a hole in a ship, you know, it starts taking on water. You got 
to fill that in somehow with something that maybe isn't as strong as what. You 
know, as the part of the ship that you poked a hole through whatever, but it 
resembled that piece as closely as you possibly can. So you can, so you can kind 
of sidestep the issues with losing the confidence that you lose by marking in 
the first place.


**Michaela:** [00:06:11] Yeah, I think you have a very, very good example. I 
would like to put another example, which I think is another reason why we have 
marks and it's a little bit, probably more trade-off recent, right? So charging 
something is very reasonable. We think, well, we can't do that. But for example, 
I think mocks are also, they also play a role for speed.
Right. So I am, I'm really obsessed also with speed for engineering teams, 
because I worked at very large corporations. So I know that if you have large 
software systems, speed always become somehow. You know, I saw that should be 
also in the front of your mind. And so. Let's say they are waiting for another 
system and it creates something, let's say a PDF, right.
This can take. And if it, even if it's just taking a few seconds, right. If 
you're thinking about how many tests you're running, this can become really 
cumbersome or, you know, you're spinning up a whole database or, you know, 
whatnot, something like that. If you're thinking about isolation of tests, 
right.
Again, then we were thinking about that. We actually have to create the systems 
and this can take some time. So. I think speed is another reason why we actually 
have to make trade-offs. And I really like to think about trade-offs a lot of 
things are trade offs, like also in code reviews, we have a lot of trade-offs to 
make, right?
How many people do we put in a code review? The more people we are putting on 
the code review, right? Maybe the better our feedback becomes, even though there 
is like the bystander problem. At a certain level of, of people that you're 
adding, but let's say between two, three people, we have to think, well, maybe 
one person is enough just because of the speed.
And here, I think with, with marks the same thing. So sometimes we want to mock 
something because we can save real time that we might need to, to have our tests 
pass faster. What is your thought about that? 


**Kent:** [00:07:56] Yeah, that's a perfectly reasonable trade-off for making. 
And I think it's just important to recognize that it is a trade off.
A mistake that I see people make is they, they go for full on mocking of 
everything. Let's isolate all that, our tests and things. And you can that 
example of a PDF that takes some time to generate as a great one, because I 
agree if you have just a full suite of integration or end to end tests, and each 
one of them is going through that code path.
Well, You, you get the confidence that you're looking for with that particular 
generation code by generating it just one time. Now you don't need to do it 
every single time, you know, unless there are certain parameters or something, 
but you're getting the benefits of the integration. By just going through this 
one time.
And so every time thereafter is what we call over-testing where you're, you're 
double testing or triple testing where you, you end up testing it more, but 
you're not actually getting any more confidence because you already got the 
confidence that it works. And so. For a situation like that, you, you have the 
two extremes where one says, let's just mock everything and I'll test this and 
isolation and this in isolation, and then just pray that they integrate, or you 
have the other side of it where it's like, let's just test everything in 
integration always.
And I would tend to go on on the far end side of let's test everything in 
integration. Because I, at least I'm not losing any confidence. And, and then I 
would work my way back to optimize things for, for test speed in that case. So 
if there really was a situation where every single one of these things is taking 
this like a significant amount of time longer because of this, then I will.
Keep the real deal for one of those. So I maintained my confidence and then just 
mock for the rest. And I think that's a reasonable approach. It's just, you 
really want to make sure that you recognize the trade-off that you're making. If 
you don't have any tests that verifies the integration of these things.
And so this is where like the different tests levels really comes in handy in 
our conversation here. 

**Michaela:** [00:10:01] Yeah. So I actually want to maybe open the box of the 
Pandora a little bit with, you know, if we are talking about the reality of our 
system, then we are thinking about, well, you know, you have the units, you 
have, you know, system or integration tests with a lot of marks you have maybe 
done without a lot of marks.
Right. Uh, but also we have to think about our environment. So, what are your 
thoughts about, you know, testing in the test environment, in the staging 
environment? How similar can we make our environment to the real environment 
that we have and, you know, and then taking the whole thing a little bit further 
and thinking, well, why are we not testing in production?
Right. Do we have to be there? The people that, that test can we have our users 
test, right. And what role do automated tests play for this whole idea of 
testing and production? Having, you know, feature flags, having real users 
actually test out our. Our system, really small pieces of, you know, large user 
bases.
And then we quickly can also see what's going on here. So how do we balance 
that? And maybe let's start with, with, with the environment question, right? It 
should be having like a test environment. How, how do we make sure that this is 
really representing our real production environment and things like that?

**Kent:** [00:11:11] Yeah. Yeah. So I can't remember. I recently had a 
conversation with someone about this and it actually may have been our 
conversation last time. So if it was then let me know, but somebody told me 
recently and it makes total sense to me that Netflix actually will do AB tests 
or a feature flag and just enable a new feature for a very small fraction of 
users or, or they actually will.
If I remember right. Whoever it was telling me this, they, they will enable a 
feature and just roll it out very slowly. And then they actually have an 
automated process that will, as it's monitoring error rates and stuff, it will 
automatically roll back on that. And so when you have the user. Based that 
Netflix has, then you can do stuff like that because you were talking a couple 
hundred or maybe a couple of thousand users out of their enormous user base will 
have like a small problem where their video won't load right.
Or something. And they'll just refresh and move on with their lives or whatever. 
And so like, Yeah, you could, you could actually just totally go a feature 
flags. Don't worry about testing before deploying and you just test after 
deploy. And I actually don't think that's a terrible solution for a company.
The size of Netflix or Facebook, Facebook does something similar where they with 
react. You can build react with certain profiling features enabled, which just 
add a small performance hit to your, to your app. But it's big enough that they 
don't enable it by default. And so they, they just enable this for a small 
fraction of their users and keep monitoring things as new releases come out and 
then they can roll back if there's any spike in some performance problem.
And so, yeah, you can, you can kind of segment users, you can add monitoring and 
then you can actually. Like actually test in production. So there's somebody 
that I talked with on my podcast chats with Kent. Her name is Tanya, and I'm 
going to find out really quick where she works, because it's a company that, 
that does actually, maybe I'll I'll look it up when you're asking me the next 
question.
Cause I don't want to 

**Michaela:** [00:13:09] wait. Take your time. Just look it up. 

**Kent:** [00:13:11] Yeah. Yeah. So it's, my podcast is called chats with Kent 
and the conversation. It was very interesting. So I do recommend that people 
take some time, but yeah, her name is Talia Nazi. And she works at a company 
that does feature flags that I'm looking up right now at split.
Yeah. So a split just manages these feature flags and she really promotes 
testing and production. And this conversation, when is all about that testing 
and production. Very interesting. It's actually the same season where I had you 
as a guest. So people can listen to your, her episode is right after yours.
So, but the idea is that. When you have feature flags, you can just enable new 
features for different users or for a small subset of your users. And then you 
actually write automated tests that have those feature flags enabled. And if 
you're really worried about it, or if it's a brand new feature, then the only 
user quote unquote would be the test user that you have running through these 
tests.
And so you go ahead and deploy, you run all of your tests in production after 
that deploy. And if there's a problem, then you can roll back and it's fine. I. 
I think that's an, like, that's probably a thing that you should do. It makes a 
lot of sense. I never have done this myself, but it sounds like a very 
reasonable thing to do, but I struggle to jump on board with, with doing that as 
a, a, the only testing strategy in particular, because like, it works great for 
new features that you haven't enabled yet.
And that you're, you're testing as you're getting ready, but once you've enabled 
it, If you release that and users start experiencing problems before your test 
can report to you that there's a problem and you can roll back, uh, then like 
you, you could make it so that for a few minutes, people can't check out, which 
would be very bad for you depending on the size of your business.
And so. I think tests like testing and production is the ultimate way to get 
confidence that your software works when your users are using it. A user 
monitoring is a fantastic way, because then, then you get like an actual user 
was actually using the software and this was their actual experience. Like you 
can't get much better than that, if you have good monitoring in place.
And so all that. Other testing can do for you. There, there actually a couple of 
things that a testing before production can do for you. And one is making sure 
that no user experiences, those bad things in the first place. And so if that's 
really important, you know, if you have Netflix size, your user base, then maybe 
you don't care about the, you know, Dozen or so people who had experienced a bad 
experience, I guess, but it's about, I think most people don't want any of their 
users to have a poor experience.
And so, yeah. Testing before production, that that's kind of a good argument for 
that. And then the other is your, your testing speed because it's, it's really 
not reasonable or feasible to do a lower level testing in production. You can 
really only do end to end testing and production, which, you know, is.
Is great, but you, you end up doing a lot of over-testing and the test takes 
much longer. And so it's, I would suggest that testing and production is a good 
idea. And just one additional type of tests that you could add to your test 
suite. 

**Michaela:** [00:16:28] Yeah. So one of the things that I think is really, 
really important that we stress it is that whatever you're testing would feature 
flags and have actual users impacted you have actual users in perspective.
Right? So let's fix is a good example because I, I don't know, maybe I'm the one 
that always gets the feature flag. You know, it, it's something that if your 
user experience is well, it's true, right? You have millions of users. So if 
100,000 people, you know, experienced something, what does this mean? But you 
know, it's not 100,000 people it's, there are so many features.
Like there's so many different things that they are testing. So. It will always 
impact one part of those, you know, millions of people. And so overall, I think 
everybody has a little bit of a worse experience using the app. I'm not, I'm not 
against it, but I'm just saying, even if you have like really large user bases, 
you have to be very careful about the image that you're putting out there.
Right? So this is your software and people are like for Netflix, you're paying 
their other providers as well. Right? Always also depends on the shows. If 
they're not there, maybe you're still sticking with this with this app. If 
you're, if you're not happy. That at one point, people are annoyed and they are 
not trusting.
And you're losing the trust of your, of your customers, which I think is not a 
good thing. And so I think another thing you mentioned the size, right? The size 
is I think really important if you're thinking about feature flags and testing 
in production, AB testing, because sometimes, you know, if you have like a 
website or a system, right, and you have like hundred of users per day, you 
don't get enough.
Quantitative data to actually make any conclusions out of their behavior. Right. 
So I, when I worked with one company, they had a lot of monitoring around their, 
their system. I'm not sure if I can say which company. So I just not say, but 
when they had like a company, so, uh, a software system to make phone calls, 
right?
Like voice calls. And, and so what we did there is we were monitoring. You know, 
how long are the calls, for example. Right. And so you need a certain user base 
to actually see variances in that. Right. So we had also, things were adapting 
with the time because it depends on the day that you're having on the time that 
you're having.
Right. So there was some artificial intelligence around that that could actually 
understand, you know, what is the frequency of calls and how long are they 
normally durations for this large user base also for the right region and things 
like that. Right. People to actually use your system to be able to build 
something like that.
And it learned over time. So it knew that, you know, three weeks ago, you know, 
the average duration of a call was 45 minutes or, you know, 44 point something 
minutes. And so if today the average would be 30, right? So you would have like 
some, some, some range where it could vary. In between, right. If it's something 
is going on, right.
So we will re would raise by Tampa, some alerts and things like that. But as I 
said, you need some, if you're just starting out and let's say you have like 
1000 users per day, you're probably not able to do, to build a system like that. 
Right. So I think. Testing in production and especially AB testing is very 
powerful, but you need a certain volume of users, not only so that you cannot 
annoy everybody, but also to actually make sense of the data that you're getting 
from, from, from the tests that you're running.
Well, so something else that I wanted to talk with you is we talked a lot about, 
about testing and we were very language agnostic, right. But you're coming 
really from the JavaScript and react side. So audio, some language agnostic, 
things that you think holds true. And what are some very specific things that 
you think are important for JavaScript?
Something we talked about was for example, that, that we have like the type 
checking, right? For example, static analysis. And those things could be more 
important for JavaScript systems, right. Or, or a system where we don't have the 
type of system behind, but are there some other things that come to your mind?
But we think, well, this is really specific to react and JavaScript. 

**Kent:** [00:20:34] Yeah. So the user interfaces are kind of unique in, in 
testing. I, I think that, uh, a lot of people, or really used to testing our use 
of testing backends and historically over the last decade, maybe this, this has 
kind of changed actually in the last couple of years, but most people that I 
would talk with would say, You know, testing us is a waste of time focus all of 
your tests on the backend, and then just pray that the front end works.
Maybe you have a couple of end to end tests, but then the  that were written 
were very easy to, to continue passing, even if the UI was totally broken. So 
the, there hasn't been a whole lot until like in very recent years there hasn't 
been a whole lot of love for testing the front end. And the reason I think is 
because our tools were not well equipped for testing our software, the way that 
users use our software for the front end, you know, unless you like.
Build some sort of AI machine that can look at the screen and you, and, you 
know, interact exactly that the user does, then you're going to be like, that's 
very difficult to do it. Remember, like our goal is to get confidence and the 
more your software or the more your tests resemble the way your software is 
used, the more confidence they can give you.
Well, UI is used by people with fingers and hands and, you know, they're 
clicking around and whatever, or, you know, if somebody's blind to, they're 
going to be using a screen reader, that sort of thing. And like, that's really 
hard to automate that. And so the tools that we had developed were pretty, you 
know, not resembling that because it's hard to resemble that with software.
So what's, what's changed in recent years not to, to push my own stuff too much, 
but I mean, I guess so is that I created testing library about two years ago. 
When I was really frustrated with the fact that the tools couldn't resemble the 
way my software was actually used. And so what testing library does is it 
enables you to.
Interact with your webpage or with your react components in the same way that 
your user would. And I actually, before I get too far down, this, the reason 
that I think that back-end was typically tested better and more frequently is 
basically because. Like, I think most people recognize that you want to try and 
test your software the way that it's used.
And it's easier to test it the way that developers use your software, right? 
Because the way developers use your software is through other software. And so 
if you're writing software to test software, the way that other software uses 
your software, then it's a lot easier to do that. Right. And so like you're 
hitting API, just like the developer would, but it's hard to do what an end user 
would do.
Would do, that's why the UI has been typically very hard to test. Uh, and also 
the UI is hard to test because you're, the designs are always changing and 
because our tools were so implementation detail focused, because that was really 
the only way to test things. Anytime the design change that that would break 
your tests, like were, were.
Relying on the order of Dom nodes and stuff like that, you know, you're doing 
your X path or, or some class name or something like that. So it was really easy 
to break things with UI. So testing library comes on the scene and I say, users, 
aren't looking for a Dom node at all. And they're not looking for a react 
component.
They're not looking for any of this. They, they are looking for an input field. 
They don't even know that it's an input field. They just want a thing that they 
can click on and then type into. And they want that to find the one that is 
labeled with a certain text. So if I've got a login form and I want to log in 
and here it gives me my username.
And password as an end user, I'm going to look for a thing I can type in that's 
labeled username and I'm going to type my username in, and then I'm going to 
look for a thing that's labeled password. I'm going to type in my password. And 
then I'm going to look for a link or a button or something that indicates I am 
going to send to this information.
Right. That's what the end user is thinking. And so that's what your test should 
be thinking. And so testing library gives you API APIs. To access those Dom 
nodes for those things. So it is dumb nodes that you're interacting with because 
that's really the, our pro programmatic API for, for these types of software, we 
do have dumb nodes, but then it gives the API set.
It gives you, you don't very often have to actually interact directly with the 
dumb nodes in your test. You say, okay, go get me. The thing that's labeled 
username. And then I want you to type into this thing. That's labeled username 
and testing library will take care of going to get the Dom node for you and 
firing all of the same events that the user would fire it.
If they were to type in these characters and, and then, you know, go get me the, 
the button that says sign in and I want to fire a click event on that thing. So. 
We're simulating exactly what the user would do. Okay. Find this field, that's 
labeled username type in my username. Find the field that's labeled password 
type in my password.
Find the button that says sign in and click on that button. And then we'll move 
on with our test. And that's, that's the unique and interesting thing that 
testing library does. And it does it for your. Like, whatever framework that you 
have. So there's react. Testing library was the first, and then I realized how 
little react had to do with it.
And I pulled it out the core into Dom testing library. And now we have testing 
libraries for really anything that you can imagine. There's view there's. 
There's angular, like really all of the frameworks, there's also puppeteer and 
play. Right. And Cyprus. And I think somebody is working on a selenium testing 
library, which couldn't really use the core, but they're going to just 
reimplement it.
So that's, that's the basic idea is we have this core way to interact with the 
Dom that. Is similar to the way that your users would. And then your test can 
just resemble the way your software is written. And what is really great about 
that is it means that you can now finally refactor or redesign your UI and, um, 
your test should continue to pass.
Which means that your test can finally give you confidence in refactoring, which 
is a huge reason that we have tests. 

**Michaela:** [00:26:52] Yeah, it sounds really, it sounds really amazing. And I 
can totally see how, you know, you're not looking for this Dom element or as you 
said, right. We also had like the other way of those testing, your UI testing 
frameworks, or like coordinates, right.
I don't know if you have worked with something like that, but there you really 
have the coordinate on your screen. Right. So it also depends on how large your 
screen is, where this element is and things like that. Right. So it's very, very 
technical perception of the system again, which doesn't really.
Somehow reflect the user, but you know, there still is a little layer that 
somehow not tested and that would be really the visual representation. So I 
could have, you know, let's say a button and the button says user name, or, you 
know, I send it or something like that, but it could be that actually. Yeah. I 
can't see it as a, as a user.
Right. So it could be hidden or it could be, you know, to the background color 
and the foreground color could be so similar that you don't really see it. 
Right. It could be wide or wide, something like that. Or, you know, that one 
button or one element is before something else. So how do we, how do we make 
sure that those things are still tested?
There's I think there's still this thin layer. What do we do about that? 

**Kent:** [00:28:07] Yeah, that's a great point. So there are some automated 
things that we can do for, for some of those things. I'll preface all this by 
saying, you cannot automate all of your accessibility testing. It's just not 
possible. And so accessibility testing is very important, but there are 
definitely things that you can automate.
And there are tools for this. There's a tool called just acts, acts as a very 
common tool for accessibility testing, both manual and automated it's from DQ 
labs. Really recommend people who want to get into our accessibility testing 
should look into this tool. And so, like, it would be able to tell you certain 
things about whether your labels are properly associated to things.
And actually, this is one of the nice things about testing library, because it 
actually uses. The accessibility API for finding dumb nodes, your fields are not 
properly labeled, then you're not going to be able to find the field. And so you 
say, well, go find me the username field and I'll say, okay, well I found the 
label, but I can't.
I find that the input that it's too. So a lot of people, as they start using 
testing library, find that they catch a ton of accessibility bugs. But that 
doesn't help with the visual aspect, if it is like a white on white or 
something, or a hidden behind something. So this is where acts would come in and 
it can help find those kinds of issues.
If you're using Cypress testing library with Cyprus, then Cypress, won't allow 
you to click on things if they're hidden behind other things. And so you get a 
lot of confidence, like accessibility, confidence from that, but then still, I 
don't. I'm not certain of this, but I don't think that Cyprus is going to help 
you with color contrast issues.
And then aside from that, like, What if somebody makes a typo and actually flips 
your whole entire page upside down, which can happen like CSS, amazing and 
magical and scary, right? And that is a possibility. So, and all of your tests 
would pass even though like every everything in your page is upside down.
And so this is where visual regression testing comes in and there are some 
really great tools for this. I personally. I have never actually used this tool 
at production scale, but I've, I've learned enough about it that I feel 
confident recommending it to people. And it's called Applitools, it's a P P L I 
tools.com.
It is paid and it is not cheap. It's free for open source. So it's definitely 
something I recommend people try out, but it is very, very good at what it does. 
And basically the idea is you're running all of your tests and you say, okay, 
Applitools I want you to. To take a snapshot of this and what it does.
Like people listening have probably heard of tools like this. There was one 
called Huxley that was out of Facebook years ago. Uh, I tried that it was really 
finicky. Like it's really hard because basically it's like taking images and 
then comparing them and that. Can be very finicky. Well, Applitools just smooths 
out all of those rough edges and makes it really easy.
And instead of taking the screenshot on your local machine, it actually will 
take the Dom and everything of your app at the time that you said, okay, take a 
screenshot. It will zip that up and send it to their servers. And then they will 
pull that up in their grid of. Browsers and every viewport size that you can 
imagine and configure everything.
So with, with just a single test, you can get cross browser testing, like a 
single test run in a single browser. Uh, you get cross browser testing. You 
could even run it in just JS Dom. So not even in a browser and still get the 
confidence that it works in a browser by using Apple tools. So this is an 
enormous.
Like benefit because you now don't have to worry about running your same tests 
across 30 different browsers and viewport sizes and stuff. You just run it in 
one and then let Apple tools show you that it actually will work in those 
others. So a huge time-saver and it gives you all of the confidence about, you 
know, color contrast and, and those kinds of things.
Like somebody flipped the whole page upside down. Like that's not good. So you 
can. I would suggest that this is another tool to add to your tool belt, to get 
confidence that the software is actually working. 

**Michaela:** [00:32:14] Very cool. You answered actually, so many of my 
questions now I didn't have to ask because especially browser compatibility, 
right.
This is a hard, it's a hard problem. Right. Do we know that it works on all the 
different screen and devices and sizes and you know, we really get headache just 
thinking about that. 

**Kent:** [00:32:34] Yeah. And actually on that, I just mentioned also that if 
we're talking about performance and that sort of thing, like. Yeah, sure.
Maybe the test run pretty fast and everything's running pretty fast for you. 
When your tests are running on your Mac or in your CA if you want to actually 
run it on a mobile device, low end, okay. Low power device, then it's really 
difficult to get that performance metrics without actually running it on that 
device.
And you, you could probably, you know, you get sauce labs or something like that 
to. To run across everything if that's what you really want to do. But I would 
suggest that most people could probably get by, by just making sure that it 
works visually on those devices and then adding performance monitoring in 
production and just keep, keep tabs on those lower end devices and make sure 
that you don't have any regressions.
So this is one area where I think it's probably okay to let the user suffer just 
a little bit because the. The amount of suffering is probably pretty minimal. 
And the amount of costs that it would take for you to, to run your tests on 
those lower devices is probably higher than, than the benefit that you'd get by 
just.
You know, versus the alternative of, uh, just adding performance monitoring. So 
Applitools, isn't going to give you the, like the full picture of running cross 
browser, but it will get you as far as I think is reasonable for 99%. Of 
applications and that is what we call it. Good enough. 
**Michaela:** [00:34:06] Yeah. I think, especially when you're talking about 
performance, we as developers that really have nice machines and, you know, 
probably also nice phones, a nice take in general 

**Kent:** [00:34:17] sometimes.

**Michaela:** [00:34:18] Yes, exactly. Right. It's very difficult to imagine 
that, you know, even a large portion of the population, right. Doesn't don't 
have access to data. And I think if you're not. Careful about that. This can be 
a big, big hit for your business as well. Right? Because you're, you're not 
considerate of, you know, a large portion of the population and people that they 
also have access to your things.
So I had an interview with chair recently and she now works at Apple and she had 
like a lot of gigs beforehand. And she told me that because before she got this 
really nice jobs, she also didn't have like really nice. Uh, phones and, you 
know, so at that point, because she was suffering, she was one of the best at 
her company to really be careful and considerate right.
Of, of people that don't have like a nice. Yeah, nice Tash and nice internet and 
connections and things. Yeah. 

**Kent:** [00:35:14] Yeah. I, I do think that it takes a certain level of 
empathy that you need to, if you don't have experienced yourself, you need to 
try to put yourself in people's shoes. And so, yeah, I definitely don't want to 
give the impression that we're just like, okay, with those people's suffering.
I think that it's important that. Especially when you're building something new 
that before you ship it to production, you at least simulate that type of a low 
end device on your machine like that. We have tools that will do that. It's 
very, quite simple. Actually use the Chrome developer tools. You can throttle 
things at your CPU down and stuff.
And so at least simulate it, but even better, just get one of those devices and, 
and throttle like. Routers these days can throttle, you know, your, your network 
speed and everything. So you can actually experience what that's like and try to 
measure it so that you can improve it and improving it for the lower end devices 
will improve it for everybody.
So like, it's, it's not like you're, you're just doing work for the, you know, 
2% of your user base. And the interesting thing about that is that. Maybe the 
reason that only 2% of your users are on low end devices is because your app is 
so hard to use for low end devices. And so maybe if you improve it for those, 
your user base will increase because it's, you're, you're accessible to those 
people with lower end devices 

**Michaela:** [00:36:33] and also Google ranks you higher, at least that's what 
we say.
Right? So if that's one of your goals anyway, well, one of the things that. Came 
to my mind, we were talking a bit about it and you were touching on it for 
different things for the UI for performance is manual testing. Right? So we are 
talking a lot about automated tests Mo mainly because we are developing, but 
what about manual testing?
And also it's been a big shift, I think, over the years, right? So there were a 
lot of QA teams, a lot of manual testers. For example, when I started at 
Microsoft, there was still tons of teams in divisions that are chests. Focusing 
on testing the software system. And then, you know, there was this whole shift 
in mindset that, well, somehow they are integrated and you know, those manual 
testing teams actually went a little bit away or were less important.
And I think you can see that at many, many other companies as well. So it's 
manual testing, still a thing is that still needed? When is it needed and how 
does it, how does it, one of my biggest question always is how do you see. The 
fit between manual testing and continuous integration, right? So we are 
constantly pushing to production.
You know, we want to make this cycle time really short, but still there should 
be some time that, you know, if you have some manual testers there that they 
take care of, of our changes before it actually hits production, or is it also 
in some continuous. Increased release testing cycle. I don't know. What do you 
think?

**Kent:** [00:38:06] Yeah, well, you know, if, if we extrapolate what's 
happening in the software world and interest in the world in general, we'll see 
a trend toward automating things and, and it's a very reasonable trend. So like, 
I, I'm really glad that the process of extracting money from my bank account has 
been automated so that I don't have to like go to the bank to get money from one 
place to another.
And so like, Just so much of, of things have been. In fact, I have never, I it's 
been like years since I actually used a cashier at the grocery store. Like, so 
we're, we're automating all sorts of things and there are good reasons to do 
that. And we, we start first with the things that are more painful and so.
Like manual testers. Let me, I should have said this first, they still have a 
place for sure. But eventually we'll probably get away from even writing the 
software ourselves. Like, I don't know how far into the future that is, but 
eventually I envision a future where most of the software is not written by 
humans.
And so it's just a matter of like how much of this can we automate and still get 
confidence that things are working. So eventually, like I. I, I think that 
eventually we will have fewer and fewer manual testers and we'll be able to 
automate most of our confidence. And I think actually many, many companies have 
no manual testers.
Like most smaller companies, bigger companies probably do have, have some manual 
tests. 

**Michaela:** [00:39:32] And is it like dedicated? Sorry. Is it dedicated 
testers? Because what I see is that. The testers out of developers, 

**Kent:** [00:39:37] right? So 

**Michaela:** [00:39:39] they're writing think the automated tests, but also 
whenever they deploy, they know, clicking through the website or program or 
whatnot.
So somehow the tester, especially in smaller companies is the developer. 

**Kent:** [00:39:51] Yeah. And frankly, it probably shouldn't be that way. 
Right. Because as a developer, you have all of these preconceived notions of 
what works and what doesn't and, and you can't. It's harder. I I've known manual 
testers, really brilliant manual testers.
And they ha have had this way of just thinking of different ways to use the 
software in a way that actually breaks things. And so I, as the developer, like 
never imagined things would be used in this way. So like, there's definitely a 
certain skillset that they have that I, that I don't have. But even when I was 
at PayPal, that was like, w we did have manual testers, but I did not know any 
of them.
They were not on my team. W they, I didn't. I honestly don't know how it all 
works. So sometimes I'd get a report from somebody I'd be like, Oh, okay. So 
most of the time it was just, okay, we write our manual, our automated tests. We 
run those in, in CI. And after a deploy, we're just like rapidly going through 
as many things as we can imagine, just to make sure that like, you know, do a 
sanity check or whatever.
So yeah, I see this trend as well of fewer manual testers and, and even fewer 
dedicated manual testers. And as your automated tests, confidence increases your 
need for manual testing, whether it be a dedicated manual tester or yourself is 
going to decrease. And so I think that as our, as the ease at which we right.
Automated tests increases. We'll see a reduction in the need for manual tests. 
And honestly, that's a good thing. There are so many problems with, with manual 
testing. There are lots of benefits, but, but so many problems and not the least 
of which is the, the amount of time and resources that it takes. Uh, a computer 
that can move at the speed of sight is as much cheaper.
Then having a, uh, human clicking around on, on the screen. And so I, I see a 
place for manual testers still and in the long-term future, also quite likely, 
or in the next decade, we'll still probably have manual testers, but I do see 
that the need being decreased and this could be, you know, all framed by my 
developer perspective as an automated tester, but that's.
That's my perspective. 

**Michaela:** [00:42:05] Yeah. I also think that the point that you raised 
about, you know, that we are, if you are developing your software, right? If you 
are the owner, the writer of that piece of functionality, you have a pretty 
clear idea how the things should work, how the concepts, you know, map together.
So using it in a very. Unintentional way is red or heart. Right. So you're 
probably destined for testing the happy path, but that's it, everything else, 
you know, is a little bit comes, doesn't come. So, so naturally. 

**Kent:** [00:42:36] Yeah. And all of the like unhappy paths or the sad paths 
you've already thought about. And so you coded for those, if so, they're, 
they're probably things outside of your vision that, that you hadn't really 
considered.
And so you don't have. Uh, code to handle those cases. And so like, you are not 
the one to discover those, because if, if you were then you would have coded to 
handle those cases. And so you really need somebody else to go through and 
consider somebody who doesn't already know about all of the educations that you 
had already thought about, because yeah, like you already coded for those, all 
of those edge cases.
So you going through it, it's probably not going to do any good. You need to 
have somebody else find things that you didn't think about. 

**Michaela:** [00:43:20] Yeah, true. I mean, what comes to my mind now is when 
we are coming back, it's not really accessibility and not really usability, but 
a little bit, right. If you're doing user studies where we have people that we 
are observing, right.
And I have done a couple of user studies where you have really people sit down 
and haven't seen your software before, or, you know, various degrees of 
experience with your software and you look at how are they looking at your. At 
the screen, where are you searching? You know, where are they struggling?
This is very manual work and it's not, it's not really testing per se, right? 
It's a little bit different. But on the other hand, it's testing, it's 
understanding your software and not probably that it breaks or that there are 
great regressions, but, you know, It's the concepts that we made and the ways, 
you know, you navigate the software and, you know, the, the, the features where 
they are, you know, we're in the menu and things like that is that actually 
understandable to people.
And this is very, this is a very manual work. Do you see some way how we could 
automate that? Or maybe there is some that, that you know of that I'm not aware 
of? 

**Kent:** [00:44:24] Uh, I don't think that that's really automateable per se, 
but this is where AB testing is like reigns as King. Like that's, that really is 
the only reasonable way to do this.
At scale at PayPal, we had user testing, you know, eye tracking software and all 
of that. Like. I, they, they showed us a couple of videos and we're like, all 
right. So what do we do? Can you tell us? So like, there are people who do this 
for, for their living, but, um, it really, it comes down to like, I think that 
it's reasonable to expect that people specialize in the user experience.
And so they, they have come up with a couple of ideas of things that they would 
insert into it. Like they would expect would be a reasonable. Interface, the 
developers go implement all of them or all like the ones that everybody votes on 
or whatever is good. Maybe they do some user testing before, but then you just 
throw it out there as ABCD testing to see which one is better.
We did a lot of this at PayPal and then. You know, you have these experiments 
and things with different feature flags and that sort of thing. And then you 
just pick the one that wins, that turns into the most, you know, that increases 
the metrics the most, or decreases the metrics that you don't want decrease the 
least.
And I can't really think of anything much better than that. So that really is 
kind of forcing your users to test for you, but like when that's the best that 
you can do, then that's what you do. 

**Michaela:** [00:45:54] Yeah. I have to say that. Probably the first thing that 
I partially disagree a little bit with, because I had done a lot of data 
analysis, a lot of working, a lot of mid metrics.
And so I always, so I did that user study is different studies in general about, 
you know, how, you know, how people even understand software or something like 
that. And I think that data can be extremely, extremely helpful. Right. So this 
can be a very powerful things, but also it makes it a little bit blinded.
Right. So if you're throwing it out and you have like, No, maybe you have four 
versions. You will only have those prohibitions and the metrics are coming from 
these four versions and whatever your, whatever you think the metrics mean, this 
is what they will mean to you. Right? So, but if you are sitting really with 
people.
So I, so whenever I did the study, I complimented every data analysis, every 
quantitative analysis that I did where we said, well, you know, what are, what 
are 40,000 engineers doing? Right. And we're looking at the commit data, for 
example, how they are working in your new. We see, for example, test smells 
right, and go down.
And then we correlate that, right. This is really quantitative stuff. I always 
complimented that with user analysis. Qualitative data. Right. But we go and we 
talk to some of those engineers and we actually go through the data for example, 
that that is out there or not even with the, with the results in hand, but just 
sitting with them and looking at, you know, what are some tests smells the day, 
for example, CE or you know, other stuff that we are looked at.
And very often this gives you such a rich. Information about things that you 
didn't think about, or also how you can interpret the metrics that you have. So 
sometimes the metrics tell you just a very one-sided view. And I think it's a 
little bit similar to what you said as a developer, right? There's a developer.
If you want to test, it's very hard because you cannot, you cannot. Remove 
everything that you have, everything that you know about the software system. 
And similar here you are your chest. You can just collect metrics about things 
that you thought of and versions that you created. But if you're actually 
sitting with the people, right, if you're asking the people, if they're going 
through this could really open up complete new ideas of how, how to make the 
software much better, or much more user friendly or what not.
Right. Or maybe a new, maybe even a new. And you business idea or something. So, 
yeah, I'm a big fan of still having this personal encounters and. Yeah. More, 
more direct data. 

**Kent:** [00:48:25] Yeah. I don't think that we disagree. I think that that 
element is very important. The problem is how well that scales to every feature 
that you, that you're implementing, because it does like you have to hire an 
entire person or maybe multiple people.
To, to spend their jobs doing that. If you want it to do that for every feature 
that you could AB test. And so at PayPal, we, we definitely did that. We would 
give them, you know, here's version one, here's version two, we'd have, you 
know, I think like a dozen people or so that I saw you some of the software that 
we were working on.
And it's easier to do that for new software, but if you are. Um, modifying 
software. We actually did that for, for some like modified features as well. But 
I think that if you have the time and resources to dedicate to that, uh, user, 
um, interaction and interviews, you really should. And probably if you don't 
have those resources, you should get them because I think it's, I agree with 
you.
It's very important. I think. And that's where like automating this type of 
process really falls over. And that's why I say like the, the best you can do as 
far as the automation point is to do this AP testing and see which one ends up 
working better. You make a very good point though. Like those, those metrics, it 
may be.
That's a, is working out better than B, but for reasons that you don't know, 
like you, you think that it's these, this slight difference or this logo or 
whatever, but you can't really be sure unless you talk with people about it and 
watch them use it. Yeah. 

**Michaela:** [00:49:57] True. And also it could be that you're discovering 
version C that's even much better than AOB.
Right. But yeah, you're also very, very right that it's it's we have to think 
about this scalability of things. Right. But I think especially like, I think 
that it has, or should have a place no matter how large or small or early or 
late your software is. Right. So as you said, you probably don't have to do it 
for every feature.
And then before you're not doing it, it's really good to have those AB tests 
without any other input. Right. In general. I think if you're starting your new 
software system, right, let's say you're very brand new startup founder or 
something. I think that the best you can do instead of, you know, going to the 
data, because this is really something, instead of just creating whatever you 
think you want to create.
Talk to your customers, what do they want? Right. And then also how you ask 
those questions. And I think here, you probably don't have to have another 
person. You have to educate yourself a little bit about how to ask these 
questions without you getting very biased answers. And, but, and then later on, 
if you have a larger corporation or a small company, I think.
Probably you don't do it for everything, but for every major release or major 
idea that you have start with the, with the customers that will the users ask 
them, you know, really one-on-one, what do you want is that, you know, how do 
you feel about that? And also just observe them how they are, how they are using 
yourself, I think is very important.

**Kent:** [00:51:27] Yeah. So like at the end of the day, that's where we're 
making this software for people. We better figure out how they feel about it. 

**Michaela:** [00:51:35] Yeah. So they actually talk quite a bit already. Do you 
have something on your mind that you think we haven't covered in this, in this 
episode? 

**Kent:** [00:51:43] I, um, no, I don't think so. I would encourage it.
Anybody who's doing UI testing to really give a hard look at testing library, 
even if your language of choice for you, UI is not a JavaScript, like you're not 
building a web application, maybe a native desktop application or something, the 
ideas behind testing library or what make testing libraries special.
And so I'd encourage anybody to take a look at that. And, and see how they could 
integrate those ideas into their stuff. The other thing that I'll just mention 
here is if somebody who does want to improve their testing skills and abilities, 
then testing, JavaScript is a really great resource. So testing, javascript.com 
and it has stuff for both the front end, as well as the backend, it's all 
JavaScript.
So you have node on the backend, but it's. Pretty JavaScript specific the tools 
and things are JavaScript, but there are a lot of concepts in there as well. So 
if folks aren't using JavaScript, they will still get a lot of value out of 
testing JavaScript too. So I'd just throw those last little plates in there.

**Michaela:** [00:52:44] I will link everything in the show notes. And, uh, I 
will also link probably all the tools that we talked about. Or did you mention 
also in the show notes? So thank you, Ken, for being on show for talking so much 
about testing with me and spending your time with me. 

**Kent:** [00:53:01] Yeah. Thank you so much for having me twice.
I really I'm honored. Thank you. 

**Michaela:** [00:53:07] Yeah, it was really fun. Thank you so much. Okay. 

**Kent:** [00:53:10] Bye-bye. 

**Michaela:** [00:53:11] Bye. I hope you enjoyed another episode after self 
engineering unlocked podcast. Don't forget to subscribe. And I talk to you again 
in two weeks. Bye.


