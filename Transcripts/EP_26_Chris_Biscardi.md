# Transcript Episode 26 with Chris Biscardi
**Michaela:** [00:00:00] Hello, and welcome to the Software Engineering
Unlocked podcast. I'm your host, Doctor McKayla, and today I the pleasure to
talk to Chris Biscardi. Chris has an independent consultant that works with
startups built on open source. He's also a blogger, streamer, and the creator
of the awesome Party Corgi community. Before he worked for Dropbox.
And now he builds cool new frameworks such as Toast. But before I welcome 
Chris, let me tell you about my awesome code review workshops. Yeah, in my 
code review workshops you, and if you want, your whole team, can learn how to
get the most out of code reviews. Because if we are honest, code reviews are
very time consuming and therefore also a very expensive engineering practice.
Well, that's where I come into play. I help teams to make code reviews 
their super power instead of an expensive bottleneck. And to make it easier for
you to find my workshop I got a brand new domain called AwesomeCodeReviews.com. 
So don't hesitate to hop over to AwesomeCodeReviews.com. Now it's a great time 
to book a workshop before the year closes or to propose it to your manager.
But now let's go back to Chris. Chris, welcome to my show. 

**Chris:** [00:01:09] Hey, thanks for having me. 

**Michaela:** [00:01:10] Yeah, I'm really glad. So, Chris, uh, one of the
things that I think I'm very interested in, I think a lot of my listeners are
interested in is how come that you are now an independent consultant? What do
you do? And especially I see that you have picked somehow a niche, right?
You're not a general, independent software engineer, you know, taking on any 
project, but somehow you make specifically clear that you're taking on projects 
that are, has a startup culture behind them, right? So they are having this new 
element in it, but also they are built on open source. Why did you pick that?
And, um, yeah, what's, what's the reason behind your choice here. 

**Chris:** [00:01:51] Yeah, I guess um, to me picking it seems a little bit 
like too much of a, uh, I guess I don't know how to phrase that, but basically 
like when I started my career and, uh, I was an early engineer, uh, I started 
out freelancing for smaller open source projects and that's how I made my first 
money as a engineer.
So I didn't become an employee until about halfway through my career. And then 
when I did become an employee, I started working for companies like Docker who 
have very, very large open source presences. So I started out in open source. I 
continued in open source. And then when I went back to freelancing and then 
eventually consulting, it was something that I just kind of like already had an 
expertise in, right?
I guess we'll talk about Party Corgi later, but like the whole like open 
source community and how do you deal with PRs and how do you deal with the 
community at large and, what do you decide to work on and how do, what do you 
tell to what people to get everything to move forward in a way that is 
collaborative and, uh, results in the best result for the community, as well as
the company.

**Michaela:** [00:02:55] Yeah, that makes total sense. So when you say you're
you work with startups that build on open source, do you mean that they are
using open source to build their software and that could be proprietary? Or is
it really also startups that then open source their systems? Or could it be
both? 

**Chris:** [00:03:16] It's usually, uh, startups that have a very large open
source component.
So for example, I did some work with Gatsby. And Gatsby's core software's open 
source, right? Docker's core software was open source, like the Docker CLI and 
things like that, um, and then a bunch of the other, like clients that I've had
have had large components of their business reliant on open source. So it's not
just like, "Oh hey, we use NGINX as a load balancer."
Like, yes, you're technically using open source, but it's not quite the niche 
that we're talking about here in terms of the business is dependent on an open 
source project that has a large community presence. The community health sort 
of indicates the health of the company in a way. Um, so it's, it's that kind of 
specific.
Um, but I have taken contracts from places that are sort of like just using open 
source and they have a specific project they need me to work with and whatnot. 

**Michaela:** [00:04:09] Okay. Yeah. I see. Yeah, but this is, as you say, it's 
quite the difference, right? Also the things that you mentioned that these are 
large projects, right?
So, um, when you were saying startups, I was thinking this, you know, three 
people over there that have this idea, um, they want to have a startup and they, 
they may be outsourced their, their development or something like that. But it 
seems that it's a complete different, different way of consultancy, which is 
really focused on understanding community.
As you said, understanding how open source works. So they are not only using 
open source, but they are producing open source. So they have to believe and
know their the way in and out, right? That's really cool. Um, and when you're 
looking at these different clients that you worked with, right? You said Docker, 
you said Gatsby, and they're all open source.
Do you still see that there are a lot of differences in terms of how to develop 
software or is it all same, same, right? Is it because it's open source it has 
a similar mentality? Um, how software is developed, how people collaborate, how 
people interact, you know? 

**Chris:** [00:05:16] Oh, that's like, to me, that's like such a big question.
Uh, I could probably talk about that for an entire podcast episode again and 
again. Um, yeah, I mean, there are similarities and there are differences 
right? There, there's similarities in the sense that like they're open source 
projects. So there's the feature of like having a community around it. Or having 
users, um, I don't necessarily consider those to be the same, right?
You can have users of an open source project without having a community, right?
And you can have a community around an open source project that doesn't, 
uh, sort of like feed into your business. You have to think about that whole 
system as a whole system, as opposed to being like, "Oh, we're just gonna throw 
some code up and GitHub and like, yay, we're an open source company now."

