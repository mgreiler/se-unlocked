---
episode: "Transcript Episode 76 with Abi Noda"
permalink: /measure-developer-experience/
status: publish
type: transcript
--- 

[00:00:00] **Michaela:** Hello, and welcome to the Software Engineering Unlocked 
Podcast. I'm your host, Dr. Michaela, and today I have the pleasure to talk to 
Abi Noda, CEO, and founder of DX, about measuring developer experience. 

But 
before I start, I want to tell you about my code review workshops. I have worked with 
engineering teams for over 15 years now on improving their overall happiness, 
productivity, and developer experience.

And I know that code reviews can be a well quite challenging engineering 
practice. The reason is that we all assume developers know how to do good 
code reviews, and that they have the technical and social skills, but we don't 
actually give them training or instructions on how to do them. In addition, it's a 
team practice.

This means that we have to coordinate our efforts, we have to have some 
organizational maturity, and we have to have a shared understanding and shared 
values of what's important during code reviews. But many teams really suffer 
from many pain points such as long waiting times, high workloads for experienced 
engineers, or inconsistencies in their reviews that are done throughout the 
teams or the organization 

This is why I specialize in helping development teams make code reviews their 
superpower. While doing empirical research at Microsoft and working with all 
major product teams such as Office Windows or Excel, I gained tons of industry 
experience and I share that during my code review workshops. The goal of those 
workshops is to make code reviews fast and, at the same time effective.

