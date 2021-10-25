# Episode Liran Haimovitch

**Michaela:** Hello and welcome to the software engineering unlocked podcast.
I'm your host Dr. Michaela and today I have a special episode for you. Two weeks
ago I talked with Liran haimovitch, the CTO of Rookout - an effortless debugging
tool. Our conversation was so much fun and somebody on Twitter actually asked me
if I could make it an episode, and I thought, well that's a brilliant idea. So, 
today I'm sharing my talk with Liran Haimovitch on the challenges and struggles
for getting to high-quality software. Enjoy.

**Maror:**[00:00:00] Um, hi everyone. And welcome to our webinar today on the
secret to high quality code. We're really excited to have you all here with us.
Uh, so let me introduce you to Dr. Michaela and Liran Haimovitch, the stars of
today's webinar. Dr. Michaela has been helping software teams build high quality
software in an efficient and effective way for 10 years, and her mission is to
lead teams to unlock their full potential through company workshops and team
coaching sessions. 
 
Liran is the co-founder and CTO of Rookout, which is a live data collection and
debugging platform. He's an advocate of modern software methodologies like
Agile, Lean and DevOps, and his passion is to understand how software actually
works. So when he's not thinking of code, which is rarely, usually diving,
hiking, or writing a new Rookout blog. Um, and so before we get started, I just
want to remind you all that we do have time for questions at the end of the
webinar; So please don't hesitate to leave questions in the question box and
this will be recorded and we will be sending you the recording at the end. So.
You're on McKayla, please take it away.

**McKayla:** [00:01:02] Thank you so much for your really nice and kind
introduction. I'm really excited to talk with Liren today about, um, high
quality code and get his whole perspective on this topic and pick his brain. So
yeah, I'm really thrilled to be here. 

**Liran:**[00:01:19] It's great to be here with you to discuss so many
interesting topics.

**McKayla:**[00:01:24] Yeah, really cool. So in, in the beginning we discussed a
little bit, like what should this webinar be about? And we thought like, let's
come up with this idea that we are asking each other a little bit questions
that, you know, are burning questions for ourselves or that we very often, you
know, encounter. And, um, so I want to start with that theme and I want to ask
you about the challenge that you see, or the challenges that you see that, uh,
engineering teams face nowadays, with really moving fast. Right? So there's like
this accelerate the book, for example, there, the DORA metrics, the many other
metrics around code velocity. So it's apparently something that we want to do,
right? We want to move fast. We want to be productive, but what are the
challenges and how can we actually achieve that?

**Liran:**[00:02:12] So, I can say from my personal experience as well from
pretty much everything I've read on the topic, the best way to move faster is to
work in smaller units.

You mentioned DORA, the DORA metrics and accelerate, and they're constantly
about, you know, roundtrip time for new features and the amount of new features
that are being released and how can we build in it? How can we work in smaller
unit to work? And the reason for that is because smaller units of work allow for
much faster feedback cycles that allow you to learn much more; you get more
feedback, you get, you learn every step of the way you learn more often, and you
also delivered more value to the end customer on a more frequent basis. And in a
way that's actually driving a lot more value. I guess the biggest challenge is
actually, how, how do you do that? How can you keep moving ever faster? How can
you deliver in smaller units while still keeping delivery efficient? And I found
that one of the best way, the best way to start is quite often culture. And we
talked a bit about you, eh, doing  some recent research for that. So I would
love to hear about that. What do you think about how best to build a better
culture and how to promote a culture that deliver faster and deliver in smaller
units of work? 

**McKayla:**[00:03:34] Um, I'm a big advocate for, for great, uh, culture,
right? Who isn't? Somehow everybody wants to work at the company that has a
great culture, but unfortunately not everybody is. I'm currently actually doing
a research project that's the one that I talked with you about a little bit is
on productivity and work culture and the experiences of developers at their
companies. And so I'm doing right now, a qualitative study, a grounded theory
study where I'm really trying to deeply understand how are people experiencing
their workplace and what factors are influencing their satisfaction, their
happiness, their productivity, and what enables them to move fast, as you said,
to be productive, to be their best selves.

And, you know, there are some factors around obviously release, for example, is
one that's also covered by the DORA metric. Um, how has the release
experienced? And here I'm not only talking about metrics because, I think on one
hand, I'm extremely data-driven; whenever I was working with teams or am working
with teams, also at Microsoft, we did a lot of the research that was very
data-driven, but it was also, and this was very, very important for me, always
qualitative as well. Right? So not only you're looking at the data, which gives
you a very include complete picture, but you're understanding, trying to
understand the whole experience. And so this research study is really looking at
the whole life experience of developers. So on one hand we have like metrics
like, um, you know, release cadence or from time to commit or from time to merge
and so on. So what's very quantifiable, but on the other hand, you have um, the
impressions and the perceptions of people around that. Right? So are they
feeling better with it or, um, are they feeling worse. And the same is true for
code reviews and so. A lot of the things can relate back to culture and culture
is somehow enabler here, right?

So we have like this practices around those areas, let's say release. These
feedback loops that we have, release is actually a feedback loop. Code reviews
are a feedback loop, right? Talking with product management is a feedback loop.
How seamless, how smooth can we make them? And culture is really an enabler for
that.

Why is it an enabler? Because if I'm allowed to say, if something is wrong or if
I'm allowed to experiment, even experiment with some failures, right? Like I try
something out, I try to work different with product management. It doesn't work
out, what happens, right? What are the consequences of that? And that's why
culture is so important because if people feel that they can experiment, if they
feel that they can also express their opinion on it, they will drive more
improvement. Right. Um, the research is really a lot about improvement; how much
improvement can people um, drive and they normally know what's good.