**Michaela:** [00:06:00] But isn't community also ecosystem because somehow if
I'm thinking about open source and I think about a Gatsby or also what
WordPress, for example, I think there is also not only communities also
ecosystem, right? So that building, people are building upon your stuff. Um, do
you see that there are two different things?

**Chris:** [00:06:16] Yeah, I think there's, there's sort of like two 
different approaches in my head. There's the sort of competitive approach to it 
and there's the collaborative approach to it. Um, and then sometimes they're 
mixed up in the same company, right?
Um, but when you talk about ecosystem versus community, I think it's a 
community when you're all working together. Um, and you feel like there's enough 
space in the pie for everybody to take a slice and continue forward. Um, and 
realistically, I think that's the better option in the long-term. Because the 
companies that I've seen take the competitive approach with their ecosystem 
itself, in which case I wouldn't consider it so much of as much of a community.
Um, they end up sort of like not doing as well because people are worried about, 
"Oh, if we do this, what will they do, right? If we build this, will they launch 
their own? And then what do we do at that point?" Whereas like, if you're more 
collaborative, as you generate these software projects and work with your 
ecosystem, you end up having a community that reinforces itself and grows,
right? 

**Michaela:** [00:07:18] And I mean, I don't know if this is, um, too 
confidential or you don't want you to talk about it, but could you give some 
examples of open source projects that are more community driven versus some
that don't have a community or that are more ecosystem driven?

**Chris:** [00:07:37] Sure. Um, I feel in some ways that, uh, like Kubernetes is 
almost an ecosystem driven, uh, environment. Um, I'd probably placed that more 
on Docker being ecosystem driven than Kubernetes, but Kubernetes also has a 
strong sort of ecosystem around it. Um, there's also a lot of community in 
Kubernetes. So if you're looking at like a place where both exists, that's a 
place where both exists.
Um, I think that Docker took more of the ecosystem approach and was probably a 
little bit more competitive than a cooperative, in general, but yeah. And then 
you start looking at the other end and you start looking at like, who's really 
community driven and you look at Vue, right? And you look at Rust and those 
feel very community driven, right?
Um, when Rust succeeds, everybody succeeds, right? When Vue succeeds, 
everybody succeeds. Um, when Docker succeeds, not necessarily everybody is 
succeeding. 

**Michaela:** [00:08:31] Okay. And so how do you think that what's, what's the, 
what's the core to that? That you know, if we have, if you build something, 
how can we make sure that if one succeeds everybody succeeds, I mean, this is 
such a nice, um, way a mindset, right?
That we can strive for, but what are some of the things that we can do actively 
do to get to that point? 

**Chris:** [00:08:54] Yeah, I think that falls back onto the idea of, are you 
going to be cooperative with people or are you going to be competitive with 
people? And there's a lot there, there's a very interesting dynamic that we
will probably get really, really deep into.
Um, but I won't get too deep into that is like the VC funding and open source 
startup dynamic. And that kind of like forces you into this competitive nature 
because you often feel like, um, as somebody who has taken this money that you 
need to win, right? Uh, and sometimes that crosses over or often that crosses 
over into, I need to win at the cost of other people.
And when, in reality we think of software. And if you, if you've read books like 
working in public and whatnot, you understand that like, if you were taking milk 
from a cow or like trees from a forest or something like. Sometimes those are 
renewable, but they're kind of finite, right? Like there aren't infinite amounts 
of trees and there aren't infinite amounts of cows.
Um, but there's almost infinite amounts of like the ability to download a copy 
of the software, right? Like if I download the software, it doesn't prevent you 
from downloading the software. So there's a sense of where this like competitive 
versus community, uh, dynamic plays out on almost every level. Um, and it's 
fundamentally informed by the way that software works and like software 
distribution works.

**Michaela:** [00:10:12] Okay. Yeah. Well, this brings me somehow also to your 
community, because I feel that your community is really awesome place to be in. 
Um, it's called Party Corgi. Yeah. It's a platform. It's a community for 
creators. That's how I would describe it. But, um, maybe you can go into more 
detail. What's your vision with it?
And what's, you know, what's the heart of this community and, why do you think 
what's, what seeds did you plant and what are people doing in this community 
that, you know, people are feeling so welcome there? 

**Chris:** [00:10:46] Um, I think it comes down to a number of different things. 
I've thought a lot about why, why people feel welcome here.
Cause I've heard that from a number of different people. And, um, I don't know 
if I would say that it was necessarily intentional, uh, that that happened. I 
think that when, when other people look at what I did and they're like, "Oh, 
obviously it would have ended up like that." And I looked at it and I kind of
go like, okay, I didn't know it was going to end up like that.
Um, I hoped it would end up like that, but, uh, like, do you really know when 
you're starting something? Uh, not really. And like Party Corgi started as, um, a 
smaller, like, not really grandiose vision, right? So I guess, let me backpedal 
a little bit, and like Party Corgi is a community of creators engaging in a 
community of practice.
And what that means is that it's a community of people who are, uh, engaging in 
the practice of a thing, whatever their thing is. Uh, often it's content 
creation, it's blogging, screencasts, Egghead videos, things like that. Um, 
sometimes it's just regular engineering work or design work or something like 
that.
Um, we have channels, for example, for JAM stack and serverless, we have channels 
for content creation and newsletters and, uh, doing like an indie hackers 
product business, right? Um, but then we also have people who are, um, doing 
music or baking or growing plants and things like that. And those channels work 
in the same way, where they're about the practice of like caring for your plants 
and sharing pictures with them.
Uh, pictures of them, sorry, with, uh, other people and, um, like showing what 
you've cooked and sharing your recipes and like, And it's this idea of the 
community of practice, where there's a big group of people that get together for 
a common purpose and support each other through that purpose. And that is sort 
of what Party Corgi network is to me today.
Um, it is a housing that creates shared infrastructure that supports these kinds 
of, uh, communities inside of it. 

