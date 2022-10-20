---
episode: "Episode 50: Do not measure productivity"
permalink: /dont-measure-developer-productivity
status: publish
type: transcript
---

[00:00:00] Michaela: Hello, and welcome to the software engineering unlocked 
podcast. I'm your host, Dr. McKayla, and today is a special episode. Today is
the 50th episode. Can you imagine? Time flies! And as I announced last time, 
this one has a new format. It's not an interview. No, no, no. There's only me
talking.There's no other person joining me. Well, I want to tell you a little
bit about the research that has kept me so busy over this year. I spent really
hundreds of hours investigating what makes developers happy, productive, and
satisfied with their work. I was especially looking at the concept of developer
experience and what that is, well, that's the content of this episode today. 

What inspired me to talk about this is that I recently gave a keynote at a large
internal conference at a large corporation to over 1,300 developers. And when 
I was preparing this talk, I thought, well, this could be actually an interesting
topic also for the podcast. And it's something that I know a lot about that I
spent many years actually researching being in this area. And so, I wanted to 
tell you a little bit more about developer experience and code reviews, 
obviously and productivity. And today's episode is really about productivity
and developer experience and you know, what those two concepts have in common 
and what makes them different. And let's try it out. Cut me some slack, please,
because as you know, I'm experimenting with the new format and I would also love
your feedback. So I will link at the end a survey. You can always go to the survey 
and let me know what you think about it. Let's start. 

[00:02:00] We start in 1440, that's right. 1440. We are not starting in 1940. We 
start in 1440. In 1440. There was a very unsuccessful businessman that wanted
to reveal a new and really astonishing invention. And he was hoping it'd with
this new invention, you will be able to pay off all his debt. In fact, he did
not manage to do that, but what he revealed was really, really unique and very
game changing. It changed a lot. Do you know what it was? It was the printing
press and the guy that revealed that was called Johannes Gutenberg.
And the printing press was a machinery that the allowed to print books and other 
documents extremely efficiently. And what this means is that now books and 
documents could be manufactured in mass and it could also reach masses. So it 
was not only one book that was super expensive because it was hand printed or 
handwritten, but they could now print really a lot of books and became much 
cheaper so everybody could actually buy one. And this invention lead to many 
changes, right? It laed to widespread literacy and education, especially of the 
middle-class. And also change of thinking came with that suddenly a new thoughts,
you know, became, could spread around very easily. And so this invention also 
played a key role in development like the Renaissance or reformation or age of
enlightenment and the scientific revolution. And so it permanently altered the
structure of society through mass communication. And this is why this printing
revolution was so important. But also with this printing revolution and new 
thought was really made to work and that is productivity. So in comparison, 
if you had this printing press, you could produce up to 3,600 pages per day. 
But before that, you could only print 40 by hint printing or only a few by hand
writing, head copying. So we really saw that suddenly we can produce much more
efficiently.

But this was obviously only the tip of the iceberg, right? There was the 
industrialization which came later starting mid 18th century and more and more 
production processes became driven by technology and by machine. And also the 
machines, like the printing press that was first hand operated now became 
operated by steam engines and electricity. And this led to another level of 
mass production and the thought of productivity became even more engraved in
our minds. But it also meant that a lot of professions became obsolete. Right. 
So we, we didn't do everything from start to finish, like producing a shoe. 
There wasn't like a Shoemaker that would know how to do that completely. But 
new professionals were born and that was the factory worker. And because we 
were so focused on making the production process more effective and efficient, 
we realized that actually, if you do fewer steps and be very focused on a task
that this would lead to better results, more quality, but also really a higher
production scale. And well this means that only even nowadays, right, a lot of
those factory workers only have to do a few hand movements or tasks. So, with
this, we could really reach a productivity level that we haven't seen before, 
but you also noted that industrialization wasn't where we stopped. Right?