If that sounds interesting to you, hop over to [awesomecodereviews.com](https://www.awesomecodereviews.com/) or write 
me an email to book a workshop. So visit [awesome code reviews.com](https://www.awesomecodereviews.com/) today. But now 
back to Abi Noda. 

Abi Noda is the CEO of [DX](https://getdx.com/), a platform for measuring 
developer experience. Previously he worked at GitHub after his startup, 
PullPanda was acquired by them.

I know Abi from his work on code reviews and I was lucky enough to have worked 
with him on the research behind dx. So today we will talk about our joint 
venture to define and research develop experience. About developer productivity 
and most importantly, about improving engineering processes and practices.

So I'm super, super thrilled to have Avi here with me on the podcast. Hello, 
Abi. Welcome to the show. 

[00:02:23] **Abi:** Thanks, Michaela, excited to be here and so happy to be able 
to chat with you about developer experience. Yeah. Yeah. 

[00:02:29] **Michaela:** So developer experience, I think, uh, some people know 
the term and some people are completely new and probably ask themselves 
developer experience.

What's that? Right? Can you briefly share your definition of developer 
experience? 

[00:02:43] **Abi:** Well, of course, I'm gonna turn this question back around to 
you in a moment. But as we both know, defining developer experience was a 
journey in of itself. When we began our research, we had a vision, a thread of 
an idea of what developer experience was. But it wasn't until we spent a lot of 
time going through prior literature concepts from prior research in psychology 
and built on that, that we were able to actually.

Create a definition that was concrete for what developer experience is. So in 
our paper, of course, we define developer experiences as how developers think 
about, feel about, and value their work. In layman's terms, developer experience 
is about the lived experience of developers. The joy, the frustration.

The bottlenecks that they experience in their day-to-day work. And encapsulating 
all those different factors which affect their experiences. That to me, 
and in our research is what developer experiences, But how about you?

[00:03:45] **Michaela:** I normally say, right, just in my practice, 
right? So not with a research hat on.

I would just say a good developer experience is if I can do my work joyfully, 
right? So I, I really like this, uh, way, and I, I actually got that really from 
the interviews that we did because we interviewed a couple of practitioners, right?
Engineers, software engineers, and ask them about developer experience.

And I think this really stuck with me, right? So, doing my- Because 
I asked the people, what is a good developer experience? 
And I think this came up in different ways, obviously, and with different terms. 
But this stuck with me, right? So doing my best work joyfully, not some 
work, but best work joyfully, right?

So it's fun and it's joy, it's quality, and I think everything is just in this 
little sentence. So I, I normally really go back to that. Um, yeah, yeah, yeah. 

[00:04:37] **Abi:** Yeah. I like that a lot. And I remember when you came up 
with that line, we all loved it. Right. Yeah. And I think it's a good 
approach to define developer experience in that way by really a concrete 
depiction of what good experience looks like and what.

Bad experience looks like. Because I think that's more concrete than just the 
abstract definition around feeling and thinking. Yeah, yeah. The psychological 
concepts. Yeah. 

[00:05:02] **Michaela:** True. But I think also it was very clear for us when we 
did this work that if we are too vague about it and too practical about it, 
that from a research perspective, this is not gonna work.

Right. So we've really had to dissect this idea and look into it. Something else that
What's interesting for me, because you were saying you, you want to look at, you know, 
the real experiences and we have to make it practical. What was interesting for me about
developer experience is that some people can have a, a crappy 
code base and still have a good developer experience, right?

And you can have a crappy code base and have a horrible developer experience, 
right? So can you tell us a little bit about the factors that we discovered, 
um, around developer experience and what are those? But what are factors, right? 
What, what does this even mean? Factors of developer experience. 

[00:05:55] **Abi:** Sure.

Well, I'm first speaking to the expert on this cuz you've led much of this part 
of our study. But you know, one thing we looked at in our research, of 
course, was what we called factors, which are the aspects of the work 
environment for developers that affect developer experience either positively or 
negatively.

So we identified over 25 factors in our research and building on prior research 
into developer productivity. Things such as psychological safety or product 
management processes. Or having clear requirements for tasks and building test 
tools. All these different factors make up developer experience. And I think the 
first part of your question was referring to another discovery we made in the 
research, which was the contextual characteristics which affect developer 
experience.

And I think this was the discovery you really made, and that was that. Developer 
experience was not just about the surroundings of an individual, like the tools 
and the work processes, but it was also a function of an individual person's 
context. What their expectations were, what their day-to-day consisted of, how 
many years of experience they had, or what previous companies they had worked 
for.

So both the work environment as well as the individual lens of a person 
make up the overall developer experience in terms of how people think about, 
feel about, and value their work.

[00:07:24] **Michaela:**  Yeah, that's true. And actually, now that you bring it up, 
I think about it and I was really fascinated by that because previous research 
that we looked at, they really looked at the factors, but never had this 
contextual thing about it, right?

That it's actually you. Right? So we can have the same experience being the same 
company, the same team, and you think it's cool and I think it's right, and it 
depends on the position that we have in our expectations, as you said and so on, 
right? Yeah. So yeah, this, this research was really fun. I really liked it.

I think I talked about it on this podcast already, one time. And I'm going to 
to link our paper as well. But I want to go a little bit deeper 
in this podcast with you now, because you actually productized this idea, 
right? So you build a product around this and you actually help 
people really measure developer experience, right?

You help help companies measure developer experience. And with these 
measurements, they're driving improvement processes. And obviously this is, you 
know, this is what I'm super interested about because I look at one aspect, 
right? I look mainly at code reviews, work with teams on measuring code 
reviews, knowing the pain points and then improving their code review 
processes, right?

So you have this a little bit bigger picture here. You look at testing 
probably, building, right? So you can tell us more about this. So you look 
at developer experience in general, and then measuring that. And then I 
think the improvement is a little bit out of your scope, but you probably have a 
lot of insight into, you know, what makes teams successfully improve and 
change their processes and practices.

So I really want to dig deep into your knowledge here and, um, and also so that 
my listeners hear about what you learned about this. 

[00:09:07] **Abi:** Yeah, well there, there's so much there to unpack. And of 
course our most recent paper, the ECM Paper on developer experience is 
really aimed at moving this conversation forward a little bit, particularly on 
the measurement side, and providing a glimpse of how organizations are tackling 
developer experience internally.

However, one thing I would start by saying is that you know, when we did our 
research, Michaela, we found that there was this big awareness gap within 
organizations. Developer experience and the friction points and the 
bottlenecks. These were things that were so obvious to developers on the ground.

Yet we also heard them talk about how it was difficult to actually move 
solutions forward. Or get leadership to care. And I think what's happening 
in the industry right now Is really the sort of a chronological 
progression of what we discovered in our research. I think leaders and companies 
are just now starting to open their eyes and become aware of the challenge and 
the opportunity that developer experience represents within their organization.

Yeah. So, as we talk about how organizations are measuring developer 
experience and how organizations are improving developer experience, I wanna 
caveat the discussion by saying, I think this is rapidly evolving. Yeah. And a 
lot of leaders in organizations are still trying to figure it out.

[00:10:27] **Michaela:** Yeah. And maybe something that I want to add here, 
because sometimes I'm blown- it's blowing my mind actually that I, 
I'm now daring to say it.

I think I'm the only one that's out there in the internet that's working 
actively since four years on improving code reviews, working with teams, giving 
workshops, and helping them turn around their horrible experience on code 
reviews and, and helping them to make them. And I'm always like, "Why is nobody 
else doing that?"

But I think this will change. I actually think this will change, right? 
There will be more people maybe looking at developer processes, helping 
people improve, doing change management, and things like this. But yeah, I'm 
still like, I'm still baffled. I'm like, this is so obvious, right? Like people 
are- And there's so much money going into horrible engineering practices,
people that suffer in code reviews that get all, you know, these negative things of 
bottlenecks.

Toxic behaviour nitpicking, you know. Like, I mean, I have a list of things, pain 
points. It's huge. Right? And there goes so much money into 
this practice that is not done in a nice way. And the benefits like  
knowledge sharing and, you know, all of that, they diminish, right? And I 
wonder why is nobody doing something about this.

Right? And, so yeah, I totally see what you're saying. It's new, right? 
People don't know exactly what they're doing. Or this is maybe too far. 
But we are really early, I would say. We are really early and there were things 
like Dora for example, right, which is on a very different level. It's a very 
like on a very large scale level. Very few things that we are looking at.

And this is what we try to measure and to improve. Maybe you can talk a little 
bit about the space. And Peggy, Margaret and Story(??) for 
example, Dr Margaret and Story(??) worked with us. Also on this research, 
right? She's also author of space and so on. So, there are some, you know, 
first seats I would say in this area.

Uh, but it's, it's early. Yeah, it's early. So, how do you see that? 

[00:12:31] **Abi:** Yeah, it's definitely early and it's exciting to think about 
how all the dots are connecting when we look backwards. I think things like 
Dora, which you've mentioned, and the Space framework, really, they are all 
relevant to developer experience. Although in terms of the way in which they're 
applied, I don't think they really get at the problem of how to really 
understand and improve developer experience.

[00:12:54] **Michaela:** Yeah. Maybe quickly say what Dora is in space. I let you tell 
the people.

[00:13:00] **Abi:** Sure. Yeah. Dora stands for DevOps Research and 
Assessment. Dora was a company started by Dr. Nicole Forsgren, who of course we 
work together with today. And Dora was focused on investigating a construct 
called software delivery performance, which is different than the construct 
we're focused on, which is developer experience.

And the construct which Space was focused on, which was developer 
productivity. And Dora and then the book that spun 
out of the company accelerate. And then the annual reports that are continued by 
Google today have been an ongoing investigation into the link between software 
delivery performance and business performance, as well as the inputs and 
capabilities that drive software delivery performance.

And so most people know of Dora through the popularized four key metrics, lead 
time, deployment, frequency, yada yada. Yeah. But really the research program, 
those are the, you know, dependent variables that are being studied against the 
numerous capabilities, practices, and inputs. Things like version control or 
trunk-based development or continuous delivery.

Accelerate was really born out of the early days of the DevOps movement and the 
movement toward continuous delivery. And then fast forward a few years, Space 
was born. And space was written to try to demystify the conversation around 
developer productivity, which of course is still an elusive problem space and 
not solve developer productivity.

However, what Space did was provide a sort of meta-analysis or summarization of 
all the prior research that existed on developer productivity. Of course, much of 
that research was led by Dr. Margaret, and Story, Peggy, who we also work with 
today. And you know, Space tried to create a practical framework for thinking 
about all these different aspects of developer productivity that have emerged 
through practitioners as well as research.

And put that into a simple framework for organizations to think about. Yeah, 
and I think one of the interesting things about Space was it really made this 
point explicitly that you can't reduce developer productivity to a single 
number. You certainly can't reduce it down to output metrics like commits or 
number of core requests.

And I think what sort of has opened the door and inspired us in our 
research around developer experience was this idea in Space that you have to 
factor in the perspectives of developers themselves. Their sentiment, their 
attitudes and opinions toward their work are a big part of measuring and 
understanding developer productivity as it is also important to developer 
experience.

[00:15:42] **Michaela:** Yeah. So I would say what everything, what is uniting 
everything is we want better outcomes for the business, right? As you want 
better work experiences. And then there are different ways to get that 
right. Dora is all about, okay, I'm deploying very often. I have small changes. 
I can roll back, I can react to failures and so on, right?

So there's no Friday deploy and then everything goes boom and we have to work, 
you know, like several days to get that back. So it's somehow 
measuring from this perspective. Then Space is all about productivity. Please 
don't look at how many stories that person closed or how many 
added lines they added and say, "Oh, this person is especially, or specifically, 
very productive because they added 1000 lines yesterday to our code base."

Right? And then developer experience I think, why I was so fascinated by it is 
because it's really about how do I. I think also dev developer know best. This 
is what I deeply believe, right? They know. And then you have the surrounding 
of, you know, circumstances that force you into practices or processes 
or, you know, have to deal with things that are a little bit out of your 
control.

And if we pay closely attention to what the developer says, "Oh my 
God, this is horrible." And if you can turn those moments around into, "Oh 
yeah, this is working." We get a really good output for our business. Right? So I 
think this is a little bit different way of thinking about it. But 
can you tell a little bit of how, how do you measure that?

Because you formed this platform for measuring developer 
experience the X(??), right? So, how can I imagine that? How do you, you know, 
measure developer experience? How do you do that?

[00:17:29] **Abi:** Yeah. I would reiterate what you said 
around, you know, our focus with developer experience being guiding 
organizations to focus on the pain points of developers, which are surfaced by 
the developers themselves.

And the thesis around this is that if an organization focuses on those things 
and improves them, then you can improve developer productivity. So this is 
around improving developer productivity. Similar to the narrative around things 
like Dora and Space. Now, when it comes to how to measure developer experience, 
it was obvious from the beginning that you couldn't measure or understand developer
experience without heavily relying on the perspectives of developers themselves.
And in more technical terms, this a practice of turning feedback and perspectives
of people into quantitative measurements is called psychometrics, also known as surveys. 
And so in terms of how to measure developer experience, the primary approach that 
organizations need to follow is a survey-based measurement approach.

They need to ask developers questions about how they feel about the work, what 
their actual day-to-day workflows are, and take those inputs and then use 
statistical methods to turn those into both qualitative and quantitative signals 
that they can use to understand where they're at. And measure progress as they 
attempt to improve.

[00:19:00] **Michaela:** So you actually built the observability platform, not for our 
software, but for our software engineers. Is that, is that correct? 

[00:19:09] **Abi:**  Well I love that analogy. Yeah, I love that analogy. Cause one 
book I've read that I really love it's called 'How to Measure Anything', and it's 
a book on how to measure intangibles.

And in that book they have a chapter where they, it's titled 'Humans', the 
ultimate measurement instrument. And I was recently speaking to someone 
and talked about how a thermometer, a digital thermometer is a measurement 
instrument. It takes an input from the air. I don't actually know how to 
thermometer works, but it takes an input and it spits out Signal.

It spits out data. And the human brain can do that as well. Humans can 
observe the world around them, observe the processes and tools, and then spit 
out data into our systems such as DX, a platform for metric developer experience, 
where we can turn those signals into numbers and insights. And so I, I love your 
analogy.

Absolutely. We're using humans to give us data about our tools and systems.  

[00:20:11] **Michaela:** Yeah. So, now we understand why it's important. We 
understand, I think, what we are doing here. We are measuring our experience and 
identifying, for example, pain points, right? What's the next step? So you, 
I know that you have already tons of engineering organizations that use DX, 
right?

So you have tons of insights. You're also, you're still interviewing many many 
people, right? Engineering managers, VPs, people from the platform teams that 
really are only focused on measuring developer experience and improving 
developer experience. But where to go from there? Let's say we know. Let's say, 
our testing infrastructure sucks, right?

What's the next step? What are people doing? What's successful? What makes you 
successful? Because I've seen it, right? I do it with code reviews. And I know I
have a lot of companies that try to improve their code review 
processes internally. They maybe even know what their pain points are.

Maybe they don't know exactly. But then they fail. And so, so it's not 
that easy. Change management is not easy, right? Improvement comes not 
naturally, I would say. So, what's your take on that? What does it take to make 
positive change and impact on developer experience? 

[00:21:25] **Abi:** I think one of the things that I've learned that wasn't 
clear at the beginning of this journey as the importance of executive buy-in. As 
we know from our research, developers are often frustrated with how obvious 
these problems are to them, yet how little the business or leadership seems to 
care.

And I think one trend we're seeing in the industry as a whole is that the 
C-Suite is starting to care about developer experience. So companies like 
Microsoft, Atlassian, Spotify, all have developer experience KPIs. As C-level 
metrics for their organization and everything as far as change management is, 
change management is cascading down from there.

It's very difficult to drive substantial change in an organization, especially 
change that requires human processes, not just fixing technical systems without 
buy-in from leadership. Once you have buy-in from leadership, I think there 
are two primary modes for improvement, and we can talk later about specific 
examples and where the challenges are in each of these modalities.

But one mode of improvement is really top-down initiatives or sweeping 
cross-cutting initiatives led by upper-level leadership or dedicated developer 
productivity teams or platform teams. So, for example, you brought up around build 
and test tools, for example. That is a very common foundational level challenge 
that is often well addressed by a dedicated platform team or dedicated developer 
productivity team that tackles that problem looking across an entire organization.

The other modality for how organizations try to improve developer experience is 
by focusing on enabling local improvements on every individual team across the 
organization. Michaela, in our research, one of the things we found was that 
developer experience and the entire software development life cycle and that 
a lot of the challenges were specific to the context of individual teams.

It might not be that there is technical debt that is really the entire 
organization. It might just be a specific component or part of the code base 
that one team is working on. And as you know, with code reviews, it might just 
be the processes of one team. It might not be a systemic issue across 
organizations.

And so the second mode of improvement focuses on providing education, 
insights and support to local teams to enable them to drive their own local 
improvements to the issues that are most pressing for them. 

[00:23:56] **Michaela:** Yeah. So something that, you know, when you said the 
first thing we need buy-in, you know, we need people behind higher up 
management must, you know, stay behind us.

The only thing that came to my mind is we need money actually also, right? 
Which is the cruel reality, right? We can be very engaging and very 
enthusiastic about something. But if you're not willing to spend money, then 
I think it's going to fail. And I mean money here in this way of, "I have to 
dedicate engineers to build, uh, out our testing tools," right?

This is, it's not for free. I have, you know, let's say five people or maybe two 
people, or even one person, right? I have a whole full-time engineer of 
working on something that's not going directly to the business. And I think 
sometimes people really struggle with that. Also for local improvements, you 
can say, "oh yeah, we should really work on that."

But in addition to what you all do on your regular basis, in your 40-hour work 
week or whatnot, right? Then I also want you to do this, but I don't give you 
time for that, which means I don't give you money for that because if I give you 
time for it, half of your work or 20% should go into this improvement, right?

So, sometimes we don't talk about it. I think people always talked about, 
you know, yeah, we have to have commitment or buy-in. But actually, we have to 
throw money at the problem as well, right? So, or willing to be spending 
money on that, right? And another maybe the second question, 
I always ask two questions.

So you have two is that I also have seen that, right? I've seen that people get more 
into that. I saw that, especially around the end of or  beginning of 22, I think. 
and then end of 22 when the whole layoffs happen. I was like, "What's going to happen 
now?" Maybe this is also why I bring up this BUN(??) money problem here right now.

We have layoffs everywhere, cutting and so on. Have you seen something like 
this? Are people now again, a little bit more tight with their 
improvements, they are big on the vision and the ideas of improvement, but then 
they're tied on the money that they want to invest in the problem? 

[00:26:06] **Abi:** These are such important points you've brought up, and 
you're absolutely right, both of the things you mentioned.

So at the leadership level at organizations, there's a huge challenge of 
figuring out what the right investment should be in developer experience 
improvements. And at the local level, like you said, there's often a challenge 
around the conflicting priorities of local teams of, "Do we 
have time to clean up some technical debt, or do we have to go ship the next 
feature that product management told us we need to deliver?"

Both of these challenges are real common headwinds that both managers at 
the local level and executives need to confront and navigate. I think as 
far as your question around the overall trend right now, given the current 
economic state: There have absolutely been platform teams and developer 
productivity organizations that have been downsized or even eliminated.

At the same time, I think there's just as many examples of organizations 
that are doubling down on their investments in developer productivity. 
And that is because the ROI of improvements to developer productivity are 
powerful. When we think of a large organization with hundreds of engineers. If 
you can improve efficiency or productivity, and let's use those terms loosely
for the purpose of this conversation by even 1% or 2%,

then there's enormous amount of capacity gained back to the organization that 
can be quantified in terms of real dollars to the business. The challenge 
oftentimes is that it is difficult to identify what that ROI really is. It is 
difficult to quantify what efficiency and productivity mean within an 
organization.

It's difficult for leaders to convey that effectively to stakeholders to get 
that executive buy-in. So that's one part of, I think, what I'm seeing as far as 
how leaders are trying to navigate the challenge around what's the right 
investment. And there's a lot of podcast that I've recently done, conversations 
I've had with leaders at all different organizations and different organizations 
just have different philosophies on this and different cultures.

An organization like Google, for example, has historically had an enormous 
investment in their developer productivity organization that would astound 
those people out there in the industry. Whereas, you know, a lot of 
earlier stage startups probably are just starting to think about forming 
dedicated groups and investing in infrastructure and improving the developer 
experience. 

At the local team level the challenge you brought up of the conflicting priorities,
I think is a very real problem. And I think this is an example again, where 
executive buy-in is so important. When the leaders at the very top of the organization 
are talking about the importance of developer experience and developer productivity, 
that really opens the door to middle management and frontline management, having 
discussions about what amount of investment they can make at local levels to 
these problems as well.

The common challenge I see is when an organization is trying to enable local teams 
to improve without the buy-in from executives. That often leads to the problem you
described of _there's just these conflicting priorities_ and managers have no choice
but to neglect internal developer experience improvement and favor of just focusing
on feature delivery.

[00:29:50] **Michaela:** Yeah. So at the beginning of, you know, can I say 
recession? I dunno if people even say it is, but I would say it is. Anyway, 
when we all thought like, maybe it's coming and, you know, I heard, I 
unfortunately forgot who said it, but it was a conversation about 
short-term thinking and long-term thinking, right?

And that a lot of companies are actually going stronger out of such a difficult 
phase because they're having a long-term thinking strategy, right? And I 
think it's what you're saying, it's return of investment, but it's 
also if people have the understanding what it means, right? To improve something 
that's hard to measure, something that's hard to understand.

But I think it's also maybe also, you know, being able to 
see the bigger picture, right? So, to know that people that are 
happier, are more productive. People that are more productive, you know, 
are happier, productive, and more proactive. I did a lot of research and reading 
and so on in our journey on proactiveness Rich(??).

This is such an important concept that we don't talk enough about, I think, in 
our paper. But, you know, it was 10 pages or something. I think we even got, 
went over it, right? But proactiveness, you can only get that right if 
people are actually happy and if they're engaged with your company. 
And what this brings to your organization is so important, right?

So I think there's this short-term and long-term thinking. But 
something else that came in into my mind: so, there was actually a 
tweet I think by Georgia(??) recently. Have you seen it? Where he talked 
about that PR numbers are now used as stack rank number actually, right? So 
how many PRs are people opening and closing and, you know, pushing through 
and merging. And they are now used to, you know, justify who has to go 
and who has not to go, right? In this difficult time of layoffs.

And I think it's a wonderful example of how dangerous metrics can be, right? And 
I'm always, you know me for a long time now, right? You know 
that I'm, I'm very data-driven. But on the other hand, I'm very sceptical about 
metrics, right? I'm like, when somebody tells me, "So how should we measure 
now our improvements for code reviews," right?

I'm, "Don't measure the turnaround time of PRs, please don't do it." Or the number of 
prs or something. Right? So, but what about DX? Can we misuse it or have you 
seen people misuse those numbers to, or gamify the system and so on? Right? So 
most of the metrics I've seen, Dora included most of the space metrics, right?

Can be actually turned around to be evil. What about DX? Do you think it's, it's 
completely space heaven or you know. Or do we have some... do 
we have to be cautious about it as well? 

[00:32:49] **Abi:** I think all numbers can be dangerous if used in the 
wrong ways. I will say, and I'm of course a little bit biased, but you know, 
I've worked extensively with both types of metrics and in my own career. I do 
think that our approach to measuring developer experience is much less 
perceptible to the types of problems and harmful consequences that we see with 
past approaches to measurement.

And I think it boils down to the fact that measuring developer experience and 
really developer experience itself is really ultimately in service of developers 
themselves. And this is in contrast to metrics like lines of code or number of 
pull requests, even metrics like cycle time, which are often more of a top-down 
view of developers or the development process.

Look down upon by leadership, and there's an inherent tension there when metrics 
and use in that way, because of course, leadership does not understand the full 
context and full story behind these types of metrics. And oftentimes leaders are 
unaware that those types of metrics are really just fundamentally ineffective 
and invalid for measuring software development in the first place.

And so I think the devex(??) approach to measuring productivity and software 
development processes is safer. I don't wanna come on here and proclaim that it's 
foolproof and bulletproof. But I do think it's much less susceptible to the 
types of flaws and negative patterns we see with other types of measures.

[00:34:22] **Michaela:** Okay. So when I was working with a couple of teams 
actually in the past on code reviews. Even though I would say, well, when 
I'm coming in and working with teams on code reviews, only good thing 
came out for the teams, right? This is my perspective. But still, you know, I 
have experienced teams that are reluctant to actually work on that, reluctant to 
share their pain points, reluctant to do changes, right?

There are fears behind it. Different concerns and so on. Have you seen 
that as well? That people, for example, don't want to fill out the surveys? 
Don't want to say that actually they have a problem with their testing 
infrastructure. That they maybe, I mean, I'm just. From my experience 
stating here that if I'm saying I have a problem with testing, then I have maybe 
to invest time into that, you know, solving this problem, there becomes this 
expectation that we are going to improve, you know, this pain point.

And, and maybe I don't have the time, right? Maybe there is not the buy-in or 
maybe, you know, maybe there is the official buy-in, but no actually buy-in. And 
so I see a lot of problems here. Have you seen that as well? And what can we do 
about it and how can we even address it?

[00:35:30] **Abi:** Wellabsolutely. In our recent paper, Michaela, we talk about 
some of the challenges of running surveys and some recommendations we have for 
processes that organizations can follow.

But to your specific point around the concern for developers in filling out 
surveys, absolutely. There is a, just as there's a scepticism toward the 
accuracy and reliability of surveys by leadership, there's also quite a bit of 
scepticism and fear of surveys from employees and developers who may have had 
prior experience with HR surveys or other types of assessments that were used in 
ways that didn't seem productive or safe to employees.

And so success with surveys... So, first of all to your question, absolutely. 
There are many examples of organizations that don't present these surveys in a 
proper way to employees, and as a result, developers are fearful and there are, 
there's poor engagement on these surveys. I think what we see is that 
organizations that communicate and present these types of developer listening 
programs, that's what I like to call them now, survey programs, to developers 
in a really intentional and sincere way where it's positioned as, "Hey, we want 
to create a great place to work for our developers.

And in order to do that, we need feedback from you. We need feedback on what 
the pain points are in our tools and processes." And when presented in that way 
to developers and of course the data is confidential and it's not, people 
aren't singled out in terms of their responses. When there are safety mechanisms 
like that along with clear intent and communication.

I haven't seen too many instances of what you're talking about where developers 
are highly sceptical or fearful of participating. And so, with organizations that 
DX, our company works with, we are seeing sustained participation rates of over 
90%. And that's due to a combination of factors, both the guidance we provide to 
organizations on how to implement a survey program and also the safety 
mechanisms that are incorporated into our platform itself.

[00:37:45] **Michaela:** Yeah. And so you said that the intent, but 
who is responsible later on to like, we see it? Who is responsible? Like, I'm 
filling it in, I say this is all, you know, horrible here and great here. 
Who is going to get rid of the mess that I am experiencing? 

[00:38:05] **Abi:** That's a big challenge, you know. A lot of organizations 
who get started with measuring developer experience and surfacing feedback are 
overwhelmed by the amount of things they discover, almost in a similar way as 
when we did our research and we were blown away with the amount of

pain and frustration that exists in the developer experience. And so, you know, 
taking that feedback in and quickly turning it into solutions is, is not 
something that most organizations necessarily have the capacity for. And so what 
I've seen work while for leaders is to, to not promise something that's 
unrealistic, which is that all the problems will be solved.

But to start a dialogue with their developer population. It's okay to say, "Hey, 
this feedback is incredible and it will help us begin to get an understanding of 
our challenges in our, as an organization. And it will help us inform our 
priorities, not just today, but in the future." It's also okay to say, "Although 
this feedback is great, we aren't able to focus on it right now.

We can't, we can't spin out 10 teams to start focusing on these problems. We, we 
have other more important business priorities." But I think as long as there's 
that dialogue, candid dialogue between leadership, management, and developers. I 
think these programs can be successful even if there aren't concrete initiatives 
around solving problems that are immediately launched.

Of course, long term, you can't keep just acknowledging the feedback without 
doing anything about it. But I think organizations can, can bite things up 
slowly and can really focus on having a dialogue with their population, employees, 
rather than feeling like they have to respond and solve everything right away.

[00:39:51] **Michaela:** And I think this is also coming back to the, the 
research that I did with you. This was so clear from, from the people, 
right, that talked with me, and that that shared like, you know, the most 
frustrated ones and the ones that actually left their companies were the ones 
that felt like culture,

you know, the culture of it's not going to change. I cannot even voice, you 
know, my frustration and so on, right? Those were the people that actually said, 
"Yeah, this was horrible. You know, nobody did something about it. You weren't 
even allowed to speak up." Right? And so I actually laughed and changed. So I 
think this is.

What you're saying is very true. It's a dialogue, right? It's also 
important that we are not over-promising. Things are hard to change. 
Processes are hard to change. I think the tooling is maybe even a little bit 
easier. Not easy, but easier. Processes, practices, they're really 
difficult to change and it needs a lot of commitment and also some time.

But yeah, it's a dialogue. I really like that. So, well, this brings us 
actually sort of to the end, Abi. What is your, what is your wrap-up for 
this, for this conversation? 

[00:40:57] **Abi:** Well, one thing I wanted to add kind of to the current 
topic is that I see organizations trying all kinds of creative ways to address a 
lot of the challenges we've talked about, both the implementation of developer 
listening programs and also the resourcing problem, the capacity problem

we talked about. How to actually make sure that follow-up occurs and improvements 
are implemented. For example, one organization that I met with recently is doing 
something unique that I haven't seen anywhere else, which is that they had an 
existing agile coaching organization within their company.

And they're now redeploying the agile coaches to actually be the leaders 
of developer experience improvements on every individual team across the 
company. I think that's a really interesting approach that solves one of the 
problems we talked about earlier where frontline engineering managers are 
already so slammed with delivery work that they don't really have the capacity 
for working on improvement efforts.

As far as wrap-up goes, I think one thing I wanted to say earlier as 
well is that when we talked about getting that buy-in from leadership and why 
there's a challenge there and why one of the challenges quantifying the 
potential that exists in improving developer experience. I think it's worth 
taking a step back and saying that, "Look, we know that leaders care a lot about 
developer productivity and experience.

We also know that developer experience is one of the keys to improving developer 
experience." So I think the challenge here is to really find the link between 
the two, and I think that's what our research today is really focused on. The 
final thing I would leave you with, Michaela, is that earlier we talked about 
the challenge that leaders face in figuring out what the right investment 
in developer experience is. But I think that if we take a step back, it's worth 
mentioning that we know that business leaders and engineering leaders care a lot 
about developer productivity and efficiency in their businesses in general.

We also know from our research, Michaela, that developer experience really is 
the key to improving developer productivity. And so I think that the opportunity 
for us, and I think the focus of our research going forward as well, is finding 
ways to help organizations link the two and find measurements and ways of 
quantifying that opportunity so that they can advocate for the investments and 
opportunities that exist within their organizations.

[00:43:28] **Michaela:** Yeah. Yeah, I totally agree. I think this is also a 
really nice ending. Thank you Abi so much for spending time with us, 
talking about your amazing startup and sharing all your wisdom around 
developer improvement, developer experience. And yeah, thank you for your time. 

[00:43:46] **Abi:** Thanks so much for having me on the show, and it's been 
a pleasure to work with you on this research and excited to continue working 
with you on more research in the future. 

[00:43:53] **Michaela:** Yeah, me too. Okay, Abi. Bye-bye. 

[00:43:56] **Abi:** Bye-bye. 

[00:43:59] **Michaela:** This was another episode of the Software Engineering 
Unlocked Podcast. If you enjoyed the episode, please help me spread the word 
about the podcast. Send the episode to a friend via email, Twitter, LinkedIn. 
Well, whatever messaging system you use, or give it a positive review on your 
favourite podcasting platform, such as Spotify or iTunes.

This would mean really a lot to me. So thank you for listening. Don't forget to 
subscribe and I'll talk to you in two weeks. Bye.