**Michaela:** [00:12:43] Yeah. One of the things that I'm just, I'm writing a 
book about code reviews, and one of the things that I really stress in my 
code review workshops for example, is that if we are interacting, collaborating
with each other, that somehow we have a framework of rules.
Um, also about our behavior and you know, what is accepted and what isn't 
accepted. And so I'm, for example, also advising people to have a code of 
conduct for their code reviews, right? So that people know, well, this is the 
kind of feedback, or this is the kind of interactions that we want. Um, so, what 
I, what I also see with communities very often is that it's really important 
that we have such a very stable framework that we know, you know, this is how we 
are expecting to behave with each other.
And this is also the consequences if you are not, if you are not following the 
rules, right? Because rules without any consequences, are somehow just air. Um, 
what's your vision for the that? Do you have, do you have like community roles, 
uh, for your Party Corgi, Corgi community? How do they look like, have you 
thought a lot about that?
Um, what's your take on that? 

**Chris:** [00:13:47] Uh, so we do have a code of conduct and it's enforced, uh, 
very firmly when it needs to be. A lot of the wording and the mechanisms through 
which the code of conduct, uh, was drafted up, comes from the community 
covenant. Um, and I believe the domain is lgbtq.tech has another code of conduct 
that we sort of looked at, evaluated, and took some stuff from, to add to the 
community covenant and like code of conduct are great and all, um, but there's 
like the phenomenon of missing stairs, um, which I can give you a link for, if 
anybody wants to read more about that, where there's basically people in the 
community who hold positions of power, but are not necessarily at the edges
visible to be a problem, but very close to them. If you're working close to
them, you recognize them clearly as a problem. And then it's sort of like
really hard to get them out because they are, they hold some position of power
that nobody else wanted to take. And then people are like, "Oh, but they're
doing this and nobody else wants to do that, so we can't really get rid of them
cause they're like a pillar of the community or whatever." And like that's a
really hard situation and you have to kind of get rid of those people. Or like
get them to modify their behavior, which is something that we've done fairly
well in Party Corgi, I think, like when it comes to enforcement, we do things
publicly as much as possible because I firmly believe that every action that
you take, uh, with something that is like a code of conduct violation or 
something like that, or something that could be grown into a code of conduct
violation is a communication with the people who are lurking in your community,
right? So the only way that you have a conversation with people who don't 
participate daily in conversation is for them to see what actions you're taking, 
right? So the actions you take have to be very clear and public and firm, uh, in 
many cases. And if there needs to be follow up discussion with a particular 
person, I'm happy to do that in private, right?
Because I'm not looking to publicly shame somebody for making a mistake. If they 
really don't understand and they really want to get better, I'll take it to DMs 
with them. Uh, after we've made the statement publicly about, "Hey, this is not 
okay because: x, y, z," um, and then we can take it to DMs and I'll go, 
"Okay, this is why, and this is how you can fix it."
And, um, that's worked out really well. Um, being sort of like very publicly 
firm about, "Hey, this is the community, this is what we want here. Um, if you 
don't want this and you don't want to participate with these rules, then you can 
go somewhere else, then that's, that's fine."

**Michaela:** [00:16:18] Okay, so if we feed that back into software development and 
collaboration, right?
So writing software together now you're very experienced in the open source, so
maybe having also some open source perspective here, but how can we feed back 
those learnings how we actually build a healthy community? How can we feed that 
back into, you know, software collaboration? How can we feed that back in our 
interactions that we have when we are building software because somehow I feel,
especially for community, somehow it's much more explicit, right? Every
Facebook community that you are entering into, or a lot not every unfortunately,
but a lot have at least some, you know, some rules of how to behave that you
have to, you know, adhere to.
But now in software development, even, um, starting at the new company, it's I 
think less direct. Yeah, definitely have something. And maybe you have an 
employee handbook, but who reads it? Who enforces it? How do we behave? Right? 
There are, I think there are a lot of power struggles happening daily in all of 
the offices and places and remote work and whatnot, right?
All over the place. So how can we take those learnings from community 
building and to bring them into our day to day work life?