Right. They know what's going bad. Um, or what's good. And so it's really about
enabling them to act upon that. And that has a lot to do in here. The funny
thing here is that metrics are really important to want on one hand, to enable
people that we see and that we make it visible that there are problems. But on
the other hand, metrics often also hold people back. Because if I'm, if I'm
measured. By one metric. Right? Um, it means that if I'm trying something else,
something new, that's not covered by this metric. It very well, it could very
well be that I'm actually slowing down or I'm, The metrics outcomes going down
while I'm trying something out. Right. And so the question is really about
culture here again, how are people handling that? Right? Do I always have to
perform to my OKR or KPIs or what not, right. The metrics and the goals that set
around, or am I actually allowed to experiment here with things that might slow
us down for a short time when I'm doing the improvements, because improvements
are really hard to do without short term slowing down, right? Technical debt.
How are you going to work on technical debt and still keep the features going?
Right? Yeah. So this is what I am seeing here.

**Liran:**[00:07:41] That actually brings to mind the analogy from LEAN
production, where you stop the line. When you see something is wrong and you say
you have the give a individual engineers or individual employees, the permission
to call it; to stop the line and spend the time and efforts to improve things,
even at the cost of lost productivity in the short term, because it allows for
continuous improvement. 

**Michaela:**[00:08:09] Yeah, exactly. It's a really good analogy. Yeah.

**Liran:**[00:08:13] I think it's so important to create. Um, I remember I
talked a lot about feedback, but you're right. It's critical that it's not just
enough to have feedback, but it's super critical that the feedback experience is
going to be positive. Even if this feedback is negative, it's important for
people to be able to experience. Getting feedback -something positive, and in a
way that if they're changing something or developing something, or if it's a bad
product idea that the negative feedback should be, you know, about the, the
feature about the task that this feature was bad, but the person who came up
with it wasn't bad and they didn't necessarily make a bad choice by, uh, you
know, going after this feature, and people should be glad about getting those
so-called negative feedbacks and not attribute them personally. And that's super
important to the culture, to the experience, kind of, how do you go about
creating that? How do you go about building that environment where you get
continuous feedback and experience is good.

**McKayla:**[00:09:23] Yeah. I mean, I'm thinking a lot about culture nowadays
and, you know, the common sense is always all countries so hard, right? It's so
hard to change. And if I'm in a, in a bad place, you know, it's a bad place. Um,
and I think on one hand, that's probably true, but I don't hand now that I'm
confronted so a lot with that, and I'm really working a lot with organizations
and that they in displaced, I'm thinking about the small things that you can do,
and culture really begins now really coming back to something very concrete. Um,
I'm all about code review. So culture begins already in code reviews and for
example, code review feedback.

And to, in my workshop, what I do, I work with people on how to give respectful
feedback. And very often everybody thinks like, Oh, but I'm doing this right?
Like we are not fighting in the code reviews or whatnot, or, you know, or it's
only instances of that where we are mean, but it's more, it's about the
collective awareness of not only do I fight with somebody or, you know, is it an
unrespectful, but really is my mind about value? The value that I can provide to
others. Is my mind about how can I actually, you know, improve the experience of
my peers here. And I think this is something that's often not done, and this is
something very small where a team can really start actively being more aware of
that, more deliberate, more conscious about this. Um, and it starts already by
understanding code is really, really hard and everybody has, um, everybody has a
time pressure and you know, wants to deliver the features. And a lot of
engineers say, well, you know, code review is good, but, uh, I actually have to
deliver feature. So what's about the time that I have to spend on the code
reviews somehow it's missing from my feature work and so on. 

And so having really empathy around that and the experience of myself, but also
off my, off my team, that's already creating culture, um, and being extremely,
um, aware that feedback, even if it comes from a good colleague that you think
like, we are all, you know, good friends and we are really on the same page that
we still really take and this is now again, you know, slowing down, right. It's
slowing down to make sure that I'm phrasing this feedback in a very respectful
way, because we know that feedback can sting. Right. Um, and it can be
misinterpreted. A lot of the feedback comes through a tool, which means it's an
automated tool. I'm not directly talking to a person so sometimes I forget it
and we are in this automated way of um, you know, looking through the
algorithms, finding, you know, let's say edge cases or whatnot, finding
problems. And so if you are in a very technical state of mind, and then we are
hammering in our feedback and say, Oh, Variable name is wrong or, you know, or
should be different. And then going, you know, taking one step back and
thinking, is that creating a good culture? Or can I take this, you know, two
more minutes and say, Oh, you know, what about, um, renaming this and even
giving an explanation, you know, really expressing your, your mind. I think.
Driving cultural change is definitely hard and, um, comes often also from the
top, but there is a lot that teams can do for themselves. And even engineers
themselves can ask themselves every day, like, what did I do positive today?
Like I'm not only going somewhere in and they're expecting that culture would be
great, but am I actually contributing to making a good culture here? Hmm.

**Liran:**[00:12:49] I think it's so much more critical today as we are working
remotely, because as you mentioned, we're often in that technical state of mind,
whether it's on GitHub doing code review or on Slack or wherever, but behind
what's actually happening is we're communicating with other human beings. We're
not just no analyzing code and the testing stuff we're communicating to other
human beings. And as we were, many of us are working remotely quite often, or
most of the time. We can often forget there is a person on the other, on the
other side of it. And sometimes we kind of forget to act with empathy, with
compassion, and while we may be factually, correct we're not creating a good
experience for the person on the other side of that communication. 

