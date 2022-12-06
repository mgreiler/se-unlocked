---
episode: "Transcript Episode 68 Lauren Peate"
permalink: /engineering-metrics
status: publish
type: transcript
---

[00:00:00] **Michaela:** Hello, and welcome to the Software Engineering Unlocked 
Podcast. I'm your host, Dr. McKayla, and today I have the pleasure to talk to 
Lauren Peate, founder and CEO of Multitudes. They're building engineering metrics 
without the creepiness. 

But before I start, let me tell you about my latest 
project: [awesomecodereviews.com](https://www.awesomecodereviews.com/).

Yeah, all my work on code Reviews has now its own dedicated 
home. At [awesomecodereviews.com](https://www.awesomecodereviews.com/), 
you find articles about code review best 
practices, code review checklist, news about the latest research on code reviews, 
and of course workshops and courses I offer around this topic. So please hop 
over to [awesomecodereviews.com](https://www.awesomecodereviews.com/) 
and check out my latest work.

But now back to Lauren. Lauren reached it out to me after reading the paper of 
my recent study on developer experience and she said she wants to talk with me 
about high performing teams and people, a people first way to software metrics. 
Lauren worked with tech teams around the world from Silicon Valley to Middle 
East and now's New Zealand as all of those are really topics are dear to my heart. 
I'm super thrilled to have Lauren here with me to discuss. 
Lauren, welcome to the show. 

[00:01:08] **Lauren:** Thank you. It's great to be here. 

[00:01:11] **Michaela:** Yeah, I'm super, super excited. So let's go back to the 
slogan of S, right? It's engineering metrics that aren't creepy and you promise 
on the website that the team like that you get ethical team, you know, metrics 
like Dora space and so and so on.

So really to improve the team effectiveness. How, how do you do that? What are 
ethical metrics for. . 

[00:01:34] **Lauren:** Yeah. So I wanna say at first, we've recently revamped 
that website and we had a bit of a discussion around, Okay, are we ready? 
Because it's, we know it's a bold claim to say that we're ethical to say that 
we're not creepy.

Mm-hmm. . So we did have a team discussion around, okay, do we, first and 
foremost, do we feel like we've laid enough of the groundwork to be able to make 
that claim? Um, and, and we do, which is why we landed on it. And I'll tell you 
more in a second about the actions we're taking, but the second reason we put it 
on the website is because it's also an invitation to people to hold us 
accountable.

That's the bar that we wanna be building towards. And so, um, we, we, we want to 
have those conversations around how well we're doing that and where we could do 
that better. Um, but yeah, so, so, you know, what are ethical engineering 
metrics? I, there's a quote I really love from Laura Taco who's an engineering 
coach, where she talks about how engineering metrics, the key thing that either 
makes them creepy or empowering is where the locus of control is.

So is it metrics? people that teams really are using for themselves to reflect 
back things, to, to make their own decisions? Or is it, is it metrics that 
someone else is, is using to sweep in and tell people what to. And obviously 
much more empowering if it's something we can use for ourselves than something 
that someone else is using on us, or, you know, to tell us what to do.

Um, so that's the bigger goal with us at multitudes is let's put these metrics 
in the hands of the team. So building in transparency. Transparency is one of 
our key principles. . The second thing we think a lot about is what are the 
guardrails for what we will and won't measure? And so we have a series of, of 
data ethics principles that we've have also shared publicly in the interest of 
accountability.

Um, and we go through a review process with any new feature where we say, you 
know, let's test this. Let's get feedback from people in marginalized groups. 
Let's check the risk of harm. And out of all of that, one key thing that we've 
committed to is that we're not doing individual performance metrics. So we'll 
show metrics on the performance side around the team, but not around individual.

Um, and then the, the last thing that I'll say is we are, um, we've, we are also 
being really thoughtful about the people that we bring in, in right now where 
our product is still relatively young. We're in beta and so we're intentionally 
in a closed beta because we're bringing in a filter. We have afil a values 
filter for the companies we work with to make sure that they're going to use it 
with good intent.

Um, and that also they're the kinds of people that we want to have shaping the 
product in these early. 

[00:04:02] **Michaela:** So I want to come back to the first thing that you 
said, um, which was, while you, it's important who has access to the metrics? 
Who uses them or abuses them, right? So, um, and these are transparency, so I 
understand that, um, transparency means that the engineering teams know how they 
are measured or what is measured and, you know, what's, what goes into these 
metrics.

Um, There is nothing that holds actually somebody else, let's say, upper 
management from still abusing those metrics, right? Even though we have 
transparency, um, you know, we can still use that and do some ranking or, you 
know, something like that. 

[00:04:45] **Lauren:** Yeah, I hear that concern and you know, definitely 
something that we think about.

Um, so the first thing I would say is that's where, for us it's really 
important. What are the metrics that are so high risk? We just shouldn't even 
mention them. So there, there are no leaderboards on multitudes. There never 
will be. That's not, we know. Um, That stack ranking is, is, is a problem. Um, 
so, so that's one thing.

You know, something like that. That's why there's no individual performance 
metrics. So none of this, like how many lines of code did you write? How many 
prs did you do? Um, because all of those for us, you know, as you pointed out, 
even with the transparency, there's still just too much of a risk that someone 
could grab that and kind of use it in overly simplistic or reductive ways.

Um, so that's the first thing. There's just some things that we won't measure. 
It's not worth it. There's not enough value to, to compensate for the risk. The 
second thing is we have realized that we need to be really opinionated product. 
So we're not going to be, um, we've occasionally gotten requests of, Hey, can 
you just give me a CSV download and I'll play with the, the, the underlying data 
that you've, you know, aggregated and compiled.

And, um, and that's not something we're gonna do because we have opinions about 
what you do with these metrics. And one of our really strong opinions is that, 
especially because it's data about people, The metrics are the starting point 
for a conversation. They're not the answer, and that's because, say this quite 
often, even if we had every single integration in the world, even if we plugged 
into every single piece of tooling that someone is using, because people are 
complicated because we do things offline, it still wouldn't be the full answer.

We would still always need to weave in that human. And so there's things that we 
built in to the product to, to tell people, Hey, what's the human context here? 
And one example I can give you is we have these dynamic one-on-one guides where 
we raise some of the metrics that you might wanna talk about in a one-on-one.

So for example, if someone's been blocked for a while waiting for a review, um, 
or if it often happens that they're blocked and waiting for a review. But we 
pair that with questions to ask the person. So it's an acknowledgement that 
there might be, the data might say, Hey, there's something different or 
interesting here.

but we still have to talk to the, the people that the data is about because 
they'll know more about why this happened. 

[00:06:55] **Michaela:** Yeah, I really like this approach and um, it reminds me 
quite a bit, uh, on the time that I worked at Microsoft and, you know, there was 
always this request give us, you know, some data about people.

And um, also in our team we always said like, Team metrics is the only thing 
that we are actually assessing somehow. Right. But also, um, I never really, I, 
I was never really into dashboards, especially not about people. Right. Or , you 
know, some, some highlighting of some, you know, Merged and summarized and 
aggregated and, you know, changed and, and so on data.

Um, I always saw it as an investigation, right? A little bit more from a 
researcher perspective. So you look at data and I think data is so powerful, 
right? So it's, it's, it's a shame if we say we don't touch it because it's so 
risky, so we should touch it somehow. But it's very risky, right? So how do you 
touch it?

Um, and I like this idea of. Of really asking questions. So when we, uh, went 
out to have some investigations, right, and we had aggregated data, let's say 
about code reviews, for example. Um, and then you see, you know, spikes or you 
know, something, uh, going on, most of the time it's not what you think, right? 
So you think, like, for example, you.

Comparing, Right? With data, you like to compare , so you want to know something 
higher, something lower, something faster, something slower, right? Something 
like this. Um, and then you see, oh, you know, there's so many things going on 
in this project, but you know, in this project there's a different cadence or 
something, so what's going on?

And if you ask a questions, most of the time it's not as simple as you think, 
like, Oh, they are slower, or, you know, they're very often there's the context 
that really. Very, um, understandable uh, reasons or gives you reasons why 
something is happening. Right. Um, so can you give me some more examples of, you 
know, where you have this context or where you are asking for this context 
without, you know, jumping to conclusions with, with the metrics that you are.

[00:08:54] **Lauren:** Gery. Yeah. Yeah. Um, well, I'll say, So a couple things 
too. One of the other things we've been thinking about around that, and 
especially on this note of the, there's not gonna be like a one size fits all. 
This is good for everybody. And so something that we're, um, doing some really 
early prototyping experimentation with, uh, at the moment is around this 
understanding that, um, what good looks like might be different for different 
teams.

And also, um, one of the things just on your point that you'd said at the 
beginning around. Sure. Graphs are interesting, but, but no one's saying, Oh, 
I'm so excited to look at a bunch of graphs today. You know, that's not, that's 
not the why. The why is at the end of the day, we want teams, where people are 
valued, where they're thriving, where they're learning, and then ultimately 
where we're, we're building great things together.

And, and so one of the things we're playing with is around teams, supporting 
teams to set their own goals and then helping them track their progress towards 
it. So a very one. Having it be, again, it's a team conversation. Here's some 
data points, and then, you know, what does good look like for us? What, what's 
our collective agreement around where we wanna get to, and then how can we use a 
tool support people to, to kind of track that and, and get there along the way.

And so that involves things like having check-ins, um, where we ask people. So 
as part of the goal, you say, Hey, this is something we're gonna try to get us 
closer. And maybe the metrics didn't shift because we were too busy to try the 
thing that we were going to, you know, or, or maybe it didn't shift cuz we did 
try the thing and, and it didn't work.

Or maybe we had troubles, um, trouble implementing it. And so those are some 
things where, um, , as we build up this feature, we're, we're proactively asking 
people to share that back with us and then weaving that in alongside the graph 
so people can kind of have that context next to the trends. 

[00:10:38] **Michaela:** Yeah. So one question that I have for you as well is, 
um, I think metrics are always extremely stereotypical, right?

So the measure. The norm, they measure, you know, um, what a software engineer 
or developer does. As we, you know, as we imagine this typical stereotypical 
software developer that goes into work, you know, and codes something, gets 
some, you know, features and then codes down these features and goes home, 
right?

Um, but in my experience, Maybe there are like, I don't know. Um, you know, I 
don't know really the, the, the curve of, you know, how many people fall into 
that bucket of stereotypical, let's say, developer. Um, but I know from my own 
experience, I have never ever been this stereotypical developer, right? So I 
worked at Microsoft and sometimes I had the research title, which is easier 
then, but sometimes I had a developer title, and so I was a software developer, 
even though I, I was not doing this typical, Feature work, right?

I developed features, for example, for an, you know, code flow, which was the 
code review tool. Um, but it was not my main, um, my main. Task. Right. My main 
responsibility, my responsibility was really to make studies to see, you know, 
data, what, what's going on with teams, with code reviews, to talk with teams. 
And all of that could not be measured.

So if you go ahead and say, Well, you know, how many check-ins does a developer 
do? Or, you know, when is the first check-in? You know, you onboard, Oh, sorry, 
you onboard that, that person and you should have a check in within the first 
week. All of that wasn't really. I never fitted to, you know, my, my, my role, 
even though the title said something.

So how are you coping with that at, you know, at at multitudes and, and how many 
people actually fit into this? I think very narrow scope of what a person 
typically does. 

[00:12:31] **Lauren:** Yeah. Yeah, we see that. It's interesting. So we're, we 
use the tool ourselves and we dog food it. And uh, we see that cuz we have quite 
a few data scientists on our team.

And so, and sure they're writing code, but similarly, their, their processes, if 
they're doing an exploratory data analysis, that whole workflow looks very 
different from someone who's got their, their thin slices of a new feature. You 
know, turning out prs. Um, so yeah, we definitely see that, that coming through.

Um, couple of things that we think about around that. So one that's where, 
again, that, that team focus around what matters for us as a team. What are the 
goals that we wanna get to, just to, you know, that being a really key thing. 
Um, and. If I just go back to that example I just shared, of course, you know, 
when we look at it, when we have the context, we know we shouldn't be comparing 
one of our, a classic dev team with a, a data science team because the work is 
quite different.

Um, of course those metrics should look different. Um, so that's, um, you know, 
again, kind of this team view and instead thinking about one, what matters to 
us. There's one of the things, and you know, we're just a small part of this. It 
really feeds into this bigger conversation of the team norms and what does a, an 
effective team look like for us?

And then, and then what are the, the metrics that help us support that. And so 
for um, engineering teams, it's often things like, cool, you know, we do wanna 
be having smaller batches of work. We wanna be moving a along better. But for a 
data science teams, it might be more. Hey, we wanna make sure that we're getting 
really good collaboration on the different pieces of work because it's so early, 
it's so exploratory.

We know we need a lot of different eyes on it. And so that, in practice might 
mean that there's different measures that you would look at. You know, maybe for 
one, you're thinking more about, uh, a lead time or another, You're looking more 
at the, the breadth of reviewers that you're getting on each of your poll 
requests.

So, I guess, you know, similar to, as you pointed out, because of the diversity 
there, I'll go back to this point of it really is about what are the 
conversations that we're kicking off and then, and then teams kind of deciding 
for themselves, which are the metrics that matter most, um, for the goals that 
we're trying to achieve as a team.

[00:14:38] **Michaela:** Yeah. And then also when we come back to data , we only 
can measure what's somehow happening in the software systems, right? In the 
engineering systems, Everything that happens outside. And I would claim that's 
quite a bit, right? That that's a lot of work happening outside of those system 
that we can trace and track and analyze and so on.

What happens to. Work. Um, often it's glue work, but not only, right? It's not 
only glue work, it's somebody standing on a whiteboard talking to a colleague 
and you know, they're catching out something. It's something that happens at the 
coffee machine where we are talking, or maybe it's happening over zoom, right?

Because we are remote and and so on, but, uh, we are not tracking Zoom and so 
on. So, so what, what happens to all those conversations and how do they fit in? 
Is it, is it enough that we just look at, you know, what the engineering system 
tells us or. Do we sometimes, sometimes get blindsided by that? And how can we.

Overcome those, uh, problems here. 

[00:15:34] **Lauren:** Yeah. So this is one where both the, remembering that the 
data's a starting point for a conversation, but then also thinking about the 
diversity of data that can be helpful to paint a more full picture. So something 
we think about a lot is, So we're really interested in what's the employee 
experience, and of course there's a, there's a whole diverse set of data we can 
use there, but the an analogy we like to look at is what's the different types 
of data that we weave into our product development processes.

And so if we look at that, we know we've got the very in depth one-to-one user 
research, really high touch. We're talking to people, we can go, we can get lots 
of. Depth, we can understand the why, but also the the end, the volume is gonna 
be more limited cause it's so time consuming, right? So we've got that.

Mm-hmm. , we've got our surveys and we can do our nps or other types of 
satisfaction surveys and people can tell us, Hey, I liked it. I didn't like 
this. And then we have the all of our digital analytics of, okay, where did they 
drop off? Where did they rage click? What was frustrating people? And then we, 
we use that to kind of piece it together and then give us some clues about what 
we might wanna do next.

And so we see ourselves fitting in to the suite of that and employee experience. 
And if you look at it, we've got, we've got our one-to-ones great leaders are 
always doing one-to-ones and, you know, lots of reasons why. So that's the 
in-depth stuff, but, but smaller volume. , we've got our engagement surveys and 
you know, I know, um, you're involved with dx, The, the developer experience 
surveys so useful cuz then people are telling us how they feel about something.

We, we don't know that unless we ask them. So that's really important. Mm-hmm. 
and then, and then rounding it out with some of the behavioral data, which. Is 
also coming in the background. And some of, you know, we're looking at a range 
of things like who might be at risk of burnout cause they're working long hours 
or who's getting less feedback and support on their work or that question of 
where the work's getting blocked.

And so it's, it's what's the, the diverse set of data sources that collectively 
give us different pieces of the picture and then, Always, always bringing in the 
humility of, even with all these different data sources, people are complicated. 
They change, they do things offline. And so always remembering that it's a 
hypothesis and then we have to talk to people, to, to, to really test it.

[00:17:45] **Michaela:** And how do you transfer this, um, humility to humility 
to somebody else, right? Because you as a team can have it and you can build it 
somehow in your product, but then on the other hand, it's out of your hands, 
right? So you have the data. How do. How do you remind people, educate people, 
teach people to have that humility and also to, to know that those metrics are 
not the, the ground truth, Right?

So how do you remind them of that? 

[00:18:13] **Lauren:** Yeah. Yeah. So another thing that, that really matters to 
us, so I'll, I'll run through kind of the suite of ways that we think about it. 
One is having those questions alongside the data. So the nudge, Hey, this is 
part of the picture. We even in. In those, those one on one guys I was 
mentioning visually it's the graph takes up half of kind of the, the space, But 
the question and the space for both people, so the engineer and their team 
member, um, and their manager to share their thoughts is the other half.

So even visually, we're trying to say, look like this is, it's. It's equal in 
terms of the importance of these two things. So weaving in, um, those questions, 
the, then those kinds of nudges to add in the context, um, that's one of them. 
Um, the other thing that we're doing is, um, in the near term, You know, I 
mentioned we have this closed beta, and so we are only bringing in people where 
there's, we, it's more confident.

And then one of the things that we're testing along the way, there's always, you 
know, as you point out kind of, Hey, we think people are gonna use it this way, 
and then they use it in different ways in, in the real world. And so what that 
means is we have a trusted group of early folks who we can start to see what it, 
how they use it in the real.

Um, and we actually have had features, We had one in particular, I can think of 
where we got it was, it was pretty much done and we started to put it in the 
hands of people and then we were like, Nope, you know, we're not in, in US 
looking at the actual usage data. So our own digital analytics on our app, yeah.

It, it wasn't being used in the ways that we thought it was. Um, so we've, we 
actually have had one in particular that, um, got all the way out and then, and 
then we pulled it back. And so there's kind of those checks even at the very. 
And then the last thing I'll say is on that accountability side, we're actively, 
we actively seek out academics and activists and people who are really close to 
how our system is causing harm.

Um, especially one of the things we think about a lot, we know that people from 
marginalized groups have even like more examples of, of how data has been used 
in harmful ways against them. And so, Actively showing our product to those 
people. We had a call earlier this week where we said, Hey, tell us, tell us the 
risks.

Like let's talk through it. Um, and so yeah, wanting to make sure that, that 
we're getting those other eyes, cuz of course we can have our own, uh, kind of 
assumptions and, and we wanna make sure that we're testing those. . Yeah. 

[00:20:35] **Michaela:** Yeah. Um, I, I got a question yesterday on, on Twitter 
about mob programming, assemble programming, right?

Where you program as a group, a peer programming, but really people are nowadays 
focus very much on this mob and assemble programming and, um, if I think it's, 
it's, it's better or same as code reviews and how they compare and so on. And I 
know that some people really love mock programming, assemble programming, right.

Um, But I, on the other hand, just thinking about my life situation, work 
situation, right? Um, my personality about many things, I get so many anxieties, 
I, I feel already drained if I think about it, right? Um, and, and, and I 
wonder, for example, what that means, right? And I, I don't know. I mean, I'm 
just one data point.

So I don't know. I would love, maybe I should reach out and ask a little bit 
like female, uh, male, right? Or woman and men. You know, um, life situations. 
Do you have kids or not kids, but what, what it means for me? There are a couple 
of things, right? First of all, it means that there's another person at least.

Maybe a whole group of people that are, you know, very close to me, you know, 
that I have to interact for a long time. Um, which I know I, I like it, like to 
check in like an hour. It gives me so much energy, right? And doing some peer 
programming sessions is something that really energizes me and, and I feel like 
yes, that's great.

So if, if there is some possibility to. I'm very much a fan of it. But then 
also, let's say I'm working one and a half hours with a person. I'm so happy 
that I can switch off and be by myself, you know, and do my own thing and my own 
thinking. And there's another, you know, not another person that, that pokes me 
or that I have to somehow behave or, you know, so many things.

Um, and then if I think that I have to do that the whole day long, or even just 
for a couple of hours, I feel extremely overwhelmed. Right. So this is just. 
Personal, what gives me energy, what takes energy, Um, thing, right? It was the 
same when I had to go to the office, all these people around did the noise, 
right?

This was too much for me, and I'm so much better, so much more productive if 
I'm, you know, this is personal at home, you know, and, and, and I'm checking in 
at certain times and I love to go to the office, but just for a couple of hours. 
The best is like going two hours to the office, you know, checking in, talking 
with people, then going home, working at home on my own.

Um, and then the, the, the second thing, which is a little bit of a different 
area, but comes back to, um, your life situation, right? Uh, assemble or mock 
programming means that we have to work synchronously, right? So I have to have 
time when you have time. Um, and this makes it extremely difficult, I think, 
for, for a lot of people, right?

Be it that you bring your kids to school in the morning, or you're looking for 
some elderlys, right? Um, I have very weird schedules since I have now three 
kids. Right. Um, but I have very weird schedules. I work on the weekends. I work 
sometimes in the nights. I work very early on. Right. So thinking about how I 
could fit that to another person's schedule, I dunno.

So what do you think about this and, and how does that, you know, come back to 
the intra engineering metrics that we see that we measure? Right. Especially 
synchronous, as synchronous work styles. I think. Show very different in, in the 
metrics. They can, you know, set up our, you know, metric system a little bit.

Like, do you think, wow, something, some outliers here, right? Mikayla, what is 
she doing on the weekend here? Maybe she's burned out or, or she's not checking 
in something at three, 3:00 PM like maybe should put down a pip or something, 
you know? So what are your thoughts about this ? 

[00:24:18] **Lauren:** Yeah. Yeah. We're seeing, um, as you were talking, I was 
just thinking of kind of the range that we're seeing across all the companies 
we're working with.

And, and it is, it's, it's a pretty broad range and we see some teams where they 
love mobbing, um, you know, ensemble programming or pairing. Um, I would say, 
excuse me, We've especially seen some, It be really helpful. As part of the 
onboarding process one. So, um, we quite a few of our companies, maybe their 
normal isn't to do pairing, but when they have a new team member, then they say, 
Yep, sweet, you know, this, this is how we're gonna get you up to speed, is 
you're gonna pair with someone who's been around for a while and then, you know, 
you're kind of getting a, a bit of a guide to figure out your way through the 
code base and all that.

Um, so that's one we've seen quite a bit. Another place where we've seen it be 
really helpful is, um, sometimes when a team is, maybe they're trying to do a 
bit of a reset about how they do collaboration. And we've seen this sometimes 
happen as a company is scaling. Maybe in the earlier stages people were working 
more independently.

It was very just like, ugh. You know, the, the, the product was small enough 
that the code base was small enough that you could just say like, You do this, 
you do that. We kind of have our. And then maybe as they're growing, there's no 
one has, you know, can really know all the things anymore. You need to kind of 
be getting more of those, um, sort of that feedback from other people about kind 
of how it might impact other, other parts of your product.

And so, We've also seen that pairing be really helpful for kind of the, the, the 
like cultural shifts at those times when you're trying to say, Look, we wanna 
just do a bit of a reset to say we're gonna, we're gonna be doing lots of 
feedback and so to kick it off, here's a moment, you know, here's a period where 
we're doing a ton of feedback.

Um, so there's a, a couple specific examples where it's been, we've seen it be 
especially helpful. But yeah, we're definitely seeing a whole range. And then 
shifting to your question around, well what does this mean for the metrics? It's 
something. We've been mulling over because we know there is this rise in pairing 
and mopping, and we really love the, the benefits that it can have for knowledge 
sharing.

Um, it, it's not within GitHub today, there's not easy ways to see that. So to 
be really honest, it might just end up us being at some time doing a feature 
request to them to say, Hey. Pairing and mobbing is a thing. Can, can you have a 
way of acknowledging that? Um, but in the near term, one of the things that we 
do have is issue tracking data.

And so there it can be a little bit easier, at least to see if a couple people 
are picking up a ticket. Um, so that's one way to see it. And then another thing 
that we're thinking about, and, and I will say this is something that is, um, 
it's, it's, it's still an area we're molding over and is more future focused for 
us.

But it could even just be a little context note that people add, you know, as 
we're thinking about what's the context on these pieces of work. Um, It could be 
that, you know, maybe two people were, were pairing and it was consistently one 
person who was the main PR author. Maybe, you know, maybe it's that new team 
member, the more experienced team member and they had the new team member kind 
of take the lead.

Um, the, we're thinking about, okay, well maybe that's just another context note 
that we include on the data to say, Sure, it looks like this person dropped off 
in their work. But actually it's cuz they were working closely with this other 
person. 

[00:27:27] **Michaela:** Yeah, so when you tell me all of that and um, I getting 
a little bit, a better picture of the metrics, but maybe in the next question we 
really deep, deep dive a little bit what the metrics are.

But what you're also telling me is that it seems like a lot of work to work with 
this system, right? So you have your data. I think a lot of people that go for 
metrics, they want. I click a button and then there is the answer, right? So for 
me, this seems very involved. I have to be very intimidated, uh, uh, intimate 
with the, with the system, right?

I have to be very close with the system. I have to look at the data, I have to 
make those nodes right, which, uh, for me seems a little bit like, uh, leaving 
comments in code . Are people doing it? And how much work is it to leave those 
notes and say, you know, Oh, actually a system, you know, you don't know. So I 
know, and I'm really extracting my knowledge and put it in the system, write it 
down.

[00:28:20] **Lauren:** Yeah, I'm glad you raised that. So, a couple of things. 
Um, one, because we're pulling in passive data, once the integrations are set 
up, it's no work to get the insights like they were surfacing it and, and 
saying, Hey, you know, here's the things that are popping up that are 
interesting. And in practice those types of context notes.

Um, you know, one, our, our first goal is how do we help? Where people should be 
spending their time. So it it, our goal is it's not, Hi, here's 20 graphs, and 
you have to look at all of them. Um, we're, we're always working on how can we 
do a better job of servicing the things that we think are going to be the most 
interesting for you to focus on right now?

So that, so that's one. What's the stuff that. It's, there's been the biggest 
change. Maybe if you've set a goal, it's further from your goal. And then the 
second is on those areas where it's a question or there's context pieces that, 
that really just pops up for the critical things. Um, so, you know, a lot of the 
time especially, Our tool, we're first and foremost thinking about a team using 
it for themselves.

So they, a lot of times they have that context. There'll be a, a, you know, a 
manager, a team member will look at it and they'll already know like, Yep, cool, 
these two people working on this piece of work. Um, And so those contact notes, 
it's really more for teams that are thinking about, uh, how someone else who's 
not on the team, you know, if there's like a senior person, they're, they're 
gonna be having conversation with, that's where the context notes starts to 
become more important.

Um, but yeah, in the day to day, to be honest, it's, um, you know, we're, we're, 
it's, it doesn't require the effort, but for the teams, It for us, what's 
important is the teams that are worried. If, if there is a team that's like, 
Hey, we want to make sure that this data isn't used against us. The context is 
really the answer for the teams that are in really high trust organizations, and 
there's less of that worry, the context.

People can kind of trust that, you know, no one's gonna make a reductive 
decision off of these metrics. And so, um, there's less of a need to, to put 
that time and effort into all the. 

[00:30:21] **Michaela:** Okay. Yeah. Um, so we talked about the metrics. I want 
to know what are the key metrics and then what are the metrics that most people 
use?

Right. You, you also said that you have analytics inside, and I think especially 
as a startup, right, , trying to figure out where to go, Um, you probably have a 
lot of knowledge about how do you use your systems, what do people really like, 
which features do they not use so much? So probably also, which metrics are, you 
know, maybe in.

Thought, uh, the most important ones. And then does this deviate a little bit 
from what you see actually that people use or, you know, how is the usage of 
this matrix? Yeah. 

[00:30:59] **Lauren:** Yeah. So the, the top buckets that we have is one around 
how the work is flowing and where it's getting blocked. And with that we've 
really leaned on the door research because you don't need to reinvent the wheel 
there.

Um, and then the, the counter to that. So that's more of the process side, as we 
like to call it. And then on the people side, we've got metrics. Wellbeing. So 
indicators of who might be at risk of burnout and also around the support that 
people are giving and also receiving on their work. Um, so that's high level and 
I'll dive into the, the deeper part of it in a second.

Um, one thing I will say though is, so Dora of course, has been around for a 
while, and then the, the space research that came out, it was lovely because 
what we've been doing in the background is we are on the process metric side. 
We'd. Really leaning on the door research. And then on the people metric side, 
we've been leaning on a few different research sources.

And so what was so lovely is now there's actually one paper that has that, that 
broader picture that we can point to. And of course, you know, we're still, 
we're still leaning on the other research as well. Um, but, but we really love 
that as an encapsulation of this holistic picture that we're trying to show of 
not only.

We doing in terms of getting the work done, but how are we doing in terms of how 
we treat each other? So I'll 

[00:32:11] **Michaela:** give a couple, maybe, maybe we can, Sorry, maybe we can 
tell my listeners a little bit what them do. Metrics are, because I'm not sure 
they know it. Right. But I think just to, to highlight for them what it means, 
right?

It's lead time, right? This means also how long does it take something to reach 
the code base, right? It's time to failure, right? Or um, uh, to recovery, 
right? How, if you have an era, How fast you come, come back. Um, what else is 
there in normal? Yeah. 

[00:32:35] **Lauren:** Yeah. Lovely. We like to think about them as, um, two of 
them are a little bit more on the kind of speed or quantity side, and the other 
two are a little bit more on the quality side.

Mm-hmm. . So the, exactly as you were saying, we've got lead time. That's, um, 
thinking about from when we start doing the coding until we get it in the hands 
of customers, how long did it take? So, mm-hmm. , Um, in practice it's usually 
first commit. To, to like how long it takes from there to time to getting in 
production.

Um, so that's lead time. Then deployment frequency, so that's how often we're 
getting something in the hands of our customers. So you can see both of those 
are really on. What's it gonna take for us to get that value in the hands of the 
end user? Who's gonna really benefit from it? Um, and then more on the quality 
side, the two metrics there are change failure rate.

Mm-hmm. . So how often when we release a change does it end up failing? Mm-hmm. 
. And then the second, as, as you mentioned, is meantime to restore. So exactly. 
When it fails, then how long does it take us to get that system going again? 
Yeah. So yes, really lovely, um, set of metrics. What we loved about it and um, 
people see this in the research is it's, they're metrics that are linked with 
the financial performance of companies, but also with the psychological safety 
of teams.

And so it's this real nod to what we know from other research about how an 
effective team is one where there's trust and that psychological safety between 
team members. Um, yeah. So yeah, so that's on the cool, the process side. And I 
would say that out of those, One of the ones that people are looking at the most 
often is lead time.

And then we have a few different things we built in to let people to start to 
dive deeper and diagnose where might it be getting blocked? What might the 
blockers be? You know, where can we start to shift things? Um, so that's the 
biggest one on that side. And then on the more people metric side, we look at a 
couple things.

So one is how often people are working outside of the hours they want to be 
working. So that's an important phrasing. Yeah, . 

[00:34:28] **Michaela:** That's so 

[00:34:29] **Lauren:** interesting. But it, this one is one we've, we've been 
doing some tweaking around and, and there's, there's more, a lot more we wanna 
do with this one in the future, I will say too.

Um, but because people work so flexibly, you know, this, where you see so many 
people who are doing the, I do some work and then, um, I took the dog for a walk 
and then I did some more work, and then the kids got, School and we did dinner 
and bedtime routines, and then I did some more work and you know, and these like 
interesting patterns.

There's a great piece of, there's a great article recently that said we've gone 
from bimodal days, so sort of work in the morning, lunch, work in the afternoon 
done to try modal days because now you're juggling in all sorts, even more life 
things. Yeah. So yes, we're, we're absolutely seeing that. And so at the moment 
we say, Hey, you know, tell us kind of like what, what are the concerning 
patterns for you?

And then, and then that's what we'll highlight. One of the things that we'll be 
weaving in even more as we go is that learning of, well, what is your normal, 
you know, maybe you think your normal is one thing, but actually in practice 
your normal is something else. Mm-hmm. . Um, so, so that's, that's on the 
roadmap for that wellbeing metric of actually reflecting back to.

These are the patterns and then, um, you know, one that might be an insight for 
you, but then two, just flagging the work that happens outside of whatever your 
normal is. So that's the wellbeing side. . And then on the, the collaboration 
side. So looking at who's giving lots of reviews on other people's work.

This is an example of something we really care about, which is glue work. So the 
work that, um, many people are often familiar with this, but just in case glue 
work is the work where it's not necessarily the, like, I built this, Hey, I 
achieved this outcome all on my own. Glue works, the work that makes everyone's 
collective effort better.

And so it might be the reviews, it might be coaching and mentoring others. Um, 
it might be doing documentation, might be facilitating meetings and making sure 
people are clear on follow ups. So, you know, there's a whole mix of, of kind of 
human and and technical things that fall in that bucket. Um, And we know that 
people from marginalized groups are both more expected to do that glue work and 
less appreciated when they do do it.

Um, and the other thing is that leadership is essentially glue work. I mean, you 
know, as a leader, people, you have less and less time to actually go do the 
building yourself, and, and your job starts to become more and more, how am I 
amplifying others to do their own building? Um, so for a bunch of reasons, for 
fairness reasons, and also because it's important, um, we're.

Really thinking about and, and you know, already had these indicators around 
who's doing the reviews. Let's go celebrate those people who are contributing a 
lot to the team in that. So that's one. The other one we look at is who's, um, 
the feedback received and in particular who's getting much less feedback.

And so, you know, we know that, um, getting less feedback, it can mean that 
we're not getting the codes, has high quality of a position. We might not be 
catching things. It might also impact that person's own learning a development 
if they're not getting the same feedback opportunities from their peers. So 
that's another thing.

We wanna make sure it's really fair and that, that that feedback is going across 
the team. . And then the last thing, and this is one of our favorite pieces of 
analyses, is then showing the patterns of feedback both, um, between teams. So 
is there a team that's a silo and is often working on their own? Is that 
expected?

Maybe it's expected, but maybe it's not. And then within a team, what are the 
patterns of who's supporting whom? Um, we were just having a conversation with 
someone today around how they've noticed that there's a couple people who are 
kind of almost becoming their own sub-team, and so they wanna have more of a 
spread of interactions across the team cuz they, they wanna make sure there's 
that, that knowledge sharing across everyone, not kind of embedded within a 
couple people.

So anyway, those are all types of trends that, that we see people looking at. 
And on the people side, it really. Um, the metrics around how, the patterns of 
how we're giving and getting support that, uh, we see people looking at the most 
often there. 

[00:38:21] **Michaela:** Yeah. So for the process, uh, metrics which are 
following Dora, Right.

I totally understand the team aspect, Right. But for the personal or for the. 
For the human side, it seems that even though you said you are looking at the 
team and only at the team, it seems that those are all individual metrics, 
right? So it's all a metric about you and how you do, and how you, you know, 
what are your work hours, how much.

Feedback do you give and receive? So it's not really a team metric anymore. 
Right. 

[00:38:49] **Lauren:** Let me, Yeah, so, so that's a clear, um, a good 
clarification, which is we don't show any individual performance metrics. So 
anything on the process side that starts to look at, like the work that I did 
mm-hmm. more activity Output.

Yeah, exactly. Like, so we don't, we don't do, if it's like PRS lines of code, 
that type of. We don't do it at the individual level, the people metrics, 
because they're much more around who are we going to support, who's overloaded? 
Those ones we do show at both a team and an individual level. Okay. And so the 
types of insights at a team level might be, um, you know, I mentioned that one 
where we're looking at the patterns of interactions across teams.

We might see that a team is, is siloed and isn't having lots of interactions 
with other teams. And so that might be something. And again, could be expected, 
but, but could be not. Maybe we, um, have shifted the type of work they're doing 
and we actually expect them to be collaborating more closely with another team.

Yeah. So, so we've got those team level metrics and then we also, as you noted, 
have it at the individual level. And that's very often, you know, one lets us 
celebrate. So that glue work example, we wanna celebrate the people who were 
putting in what is often very unseen effort to lift up others on the team that.

One of our goals is to really highlight that. Um, and then we also wanna 
highlight if someone's not getting the same growth and development 
opportunities, cuz they're not getting as much feedback as others. So 

[00:40:11] **Michaela:** what are the signals that you're using? Because, okay, 
one is code reviews, right? So who participates on code reviews, Who reviews, 
who gets feedback, How much and so on.

So I understand that. But what are some of the things that you can measure to 
measure the glue book, right? So if somebody sets up a meeting or, you know, 
make sure that everybody is on time, sends around an email for that. Um, do you 
have like your, your, uh, you know, your probes everywhere in my email system?

Do you have it in my Zoom or in my teams or, you know, what kind of monitoring 
is going on here that we get this data? Um, and, and yeah. So, so what can I 
expect? 

[00:40:50] **Lauren:** Yeah, Yeah, so we're an early stage product, so at the 
moment we've got both GI analytics and then also issue tracking data. Um, we 
have a Slack app, but that's more for the kind of alerts and nudges going out on 
the behavioral side.

Um, although we will flip it and do a Slack integration as well. Um, So, so 
that's kind of what we've got on that side and on the glue work. Some of the 
other integrations that we will be adding on that are in the roadmap are around 
who's updating the, our documentation. So our wiki , who's making sure that 
that's all up to date.

Um, that is another one that we're really interested in. Something else as we 
weave in that Slack integration will be things like, Who's kind of doing the, 
the roundups, you know, chasing up people on, like how things are going and, and 
updating people there. Um, so there's a few that are coming in the near term 
around that, um, as we, as we kind of add our, our extra integrations.

[00:41:44] **Michaela:** Yeah. Really, really cool. So, um, when you reached 
out, you said to me, we should make sure we are not focusing on the 10 x 
engineer, but the 10 X team. I'm obviously very curious. What is a 10, 10 x 
team? Right? What are, what are some signs of a 10 X team? When is it a 10 x? 
Yeah, I love 

[00:42:08] **Lauren:** this. So for me, there's two key things that need to be 
in place for a team to be 10 x.

And actually, let me just back up. So many people are, might be familiar with 
this trope of the 10 X developer. It came out of, there was some research, um, 
it was in the like late seventies, early eighties, where they'd done some 
measures of different developers and found that, oh, some developers, and mind 
you, this was.

Even their metrics were, were reductive themselves. So they were looking at, um, 
I think it was along the lines of things like lines of code and, yeah. Anyway, 
so they were saying, Cool. Yep. Some developers, they just do 10 x the, the 
output work from other developers. And so it's, it's quite an old trope. Um, 
Some of it is, is a little bit outdated.

And, um, so the 10 x team one, the first thing I'll say is we know, for example, 
from the door research that the teams that are doing the best on some of those 
metrics, not only are they 10 xing, the teams that do the worst, they're, some 
of the stats are pretty absurd. So need time and meantime to res. Door.

The best teams are send 6,000 times better, both of those and faster than the 
ones that are, are doing the, the worst on them. Um, so, you know, I've, I've, 
we've gone with 10 X team because feels very achievable. But in fact, some of 
the, the. Research shows that it can go way beyond that, which is great. Um, but 
yes, how do we get to be a 10 x team?

So for me, there's two key hallmarks. One is we have high expectations, and then 
the second is that we have high support to help people meet those expectations. 
And so, as you might imagine, a lot of this is the really human work. Um, on the 
expectation side, a lot of that is around the clarity. So things like growth 
frameworks are.

Wonderful for helping set the expectations of what does development look, look 
like in this organization. Um, that's also where. Us practicing our skills of 
giving really kind, but, but clear and candid feedback is helpful too. Um, so 
yeah, that's the, you know, the expectation side and, and also the expectations.

There's kind of expectations for individuals, but it's still expectations for us 
as a team or for us as a company. And so what really does success look like, um, 
across those? And we've got tools like OKRs, um, or, you know, at a company 
level, thinking about what's the bigger vision of what we're. So that's that 
side.

And then the support side, it's, it's knowing, it's really an acknowledgement 
that, um, we can't go after big things unless we know that, that there's gonna 
be people who are gonna back us up. Because when you go after big things and you 
do big challenges, sometimes it's gonna fail, It's not gonna work. And um, so 
the support side is everything from.

Creating an environment that's inclusive and equitable. Um, for us at 
multitudes, we've shared we're trying to do a good job of kind of sharing our 
work in practice. So we shared a few, a few blog posts about what that's looked 
like. But one of the examples for us is having regular training on topics around 
equity and inclusion.

So, uh, like colonization and, and the history of it and you know, how it's 
impacting us today. Um, sometimes some, some topics that are, are pretty big 
topics. Um, we're talking. White supremacy at work. And you know, and again, I, 
these are big topics, but, but we would rather talk about it. And, um, we think 
it's important to face these things to, to make sure we're, we are creating an 
equitable environment.

Um, so that's one example. But also support is the soft things. Like do we have 
a flexible workplace? And you gave such a great example earlier of how what 
helps you thrive at work is not, it's not like, you know, hours on a call or 
hours in the office. What's amazing is you, you're super clear on what helps you 
thrive at work and what you need to do a great job.

And so, you know, we, that's, it feels like such a clear win these days of, of 
course we should give people flexibility because we do have, have different ways 
that we really succeed. So yeah, in brief, that's, that's kind of the high level 
how I would 

[00:45:51] **Michaela:** lay it out. Yeah. Maybe coming back to the last thing 
that you said I, I'm thinking about, about this a lot.

Right. And I think the only way why I can be so clear about it is because I'm 
self-employed . So I'm my own boss, right? And I think about myself and, you 
know, get, get on track with myself. And I actually had like a, a question 
yesterday from one of the tech mom group that I'm in. And so this, this mom 
asked, Yeah, how can I, you know, she has a two month old at.

And a full-time job and wants to strive there and no, no, uh, childcare, right? 
So what can she do? And so on, and, you know, Yeah, I, I, most of the, most of 
the comments were just to get childcare, right? , you can't do it, get 
childcare. Um, , which is, you know, which is amazing because it gives, uh, 
somehow permission to get childcare.

But then there are people like me, I don't want to get childcare, . Um, so I, I 
had my, I had all of my three kids at home, right? But it also means you have to 
work really differently and. Uh, and then, you know, my comment was that I'm 
self-employed and I'm so grateful for it, right? Because it means that I can 
take, you know, the time and I don't feel guilty.

I'm probably a very, um, I always have been a high achiever. Um, and so it would 
feel really horrible for me being, you know, at an office and knowing, you know, 
there are those expectations and I'm stretching them so far, you know, like so 
far. I don't know if, if people would be okay with it or not. Right. So, um, 
right now I can't imagine that anybody would hire me

Oh. 

[00:47:30] **Lauren:** Or, you know, No. Yeah, sure. 

[00:47:32] **Michaela:** I, No, I don't think so because, uh, I'm, you know, I 
would also take that time. Right. And when the baby is awake and the baby is 
number one, and then the baby's sleep. Then I'm really quick. You know, I 
learned that I'm really quick, like at the minute that the eyes go shut, I'm 
like, Okay, where's my keyboard

Yeah, fair enough. Um, but um, yeah, so yeah, what I'm saying is that I think 
flexibility is really good and I hope that more and more companies will 
understand that. I think we are going some way there, but I don't think we. 
Quite there yet. Right. So I think there's still a lot of stereotypical 
thinking, what means to be productive.

Right. And, and coming back to this really old thinking of when I'm in the 
office in my chair, then I'm productive. Right. Which is so far fetched. Right? 
Um, yeah, I was working at the large company, uh, during my study time and then, 
um, it was one of those very controlling companies, so you weren't allowed to 
have any stickers somewhere or pictures somewhere.

So very clean desk policy. All desks were, um, somehow facing others so that 
everybody could watch your screen. If you're not doing something, that's not 
work, right? We had like, yeah, we had like, uh, white lists of, uh, you know, 
uh, um, websites that we could go to and not other websites because they're all 
blocked, right?

So that you really do your work. And then what actually happened is that people 
were in the server room, , you know, doing some stuff, hiding in there to get 
their. The fair share of, of downtime and and so on. So I don't think people 
were really productive. I actually think it's the least productive company I 
ever worked with.

Right. Or for, So 

[00:49:15] **Lauren:** interesting. Yeah. Yeah. I mean, not surprising. Yeah. 
Yeah. And also, you know, that server room example, people will find a way . 
Yeah, yeah. You get to right. Like, um, yeah. Just better to, and, and I think, 
I think this is where clarity of expectations helps too. Because to me, to be 
honest, It's a lazy management approach to say, We're just gonna look at the 
number of hours that I could see you sitting somewhere working.

Instead of saying, Actually, what we care about is that we achieve these 
outcomes as a team, and this is your role in, in helping us achieve those 
outcomes. And then if you help us get there, You, you know, it shouldn't matter 
what time of day you did it or even the hours that it took for you to achieve 
that thing.

Um, because people work differently and, and, you know, and, and we wanna 
appreciate that. And so, yeah, I think that's where I think if we say like, 
actually this is what we care about, This is where we wanna get to as a team, it 
takes a little bit more work, but, but it's just, it, it then allows more 
flexibility than the old rigid.

You know, I need to see you sitting here eight hours a day. And, and that's how 
I know you did your job, . 

[00:50:18] **Michaela:** And, and I think it also, I mean, it's a little bit of 
burden for the, let's say the company or maybe the, the founder, the ceo, Right. 
The leadership team to really think, what's this worth? Right? So I want to, 
and, and thinking about outcome.

I want this feature. What is the worth of this feature? I want this blog post. 
What's the worth of this blog post? Right? And this comes into, maybe that's why 
I'm saying self-employment is much better because we are more thinking about 
those things, right? So if I'm making a contract with somebody, they tell me 
this is, you know what it's worth to me.

and then I say yes or no, and it, you know, if I put in 10 hours, I put 10 
hours. If I put hundred hours, I put in hundred hours, right? And so this is a 
little, little bit of a different conversation and I think it would be just fair 
to also have that. At companies maybe. Um, 

[00:51:06] **Lauren:** That's interesting. 

[00:51:07] **Michaela:** Yeah. Yeah. And I think that maybe quite some people 
would earn quite much, much more.

Right. Because they are valuable to the company and and so on. But yeah. Anyway, 
this is a completely different conversation. No, and we are going. 

[00:51:19] **Lauren:** Yeah. Oh, the last thing I'll say on that too though, is 
I think that's also where, um, so I, I sort of glossed over it, but one of the 
pieces of research, it's been around for a while, but honestly it's, it's 
becoming a classic, which is the project Aristotle research around why 
psychological safety is so important, and essentially, long story short, Google, 
so they notice that, you know, same high hiring bar across the company, but some 
teams were just performing so much better together than others.

Two years of research and looking at 200 teams later, you know, this is Google. 
The number one thing was the amount of psychological safety on that team. And I, 
I think part of it too is when there is that safety, when there is that trust. 
You know, I feel so fortunate that, that, um, like I, I love my team cuz I can 
really lean into this.

Um, with, when we can lean into this together, and it's just when there is the 
trust, you just know, you know, you know people have got your back. You know 
that they'll understand that you tried your best. And even if it, you know, that 
thing didn't work, that, that they're not gonna judge you for it. You know, 
they'll, they'll see you striving.

Um, and we also, we don't lose time then doing these. These kinds of, you know, 
these like funny rules or having, or having to work around funny rules. And so I 
think it just like the trust and the psychological safety, it's actually just, 
it's kind of like a, a lubricator for everything else to, to just make the rest 
go more smoothly.

[00:52:39] **Michaela:** Yeah, I think so too. I think it's, it's probably most 
important that you can just be up front and talk about what you really feel and 
you know how it's going and. You know, without thinking that you will be 
punished, which is sort of the bottom line of psychological safety, right? And 
so, yeah, I totally see that.

And, um, I have been at many different workplaces. Uh, psychological safety 
hasn't been always. Top of mind. Right? And yeah, and I think, I mean here in 
Austria, which is culturally, again, it already starts with school. School is 
not a very high, psychologically safe place, right? Mm. And it, it goes further 
with university.

It was not a psychologically safe place, right? And so from that entering work, 
Not expecting, you know? And I think just with, with age, I learned that 
actually it's something that I can expect, Right? That I can also ask for or 
that I, you know, and it's a privilege as well, right? Because Yeah. You know, 
if you need the job, you need the job.

You just have to go and, and work there. Yeah. That's so true. Yeah. Well, 
Lauren, thank you so much. We are, um, really on time now. I don't want to, you 
know, to take more time, uh, than, than I promised that I, uh, that this will 
take for you. So, um, is this something that you want to share with my 
listeners?

Something that they should take home, especially looking at metrics? Um, um, 
maybe some, you know, like the key thing that you would say them. Um, tell them 
about metrics and how you should use. 

[00:54:08] **Lauren:** Yeah, I mean, I would say two things. One, have the 
really should all start with the, like what matters to us. The, the metrics are 
simply a way for help, but to help us get indicators and sign posts of how are 
we doing at the things that measure that, that are what that matter to us.

Um, so that's the first one. And the second is that see the metrics as the 
starting point for a conversation rather than an answer. And, you know, it, it 
doesn't have to be every metric we need to discuss, but the metrics that are the 
most surprising or, um, different. . Those are the ones where whatever the 
conversation is, it'll probably help us surface some, some interesting things 
that have been going on, um, for our teams or, you know, with the underlying 
data.

Um, so yeah, that's my, that's my key takeaway and yeah, we're, you know, we're 
in, if you're a values aligned organization, if you're an engineering leader, 
who cares about people. Um, we do have a beta where we're bringing in a, a, a 
group of people, um, who our values aligned to, to give 

[00:55:05] **Michaela:** us that. . Yeah. Cool, cool.

So I have a last question for you, but then we really cut it short. . Okay. We 
can't stop. What about project based metrics? Because this is something that I 
normally recommend, right? So I'm not saying, Oh, this is the set of our metrics 
that we look now on for the next 10 years, but more like, You know, we are 
discussing and we think codery suck right now, right?

So now we are getting a bunch of metrics that we think are valuable and we track 
them, let's say for half a year. And then we really do some action in this area. 
And you know, when we feel better with our codes, we toss those metrics, we 
don't need them anymore and we take some other metrics. You know, take some 
other pain points that we are feeling, let's say about, you know, failure time 
or you know, time to recovery or something.

Mm-hmm. . And then we work on that for half a year or whatever it takes. Right. 
Three months. Um, and then we toss those metrics away. So this is how I normally 
work with teams. Um, do you see people do that? Um, do you recommend that? . 

[00:56:02] **Lauren:** Yeah, I love that. So we we're, um, we're seeing people 
do that in practice. We could do a better job of supporting that with our 
product.

That's something we've talked about is actually, um, kind of the, like basically 
doing an upfront question of what are you most focusing on and then having the, 
like your whole flow through the product really shift based on what is your 
number one goal today. So, um, something that we really wanna support more.

Um, but yes, in the meantime we do see people kind of, you know, like shifting 
their, their focus within the product and I love that. And the reason I love 
that is cuz it's such a sign of success. Um, I, when I was early in my startup 
days, someone told me once that there will always be problems. But success is 
that the problem has changed.

Mm-hmm. . And so this feels like such a great example of that is, you know, I 
love that you, yes, we had something we were worried about, but at least we got 
that to shift and now we've earned the opportunity to go worry about something 
else. . 

[00:56:56] **Michaela:** Yeah. Yeah. I love that. That's really nice. Thank you 
so much. Well, Lauren, thank you so much.

Thank you for being on my podcast. I really enjoyed talking to you. I could go 
on and on. Let's stop here, . Okay. 

[00:57:09] **Lauren:** Thank you. This was such a pleasure. Thanks for all. 
Thank you. 

[00:57:12] **Michaela:** Bye bye bye. This was another episode of the Software 
Engineering Unlocked Podcast. If you enjoyed the episode, please help me spread 
the word about the podcast.

Send episode to a friend via email, Twitter, LinkedIn. Well, whatever messaging 
system you use, or give it a positive review on your favorite podcasting 
platform such as Spotify or it. This would mean really a lot to me. So thank you 
for listening. Don't forget to subscribe and I will talk to you in two weeks.

Bye.