**Chris:** [00:17:31] Yeah. I mean, I think that, um, when it comes down 
to it and you talk about open source and community and like the Party Corgi 
network, uh, community, those are basically the same thing, right?
Um, and if you look at the way that Rust runs their community, uh, is a 
pretty good example of like generally speaking, how to do things. There, there 
was a talk recently that I watched about how Rust handles their community, 
called something like, "Why wasn't I consulted?" was the title of the talk and it 
goes over like, uh, how different groups are set up to own different pieces 
of the Rust of community, for example.
And it's very similar to the way that Party Corgi has different people owning 
different channels and responsible for different sub areas of the community, 
right? And like Rust is far, far, far bigger, so they're further along and
developed. Um, but I truly believe that, like if you're trying to build a group
of humans together, uh, working towards common purposes that this approach of
that I took with Party Corgi and whatnot is the same approach that you need to
take with open source is the same approach that you needed to take with your
business. Uh, if you want this to be a positive thing going forward and
self-reinforcing, right?

**Michaela:** [00:18:42] Okay. And so if you could summarize it, what is that 
approach? So what can we take and how can we take it then? You know, what's the 
ingredient for that? What's the recipe?

**Chris:** [00:18:55] Sure, um, so, I guess in the early days, like show up and
show the values that you want in the community, right?
Like, um, the, like me as the first person, um, I had to do the things 
that I wanted to see other people do, and then people will self select in and 
out of that. Uh, as they see you doing things, and I think that's when it comes 
down to it, that's the most important thing. You have to be very conscious of 
what you are doing and the behavior that you're displaying.
Um, and how that influences other people to act. Because for example, um, as a 
leader of the Party Corgi community, if I do something, it carries a lot of 
weight, right? If I come in and I say, "No, that's not okay," um, there's a lot
of people that will not contest that, right? They'll just say, "Oh, this is how
this community operates" not, "Hey, Chris, maybe you fucked up here and maybe
you shouldn't, uh, shouldn't have done that and should have done it a different
way." Um, there's not a lot of people who will do that because I represent, uh,
what a lot of people view as the community, as one of the people who started it,
right? Um, so I think it's super important in, in like the primary takeaway I
would, I would to take away is that the things that you do as the person who 
found the community or the company or the project will influence how people act
for the rest of the existence of the community?

**Michaela:** [00:20:16] Okay. And so do you have also some, this is somehow if 
you are really in a position of power, right? We are the creator. We are maybe 
the startup founder or early employees or something. How can we do that as an 
employee in a larger organization, in something that we know has already its
own pace, its own culture, its own, you know, makes and makes off different
things? How can we instill a little bit of this, what, calmness in our own team,
or is it sometimes just that we have to be, um, can we actually trigger some
changes? I don't know if you have some experience with that, uh, working with
different communities that you are not a leader of, but that you're entering in
and you're, you're thinking, well, how can we, you know, change maybe a little
bit or put it in the right direction?

**Chris:** [00:21:05] The answer to that is that, uh, if you don't have any 
power in a situation, like a company or whatnot, you probably aren't going to 
affect much change. Um, so if you're going to try to affect change, you either 
need like collective action. There have been, uh, things like petitions at 
companies and, uh, sharing salaries and spreadsheets and things like that, 
right?
Like if you really want change, you need, uh, a lot of collective action to 
compensate for the power that you individually do not have, but as a group you 
have, and like, if you don't have that and or you don't have the ability to get 
that, and leadership is not in a position to want to give that power to people,
cause that's what they have to do for change to happen, um, then you have to 
leave and go somewhere else or you will spend your entire time there fighting 
this fight or fighting this fight and you will burn out and I've seen plenty of 
people be like, "No, I'm going to fix this from the inside." Um, and then that 
results in burnout because they care so much, they put so much of their energy 
into it, tt takes over their life. And then a change doesn't happen because the
people with the power don't want it. 

**Michaela:** [00:22:14] Yeah. Yeah. Oh, um, that's very depressing, but yeah. 
Yeah. I agree. I also think that it's a, yeah, it's really hard if, if you are 
not having any power to do anything, but I also think that maybe in the little 
we can change and influence a little bit, the people surrounding us, right?
It could be our colleagues or our, our inner. Maybe our manager that manages 
us, we have some conversation and we change it a little bit, the perspective 
of, of the people. Um...

**Chris:** [00:22:52] Yeah, for sure. 

**Michaela:** [00:22:54] So, what I wanted to talk with you about also is so for 
engineering practices, and I started a little bit with that.
Um, so when you coming into this project, right in these startups, what about 
the software engineering practices that you see? What are some of the things 
that you, as an independent consultant bring into that, and maybe that has again 
to do with, uh, with, with, with power and a little bit, like what can you 
influence and what can you just, you know, except as, as it is, right. If
you're going into, you know, a new work arrangement, um, and you see that some
of the practices are not done in the way that you would like them to, to be
done, uh, can you, do you feel that you can change that? Do you try to change
that? Um, do you adopt to the processes over there and in general, how diverse
are the processes that you are seeing?