**McKayla:**[00:13:35] Yeah. And actually about the factually correct thing, I
have learned over my, you know, my time in the industry that the seldom leader
case, seldom leader are very, very active, you know? And I think sometimes you
forget about that and, this is two perspectives. Cultural views are a place
where two perspectives really are, you know, they are, they are the benefit of
it. And there are also the problem, right? That you are constantly having
somebody that looks at the same thing and say, well, but I'm seeing something
else, right? Like I'm seeing technical debt and you say, but it's fine. You
know?

**Liran:**[00:14:15] The thing is engineers so often feel like they're factually
correct. Even whether it's or not it's the case. I just, and quite often we're
not actually factually correct. There is some degree of, eh, you know, afraid of
common sense and various options, and there is not one single truth out there,
but even if there is even if you there is, and you're convinced that there is in
your, on that single spruce, it's still communication. And you must not forget
that there are other things beyond fact, too, and more often than not, there are
actually no facts and it's just your opinion, which might be very good and
professional, but it's just an opinion. 

**Michaela:**[00:14:59] Yeah, very true. And a lot of the time it's about
strategies. And about the unknowns that you know, that the unknowns unknowns
that we actually make guesses and decision and B we don't know if they are the
best ones. And we even in hindsight, we cannot decide like if we could have, you
know, if you would have done it differently, would we have a better outcome? We
don't know. Right. So, yeah, it's, it's, it's really dealing with that and, and
embracing that and maybe reminding maybe something that we can do also, always
over time to build this culture is reminding us of that. Right. It's a little
bit like we have to remind ourselves of the central things. We have to remind
also ourselves that we are dealing with so many unknowns and that on one hand,
you know, we are, I think at, at one point we have to go and say, Well, we don't
know better. And maybe some people disagree here, but now is the time that we
are, you know, buying in and going this way together. And I think this is also
important for engineering teams, right? So in one of my code review workshops last
week, for example, I give them a code base and it was, um, it seeded with
errors, right? So it has issues and they asked the team to, to find those
issues. And there are, you know, they are. Issues about readability,
maintainability of the code, but there are also security issues. And so then we
had a discussion about, you know, um, so there are a lot of issues. So how are
you going to communicate to the person that wrote that code about those issues?
Are you going to tell them all of them at once? You know, do we make like a plan
around what should be, um, worked on first? And there was, for example, this
discussion then between two senior engineers and they were saying, well, once by
saying. Yeah. Um, so everybody agreed that, you know, sending them 300, 300
problems at one point is not the right thing to work with this junior. So, um,
they were thinking, well, let's do it in, in phases, but it didn't, they
couldn't agree. Like if security issues are more important than readability
issues or not only readability, but making the code work. Right. So there was
this discussion that, well, this is early stage, so it's, it's probably a
prototype, so we should have to, you know, show. So let's do it. Make it correct
first that it works and then work on the security issues that they had, like
they had, there were injection box and cross site scripting products and so on.
Right. But in the end, you know, like the whole team was discussing it. They
couldn't really find a way forward. Right. There was one side that was very
convinced that, well, these are really critical security bugs and they were
really critical. And the other was like, well, but it's, you know, we use it
internally right now. It's a prototype. So let's make the functionality work
first. And so what, there was a back and forth, and I think this was a really
nice example of, I couldn't tell, like, I couldn't say like they wanted me to be
now the referee and say, Oh, you win. Right? Like the security team, Vince, we
first do a security or we first do inability, but there is no right or wrong
answer. It's just the strategy that you're going to do. And probably that you're
not doing, you know, again, not sending all the issues at one is a good one. Um,
but then in the end, it doesn't matter if you do one or the other, as long as
the security bugs are not coming out right. In, in production. Um, yeah. And,
and I think here it's really important to step back from this discussion at one
point and say it's actually a nonsense discussion. Let's, you know, flip a coin
and do one or the other. Um, yeah, this is what I think about this. So a lot of
the things is really. It really depends. And then we have to make a decision and
if we made the decision, this is the important thing. And then everybody has to
buy in and not like, keep this resentment and say, Oh, the security or pre
approach first. Right. And I think it's stupid. And so that's why I'm blocking
here, which is culture. I think. Yeah.

**Liran:**[00:18:49] So actually it's not, it's interesting that you
mentioned that because it's such a big topic. And I mean, so much effort goes
into code reviews and often becoming the bottleneck, both for whoever has to do
the code review. And, you know, spend the time and walk and provided feedback in
both wherever need, wants to get, just to get this code out there. And they're
just trying to, and, you know, they've just finished developing the feature.
They just want to check off the it's been called of you and send it out there.
So kind of what strategies should company follow to speed up their code reviews?