Mid of the 20th century, the digital revolution took place. And this is really 
important for us, because now automation happened and that was enabled by 
computer. And once again, it's replaced a lot of professions, but also it aided
a lot of professions. Right. And so when computers took over work, that before
hand was only done by humans, they could do it faster and with less errors than
human. This technology was much more versatile than a technology before. It's 
not one machinery that can do one task, but it's a machinery that can do so many
tasks in theory, perform endless operations. And so it's very important to ask 
about, well, what can this technology enabling even at a Loveless?? already ask 
herself?

Well, can computers even think, and she concluded a machinery is only as 
intelligent as we instruct it to be. And while AI promises to shift us, we are 
not there yet. So we have to instruct machines. We have to instruct the computer
to do it. And so this is all professional software engineers, developers, right?
But there is also product managers,architects, testers, UX designers, and many 
more. Many more that really are needed to work with this versatile new 
technology and make it do what we want it to do. The problem is that productivity
is still on the forefront of our minds. And it's a goal that we have, right.
But we face this dilemma that now these professions it's not about doing so much 
as it's about thinking. So the fuel of the productivity is our thinking, not so 
much our doing and now assessing and grasping what productivity even means becomes
extremely difficult. Yet we try we all know that, you know, if we want to measure 
productivity, we can do it by lines of code. We can also measure our productivity
by the number of meetings we attend. And the company, unfortunately, does not 
automatically get more successful as we write more features. It doesn't get more
profitable with that. It's not a guaranteed recipe. But still we try and we also
try to measure productivity because somehow we want to be accountable and we 
must be accountable. Organizations want us to be accountable. Our team wants us
to be accountable. Right. And so we have to demonstrate our contribution and this
thought of productivity That's very connected to activity and output is on the 
forefront of our minds. And so, we're measuring. unfortunately, some companies, 
some teams are measuring lines of code or features now, those kind of things 
because we can easily access it. And I think there's this heritage that we have
from how we did it before. But it's not as accurate anymore as it was before and
so yeah, I want to talk about that a little bit about productivity and how can
we assess it and an interesting, very new. Approach to assessing this productivity 
problem comes from Nicole Forsgren from GitHub and Margaret Scaia from university of 
Victoria. And then there are a lot of Microsoft research faults like Chandra 
Mudela and Brian Hook and Jenna Butler.

But what did they do? Well, they created something called the space framework.
And the whole idea behind it is let's look at productivity and let's try to 
measure it. Right. And I think that the biggest takeaway from their work that 
they did is that. Well, we cannot measure productivity with one metric to one, 
you know, with one single dimension. And, and I think that's very true and 
there's also a really excellent book. I will link everything in the show note,
which is called rethinking productivity in software engineering. It's not that
new anymore. I think it's 2019 or something. And it's editor was Tom Zimmerman
as well, also from involved in the space framework and Caitlin Spassky. There 
are alot of different researchers around the world actually write some essays,
that are based on their research that they do about what does productivity mean?
And here we have also to other people talk about well, there's not a single 
metric, right?

This is something that actually comes also from Kathleen's Bardowski and, her 
colleagues at Google, right? Where you say, well, let's actually not one similar 
metrics. You cannot compromise that. And if you look through the book, you will 
see that productivity can have so many different dimensions and people look at 
so many different things.

What does productivity even mean? And by coming back to the space framework, I 
want to talk a little bit about this. And they said, well, there's not one 
dimension that we can measure productivity, right? So like lines of code, but
there are different dimensions that you have to look at. And they, I think 
they are really interesting because it's the first dimension it has to do. You
have to measure something around satisfaction and well-being, right? So this is
helpful filled our developers with their work, with the team, with the culture
or how happy and healthy are they? Then you have to measure something about 
performance. And this is more in terms of outcome than output, right? Output
would be well, the, the features, right? The number of features, for example, 
that we do, but outcome would be more, oh, how happy our customer. What's the 
quality of our software that were developing. And does it make revenue, right?
Something along this lines. And then you talk about activity, right? Activities 
very often in the center of our minds, when we think about productivity and it 
would be for example, commits how many commits are happening or, you know, what
are you doing? That very easily maybe can be measured through our systems that 
we have. Another dimension is communication on collaboration, right? How people
in teams communicate and work with each other. And again, the idea is how can 
we actually measure that? How can we put it into a metric? And the final thing
is efficiency and flow, right? Do developers have minimal interruptions or 
delays for there work?