**Chris:** [00:23:46] Uh, it depends a lot, right? Like, um, for example, if 
somebody is using, I'm not going to name any video production software, but like 
if somebody is using some video software to have their meetings that is awful 
and preventing their teams from communicating effectively and whatnot, um, uh, 
maybe like maybe I can suggest something new, but probably not, right?
Like probably the situation is going to be that the company that I'm 
working with already has established practices for the tools that they use for 
communication. And like telling them to move from Slack to Discord is a 
nonstarter, right? They're just not going to do that. Um, so there's things
that you have to adapt to, and there's a lot of those as somebody who comes in
as a third party, right?
This is not a, um, like I will come in, I will give my expertise in certain 
areas, technical or community based or whatnot. Um, and they will either take my 
suggestions or they won't, but they are paying me for me to tell them what I 
know from my expertise and years of doing this, and if they don't take that 
advice to do it, uh, there's nothing I can do to force them to, right?
That's not my job and that's not what they're paying me for. And, um, you know, 
that's kind of like, like you said before, maybe it's a little bit depressing 
where like you see problems and then you can't fix them. Um, but there is a 
certain level of, uh, when people pay you as a consultant to come in and share
your expertise with them, uh, there's a different level of respect that I've
seen compared to being an employee. Um, where I could say, like, I can use my
power as a consultant because people are paying me for my expertise and if an
employee says something and I'm like, that is the right thing to do, I can
repeat that and sort of like raise their voice to the level of the people who
are listening, right?

**Michaela:** [00:25:43] Amplifying that. Yeah. And so how do your contracts 
look like? Are they like long term or you're just going in, you know, for a 
couple of hours consulting on one specific topic, or do you, you know, are you 
with the company for several months and help them on an ongoing project or 
something like that?

**Chris:** [00:26:02] It depends. Definitely, um, there's work that it doesn't 
make sense to hire me to do, right? Like the, um, if you just want a couple of 
buttons created on a site or like some CSS written or, um, like a, a one off, 
uh, CI pipeline built or something like that, I'm probably not the best person
to do that because my rate is not commensurate with that work, right?
You probably want somebody who is a bit earlier in their career who maybe 
has a little bit less experience, um, who needs to gain some experience to do 
those. Um, so I'll come in, uh, and like advise on a JAM stack adoption, uh, 
process, right? Like this company wants to move their sites from whatever 
they're doing to more of a JAM stack approach to simplify their DevOps pipelines 
and things like that.
Um, and I can give a lot of advice around from, to get them from where they are, 
to where they need to be. Um, and that can come from just like a one hour 
conversation all the way to like, Here's a week and I will come back with a 
written document about here are all my suggestions on what you need to do to get 
it from here to there.
Um, and this is the business value that you'll get out of that. And then they 
can make the decision informed now about whether that's the right move or not. 
Um, and then there's a longer term contracts, right? So the work I did with say 
Gatsby, for example, uh, they wanted me to actually do work on their community 
and their, um, uh, open source project and things like that.
So I was writing code and doing, and doing user research and working with the 
community to, uh, bring Gatsby Themes to life. And some other things like
gatsby-plugin-mdx, um, and that is a longer term R&D project. Uh, so that was 
framed more as a retainer than a, um, like short term project. 

**Michaela:** [00:27:50] So, I think what is super interesting for me and for 
many of them and listeners, I guess, is how do you get started with that?
You're a little bit outlined did that you were actually already freelancing in
your early career. Then you went to work with some of the startups and some 
companies, and then you went back to, uh, independent consultancy work. So what 
would you advise somebody that wants to, you know, get their own things, start 
their own business.
Maybe not the same thing as you did, but in the software engineering, you know, 
in the software engineering area, what are some good ways to maybe get exposure? 
Um, I think I heard you saying once, uh, be visible and people will come to you, 
but, hmm, how, how does that work? How can we, you know, how can we achieve
something like that?
How can we even kickstart it, get the foot in the door.

**Chris:** [00:28:41] I think that, um, people, uh, grossly overestimate, the 
amount of writing you need to do on the internet to be perceived as an expert in 
a field. The truth is that most people don't write about stuff. Uh, so with, say 
three to five well-written blog posts, you can be a visible expert in a specific 
field that you want to start freelancing or consulting in, or, uh, however you 
want to approach it, right?
Um, and that's, that's really my advice. Um, I will caveat that with say 
I got my start like 10 years ago, right? So, um, yes, I know that this works, 
uh, I've seen people do it today. Um, but keep in mind that I started a long 
time ago. Um, and I've been doing this for awhile, so like, my advice for 
getting started today might not fit your exact situation.