**Michaela:**[00:19:27] So, um, I totally agree that code reviews can become a
bottleneck and they're coming with a lot of pain points, but I think especially
this. This mindset of, you know, cultivate is just another hurdle. Um, that's
something that people have to work on. Right. So, um, we really have to
understand and carve out also, what's the benefit of the code view? Why do we do
it even here? Right. And if the feeling of the engineering as well, I just
wants, uh, I want to look good to me and that's it. Um, then obviously it's a
delay and it's a bottleneck and you know, the value. Probably isn't that high
because even if the person gets good feedback, you know, if the person that
receives it, doesn't actually want it, you know, what's the value of that. So I
think that a lot of those is really for an organization and for a team to think
about what do we want to get out of contribution? And there is a lot of
imperative studies also that really show that the benefits like. Um, improved
code base, readability, maintainability, um, less, you know, less issues, less
bugs, defects in posts and pre-releases, um, all of those are happening.
Culture-based, there's a lot of mentoring and learning happening. There is
advantage knowledge sharing, but it's only if I'm open to it. And if I'm very
clear about what I want to get out of here, because if I want. Let's say if I
want to find it bug, it would be the best to ask a person that's familiar with
the code to be on this code review and not, you know, a junior, but if I want to
have this learning expect more in, in, you know, in the center, then obviously I
ask somebody that maybe hasn't seen that code part before, so that they get
familiar, that I have knowledge dissemination that I have more people that are
familiar about this code base. And I think most organizations. They're not real
bear. They, they hopped on this code review bag and because the hopped on, you
know, to pull request, model to development and pull requests and code reviews
are not the same. And so suddenly they wrote a pull request and they felt like,
Oh, before I pull it in and look at the code and because I'm looking at the
code, it's already a code review. And so now I'm doing code reviews and I want
all of these benefits without actually investing I'm investing. And then here it
comes back to this slow down. Right. So I have to probably slow down first.
Really find out with my team, what is it that we want to get out of code
reviews? How are we structuring our processes, our practices, and this has to do
a lot, right? Like, depending on the risk profile of this code review, who
should be on the code review would ask for feedback, how long should it take
them? What issues are they looking for? All of that can actually be designed and
very deliberately made. And then you're getting really a lot of benefits out.
But if you're not doing that, yeah. Then you're in this state where. He just
wanted, it looks good to me. Right? The other person knows you just want that,
but still feel a little bit pressure, um, that they have to look at it because
if it goes in, they're also responsible. And so there's this delay, um, and you
don't want to spend time for it, but you have to, you know, and then you having
an, I actually have a, if you look on my website, there's the code through your
quadrant. Um, and this means like it's, it's, you have to access and it's the
speed of the process and the value. And this means that you often have them.
Organizations that are slowing speed. And low in value. Right? So they are low
in, in speed. They're very slow. They're bottlenecks and they don't get value
out or that they're fight fast because they're just giving out. Looks good to
me, but they're not getting value out of this. Right. But even if you're waiting
for look good to me, Like say half an hour or an hour or four hours, it's still
slowing down your process. And the question is, was it worth it right? If people
are not really taking the time to review. So in the end for me, it was probably
a very long answer to your question, but it really comes down to what, why do
you do code reviews? Right. And do you have to have an answer for that? And
probably depending on the code change, the risk profile of the code change and
the code change, you will have different answers to that, or this code review. I
want that, you know, my junior engineer knows how that works. And so I'm sending
it over or this, this code changes about how we are doing the checkout. So I
definitely want, you know, two more eyes, um, to make sure that there are no, no
defects going out. Right? 

**Liran:**[00:23:47] Yeah. I mean, that sounds so complex. Can't we just
automate this and install some tool and get it over with?

**Michaela:**[00:23:55] I definitely parts of it. And I think that a lot of
people are, are, are doing stuff that tools should do for them. Right? So they,
they, they are mocking on, you know, style issues they are talking about, you
know, some, some things that actually study analysis tools could find. Um, or
automated code review tools, whatever you want to call them. Uh, in the end
it's, it's, linters that checkers steady analysis tools. Right. And they are
actually much better than, than people. To find certain, certain errors and
certain problems with your code, they can actually, you know, they can walk
through your code and really find out, you know, if they're, if, if some code
paths are not called and tell you, Oh, this is actually not going to call it.
Or, you know, really also bugs study analysis bugs, but they are limited. So
it's, it's not something, you know, they are not, you cannot comply, uh, replace
the, the manual review. But you can replace a lot of that, you know, nitpicking,
which is very unproductive in code reviews. Um, it doesn't matter. Like why
would you have an engineer spend time on finding certain types of errors? If a
tool could do it automatically? I'm I'm all for automation. I think it's so
important to automate whatever you can automate here. Yeah. Are you using, are
you using some automated tools in your pipeline? 

**Liran:**[00:25:15] So yeah, we actually adopted a GitHub advanced security. A
few months ago at Rookout. And it was actually a pretty good tool for us. It
allowed us to gain some insights, actually both brought us a lot of insights
into some of the other code that broke out and kind of knowing where we might've
pitfalls, but it also managed ha ha is helping us moving forward, knowing that
it could work coder pushing through discussed meeting there. You know style checks
and best practices, especially when it goes to more junior engineers or engineers
or working in environments that are not a strength. Let's say, I know most of our
full stack engineers spend most of their days between a, you know, react and
node JS, but occasionally they dive into Golang. And then all of a sudden,
they're not as fluent in, you know, what can go wrong and how should the code
views. And some of those arrows can easily be caught by those automated static
analysis tools. Also, it's a very useful tool personally, we've, we've recently
developed support for Ruby and surely within that skeleton of project, we
started with Rubocop, which is a very, very strict, eh, who ruby linter. And
that's actually provided us with a lot of insight and kind of kept us very
honest as we were developing the code, keeping functions, very short, creating a
very orderly and well structured code. And that's kind of something that it's
always a dilemma for me when starting a new project. Do you go ahead and spend a
lot of time building the skeleton, building the CICD building, building linting.
At the beginning of the, you wait for it later on, because you know that later
on, doesn't always get by. And if you're adding a linter to an existing project,
and then all of a sudden you're getting, you know, dozens of errors, then you
might not be, get going around to fix them because it's too much work and that's
always kind of a dilemma. But for that project, it was a very good experience
for us in developing high-quality code.