And if you look at the space framework, I'm going to link that as well. Then 
they have some example metrics, right? Because it's all about metrics. And 
they give some examples, right? Like for satisfaction, you could have a 
developer satisfaction survey. So you know, a little bit about how people
feel about it, about their work. For performance, well you could have cultural
review. For activity,you could have the number of code reviews completed, right?
This is really just activity metrics and then communication and collaboration 
would be well. You know, PR merge time is something that they came up with, 
right. And efficiency and flow would be the code from your timing. And while 
I think it's really one of the most holistic views on productivity that I have
seen so far. And I think it gives a good balance between those things. I still
have the feeling that we are trying, you know, to measure things that are very
often meaningless, right? Like for example you know, PR merged times. It has a
meaning, but most of the time, I would say the meaning comes from really looking
closely and qualitatively at each of those PR merge types.So if you put up a 
dashboard, what will they say? What, what will happen to all of that? And then
also, how can you combine those different metrics that you're now having and 
get this, this holistic view of productivity? I think it's very difficult 
understanding. 

And there's also a nice essay, very short essay.So if you want to read it I will
link it from Amy Cole as she's a professor at the university of Washington. And
she says why we should not measure for activity. And she wants us to be really
cautious because it can send the wrong incentives. So when you're measuring, if
you start measuring, for example, cultural view velocity, what will happen if 
people know it? And if you didn't know that this is actually something that you
that you judge and is the changes in behavior. Is that really what you want? 
Do you want them to finish that faster? But you know, are you lacking somewhere
else? I think it's a little bit tricky. 

And so I find the space framework extremely inspiring, but for my research, we 
took a little bit different standon the whole part. And it goes away from 
measuring productivity to measuring developer experience. Because there's a 
lot of research that shows that productivity and satisfaction go some how hand 
in hand. They some how influence each other. They are entangled. The people 
that are more motivated, they are also performing better. It's a lot of research
around this. And so developer experience was something that we thought well, 
instead of looking at those metrics and really about productivity, let's think
about how do people feel about the work, how do they think about their work and 
how to do value work, which is our definition of develop experience. So what are
the encountered in their day-to-day work and how does this make them feel? And 
so we also looked at different dimensions that are influencing how a developer 
feels about their work.

I'm going to show and tell you a couple of those dimensions. So we also thought 
about collaboration and culture. You can see there is a parallel to the space 
framework. We thought about developer flow and fulfillment. I would say to 
omehow goes into this efficiency and flow area. We thought about product 
management, which is not really there. Right. So it's different. And 
development and release, which is really the tooling. And I think this is also
very different. And so if you assume in a little bit to this developer experience
framework, and I will link that as well. But I think that the basic concept is 
quite different, we don't want to have any metrics around that, but we really 
want deeply to understand what impacts, how good a person can do their work. 
A developer can do the work, right. And I define it as well. Developer 
experience is all about doing your best work joyfully. Right? So that you can 
do your best work and it's fun.

And so I did really a lot of interviews with people and I think this fun aspect 
that I'm proud of my work. I think this came up a lot. And, and so we wanted to
understand what's impacting people and we started culture collaborativeness, 
right? So supportiveness how connected to a field with my team? How, how safe 
do I feel with my work environment. All these are reallyimportant. There's a 
lot about product management. Is that actually going very well? Do we have 
clear goals, requirements? Can we work iteratively, right? Do we have reasonable
deadlines? I mean, do you know how unreasonable deadlines destroy moral. It's 
crushing it's soul crushing. I heard stories with the soul crushing activities 
that we have, we definitely reduce our productivity. We reduce our performance,
right? So we want good experiences for our developers. And so this developer, 
extreme Springbrook book is really all about, understanding what makes for a 
good day, what makes for good work for joyful book that people can nicely work.
And I think  it's all about how do we assess that? Right. So and it's not metrics, 
we don't crawl data from GitHub or GitLab and then, merge it and then there 
comes out the number. It's really about understanding, I think this is so 
important. So this is really where I'm coming from. I always think it's about 
understanding what's really happening. So let's say one of the things in the 
bucket of development and release would be the code based help. So really 
understanding how is our code base help, but not one metric that tells us, 
we scored a 71% out of a hundred.

