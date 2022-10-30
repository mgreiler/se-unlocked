# Transcription

[00:00:00] **Dr. McKayla** Hello, and welcome to the Software Engineering
Unlocked podcast. I'm your host, Dr. McKayla and today I have the pleasure to
talk to Jess Rose. Jess is a technology professional and keynote speaker
specializing in community building outreach and developing better processes for
talented technology. She is passionate about fostering more equal access to
technical education, and digital spaces.

But before I start, let me tell you about an amazing startup that is sponsoring
today's episode
[Mergify](https://www.mergify.com/?utm_source=social&utm_medium=podcast&utm_campaign=SeUnlocked).
You know, I'm all about code reviews and pull requests. Having your teammates
review your code can be super beneficial, but it also can create a bottleneck
and slow down your software development. With Mergify, your team can be way more
productive with GitHub. Mergify automates all about merging pull requests, you
can specify the merge conditions, and Mergify will take care of the rest. Do you
want a specific order for merging the pull requests? Should one PR be
prioritized? Or do you need a copy of the PR and another branch for bug fixing?
No problem. Mergify can take care of all those situations. By saving time, you
and your team can focus on projects that matter. Mergify integrates completely
with GitHub and your CI pipeline. They have a startup program that could give
your company a 12-month credit up to $21,000 of value. Start saving time, visit
[Mergify.com](https://www.mergify.com/?utm_source=social&utm_medium=podcast&utm_campaign=SeUnlocked)
to sign up for a demo and get started or just click the link in the show notes.

I'm super, super thrilled to have Jess here with me. Jess, welcome to the show.

[00:01:38] **Jess Rose** Oh, gosh. And I'm absolutely delighted to be here when
you said hey, do you want to come and talk about teaching and learning? Oh, I'm
just going to be insufferable. Thank you so much.

[00:01:48] **Dr. McKayla** I'm really excited because I'm following you on
Twitter. And I see that you're creating spaces for people to learn to get better
to grow. Right. So there are a couple of things that I want to touch base on
today with you. One is the 1-1s that you're offering. So maybe, maybe let's get
started with that. Because I see you from time to time you say, you know, I have
some time available, why not hop over on a call, and I can help you with some
career advice? How's it going? What do you do with people? What kind of people
are you know picking up on that?

[00:02:27] **Jess Rose** So I've been doing this for about, I looked the other
day because I do, I do keep records and privacy-preserving records just like,
oh, what kinds of things am I talking to people about? And I've been doing this
for about eight years now. So just broke 1700 folks I've talked to over the
years.

[00:02:40] **Dr. McKayla** Wow.

[00:02:40] **Jess Rose** And you would think oh, it's going to be mostly juniors
or mostly people trying to break into tech. But just the absolute vastness of
experience is so dazzling and exciting and strange to me. I don't see myself as
especially well suited to give great advice. But on these calls, people are
almost never asking for actual advice. So a lot, most of it's just, I'd like to
be heard and I'd like someone to confirm that my experience is unusual or isn't
unusual. Or getting sort of a level check for a different area saying, Hey, I'm
based in this region, and I'm looking for work in your region. What's that like?
What's the experience like? What's the process like? I actually documented the
whole process out because I want, I definitely want other people to be doing
this if you feel like it. No pressure. And it's on my GitHub. So
GitHub.com/JessicaRose. And it should be right on there as 1-1s.

[00:03:37] **Dr. McKayla** Yeah, I saw that. I saw that on your Twitter feed. So
it tells us how to do those 1-1s and how to, what questions to ask, and so on?

[00:03:46] **Jess Rose** Yeah. And mostly just about the tooling. So how to get
it scheduled, how to get that sorted? And then because I'm a weirdo, how to get
the records of who chatted to you deleted if you want to, like, yeah, I wouldn't
keep notes on somebody who doesn't want me to keep notes.

[00:04:00] **Dr. McKayla** Yeah. And I think it's good for privacy as well,
right?. If people I don't know which topics, they are coming to you, but I mean,
some of them might be private, and you know, especially if you're having maybe,
like, I think if you need advice, you're very often not such a good place,
right? Probably more than being in a great place where you think, well,
everything figured out, you know, things are going smooth than you're seldomly
reaching out to other people. It would be like I'm bragging now to you. You're
more probably reaching out if you have some problems with your team maybe or
getting a job or something like this. Is that what people talk to you about in
the sessions?

[00:04:41] **Jess Rose** So anything from, Hey, am I getting paid right? To, Oh,
I'm getting screamed at a lot at work. Is this normal? So a lot of them are sort
of, oh, gosh, but a lot of times folks just want to explore what's going on
next. I've managed people a lot in my career. And one of the things that I
always, I always have a difficult time with, and I hope other managers do, too,
is how do you deal with the conflict? And there's always going to be conflict
between what's best to the individual person you're managing, and what's best
for the company because those are those, And one of the big things I push when I
do manage people is, hey, do you have someone external to the company to give
you good advice when I can't? Or I shouldn't give you the advice that's best for
you?

[00:05:31] **Dr. McKayla** Yeah, yeah, it's a conflict, right? Because
obviously, you don't want to lose that person. But you see that they're
outgrowing, you know, maybe the position?

[00:05:42] **Jess Rose** Oh, I really just want to chase this up a minute. I'm
always like, you don't want to lose somebody, like, you don't want somebody to
move on for your team because they were unhappy or mistreated. This is
definitely from me being a teacher for too long. I'm always pretty excited when
somebody graduates up out of a team I run. Like, of course, you want to make
sure that people have space to grow, of course, you want to be actively making
sure there's career progression and more things to learn. But and especially in
a job market, like right now, sometimes people like oh, cool, I could make a
bigger salary jump, or I could make a bigger title jump by leaving. And I'm
always pretty chill with that.

[00:06:24] **Dr. McKayla** Yeah, yeah. Me too. And my husband is also managing a
bunch of people. And but I see tension there, right? So I think he's always
really behind the people. But then upper management would be, yeah, but you
know.

[00:06:38] **Jess Rose** The business case for retention.

[00:06:40] **Dr. McKayla** Yeah, exactly. Right. And the same for, for example,
giving your raise, right. And I think, especially maybe the managers, you know,
that are really like first line, they are more for the people because they have
like some personal relationship, and then one level up, it's already like, yeah,
but you know, we don't have the budget or we don't want or we believe we can
still keep that person, you know, for this for this cheaper?

[00:06:38] **Jess Rose** Oh, well, you know, let's give it another quarter or
two and wait and see.

[00:07:08] **Dr. McKayla** Yeah, exactly, right?

[00:07:10] **Jess Rose** Baffling.

[00:07:11] **Dr. McKayla** How do you do that as a manager? How do you speak up
for your, for your people, or for your team? And how do you deal with that
conflict as well?

[00:07:22] **Jess Rose** So I think that's a really challenging one because I
think that the conflict there is still the same. What do you do as an individual
manager when the yeah, when your contractual, your fiduciary duties to your
company, run counter to your individual ethical responsibilities to the people
you manage? And or what happens when there's a conflict between the needs of an
individual and the needs of a team? And it's not a good answer. And it's not a
reassuring answer. But it depends. If somebody is facing treatment that feels
unfair, or targeted, or they're in a position that I, generally, if somebody is
in a position I'm not okay with being much more lovingly strident around, hey,
this is a topic I would really bring to your external mentor as well, and then
setting really clear limits internally about what, even as a manager, you are
and aren't willing to do. So somebody saying, Oh, you get the idea that, Oh,
maybe we want to manage so and so out, go ahead and write them up for stuff that
the rest of the team routinely does. You still have consent as a manager. So you
could say, like, yeah, no, I won't work in a space that involves maybe this kind
of behavior.

[00:08:45] **Dr. McKayla** Yeah, yeah, I think this is really important that we
are standing up for our own ethics and for our own beliefs and value and, you
know, also behind our, you know, our people that we, you know, I think we have a
responsibility as well for and yeah, so I yeah, I can totally see that.

[00:09:05] **Jess Rose** It's easy to say in this kind of job market in the West
as well. I think, are you based perhaps in Europe as well?

[00:09:12] **Dr. McKayla** Yes. Yeah.

[00:09:13] **Jess Rose** Because, like, these days for many European job markets
in tech, finding a new job feels to many people who are established for juniors
or people getting your first job, it is hard. But for folks who've been in for a
little while, and folks in different in high demand areas, getting a new job as
a junior as a middleweight, or a senior, is not as difficult as it could be
these days. Whereas if you're having to engage in management behavior that
you're just not comfortable with, yeah, sometimes changing jobs is easier than
making peace with uneasy ethical decisions. Yeah, sometimes that's not true for
everybody. And it's a very, very privileged take for those of us who have a
little bit of wiggle room.

[00:09:58] **Dr. McKayla** Yeah, I think so. And it really depends on where are
you located? And what is your personal situation, right? Do you have dependents?
Do you have like family or people that you have to take care of? And so on,
which I think makes it much harder to say, you know, I'm going to not do that.
But I think there, you know, there are boundaries, it's, it's one thing is
playing along, and just, you know, or letting the other person also, you know,
know, in the space that you have, right? You’re also like, as a manager, you
also, you can't just go and, you know, give advice directly conflicting with the
interests of your upper management because that, you know, is a problem, but you
can, you know, talk a little bit about, as you said, maybe asking you an
external person, or also I think very well, you can say I'm disagreeing with
this decision, right? And I advocated for you, unfortunately, you know, these
were my boundaries here, for example, and let them know, I think that's, that's
perfectly fine. Yeah. And I think that the problem is that if more of those
things come together, people start thinking about leaving, right?

[00:11:06] **Jess Rose** And that’s not always a bad thing. As a manager, if
you're not able to offer someone, a place that is safe, and productive, and
non-traumatic to work, yeah, it's okay, that your people move on, and actually
kind of preferable?

[00:11:22] **Dr. McKayla** Yeah, yeah, I think so, too. So another topic that I
wanted to talk with you about, and it's a little bit related to management, but
it's more related to teaching. So I don't think you have to be a manager to
teach, right? You can be, you can be, you know, Junior Dev, Mid Dev, senior Dev,
right, so we can all learn from each other. But I really see you as a teaching,
you know, expert here. Yeah. Because you're, you're bringing topics around
programming, but also, you know, advice for hiring or you know, how to get
hired. And to so many people, right, you're, you're also making these really
mass, mass online learning events, right, occur online boot camps. So how is
that going? Why did you start that and is that only for really junior people?

[00:12:12] **Jess Rose** So the first thing I want to do is like, I would
absolutely love if there was an excuse for me, Oh, yes, I'll just take all the
credit. But the free online boot camps that I've started are absolutely not just
me. So they started as 12-week boot camps, and they've been collapsed into a
reasonably intense but still part-time, six-week boot camp. And this is built
off of the freeCodeCamp curriculum. So they're a registered nonprofit. They're
amazing. We could not do this without them and without their permission. But
also the good people, I’m pointing behind me like they're back there. The good
people Class Central built a whole platform that lets us teach on so like, just
really, and Ramon is my, my co-teacher. And he's he's just, it’s almost
disgusting how lovely he is. Like, the learners love him and deservedly so.

[00:13:03] **Dr. McKayla** Cool. Yeah. So what do you teach there? Is it like
really the 101 of programming? Or is it more advanced concepts? Who is your
target audience here?

[00:13:14] **Jess Rose** So this last cohort, which just ended about two weeks
ago, I should get back to work on those. We had 15,000 unique learners across
two tracks learning either web development, which is HTML, CSS, accessibility,
really, really intro level of like first steps of programming, or across
JavaScript. And again, that sort of first steps with JavaScript, getting
started. So really sort of introductory level. But we added some additional
forums for peer support. We've got a very noisy Discord. And then some live
stream lessons and question-answer to get people unstuck. We've had such a, so I
would have expected oh, these will be beginners. We have back-end devs who
wanted to try out web development. We've got folks who don't want to go into
tech, but they do want to build a website for their business. And the thing I
was, I used to be a teacher and I used to be a linguist. And very selfishly, the
thing I was, one of the things I was most excited about was the absolute range
of the learners. We've got folks across every regularly inhabited continent. And
folks joining us in this massive exciting range of first languages. I was just
so, so people who are learning from their phones, people who are learning from
the library computers, and I just really really loved this loud, chaotic, and so
lovely and so supportive group of learners all helping each other out.

[00:14:49] **Dr. McKayla** Yeah, that's, that's really exciting. So I actually
was thinking a little bit about learning on devices that are not high-end,
right. And when I, when I started university, I couldn't afford a really
high-end computer not even a normal computer, right? So I was on this, I got, I
got one of those really cheap computers from somebody that you know, gave it to
me for free. And it was a nightmare. It was a nightmare to work on that. And
nowadays, it's obviously not the case anymore. And I'm really happy about that.
But I was wondering what about, you know, people that don't want to work on the
phone or work to, you know, on a tablet, and I'm pregnant right now.

[00:15:32] **Jess Rose** Oh, congratulations. How exciting, how scary.

[00:15:36] **Dr. McKayla** Yeah. But it's also a really cool experience because
I'm thinking, like, this is my third child. So I know a little bit.

[00:15:45] **Jess Rose** Oh, you're just fine. You're like, duh, this happens.

[00:15:46] **Dr. McKayla** I know what's going to happen, its going to happen
that I can sit here and you know, work on my comfortable devices. And so I tried
a little bit to work on my phone and work on the tablet and so on, I still think
it's really difficult. What tools do your learners have?

[00:16:03] **Jess Rose** Did somebody, somebody did one of my friends talk to
you about this? I'm deeply suspicious. So I'm going to try really carefully not
to say too much. I’m working on a little side project around this problem.
Because this is a problem I've been thinking about a lot. So right now, and if
our dear listeners, our dear viewers are, oh, gosh, what's the noun? Our beloved
audience, your beloved audience has a tool or has something in the space that I
haven't seen yet, please come and yell at me. But right now, I'm not seeing
really good tooling. I'm not seeing a good way to write to the web from mobile
devices.

[00:16:46] **Dr. McKayla** Yeah, it's not there.

[00:16:47] **Jess Rose** And this is an ethical problem for me. Because right
now we hear people talking about the next billion users, I love this. But in a
lot of cases, we're seeing people who are accessing the web for the first time,
and I love it, and I live for it. But they're accessing the web on a lot of
constraints. So they're usually on phones, they're usually mobile-only is what
we'll call those kinds of learners. They may be accessing it in their third or
fourth language, because you're going to see global web primarily in English and
French and Spanish. And they're often constrained to really, really challenging
limits on their, like their actual access to broadband or to mobile signal. And
that's something I've been thinking about a lot on the device level for this
problem. If I went, I'm going to date myself terribly. But I got access to the
internet, when I was maybe 13, or 14. And the device I use to access the web to
read the web, I could also write to the web. And we're effectively giving people
this write-only access to the web through smartphones. And that just, that
doesn't seem like enough to me. So there's nothing great yet. And I don't think
I've necessarily cracked it myself. But in the next couple of months, I would
like to, I've got a little thing I'd like to launch to see whether or not that
might be a good tool.

[00:18:10] **Dr. McKayla** Yeah. Cool. I would be super interested in that. And
I also think like, nowadays, I'm actually, I should actually be the whole day on
bed rest. But two weeks ago…

[00:18:20] **Jess Rose** What are you doing? You should be doing this lounging.

[00:18:23] **Dr. McKayla** Yeah, I should. Right, yeah. But so now I'm allowed
to be up a couple of hours per day, which is, which is great, but because I'm on
this bed rest, right, and I only can lie down, I'm not allowed to sit actually,
I experienced all these accessibility problems that, you know, couple of, you
know, disabled folks also are experiencing and I'm like, right now, I really
understand how difficult it is if you can't, you know, type, write, if you have
like these mobile devices. And I think there is really there isn't a lot of you
know, there's so much space in there. And we should really be much more
welcoming to people that can't, you know, sit on this nice computer have their
three monitors, right, the keyboard and the mouse. And it's really I mean, it's
really frustrating for me to write a blog post to make an update on Git, right,
to make a PR.

[00:19:12] **Jess Rose** I'm not ignoring you. I'm just grabbing a book to see,
so rude, isn't it? Turning away? Oh, heck, I must have hidden it somewhere. But
there's a really fantastic book from the late 90s that Tim Berners Lee wrote
about the process of inventing the web. But I've got sort of a tab in the book
because he said, Oh, okay, we had to sit down we had to define the bare minimum.
What is the minimum viable setup you need to access the web? He said, Oh, you
need to, you need some kind of CPU, we need some kind of monitor some kind of
display. And one of the things that they specified as necessary for the web was,
you're going to need a keyboard. I think that's the point that sticks me again
and again, where I think, but we've gotten past the need for keyboard in so many
other spaces. Yeah, it seems a bit lazy to have not gotten past it in sort of
the ability to do simple web development.

[00:20:12] **Dr. McKayla** Yeah, yeah, it would be so great. Like, I would
benefit so much from it.

[00:20:17] **Jess Rose** Oh, just the guilt I've got right now. I'm just like,
yes, yes, I'll get back to work. But we do currently have learned, well, in the
last cohort, we had a number of learners who were accessing the course, all via
smartphones. So they would post and we'd love to see them post, screenshots of
their code to see, hey, where's this gone wrong, but it's going to be folks
screenshotting their phone screen, and just the implication of how challenging
it would be to write, I've tried it to write a bunch of CSS on your phone, oh,
the absolute, like the strength these people have in their hearts not to throw
it across the room.

[00:21:01] **Dr. McKayla** Yeah, definitely. Definitely. So another question
that came to my mind is now you have this experience of, you know, teaching
really beginners, and also in a different space, it's a space of you are, you
know, like this, this teacher now, and they're doing an online course. But I'm
also very interested in how can we actually bring back or coming back to the
managing position, right, how can we teach and mentor within a team, right? How
can we do that for juniors? How can we do that for mid engineers? Who mentors
and teachers, senior engineers? How is that all, you know, the dynamic in a
team? And I was wondering if you have like some experience around that and some
thoughts around that topic as well.

[00:21:47] **Jess Rose** So I was really lucky. I was on a team several years
ago now out at FutureLearn with oh, gosh, Nikki, What's your surname? I'm so
sorry. I swear I know it. I've just forgotten it, because I'm a bad person. And
Belinda Sockington, who are both unreasonably brilliant and fantastic managers.
And a lot of that work on that team was around, because I have FutureLearn was
that it was a MOOC platform. How do we, how do we encourage learning? How do we
incentivize it? How do we balance it? And really, what kind of landed for me is
it's an ongoing conversation between the folks running these teams, the
individual people. I think it may be one of those issues where there's just no
one size fits all. It's a combination of saying, Hey, we have these options.
Here are some off-the-shelf learning experiences, with starting a conversation
and keeping up a conversation of what do you want to learn, what works for you?
What's best for you? One thing that I've encountered a couple of times in my
career, which I've had a really, really hard time with and my opinion on it has
really radically changed, is every now and again, I'd meet somebody who's sort
of mid-level or senior, so they've they've gotten themselves into a secure role.
They're feeling okay with it. And they wouldn't be that excited about learning
where they said, Yeah, I just want to do my job. But I want to go home. And I
think the first couple of times, because nobody tells you, but you're not going
to start managing people and get it right right away. I'm going to stay awake
late tonight absolutely obsessing over the ways I'm still not doing it right.
But back then I was thinking, Oh, how can I, how can I make this person care
about their learning? And these days, I think with the, with the world having
gotten much more stressful, and me having enough experience to see that I think
now that I was wrong. These days, when I meet somebody who's like, well, I'd
like to do my job. I'd like to do a good job at my job. And I'd like to go home,
I don't really need to move up. I don't really want to stretch and learn more.
I've gotten, yeah, like, that seems increasingly chill. I think it might be
cultural as well, I think. I'm from the States originally. And I think there's
quite a bit more fear around employment in the States. Almost everybody can be
fired at any time and that makes everything very exciting. And generally your
health care is associated with your employment. So I think I see when I was
younger and based in the States, there was a lot more Of course, you have to
keep learning, of course, you have to keep running, you have to progress.
Otherwise, something bad could happen. And yeah, I think I've just gotten
increasingly excited to see people set boundaries around where they put their
learning and where they put their interests. Yeah. Yeah, that's a very strange
take for a teacher.

[00:24:47] **Dr. McKayla** Yeah. So actually, I was talking to Cat Hicks, just a
couple of weeks ago. Yeah. And so we were talking about learning debt. And this
whole topic brought us to something where I think, you know, learning is often
something very externalized, right, where you say, Oh, I'm learning, let's say
I'm learning React, or now I'm learning Remix, right? So maybe the newest
framework or, you know, a new a new approach for DevOps or whatnot, right? So
it's something that's out of what you're doing right now. And it's a new
technology, very technology-oriented as well, whereby I think at the company,
there are so many, a little bit more how to call it but informal, or, you know,
a little bit more tactic, learning experience that you actually have every day,
right, which is, how do I communicate with this new person on the team, right?
How do I, how do I understand parts of this codebase? Can we change the
architecture for that without breaking something? And all of these are also
learning experiences, which we are often not declaring as that right, so we are
not saying, oh, you know, McKayla, today learned about new ways to do this
architecture for us or to refactor that code, or, you know, she did, she learned
about how this API works over there that she hasn't worked about, right? This is
very often not, I don't think it's so visible in the learning experience than if
I would say, Oh, McKayla sit down and learned React. Yeah, you know.

[00:26:25] **Jess Rose** And I think that's really valuable. Because even when
you say something, somebody say, I think, oh, you know, I'm just going to chill
and do a good job. And it's so easy to generalize about brains and learning to,
say, Oh, we know what we know about learning. In so much as we've learned
anything about learning like self-assessment’s messy, the study of, I'm not
nearly clever enough to have a good handle on neuroscience and learning. But
there's actually a fantastic researcher and author, Dr. Barbara Oakley, who does
a lot of work on learning how to learn. And she's been doing some work with Zack
Caceres who's a programmer, and I’m not going to tell, talk out of turn. But I
believe they may be launching a project around how we learn programming skills
relatively soon.

[00:27:11] **Dr. McKayla** Yeah, nice. Yeah.

[00:27:11] **Jess Rose** But we're primates in changing environments. Even if we
don't think about it as learning, we are getting new situations and new stimuli,
just like you said, I've got a new teammate, I'm going to learn to work with
them. Oh, I've got this API. Oh, I finally understood what's going on under the
hood. Regardless of whether or not we've set ourselves a mountain path to hike a
declared learning journey, there's still learning happening. Yeah.

[00:27:37] **Dr. McKayla** Yeah. And I think that those chill folks, how you
call them, right? Maybe they have also more capacity to actually see things that
are, you know, people that are very on their journey of, oh, I want to learn
React and the latest, you know, whatever, technology comes out right now, maybe
don't have the capacity to see, for example, oh, you know, now that the market
changed a little bit, budget shifted, we have to work a little bit different
with this team, or, you know, how can we make sure that our deadlines are, you
know, approachable, and so on? So, yeah, I think learning really happens in so
many forms. And, yeah.

[00:28:14] **Jess Rose** And I, yeah, I've always been really excited about that
as well. I think resilience is undervalued in teams often. Sorry, this isn't
very confident or it is not very definitive, but I'm going to waffle about my
biases as part of this. I really like thinking about resilience in individuals
and in teams as a resource available. And I like thinking of people as
resources, but like, someone being rested, somebody having the capacity,
somebody being ready for a little tiny crisis, or a little weird thing. That
feels like a resource right there. But I think often we really lean on
productivity so hard. How can we get. what kind of developer experience tooling
can we use to get 20% more? How can we make sure people are focused? How can we
cycle our meeting? And we're so focused on developer productivity and the
productivity of technologists, I think we often sacrifice that flexibility and
that resilience of having somebody who's not under these productivity pressures
to such a high degree. Like, we learn better when we're chill.

[00:29:25] **Dr. McKayla** Yeah, yeah. And I think it brings us back also to,
there was this glue code, right? People that are taking on responsibilities,
right, glue work, sorry, glue work, that was what it was called, right? But
people that are taking on some invisible work that are, you know, good for the
team. And, and so yeah, I think this also for teaching, mentoring, learning, I
think this can be one thing, and obviously, we shouldn't get outdated too much.
And, but I also think that it's not changing every minute, you know, like,
sometimes we believe, or we were made to believe, or this story lines around
time, Oh, my God, you know, if you're not doing every day something and..

[00:30:11] **Jess Rose** What do you mean you're not using blank? I’m like,
look, I’m very old, and I'm very tired. Like, I'm good.

[00:30:18] **Dr. McKayla** I think it's totally fine, right. And there are a lot
of technologies, that I mean, if you're working on PHP, you know, a lot of the
web runs on PHP, and it's still, you know, a good technology, and it's okay.

[00:30:33] **Jess Rose** Like, if you want to stretch a little bit, getting into
some Laravel is really, really exciting. But if you write PHP, you can hang out
and get better at the core stuff of what you do. And do a good job. Like, you
don't have to run as hard as you can, as fast as you can forever.

[00:30:51] **Dr. McKayla** Yeah, I think they're, they're, you know, good
choices to make. And I'm definitely for growth and for learning. But sometimes
people are just burning, you know, mental calories. I learned so much. I mean,
I'm actually a learner, right? I love to learn. But most of the stuff that I
learn, I never used. It's not very productive, right?

[00:31:16] **Jess Rose** Yeah, but you can't not... sorry, you've invited me on
here. And I'm just up here ready to below you. But yeah, this sort of cult of
productivity, not that you're espousing it makes me very, very, and when I talk
to new learners, and they say, oh, okay, I need to learn this, and this, and
this, and this, and this, and this. And I've heard these words, and I need to
learn this. I'm like, Babe, you can, you can show we can all chill. Like, we
don't have to learn any frameworks yet. We don't have to learn any ops yet, we
can just chill and learn the core stuff. And as these are like, one thing I
really like to encourage, especially with new learners, or learners new to a
specific space, is to go ahead and get some kind of digital or some kind of
physical space where you can dump stuff. Some people like Notion, I hate Notion
a lot. I quite like Obsidian. I don't care what you use, as long as you're happy
about it. As you're seeing all these terms, just chuck them in a big doc. Okay,
well, I keep seeing Angular, I know Angular is a thing, should I learn it? Don't
worry about whether or not you have to learn it next, just go ahead. And when
you see an article about it, throw it in the slush pile. I call it my link dump
for early learning. And that means once you've got through the foundational
stuff, you say, Okay, I've learned enough JavaScript where I can write. And I
like setting these little tiny interim goals to say, Well, I've learned enough
JavaScript where I'm able to make simple bug fixes in this open source project I
was interested in. I've learned enough. And one thing I'm excited about is the
The Art of Learning code, or the art of reading code, which is something
Felienne... is an academic who’s done a lot of work in the space.

[00:32:59] **Dr. McKayla** She's from Leiden University.

[00:33:01] **Jess Rose** Yes. You've talked to her already. I bet.

[00:33:02] **Dr. McKayla** I did my PhD with her in the same room. Roommates.
Yeah.

[00:33:06] **Jess Rose** Did you? Did you?

[00:33:06] **Dr. McKayla** Yeah, we were roommates. Yeah.

[00:33:07] **Jess Rose** Oh, is she just as delightful to study with?

[00:33:10] **Dr. McKayla** Yeah, she is wonderful.

[00:33:13] **Jess Rose** But yeah, so really getting through the basics of well,
I set out to do X, I'm doing X. Now it's time for me to go look through my link
dump file, and see, wow, it looks like I've got like 40 different articles about
Angular. Maybe that was important that that's enough for what I want to learn
next. Yeah.

[00:33:34] **Dr. McKayla** Maybe something else that comes to my mind here is
also that I think fundamentals are really important, right? So I like for
example, the approach of Dan Abramoff, right? He has like this course of Just
JavaScript, which it means that you're not starting with React, right? You're
starting with JavaScript and with the fundamentals around it, and I wouldn't say
it's really a course for really real beginners. But it's like if you got a
little bit of your hands dirty around JavaScript, it's really nice to go in and
then check. Did I actually really understand what's you know, what's happening
here? And then if you have these fundamentals, I think it's so much easier to
build upon that, them. And dive into React or whatnot, right? Whatever framework
or technology you want to add here.

[00:34:21] **Jess Rose** I think this comes back to something I've been thinking
about a lot in how we learn and teach. But like, where we abstract things out.
So in the boot camp, we're using Free Code Camp to teach, which is a, it's an
in-browser sandbox, you don't have, and they've just come out with a new beta
curriculum for web development I'm in love with. And it previews that these are
files and that you have to link to these files. It is very, very good. But it's
still a sandbox, it's still an abstraction. And the places we tend to send
learners next are things like, Okay, we're going to head over to CodeSandbox,
we're going to head over to Glitch which are still abstracting away a lot of
really, and then even when you look in to professional tooling and frameworks,
they say, Okay, let's get into React. A lot of the power behind these frameworks
are that they abstract away or that they compress, or they obscure or or smooth
over some of the fundamentals of how we work with the core technology, maybe
JavaScript or the way, Tailwind is a weird abstraction of the things you'd like
to do with CSS. And I don't have a problem with, I think as a teacher, I'd have
a hard time having a problem with abstraction. But I think that thinking really
carefully about how we do this, when we abstract things , and how we signpost
what's been taken, or what's been added gets to be really valuable.

[00:34:47] **Dr. McKayla** Yeah, I think so too. Yeah. When I was starting to
learn programming, I struggled a lot with abstractions because I just wanted to
know, or not only with abstractions, but also like, there wasn't a lot of
abstractions. It was actually very, very raw, right? It was like, Oh, you have
an Eclipse IDE open and you're writing Java code. But then you have like, oh,
let's say, you know, public void string main, whatever, right? And it's just
like, you just do it, right. And I'm like, why? What does it mean, don't worry
about it.

[00:36:22] **Jess Rose** And then we'll cover this later. And so by the time, we
will have covered it, yeah… Having been a linguist, I fear that I mentally map
language learning to programming language learning, even when it might not be
entirely suitable. But I see this happening in human language education as well,
where we say, okay, cool. Here's how, we keep we start people in the present
perfect tens for a lot of languages, I see the cat, I drink the water, I walked
to the store. And we don't send them into a present perfect world. And I think
that's true with programming as well to say, Okay, well, we're going to give you
this sandbox, or we're going to give you this framework, which abstracts away a
lot of the complexities of the grammar or the the nuance of, and I think it's
really valuable to talk about the culture of the language we use around
programming and really the culture of, of the structures we build, because it's
not transparent to people. I met with a learner in person, what a delight, in
person last week. And without thinking about it, I said, yada yada yada
bikeshedding. And thank goodness, this learner was confident enough to be like,
cool, what the heck are you talking about? I was like, oh, gosh, that's just
something we say. We say it as though everyone's going to understand it. And it
means to get sidelined to get distracted with little unnecessary details. Just
like okay, cool. You should just say that, it's less complicated.

[00:37:55] **Dr. McKayla** Yeah. I think it's not always that easy to be always
aware of how you do it. But I recall the time that I started at Microsoft, and,
you know, when you start there, it's full of acronyms. And they mean, they mean
something completely else inside Microsoft and than it would mean outside, and
it really takes quite some time. And then a lot of people get very blind to it,
and you know, just start using it as well. And you know, you start talking this
gibberish. Nobody else can understand. Yeah.

[00:38:32] **Jess Rose** But like, from a linguistic perspective, that
identifies you as a member of the in-group, doesn't it? How fascinating. Yeah,
incredibly interesting. Oh, no, no, I absolutely refuse to spend the next three
days hyperfocused learning about weird Microsoft acronyms. It's so tempting.

[00:38:49] **Dr. McKayla** Yeah, there are a lot. But I think it's the same with
code reviews, right? And with sometimes how people say, oh, you know, we have
this style of giving feedback to each other. And in my code review workshops, I
always talk You know, I always try to have people come to an agreement that we
need to use language and also, you know, phrase that in a respectful way, that's
not only for the internal, you know, internal team to understand. Because there
are newcomers, you know, in the team, maybe somebody will look at that, what you
wrote two years from now, right, and still should be able to understand it. And
so I think it's really good if we be clear about those bridges that we built
that, you know, are this internal behavior and language that we are using that
it's only, you know, it's an insider joke, and so on.

[00:39:47] **Jess Rose** Yeah. Yeah. And I think we're often really chill about
that in tech. Yeah, oh, here's a glossary of technical terms you need to know to
do the thing. We're, we're cool about that. There seems to be a bit more
resistance around when shared language or shared norms, or shared language
structures around things like code reviews are proposed because we don't need
that we know how to talk to each other. I hope I'm not putting you on the spot.
Are you one of those lucky people who speak like nine languages?

[00:40:15] **Dr. McKayla** No, not nine.

[00:40:15] **Jess Rose** Oh, only five?

[00:40:17] **Dr. McKayla** Maybe, yeah. German is my mother tongue, right?
English, Dutch, Italian, and a little bit of Spanish.

[00:40:28] **Jess Rose** A little bit of Spanish. Look at that. The fantastic
thing about chatting to many folks from Europe is, is y'all always have this
very, very beautiful, very casual, like humble brag at the end, you like, you
know, just a little tiny bit of Croatian. I'm terribly jealous. Yeah, like
recognizing that folks aren't going to be coming to, coming to these code
reviews. And I really liked that you highlight that they're going to be coming
to the uncoupled in time. I love this idea that when you leave a code review,
when you leave feedback, when you leave a pull request, when you leave code,
you're leaving a little artifact of understanding behind. So to say, Cool, we've
standardized how we talk about these, we've created a shared language for them.
Because when we go into the far scary future, we want these to still make sense.

[00:41:23] **Dr. McKayla** Yeah, I think this is really important.

[00:41:26] **Jess Rose** But also making them like giving a shared language
around, hey, maybe English, or if we're doing the, if we're doing the code
review, in Dutch, I'm in a bit of trouble. But maybe the language this code
review is in is your second or third or fifth? Let's go ahead and have some
shared language have some shared structures around feedback to lower the
cognitive load? Yeah, well, can we talk about cognitive load? I imagine you've
done it tons of times on the podcast. I imagine many programmers are familiar
with it.

[00:42:00] **Dr. McKayla** Yeah, we also have to be a little bit careful of the
time now. But maybe the last thing that I want to add here is I'm writing a book
on code reviews, right?

[00:42:10] **Jess Rose** Are you?

[00:42:10] **Dr. McKayla** Yeah, I'm right now in the middle of the feedback
section, right? So how to give feedback, how to give respectful feedback, and
how to communicate with each other and also cultural right? So how do we deal
with, it gets really hairy there, right? So yeah, what are different cultures
are expecting, what's respectful there, you know, how much you know, how harsh
should a feedback be? Or can it be or, you know, what is seen as polite and so
on? And this is not only, it's not only, it's not one standard thing, right? It
depends on who's on the team, what's the background? What's the culture? But I
think the expectation, setting the right expectations, and, you know, explicitly
stating that, and talking about that, reflecting on that, and, you know,
learning how others see those things and learning how, you know, like, if I
would talk to you I'm originally from Austria lived in a couple of countries,
right? You're from the States you're, you're in the UK now, right?

[00:43:12] **Jess Rose** I am, yeah, everything's just fine here. Very chill.
Not weird.

[00:43:10] **Dr. McKayla** Yeah. And then maybe we have another person from
Croatia and then somebody from India, right. And so I think it would be really
important for us to talk about how we understand different terminologies, how we
understand different you know, expressions in my code review workshops,
sometimes I have discussions about looks good to me. And I love those
discussions because, you know, it's just a simple term looks good to me. Most of
the time, people just, you know, have the acronym for it, right?

[00:43:47] **Jess Rose** Like it's the thumbs up emoji in my head.

[00:43:50] **Dr. McKayla** Exactly or you know, LGTM, right? And then some
people are like, oh, yeah, this means you know, that I looked through it and you
did a good job. And then the other person has no, you know, looks good to me
means that you haven't looked at my code.

[00:44:07] **Jess Rose** You just glanced at it.

[00:44:07] **Dr. McKayla** Yeah, you just want it out of your way. Yeah. And the
other person says, Oh, this means, I don't care.

[00:44:07] **Jess Rose** Sometimes, sometimes.

[00:44:16] **Dr. McKayla** And having those discussions in the team, you know,
and understanding where everybody is coming from, and that they actually use,
you know, one simple terminology. And everybody on the same team understood
something else about it, I think it's so valuable, right? And only by these
discussions, you know, we can really understand what's behind those terms and
the way that we are communicating. But I'm also getting a little bit carried
away.

[00:44:45] **Jess Rose** No, no. So I'm going to ask you about your book. And
yeah, I've just had a friend tell me that there are some questions you're not
supposed to ask about someone's book. So I won't ask any of those. Instead, I've
been told you're supposed to say, I hope it's going well. I'd like and I think
it might be useful for hopefully some of the audience as well. I had an idea for
a book that sounded really fun in my head. And I've sort of broken it down into
chapters into essays and trying to write a couple of chapters. And my goal in
writing a couple of essays is I'm trying to talk myself out of writing a book.

[00:45:22] **Dr. McKayla** Yeah, I've heard that. Yeah.

[00:45:23] **Jess Rose** Do you have any advice for not, like, it's the worst.
It's the worst idea ever. No one wants to write a book like, please, please,
please.

[00:45:32] **Dr. McKayla** No, I don't have.

[00:45:32] **Jess Rose** No, I want to know what you’re doing.

[00:45:34] **Dr. McKayla** But I saw on Twitter that you said that and I
thought, like, yeah, you won't be able to not write a book with this approach,
right?

[00:45:42] **Jess Rose** I love that it sounds like a threat, where you’re like,
you’re going to write that book.

[00:45:45] **Dr. McKayla** Yeah, it looks like. I think if you're breaking it up
in essays, that become more manageable. I think you will write this book. Yeah.

[00:45:55] **Jess Rose** But for our beloved audience, for your beloved
audience, they shouldn't write a book, they should, they should definitely do
things that are not writing a book. Like, it's a terrible idea, isn't it?

[00:46:04] **Dr. McKayla** I can't, I can't say it's a terrible idea.

[00:46:06] **Jess Rose** Are you enjoying it?

[00:46:08] **Dr. McKayla** I don't think it's a good idea. But I think a lot of
people would like to write a book and I would be the last person that would
discourage them. Because I was always discouraged to write a book, right? But I
think I know what mess I got myself into.

[00:46:25] **Jess Rose** That’s what I'm looking for, there we go.

[00:46:26] **Dr. McKayla** I would just tell the people that you're getting
yourself into a big mess. But it's okay. You know, it's okay. I think people can
write books, and people should write books.

[00:46:36] **Jess Rose** The world is messy. It'll be fun. Oh, no, this is the
opposite of what I was looking for. But it's so delightful.

[00:46:42] **Dr. McKayla** Yeah, well, Jess actually, this brings us to the end
of our show, I really enjoyed talking with you about all of that. And I think we
should talk about cognition and cognitive load, and you know, all of that. So
maybe I will invite you again, to another session.

[00:46:58] **Jess Rose** I'd love to come back any time. But I'll also pass you
some contacts for folks who are much better at this than I am, I would just go
back and be like, so books. And really, your audience deserves better.

[00:47:13] **Dr. McKayla** Okay. And we will put all the things that we talked
about down there also, maybe the Twitter handle or LinkedIn profile or whatnot,
from the person that you mentioned in the middle, where you forgot the last
name, I put it there. So she will be there as well. And then, yeah, so is there
something that you want to wrap this episode up? Or?

[00:47:36] **Jess Rose** Oh, gosh, can I bully your audience? Is that doable? Is
it permitted? I've been doing advice calls all this week. And the big thing that
I keep coming back to when I chat to people, I do do them just to be mean to
people who are smarter than me is right now everything, everything is just so
big and so loud and so stressful. One thing I've really enjoyed exploring with
people is looking at ways that what they have to do, what they think they have
to do can be smaller and softer and quieter. And I think that yeah, I'd love to
gently bully folks to consider how what they need to do could be a little less.
Maybe you don't have to write that book. It can just be an essay.

[00:48:24] **Dr. McKayla** Yeah. Yeah. I like that. I actually did that this
week with myself and just gave myself permission to let go of a couple of balls
that I was juggling. And I think it's delightful. We should really do that. And
I think it's it's the time that we are many people needed. Not everybody, right.
I think a lot of people needed.

[00:48:41] **Jess Rose** There's going to be one person out there who's having a
real good week. I just haven't met him.

[00:48:46] **Dr. McKayla** Or yeah, or that got very nicely distracted by all of
the work and don't have to think about the stuff that's going on. Yeah. Okay, so
Jess, thank you so much. Thank you. It was really a pleasure talking to you.

[00:49:01] **Jess Rose** Thanks so much. I'll let you go and thank you again. I
won't get into a thank you loop with you.

[00:49:06] **Dr. McKayla** Okay, bye-bye.

[00:49:06] **Dr. McKayla** This was another episode of the Software Engineering
Unlocked podcast. If you enjoyed the episode, please help me spread the word
about the podcast, send episode to a friend via email, Twitter, LinkedIn. Well,
whatever messaging system you use, or give it a positive review on your favorite
podcasting platforms such as Spotify or iTunes. This would mean really a lot to
me. So thank you for listening. Don't forget to subscribe and I will talk to you
in two weeks. Bye.