**Michaela:**[00:27:25] Yeah, that's really nice. Yeah. There's also my
experience. Like if you, if you add that to an already existing, quite
substantial code base, right. It's just out of hands, right. You will have like
all these red flags, orange, whatever, you know, depending on the tool that you
have, like different severities of issues. And I always feel really bad because.
I know that I'm not going to be able, like to go back and, you know, redo the
past. Um, you can do it slowly by slowly, right? Like I'll voice called removal
or at five by refactoring where you say, well, if I'm touching this code, I make
it nice again or make it better and you can do it ongoing. Um, but yeah, I also
feel like for, for existing code, it somehow has this, you failed here. Um, um,
Psychological, uh, you know, by byproduct, but you'd be like, Oh, now I'm seeing
what's all messy and you cannot really do it. Um, yeah. But yeah, it's good that
it worked out. So apparently you could, could you remove all of the issues?
Could you work through all of them? 

**Liran:**[00:28:26] So we got through, and I think 95% of them ere, there were
some, a few areas where we decided that. That code is not going to be the nicest
code in the project. And that's okay. This code is mostly, you know, four, it
wasn't was low maintenance, low complexity, just a lot of, you know, lung
functions doing boring stuff. And we said, that's something we can live with
without spending too much engineering efforts, kind of fixing it up and making
it look the best.

**Michaela:**[00:28:59] Yeah. So in the interview and the research interviews
that I'm doing right now, we talk a lot about technical debt as well, and how
people deal with technical debt. And I'm asking different organizations,
different teams, their strategies for technical debt. What are your strategies?
We have like some, you know, some amount per sprint that you can use on that, or
how do you, how do you even. Um, assess the value of working on this, uh, you
know, technical, then you were talking like, Oh, we already okay with this part
of the code base, but how do you assess that? And on a more strategical,
systematic level, right? 

**Liran:**[00:29:34] Yeah. So I guess that's a two part question. And on the one
part, we do have a strategy and I can talk about it a bit, but I think it goes
beyond that. I found that for you, you mentioned actually early on that nothing
in very literal in tech is factual and most of it is opinions. And I think
that's doubly true for a tech debt. And quite often one engineer joins a project
and they decide that what's happening. Much of, many of the decisions have been
taken before they joined our tech debt there have been wrong. And I would wager
basic statement that it's. Probably the other way around. I mean, if the project
is live, if it's generating value, if that piece of code was walking from when
it was written up until now, then chances are the decision to, to do it. That
way was actually correct. Or at least descent. And engineers often jump to say
to, you know, define tech that because something is not in the latest design
pattern or something is using an older technology or paradigm, or maybe simply
because they don't understand something. So often the first thing you have to do
when you think of tech debt is actually understand what's going on and truly
think for yourself. I truly think about it. Is this truly affected? Oh, is this
something you lack an understanding? And actually that's something we were
seeing within Rueckert and with our customers that shook out is quite often used
for once you have a better understanding of the code, because you can see how
it's working and you can see inside of it, then you quite often realize that's
not actually tech debt that's the, I just didn't understand how it was working. And
once you get gain a better picture of how is it working, why is it working that
way? And none of the sudden then it makes perfect sense. But obviously sometimes
there is real product that there is real tech debt they, for the most part, we
kind of manage tech debt on a, you know, quarterly on a quarterly roadmap. We
have a very. Agile flexible quarterly roadmap while we manage our roadmap, eh,
usual, all the rollout. And you also kind of add, you know, a handful of tasks
for each team and full of mid-level mid large tasks for each team where they
can, whether they should strive for a tech debt. And obviously, you know,tech 
debt usually comes last in priorities priorities. So it doesn't always get
executed. A lot depends on the roadmap progress in general and especially on a.
Eh, eh, new tasks that get pushed in from the sales team as well, working with
customers. And there are always new requirements for improving performance, for
a meeting new criteria for giving the best experience with possibly can for our
customers. And those often override some of other stuff we have on the roadmap,
but we do try to get at least some of the tech debt cleared every quarter, just
to get a few low hanging fruits with high impact. Stuff that's been bothering
us, that's bothering the team. And also we find that having those, you know,
tasks in the queue engineers kind of find time in way to get to them, to get it
out of the way.

**Michaela:**[00:32:56] Yeah. So what, what reminds me and what I wanted to ask
you in that context is that the original or one of the very early on definitions
of tech debt was code that didn't have tests right from my Confederacy would say,
well, it's tech debt if you don't have tests, because then you really have a
hard time refactoring and often, you know, There's also this new, I was
actually, I did a podcast with him, uh, recently on, on, on my podcast and we
were talking about it and then he, and he also sat like tech tech debt is the
code that has been outlived, but a person that. Wrote it right. And that in our
days in our, in our, um, very fast pace or, you know, um, tech industry where
people will stay two years, maybe at the company, they write code and they
actually never really see it in the maintainance pace. Right. So do you see it
when they're writing it? Maybe when you're releasing it. And so a lot of the,
you know, like a lot of the, the. Code becomes tech debt, because the knowledge
is actually gone from the organization that, you know, wrote that that code or,
you know, can maintainer or understand it. What's your perspective on that? 