**Michaela:** [00:29:32] Yeah. I mean, I see it today. I see it quite often when 
people are writing, you know, 10 blog posts and they have like 10 people 
visiting the blog post, right? So it's definitely not something that you can 
easily rank. Maybe you have to push it from, uh, a few other sites as well, right?
I don't know, maybe some direct connections that you can interact with, right?
People that you worked on before, or, you know, um, having some, some personal 
network that you can activate to get the first one, two clients or something like 
that. Um, yeah.
**Chris:** [00:30:01] Networks are super important. And, um, I think 
that that's something that like, when people talk about like grift Twitter, uh, 
that's one of the things that is the problem, right?
Cause people say something similar to what I just said, and they're like, "Just
write three blog posts and you're good!" Um, and I want to be clear that that's
not what I'm saying. You can write three to five blog posts and like you still
have to have either a network or an audience or something like that, right?
Like people still need to see those blog posts.
Um, and you need the right people to see those blog posts and to do that, you 
need to build up your online presence and, uh, whether that's Twitter or
dev.to, or any of these other platforms, um, or your own site, right? Which is
a harder, but, um, better path in the long run. Um, like it requires a lot of
work to, uh, do this.
And also like those three to five blog posts that I was talking about aren't 
necessarily going to be your first, right. Like writing is a skill, uh, and 
marketing is a skill. So if you're going to jump from pure engineering work, as 
I see to doing consulting, okay, maybe you already know people that you can get 
your first clients from, um, which is great, right?
But if you're going to take the approach of, I don't know who would be my 
clients and I need to find some and generate that interest and be public about 
it. Um, the three to five blog posts that I was just talking about are not going 
to be the first ones that you write probably. Um, you're probably going to write 
a lot.
You're probably going to have to learn how to write and you're probably going to 
have to, after you learn how to write, learn how to market yourself and market 
your blog posts and market your expertise, and then you're going to learn how to 
like price things. Like eventually you're going to have people coming to you and 
you're going to have to learn how to like set up contracts and price things.
And like, what does a good client look like, right? And you don't figure out 
what a good client looks like until you've had five to 10 of them, right? 

**Michaela:** [00:31:53] Yeah. True.

**Chris:** [00:31:54] Like it's, it's easy to recognize a really bad client,
right? Um, and if you're trying to get into this one thing I'll remind people
of is that like, uh, whereas you can't really fire your employer, you can fire
a client.
So if they breach the contract, uh, the contract is over, right? If either side 
breaches it. So it's much more of a equal partnership as opposed to some kind of 
an employee-employer relationship where you can't really fire your employer, 
like you can quit, but, it's not quite the same thing. 

**Michaela:** [00:32:23] Yeah. Well, I totally agree.
I think blogging and, you know, social, having a social media presence is really 
important, but there was a lot, as you said, I guess a lot of work in it. It's 
not done with the three, five blog posts. Um, it's really hard to, to, um, get 
people to look at those. Uh, but on the other hand, I think there are, there are 
many, many benefits that when once you're getting into that rhythm, right, 
you're understanding how the community takes, how to, as you said, market 
yourself, how to write, how to demonstrate your expertise, right?
This is really, then it really becomes something very, very valuable. Um, 
something that I somehow, uh, regret, I regret is really a strong word, but I 
don't have a better English word for it, uh, right now, um, is that I haven't
started early enough, right? So I could have, you know, demonstrated my
expertise, shared with the world already while I was employed.
Um, and that, I think this is such a smart move, or why do you are a student or 
at the boot camp or whatnot, right? So this working in public and, you know, just 
sharing what you're learning in public and with the, with the world, with the
inter-world, right? And with the internet, I think that's such an important
first step because it's, it's very low hanging fruit that you can do, right?
It doesn't have to be the best, um, article. You don't have to have a niche, yeah
you just write about what you learn because you're learning, as you said, you're
learning so many skills. You're learning to write. You're learning how to publish
that. You, um, have first figure out where do I have my blog, right?
We have it on my own domain, write on dev.to, or whatnot, right?
There's so many different options. So you get a little bit into that, um, uh, 
thinking and, and build your thoughts process around it. And you're getting 
skills from that. And maybe you just do it once a month. It doesn't have to be 
every week, or, you know, I think sometimes people have these very high goals 
that you want to achieve.
Maybe it's only every three months. I see even, you know, online presence is 
where people have two or three nicely written blog posts per year, but because 
they are doing it like, you know, how fast two years go buy right? Or three 
years or five years. And then you're having something that, um, people will get 
to know you.
Um, and you're, you're getting your skills a little bit. So I think really 
starting early, as early as possible is, is one of the best things people could 
do. Um, yeah.

**Chris:** [00:34:54] Yeah, I totally agree with that. Um, I think that when we start 
talking about like, what do you actually need, um, to be like recognized as an 
expert, if you're trying to produce content or whatnot. Um, and if we, if we 
talk about this, like three hypothetical three to five blog posts, um, like 
getting started doing that while you are stable and employed and, uh, have an 
income, is the, is one of the most powerful things you can do, because then you 
don't need a client.
You can do this until you figure out how to do this. Uh, and then when clients 
come to you, you can be like, okay, is it time now for me to quit my job and go 
do this, or do I want to do this half time or quarter time with like a client to 
test out what it's like, right?