No, it's about how do we feel? Are we going into our code base and it's really 
cumbersome. If we have to fix a bug or add a feature, we don't want to touch 
this part of the code base. Well, this is really bad, right? And here we should 
something independent of some number that comes around.
It's about, you know, the flow would be how challenging was 
stimulating. How do I feel my work is? Do I feel motivated to do it? How 
often am I interrupted? And it's not, again, not that, you know, become that or 
that somebody observes, maybe the camera it's really about how do I feel? Do I 
feel uninterrupted?
Do I feel interrupted to have the ability to do deep work? And in my courtroom??
workshops, I do the same, right. So when I work with teams, when I work with 
companies to improve the culture processes, I definitely look at data. Data is 
important, but it's like a small thing. It's you know, it's tipping us off.
You know, so let's say if we are looking at our contribution, I definitely ask 
you, so how long are you code reviews taking? Which we could say, well, this is
code review velocity and this is the turnaround time or whatnot, but I don't want
you to build a dashboard and look at this number. I want you to get a feeling 
really, deeply understanding what's happening here.
Oh, you know, we feel, and maybe the best is to say, we feel it's too long. Or we 
feel it's just right. You know, this is maybe even more important than knowing 
it's a week or it's a day. And obviously there's evaluation in it, there's 
judgment in it. And then we can go back to the data and say, okay, you are not 
feeling so right, it feels, you know, we are a little bit too slow. It could be
faster. How long is it taking on Everett? And then we look at particular things
the longest one, how long are they taking? Right. And then we try to really 
understand why are you taking so long? Are there specific code reviews that are 
taking it on? Do they have some certain characteristics? Right. And then because
of that, this is really an investigation and an improvement mindset. And we can
try to come up with solutions because if you have a dashboard, then it's one 
thing, right? It's, it's making those things faster. But maybe there are some 
cultural use that can't be faster and they shouldn't be fast that it should 
take long. Right. And it's okay that they feel too long and, you know, so 
really looking at the particular uh, things. 

So I also wanted in this new to format to make my podcasts a little bit shorter,
I hope I gave you a little bit to think about and maybe the main message here 
is that productivity metrics, right? They come, they come from a different age,
I would say from a different time and I think also in a different setting, they
probably in an industry setting, they are still very relevant and they can be 
very important. But as knowledge workers. Right. But we think them do, or you 
know, where everything that we do should be thoughtful. It become very meaningless
and I think they are really dangerous for organizations. I think it's super 
atrophy?? that we, you know, sometimes take data to investigate, especially 
investigations around how are we doing. But I have never seen them really work
very valid in dashboards, maybe very short term because we have one particular 
goal, but in general, it's really about helping us to make decisions and make 
improvements, right? So the data should just help us to go in the right direction
and help us to dig a little bit deeper, right. To know where to dig deeper, 
to really look what's going on here. And I think the developer experience, I 
liked this contest concept a lot. I think that people that are happy liked to 
work that can do their best work joyfully. If you can reach that then, you know
trying to measure productivity or performance becomes really a little bit more 
obsolete, but I'm super happy to hear your thoughts on that. What do you think 
how are you assessing some of those things? Is there something, how do you keep
yourself accountable, your team, your organization. And as I said, for the 
survey, I will link it.

Maybe you, let me just know how you like this new format, this new episode, it's 
catastrophe, or was it good? A good start. Maybe some topics that you want me to 
talk about and that I was thinking about the third question then I will end at 
there. Right. So three questions. It would be really, really grateful if you, if 
you let me know. And yeah, so that was it. And bye