**Liran:**[00:34:07] So there's actually a truck out we've kind of we've wrote
and talked a lot about understandability. It's exactly what you mentioned. It's
about knowledge it's about if you're able to understand the software, the code
fairly well, then. You're the new C you can do a lot. I mean, you can get stuff
done. I mean, I think the most obvious example of that is, you know, those
simple exercises you get on introduction to computer sciences readFile from disk,
sort an array, eh, those kinds of stuff. And you know, those exercises you can
usually do right now as a senior engineer in 10 minutes, 20 minutes. And you're
done, but if you were to get the same task within the context of a very large
system, especially one you're not intimately familiar with, then all of the
sudden the same tasks can take you weeks. And then you're going to start
complaining about tech debt and lack of knowledge and documentation. And if at
the same time, or to give that same task to the two, a person who was one of the
founding team of that system, they're still going to get it done in, I know
maybe not 10 minutes, but 30 minutes. And preserving knowledge is super
critical. And at the same time, we need better tooling. We need better tooling
that would allow us to work with systems that are complex, that we're not
intimately familiar with. Obviously testing is there, as you mentioned, testing
is a form of tech that because testing is a Godwin. That allows it to operate in
a, in an area where you're not familiar with. It allows you to easily debug the
code that I, you to see it in action. Even though it's a developing environment,
you can see the code running, you could see it in action. You can make changes
in a control mirror. We know what you're changing, you know what you're going to
impact, but that's at the same time, I think tests can be incredibly expensive.
Even more so if you're not already familiar with the code, so it's kind of, you
know, a conundrum you're saying the code is not very good because it's effective
because it doesn't have any tests and it doesn't understand it, but then it's
going to be very hard for you to add tests to the code. You're not honest. You
don't understand. I think observability tools, by the way, can provide you with
some insights into how the code is walking. Right. Eh, but at the end of the
day, nothing beats just debugging the code, stepping through it, see what, see
the actual types and values of variables, seeing the inputs and outputs of the
system and seeing it in action. That's the best way to understand the code. 

**McKayla:**[00:36:45] Yeah. I think the too, when I was at the university of
Victoria in Canada, um, I was doing a research as a bicycle there. And they,
they developed a tool. I think at that point was called driver. You will not
find it because it was a research tool, right. Not really popular and bad. The
tool itself was really cool because it helped you understand cold. Um, my, my
research area was called code comprehension. And so really helping teams and
engineers understand code. And so this tool was made in a way that you could
Deepak and it showed, you know, the traces and the values as you just described.
Right. But this is like, 15 years back pretty long time. So it was very novel at
that point. Right. And so this was really used to understand coach. I think
debugging is definitely one of the ways how we understand code, right. That we
really go through it and try to understand what's going on a really interesting
resource maybe in that, um, in that regard is also a book that's coming out from
a friend of mine, Felienne Hermans it's called "The program has brain" and it
talks a lot about cognitive load and code reading. Um, there's actually a
workshop that I'm going to attend today about code reading, um, from her. And,
um, yeah, and I think this is really, this is really interesting because it
again goes into these different versions of cognitive load and also confusion
that you have with code and confusion can come, come from different sources. One
is lack. Of your own knowledge, right? So being a junior or, you know, being a
senior engineer, you have a different knowledge base. So you can actually go
back to your longterm memory and quickly access how to load the file, or you
know, how to save a file, how to close a file and so on. And then as a junior,
you have to really think actively think about this with means that you're. Your,
your processing power more or less, right? It's reduced because you have
activity after actively think about this. And we can think around four to seven
things. So if you're already thinking about those things, you know, there are
only two more things that you can add. And as a senior example, you, you. You
have that in your long-term memory. So you have seven things that you can think
about. And the interesting aspect here is also the same with what you said about
the code base. If I'm familiar with the code base, I can load parts of that from
my long-term memory. And I don't have to use my short term memory. I don't have
to use the processor for that. Right. Um, and so there's definitely, there's
exactly what you're seeing here. Um, maybe something else that I want to add
here is you said knowledge dissemination. And code reviews are really good for
that. Right? So that's why I'm saying the organization has to understand the
benefits as a whole, right? And suddenly if you understand that, well, if I can
actually have, have a, a larger part of my team, be more familiar with a larger
part of the code base, that's actually extremely valuable and it will. You know,
it will speed up your development process quite a bit. And there are also
studies on that around code reviews where we really see that, um, it teams that
have code reviews in place. They already have a Vitor understanding of the code
base than teams that don't have. Right. They're only known only know what
they're working on. Um, and so why it's slowing you down to do the reviews. It
really speeds you up. Once you have to work in this pace, right. Or in this
place off the copies, or if somebody leaves, you have other engineers that are
also familiar with. With that. And so I think there are other benefits that are
really, really, um, really important here. Yeah. 

**Liran:**[00:40:19] Yeah. I Mckayla, I'm hearing here speak, it's obvious. You're
an advocate of code reviews and you're passionate about it and you're making
great, great arguments about why it's so important and how the part, the value
fit. But don't people ever come to you and say, I don't know, it's slowing me
down. It's making stuff complex. I mean, I don't want to do pull request. I don't
want to do code reviews. I just want to skip the whole things and kind of what
do you send them? 