**Michaela:** [00:35:39] You can also wait for the good client to come to you.
Right. So before I started my business, I was really waiting for the clients 
that I want to work with. I didn't, you know, take on anything, but really what 
I wanted to do, what I thought did I have a lot of experience with. Um, and so I 
actually sit out, I think, hmm, nine months, um, to just have this client, you 
know, where everything was ready. I could have taken on smaller projects as much 
projects that I'm not that interested in or project that doesn't fit so much 
into the path that I want to go, right?
Because I think one of the most, that's why I asked you about your niche. 
I think one of the most or biggest mistake is to be, you know, everybody's 
darling or, you know, um, you know, the expert for everything, right? Oh, you 
want to PHP website oh I can do that, right? Oh, you want something with the 
JAM stack?
Like, oh, I can do that, right? You want some graphic design? Oh yeah, I can do 
that, right? Um, and I think, I think it's very easy to, to get into that. 
Especially if you need money or, you know, you need some clients, but I don't 
think it's the, it's the right approach. Um, it's much better if you're in a 
position where you can say, well, "What are the projects that I really want to 
work on? What is the expertise that I can bring to the table?" even if you
don't have it at that point, or just getting, you know, you're starting it.
Let's say you're starting with JavaScript. That's your thing. Then don't take
on something that's written in Python, right? Obviously, you can do it, uh, but
it's really hard to be competitive in that.
I mean, because you have to get the knowledge, you have to get up on speed,
right? So, uh, whatever you're charging them, uh, you will take more than the 
hours, probably, especially if you're new to that, because you feel like, oh my 
God, it takes me now 10 hours to do something that should be one hours. I 
charged him two hours.
Uh, but you still, you know, you spend 10 hours doing it. Uh, but if you're 
really good at, let's say JavaScript, then it takes you half an hour. So that's 
awesome, right? 

**Chris:** [00:37:39] Yeah. And I think that connected to that, there's 
something, um, about where if you're an employee at a company you're not an 
employee for no reason, right?
You're an employee because you're providing business value that is greater than 
your salary to the company that is paying you. And if you figure out what 
that business value is, you can turn that into freelancing and consulting and 
whatnot, right? But you have to understand it from like a business perspective 
and a business owner perspective.
Like what are you going to do to create more value than you're going to charge 
them and do that in an obvious way? Like, obviously I am creating this value for 
you, therefore you can pay me a subset of it. 

**Michaela:** [00:38:19] Yeah. Yeah. And I think it also, if you're thinking 
about hours, right? Hours is really easy to get started with.
Like I'm putting it in that many hours and you're paying me the same 
amount, right? Um, but if you're, if you're able to go away from that and say, 
as you said, this is the business value, right? Let's say a website, that's the 
value of the website that you will get with it, or a performance increase
from your website or whatnot, right? So whatever you're offering and you, and 
you can put a number to it, and hopefully this number is larger than the hours 
that will you spend doing it, right? That's, that's what we want, I mean, I
think that's, that's somehow, um, the right, the right approaches for, for what
we are working in it, but yeah, anyway, I think we rambled a little bit here.

**Michaela:** [00:39:06] I actually started reading with software engineering 
and practices. So I tried again last time. So, um, now you told me a little bit 
that you're consulting more, for example, if people want to go to the JAM stack. 
So then you're looking through probably technologies that they have there.
Um, and, and, uh, make some estimations on how much time/effort, uh, how much 
friction they will have, how much pain they will suffer, you know, uh, once they 
are getting over something like that. Um, do you also look at their software 
engineering practices? Like if they're doing testing or if they're doing code 
reviews and things like that and advise them on that, or do you leave that out?
Is that, um, nothing that's really connected to the kind of consultant, um, 
consultancy that you do.

**Chris:** [00:39:54] I mean, it's, it's, you can't take it away, right? 
Like if you're going to transition from one set of technologies to another, and 
this is like a broad approach change for you, um, you can't take away the fact 
that like, you're not doing code review or you don't have tests or things like 
that, right?
Um, there's this concept of like don't deploy on Fridays, right? And I 
think that the, the nuanced version of that is, uh, don't deploy on Fridays if 
you don't have the infrastructure to, uh, ensure that when you merge on a 
Friday, that the code can go out safely, right? That's kind of like the full 
thing, uh, you should be able to deploy on a Friday, right?
You should have the infrastructure set up such that if you merge code on a 
Friday, it should be able to go out and you should have a reasonable expectation 
that it's not going to like crash everybody and ruin everybody's weekend, right? 
Um, if you don't, then don't deploy on the Friday or don't merge on a Friday, 
even, right?
You shouldn't be merging code that you aren't about to deploy. Um, but like 
that's all intertwined, right? Cause if you want to move to like a JAM stack 
based approach, one of the things that that, um, does for you is it decreases 
your operational load, right? If you move from a server side rendered 
application to a JAM stack approach, now your problems happen at build time 
instead of at runtime on a server, right?
So, if something goes wrong with a server you wake somebody up. If 
something goes wrong with a build everybody wakes up tomorrow morning and goes, 
"Oh, why did the build fail? That's weird." And then you fix it, right? So like 
the practices of how you develop software and the approaches that you take are, 
uh, very much intertwined.
Um, and they're very much sort of like if I come in and somebody wants to move 
to the JAM stack, there's, uh, a whole assortment of that kind of stuff that I 
will definitely, uh, include in my report as it were, uh, if they are having me 
do sort of like a week long report or something like that. 

**Michaela:** [00:41:55] So, are there ever a situation where you say don't do it?