**McKayla:**[00:40:50] So, honestly, I don't, I don't have a lot of people that
have this complete mindset. I have a lot of people that would say I really would
like to skip code reviews because I don't have time to do them because my reward
system around my recognition and what I'm expected to do is something completely
else. And then I have to look at code reviews and, and this is not part of it.
Right. So I recall one person, I was just talking with them. Like we could go
around that. Right. It was part of the research again, and they were talking
about it. How, how is it? It's really difficult. They actually love code
reviews and they learn quite a lot and they would have much more, um, much more
benefit and would feel better about them. If this would be actively part of
their job description and their expectations. But it's in very many, many
organization. It's. It's window dressing. It's like, yeah, we want you to do
code reviews and it's really mandatory and they have to do them. But on the
other hand, there is no time to actually do them. Right. And I think that's,
that's what I see very often. I definitely see people that haven't had good
experience with code reviews that don't maybe see the benefits out of that. But
I also have, on the other hand, I think this is why I'm such a strong advocate
for that. I have people, really, a lot of people that have seen the benefits and
that have done code reviews in the right way. And, and, you know, with good
processes around and with a good culture around that, that they say I would
never, ever work anywhere else without code reviews, because it's a, it's a
mentoring tool. It's a learning tool. I'm learning so much more. I'm so
connected to my team. Right. And not working in a silo anymore, but this needs a
certain time of code reviews. You cannot like work on a feature for a month and
then throw over like thousands of lines of code or whatever volunteers look at
it and give me feedback, right? Like this is not gonna work, right. This is, uh,
this is definitely a frustrating experience for everybody. And in this case, I
say, get rid of it. You're not getting anything out of it other than
frustration. Um, but also be honest to yourself that you're actually not really
doing code reviews, right? You're throwing pieces of un understandable codes to
somebody else that can spend maybe half an hour, an hour to look through
thousand lines of code. What are they going to say to you? Nothing. Right. And
so maybe it's really to be about, be honest and say, if I want that, I need to
slow down, understand how to design the process. Um, maybe even get help for
doing that. Right. And then, and then really do it right. And have so many
people that really love code reviews and so many teams that are striving through
that. Um, and yeah, so definitely if you know, if they don't bring any value,
then it's really, I think it's very often the process that's just completely
screwed up and the culture around it. 

**Liran:**[00:43:39] Yeah. And do you find that companies struggled to
understand which pull request was deserved called the code reviews versus which don't, what
policies did they have in place to know to solve them out? Sometimes I know
sometimes just adding a log line and then you need to go through the same code
review process, or at least by definition, it's the same workflow as if you're
adding a big feature. So kind of how the companies go around managing the
different kind of poll requests. 

**McKayla:**[00:44:08] So I think this is really a part of, I cannot
generalize, um, because for some organization it's definitely valuable to go.
Through a pull request or a code review for every line of code that they're
doing, even if it's a log line. Right. Um, but then this is a certain type of
company and they have certain goals around it and it's beneficial. I definitely
see also, um, you know, organizations that have some code review guidelines in
place and it says we have to look at every line and it's a log line. It makes no
sense here. Um, very often here, people haven't thought about again, you know,
what are our goals with code reviews? And if you think about the goals and
it's a logline in, you know, a web website that I can update within minutes
because I have a fast pipeline, why would I go through a code review here?
Right? Why would I slow that down? What's the benefit here? Um, so I think that
organizations that are more vague about their contribution to practices and
process, and really take the time they understand that. Um, and it has to do
with risk profiles. Can engineers, do they have like guidelines to work around?
Have we thought about this as an engineering team? What are our values? Um, when
I was working with Microsoft, we had like, there were, there's not one code
review. Policy, right. It really depends. Office has a different policy than
windows. And then even in, in office, you have like different teams that have
different policies and so on. And so the teams really thought about, um, some
teams would say, well, for us, every line is reviewed. And then other teams
would say, uh, well, vs keeping, for example, refactorings if you do a
refactoring and you can show it, it's, uh, uh, And refactoring that has no side
effects, then you can just put it in or some teams would do the review after
they've pushed it, for example. Right. So after, after committed, after pushing
and after merging, they're doing the so. The, the policies really differ. And
I'm not saying that, you know, even if the differ for some teams, they were
really good for some teams do or not. Um, it really depends how, how honest and
how in there and reflected people were around their code reviews. Um, but you
can definitely be design and, you know, even have automatic things that help you
to decide whether or not something should have a code review. Right. You could
buy somebody if you think about conventional commits. Where you have certain
aspects in the commit message even right? Even those systems are in place. If
you, that you could do here, where it could incorporate some of the risk of
something, or you have against that again, as it tools around somehow assess the
risk. And that helps you to decide whether or not you need a code review or in
what depth you need a code review here, how many people should be under code
review. Right. So, so many questions, uh, yeah. Yeah. Touch on what you meant. 

**Liran:**[00:47:07] Uh, that's. Exactly. Yeah. That's that's perfect. I think
we're almost running out of time here. So maybe Mo join us, throwing a few
questions from the audience?

**Maror:**[00:47:17] Okay. So actually, a few questions did come up. If you
guys are ready for it, um, McKayla, we'll start with you. Can peer programming,
replace code reviews?

**Michaela:**[00:47:26] Okay. Um, pair programming. So I, yeah, this is
a, this is a very often, uh, asked question and my answer is no, it's very
similar to, you know, can automated contributes, replaced code reviews. I think
they are very complimentary here again. So if you have pair programming, um,
You'd probably have different code review practices again. Right. So very
often we talk about code reviews and then code reviews are that thing that
everybody does the same, which is completely not true, could be, it can be so
many things, right. If I'm looking over the shoulder with somebody and looking
at the code at the same time, it's an over shoulder over the shoulder code
review. And so pair programming could actually be one kind of code review, but
then you have to ask your, you know, for yourself or your organization again, Do
we need more? Do we need like some gatekeeping around that so that we have
another person do we need in fairness right around that? If I have two people
that are pairing very often, then you have like this knowledge silo, again, that
those two people know about the code, but maybe I want other people in that, so
we'll add them. So, um, code review can be, uh, a complimentary strategy to
pairing, but I definitely say it should look different, right? For team, the
task pairing code review should look different than for a team that does
know pairing. Yeah. Okay. 

**Maror:**[00:48:50] Very cool. Um, Liran, I think this one's for you, what's
the relevance of code reviews for compliance.

**Liran:**[00:48:58] So I think we found that there are a few, few key elements
in that I think compliance kind of often requires that, eh, some peer reviews,
every change, and I think it goes back to what Michaela said about the purpose of code
reviews. And compliance for the most part would be focusing on first and
foremost general security review, but even more. So it's an often a question of
trust and governance that you essentially know what code is going into the
system in a way. I think it's very different from most of America is been
talking about today, about, you know, in-depth review, understanding the code
and eh, me ensuring that you have all the right pieces in place. It's more about
cursory examination that you make sure that you're not, you're not changing
anything. You shouldn't be changing that the person is making that commit within
the assigned task is working on and within the assigned scope, if there are any
changes to security, sensitive area that you go through additional scrutiny. But
if it doesn't eh, you know, It's more about ensuring that whoever is made the
task, did what he was supposed to do rather than the quality of the work he did.
So that's a very different thing. And it's very important again, to kind of.
Define the purpose of the code review. Is it just about understanding the scope
of the task and the scope of the change, or is it about deeply evaluating it?
Giving feedback, mentoring, sharing, knowledge and so on and so forth. 

**Maror:**[00:50:43] Okay. Um, and Michaela, if people wanted to learn more about
code reviews, where, where would they be able to go to do that?

**Michaela:**[00:50:50] Okay. Yeah. Um, obviously I can see my
website, right? I'm writing quite a bit about code reviews, which would be
(Awesome Code Reviews)[awesome.Codereviews.com]. Or you can also go through my link.
That's my name, [michaelagreiler dot com](https://www.michaelagreiler.com/workshops/),
which is a little bit more difficult for me. We can put it somewhere, but I'm Awesome.
Code reviews, dot com should have them work as well. And, um, yeah, I also have like 
a GitHub. A project that's about code reviews, um, where I'm listing a lot of 
different resources that I find on the web. So it's not only from me, but also what 
I started recently doing is best practices from different organizations. So there 
are articles where you see like how, um, You know, for example, the Google does 
code reviews, or how is, you know, VMware doing code reviews and other, um, 
resources that I found really valuable as well. I also have like code review checklist
there on my [github](https://github.com/mgreiler/all-about-code-review) profile. Um, 
so it it's, uh, the github thing. And then my, my handle is M and then Kyla, 
G R E I L E R. And so, yeah, there, you can find also quite some stuff, um, that, um, 
that comes from everywhere that I found this valuable. 

**Maror:**[00:52:03] That is a wealth of information that everyone should
definitely take advantage of. Um, and I will make sure to send out your Twitter
handle for them too, so they get it. Um, and on the topic of learning more in
Liran, where can you learn more about Rookout? 

**Liran:**[00:52:19] So you can learn more about Rookout first and foremost, that's
[rookout.com](https://www.rookout.com/), which is our awesome website. We've just 
launched a new website. And so feel free to check it out. Also, you can reach out 
to me on Twitter at [Liran underscore last](https://twitter.com/liran_last?lang=en), 
and I'll be happy to chat with you and share more about what we're doing. 

**Maror:**[00:52:39] Amazing. Okay. So then we have one last question here,
um, and it looks Michaela like it's for you. The question is, do we need
additional manual reviews or testing if we have a study analysis tools or is 
that enough?

**McKayla:**[00:52:52] Okay. Um, I think I touched it a little bit
on that. So I definitely think it's complimentary again. Right. So if you have,
like, I definitely recommend to have studying analysis, test tools, have static
analysis tools, security tools, because they are much more systematic and they
they're defining more issues. They are less error prone. You're not overlooking
something, right. Especially for things that are systematic. As I said, Um, for
example, security testing tools are really good or, you know, security analysis
tools are really good for injection box, um, where, you know, people would have
a hard time and it's just unproductive for them to look at that. Um, you know,
in, in the, in terms of what a tool could do here, but then for example, broken
off, um, authentication or just the flow of things that is really beyond the
scope of tools right now. Right. So if you're, for example, sending out. Let's
say that you're somebody is requesting a password reset, right? So the whole,
uh, workflows through that can be very, very broken and there are no tools that,
right. An alpha example can check for that. So that definitely has to be done
manually by, by person and very similar in the code review sense. Right. So, um,
there are really good static analysis tools, but there's always things that just
the tool cannot do for you. So they are complimentary, I would say. Okay, 

**Maror:**[00:54:18] thanks. So that's all we have time for today,
unfortunately. Um, but hopefully we can also down again cause it's been great.
Um, so thank you everyone for joining us, we will be sending a follow-up email
with the recording and Michaela and Liran's contact information for whoever wants
to get in touch with them. And thank you Michaela. And thank you again. 

**McKayla:**[00:54:38] Yeah. Thank you so much. Let's refund. 

**Liran:**[00:54:41] Thank you. Thank you.