**Chris:** [00:41:59] Yeah. Yeah. Um, somebody, uh, uh, hired me and they were 
like, we want to move to, we want to move to Gatsby and we're going to rewrite 
our application to do that. And we're rewriting into serverless. And, um, I 
looked at what they were doing and it was sort of like, okay, so you're going to 
rewrite your backend into serverless and you're doing that already.
And you're committed, great. Um, Do you know, anybody that uses React at your 
company and they were kind of looking at each other and they kind of like, uh, 
not really. Um, and I was like, maybe start there, right? Like if you can't 
like, don't just jump into a JAM stack meta framework, like Gatsby, or Next or
there's something, if you don't even know anything about React, right?
Um, you're gonna get yourself into a situation where like Gatsby is a complex 
system, right? It's not simple. So is Next. So are all of these meta 
frameworks. They're not cheap, uh, from a, uh, like ex- like energy expenditure, 
uh, view, right? You, you need to know a lot to work with them and if they go 
wrong, you need to know a lot about the internals to debug them.
Um, I feel like that's a situation in which I was sort of like, well, you 
probably shouldn't do this. Like, if you really want to do this, like you can 
pay me to help you figure out how to actually move forward, but this is going to 
take a lot of work and you're already doing a rewrite for half of your 
application.
Like don't take on a second rewrite when you haven't finished the first one. 

**Michaela:** [00:43:24] Yeah. So one of the, exactly that, was in my mind all
the time I was thinking, well, one thing is to look at the technology, right?
But on the other hand, people have to have the expertise to use that, right?
And this is really expensive to also get that, um, in your company.
I know that for example, outdated stacks, tech stacks can be really a 
motivational killer, as well, right? So that you're not attracting talent and 
that your talent that you're having is not really happy and, but on the other 
hand, if you don't have the expertise for taking on something like that, it's 
it's yeah.
It's really, it's really a very hard and very terrible problem probably to have. 

**Chris:** [00:44:04] Yeah, for sure. sort of mired in legacy software that you 
built five, six, seven years ago. Now, I guess like somebody could have a 
Backbone application right now, right? And a Backbone like pre-Marionette 
application, which, um, it doesn't really matter what that is, but like that's a 
six, seven year ago, tech stack, right?
And if you haven't moved off of it by now, you're probably not going to. 
Yeah. 

**Michaela:** [00:44:28] Yeah. True. And probably it's okay. I don't know.
Maybe they don't have to? 

**Chris:** [00:44:32] Clearly your business is still running seven years later, 
so like, does it really matter? 

**Michaela:** [00:44:37] Yeah. Yeah. Well, I have a friend just comes to my mind 
that I'm a friend to the study with me and I think it's been. yeah, almost 20 years, 
he's, he's hacking, um, mainframes, I'm like, wow, you're still doing that well,
and it pays the bills and they're not going to change it. 

**Chris:** [00:44:56] Yeah, people still run mainframes!

**Michaela:** [00:44:57] Yeah, it is. Yeah. Well, I think we are coming to an end to 
this episode. Is there something that you think we haven't really touched on or 
that you would like to, um, let my listeners know maybe something about your 
community or, um, yeah. 

**Chris:** [00:45:13] Sure. Um, uh, the community is at like discord.gg/party 
corgi.
Um, We're doing a lot of Rust recently in the community, which is pretty 
cool. Um, so if you're interested in that kind of thing, uh, come say hi, and we 
can talk about that. Um, but we would love to have you around in the community.

**Michaela:** [00:45:31] Yeah. Because you're saying Rust I have one 
more thing to talk with you about, uh, I completely forgot about that.
You are working on some really cool new stuff, right? One thing is called Toast. 
Like bread toast.

**Chris:** [00:45:45] Yeah. 

**Michaela:** [00:45:47] It's actually like SpongeBob, but not the sponge for 
the toast. That's how I envision it somehow.

**Michaela:** [00:45:53] So what is that? Maybe, maybe tell us a little bit 
before, before we end this show about, about Toast and what it is and how it's 
connected to Rust and to you.

**Chris:** [00:46:04] Sure. Um, so I, uh, accidentally I say I accidentally fell 
into this specialty of JAM stack meta framework development. Um, so I built the 
prototype of a JAM stack meta framework that used graphQL to do static site 
generation, uh, that influenced Gatsby to add it to their framework. Um, and 
then I worked on Gatsby for a long time, uh, and, uh, some other frameworks and 
whatnot.
And then this is my, sort of like a total rethink of, okay, so what if we didn't 
use Webpack? And we went with ES modules, cause those are available now in the 
browser. What does that look like? Um, and one of the focuses is on performance 
and build performance, specifically. Um, and that's where Rust comes in because 
Rust has libraries that will let us do incremental computation of the build 
artifacts, right?
So that is a super exciting thing. Um, I got that working last week, so 
yeah. Uh, we built a 4,000 page site in 13 seconds, which is pretty cool. So 
that's where Rust comes in and I really like writing the language and it's a 
lot of fun. Um, and it's, it's brought some joy to my life that is, um, has been 
missing from other projects.
So I'm super excited about Toast and specifically the Rust implementation. 

**Michaela:** [00:47:22] Yeah. Very cool. Yeah. Thank you so much. And, um, 
thank you for being on my show and have a good day.

**Chris:** [00:47:30] Thank you for having me. It was really enjoyable.

**Michaela:** [00:47:32] Yeah. Bye bye.

**Chris:** [00:47:33] Bye. 

**Michaela:** [00:47:36] I hope you enjoyed another episode of the Software 
Engineering Unlocked podcast.
Don't forget to subscribe and I talk to you again in two weeks. Bye.


