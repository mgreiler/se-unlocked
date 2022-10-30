---
episode: "Episode 51: Measuring Developer Productivity with Dr. Margaret-Anne Storey"
permalink: /measure-developer-productivity-space
status: publish
type: transcript
---

[00:00:00] **Dr. Michaela Greiler:** ( _intro music_ ) Hello and welcome to the
Software Engineering Unlocked podcast. I'm your host, Dr. Michaela. And today
I have the pleasure to talk to Dr. Margaret-Anne Storey. But, before I start,
let me tell you one of my main goals for 20022. Making the SE Unlocked podcast
the best podcast you listen to. I want to eagerly await every single episode.
I have a few ideas how to achieve that, but, of course, most valuable input
come directly from you. Therefore, I would love if you can spend three
minutes to tell me how you like these episodes, and which topic you are most
interested in. Just write me on twitter. My handle is se_unlocked. Or, fill
in the little survey linked in the show notes(??). It would really mean a
lot to me.

[00:00:51] So, now back to Dr. Margaret-Anne Storey. Dr. Storey is a professor
of computer science at the University of Victoria and a distinguished expert
in the field of empirical software engineering.I had to pleasure to work with
Dr. Storey on many occasions. Even this year, she joined me during a research
I led on developer experience, looking at what makes developers happy and
productive and leads them to stay longer and more engaged in their job. Today,
I have her here to tell us more about developer productivity and, especially,
I want to know how can we measure it? How can we improve it? And so I'm super
happy to have Dr. Story or Margaret-Anne, or actually Peggy, how friends call
you. Here on my show. Peggy, Welcome to the show.

[00:01:39] **Dr. Margaret-Anne Storey:** Thank you very much, Michaela. It's
great to be here.

[00:01:40] **Dr. Michaela Greiler:** In the last episode, I talked about my
perspective on developer experience and developer productivity, and well sort of,
there was a little bit of a conclusion, bottom line, which is that I think
organizations and teams should stay right away from focusing on measuring
developer productivity and more think about developer experience. This means
like, how do the developers feel about their work? Are they feeling
productive or are they happy? Do they feel that they make progress?
Are they bothered by some tools and so on? But what is your take on measuring
productivity?

[00:02:17] I know you did a lot of studies there, so you have a lot of
expertise. What do you think?

[00:02:22] **Dr. Margaret-Anne Storey:** All of my researches that I've done over
the last few years has really pointed toward taking a lot of effort and
understanding what you mean by productivity before you try to measure it. So
what does productivity mean to you? I know that in your last podcast, you
mentioned the space framework, and that is the summary of a lot of years of
research that shows that, that there are many different dimensions to
productivity.

[00:02:47] To some people it's about pull requests, or lines of code they
committed, or features delivered to the customer, or ability to be able to learn
something new, or help other people. You can't just say that there's just one
way to understand productivity or define it. There's many different ways and,
consequently, there's different ways of measuring it as well.

[00:03:08] It's interesting to say that we shouldn't measure productivity, but
the fact is a lot of companies will still try to do that. And I think a lot of
developers also try to think about how productive am I being? Am I being as
productive as I think? I really like this pivot towards thinking about
developer experience, which is what we worked on together.

[00:03:31] And you invited me to join that wonderful project that you've worked
on. And I loved that because a lot of my earlier research really distinguished
developer satisfaction from developer productivity; They're definitely related,
so more satisfied, happier developers will be more productive and feel more
productive and vice versa.

[00:03:49] But there is this difference. Developer productivity mean to me
really is about measuring what they do, right? Or how they do it. The amount
of work that they were able to do, or the amount of value that they provide,
whereas developer satisfaction or developer experience is more how they feel.

[00:04:02] And those are two quite different things. So I really like that
nuanced change that you brought to that through developer framework.

[00:04:12] **Dr. Michaela Greiler:** You brought up two things, which I think
are also in my opinion, two extreme different things, which is the things that
they do and the value that those things bring. I thought about this, especially
in my entrepreneurial journey, it even impacts me much more, so that everything
that I do should also lead to impact and have impact and have value.

[00:04:42] Sometimes I see in literature that it's productivity versus
performance, where performance is a little bit more output oriented. But even
there, I think it's really hard to grasp. So, what is productivity? In my last
podcast, I was comparing it to the industrial age where we really have off
producing something which comes back to lines of code, and impact has nothing to
do with lines of code.

[00:05:01] You can have one line of code. It can have a huge impact. It can
be a drastic bug, or it can be a line of code that really is such a satisfying
thing for the customer. I think there are really a lot of nuances, and I wonder,
people very often, I see them measuring productivity because it's the easier
metric. I actually really liked the SPACE framework. I'm super inspired by it,
but I'm also a little bit skeptical on the metrics side of it. I think it's so
great to have it as a mental model to think about productivity in all those
different variations. But then on the end, we have like these metrics that are
very isolated, and then we try to stick them together.

[00:05:40] As I understand it, Right? You're the expert here. So I'm happy to
hear much more about that, but so we should have different dimensions and take
at least three or something. But then in the end, we were taking very
different metrics, and how are we going to combine them? What will the
combination tell us?

[00:06:07] Can we even interpret it? So these are all questions that are racing
up in my head. What do you think about that?

[00:06:13] **Dr. Margaret-Anne Storey:** I'm not a fan of developing a lot of
metrics, honestly. Let me just maybe step back a little bit and just remind our
listeners what the SPACE framework is about in case they didn't get to listen to
your last podcast, which, by the way, was great. I loved your discussion. SPACE
framework is very much an overarching framework to think about different
dimensions of developer productivity. The goal behind it wasn't so much defining
metrics, but just thinking about when we talk about productivity, what are the
dimensions about productivity that we may mean, or other people may mean. So
SPACE is an acronym, and the first letter is S, and that stands for developer
satisfaction and wellbeing. If we think about understanding developer
productivity or improving developer productivity, if we make some change, say to
improve developers productivity, we need to think about the impact of that
change on developer satisfaction and developer wellbeing. The second one is P,
which is performance. So performance are the outcomes or the quality of the work
that you're doing. And again, what performance means really varies from
developer to developer, engineer to engineer, or managers. They all have
different views about those performance outcomes that they care about.

[00:07:31] And the last three dimensions, the A is for activity, which is
what a lot of people think about when they think about development productivity.
They think about lines of code. They think about pull requests. They think about
features that are delivered to the customer. So that's kind of the typical one
that developers tend to think about when you ask them about developer
productivity. C is communication and collaboration. In the research that I did
with now, thousands of different engineers, when you ask them, what does being
productive mean to them?

[00:08:03] For many, they say it's about collaborating with others. How well I
helped others and how well I collaborated with others. And that's not surprising
because software development is such a collaborative activity. You don't write
code by yourself anymore. And then finally, E, which you also touched on, is how
efficient I can be. My ability to be able to get my work done without a lot of
interruptions and my ability to get in that very pleasant flow state, so that I
really feel immersed in the work that I'm doing. The work that I'm doing isn't
so challenging that I feel overwhelmed, but it's at that sweet spot of being
challenging enough that I feel that it's very rewarding.

[00:08:38] Arty Starr also talks about flow in her book called Flow about
software development and talks about the joy of development, which relates
again to that experience and developer satisfaction. The SPACE framework,
honestly, is very high level because it impacts all of those things, right? It
impacts how developers feel, their satisfaction, and their wellbeing, the
performance, the quality, the outcomes of the project that you're working on,
or the tasks that you're doing. And then it also looks at the activities that
you do and then how you collaborate with others. And then that efficiency and
flow part, which again, relates into satisfaction and has an impact on
performance.

[00:09:16] So these dimensions, they're not stand alone dimensions. Maybe you
make a change that makes developers feel more satisfied, and their wellbeing goes
up. So, for example, you make a change that allows developers to spend one day a
week learning something new.

[00:09:29] That could have an impact on their ability to collaborate with
others. If they don't all work on that same day, they won't hear back from
others, and it might have an impact on their activity, at least in the short
term. So you have to think about these together. In the SPACE framework paper
that we wrote about, we spent a lot of time talking about these different
dimensions and the fact that there are these different metrics. None of us, I
think, really believes that, okay, take SPACE, choose three dimensions, and then
choose three metrics, and you're done. That's not really the best way to use it.
However, doing that would be better than choosing one metric.

[00:10:11] The benefit from SPACE comes is thinking about these different
dimensions and thinking about what is it we understand about these different
dimensions. What do you and I understand about activity, and what that means to
have more outputs. When I say software quality, what does that mean to you? What
does it mean to my peers on my team? What does it mean to my manager? What does
it mean to my manager's manager? And when I say that I'm spending a lot of time
collaborating, what does that mean to you? And what does that mean to other
people? And so on. So really, thinking about those different dimensions, realizing
that any change in one is going to have an impact on the other dimensions and
coming back continuously to reflect on those and to reflect on how do we each
think about these and how do we each think these will be affected, if we do make
a change to try to improve overall.

[00:11:01] **Dr. Michaela Greiler:** One thing that came up also in the
developer experience work that we did is this idea of between short-term and
long-term. And I think, especially in measurements, are falling short in that
regard, right? With your example where you have wellbeing coming or going up
because they're spending one day learning, and then two other dimensions going
down because now they have less overlap for the collaboration, and they are
writing less pull requests or lines of code. There's also another dimension,
which would be maybe learning right? And learning then in terms of what's
actually the performance of the engineers? Do they create better things? maybe
they are inspired and all this becomes really intangible. How do we measure it?
Is it happening right now? Maybe it's happening. We see this. If you measure the
things, wellbeing, let's say we have a survey and we ask people and we see
well-being goes up, then we see from Git, well, the commits go down. We see
maybe collaboration overlaps go down. We can measure that as well, but what's
really hard to measure here is that, maybe somebody has an innovative idea. Or
maybe somebody had this idea and learned something, and this saved us from a bug
or created the more maintainable software system because of the things that they
learned here.

[00:12:17] This is a little bit my critique point here, and I really like your
stand on it. It's just a mental model to help get all these different dimensions
a little bit more organized, because there are so many things floating around.
So this helps us looking at the SPACE framework.

[00:12:35] We can at least go through some of the dimension, and we're not
measuring it, but we make a thought experiment like I did right now and say we
have a very strong feeling that, in the long run, our engineers will be more
innovative. We'll be up to date. They will learn. They will maybe stay longer
with us. I know that for every job that I was stuck, where I felt like I'm not
learning, I was very unhappy. And I think a lot of engineers are like this,
they want to learn. So, I think maybe it's a nice mental model to think around
those things.

[00:13:10] **Dr. Margaret-Anne Storey:** That's a really good summary. I'm going
to just mention some of the more recent works that I did with Brian Hopkin and
Tom Zimmerman, where we looked at alignment between different developers and
their managers, in terms of how they define productivity.

[00:13:24] And we also ask them how they define software quality, and what we
found is that there are many, many different views of what productivity and
software quality mean. If you're saying to somebody, should we use this new
tool? Should we allow engineers to spend time learning?

[00:13:40] You have to unpack what are all of your assumptions about what the
impact of that change will be on developer experience or the quality of the
product, whether it's in the short or long-term, and literally expose all of
those assumptions, but also expose what it is that you don't know.

[00:14:0] If we make this change or introduce this new tool, what are the
things that we need more information about? And often enough, I've sat in on a
lot of meetings, and people are using terms like productivity and quality, and
it's clear that they don't even mean the same thing. And yet, they're in these
meetings trying to make decisions, and these decisions are very strategic, and
the decisions are often made without really unpacking.

[00:14:26] We have comfort when we have signals of what's going on, but software
development is a very complex sociotechnical activity, and you can't reduce it to
these very simple metrics.

[00:14:39] This came out in the work that we did too, Michaela, but not
everybody's the same, right? Some engineers might be happy not knowing what the
impact is, and they may be happy helping the people around them. And that's what
they really care about: I helped four people today.

[00:14:55] I've worked with people like that. They're not egocentric at all, and
they're less focused on understanding the vision. They're happy to help the
people around them. There's no single way to measure this, even if we use
surveys as well.

[00:15:08] **Dr. Michaela Greiler:** There's so many good things that you just
said that I want to touch upon. Why are organizations striving for measurements?
The higher up, the more we want some tools. We want to understand the world. And
I think it's this idea of models of abstractions, because it's just too hard to
grasp. So if you are the team lead, and you have five engineers, you
probably have a really good idea of how things are going.

[00:15:30] Are we productive? Are we performing? And so on. If you then the
manager of managers, and you have a team of 50, I think it's really hard to
understand everywhere. Are we doing good? If you have an organization of
500 engineers, it's like, I'm flying blind, right? I'm still really, really
skeptical about building a model, which is so abstract that every model is
wrong that it doesn't reflect the reality.

[00:15:55] And it doesn't really help us. And I like what you said about, there
are things that we know, but there are unknown unknowns? We don't even know what
we don't know. And I think a lot of our activities in engineering or some of
the else is about the unknown unknowns.

[00:16:10] We have to make decisions with the information that we have right
now, to the best of our ability, and I'm really wondering if those metrics. If
they're helpful? Or is it just that we feel that it's helpful? Maybe it's, I
think it's maybe helpful for somebody that has some agenda, right?

[00:16:26] So they want to come up and now to make the metrics look great.
And it's, again, this short-term vision of, oh, I want to Excel here, I want to
be the VP of engineering here, so I make this because it's easy, right? And even
if you have five or six or seven metrics, we can tune them.

[00:16:47] We know that, we can make people respond to it. We can't show that
this is really the outcome that we strive for long-term, but it enables us, maybe,
for some hidden agenda that's more personal than what we are actually going
for this main goals. What's your perspective on that?

[00:17:05] **Dr. Margaret-Anne Storey:** I think that a lot of organizations use
metrics because it helps have a handle on complexity. If I can somehow measure
what's going on, then I can have confidence that the decisions that I made last
week or last month or a year ago were the right decisions. Or I might get data
back that indicates that those decisions were not right and that we need to
make a change. Good managers know that there isn't just one metric. They'll know
that there's a host of metrics. And I think really good managers and really good
leaders will also listen and ask the right questions to find out more nuances,
more deeper understanding about what those metrics mean.

[00:17:45] I'm not saying don't use metrics. Use metrics and also have rich
insights and be continually reflecting and revisiting your assumptions and
thinking about what are are your goals.

[00:17:57] Are our goals to sell more of our products? Well, yes. Right? Because
we need the money to be able to make sure that our developers are well paid, but
once we've done that, what else are our goals? Is it to improve the culture so
that when people come to work, they feel secure? And they feel safe and
happy and they have psychological safety?

[00:18:16] Is our goal to retain our really best talent over the long-term? And
how will we do that? Understanding those goals and then understanding which of
these metrics from a whole different set of possible metrics, I think is one
thing to do, but really looking at what do our metrics tell us.

[00:18:35] But what do they also allied, right? What do they hide? What are they
wrong about? What is our data gathering? What is our data not gathering? Every
time we define a metric, what risk are we introducing by using it? And what else
do we need to gather? Maybe some stories or insights to give us that full picture.

[00:18:56] That's why I think the SPACE framework is quite powerful, because it
helps us kind of identify a whole set of things that we need to ask questions
about and that we need to listen to those answers, to be able to make better
decisions in the future and make change.

[00:19:12] Whether it's change to address a problem or change to make some kind
of improvement. There's a lot of different things to consider, and it's an
attempt to get people to slow down and not to rush, to define metrics and then
create a dashboard and then look at it once a week and say, look, our numbers
have gone up...Wait a minute, what's happening behind the scenes here?

[00:19:31] **Dr. Michaela Greiler:** So what comes to my mind when you talk
about that is the goal question metrics framework.(??) And it's a little bit of a
different approach. I always say, do not measure productivity. You know what I
mean by that is in this very simplified way. I think the data is so, so
powerful, and I think those things are two very separate areas. The critique
that I have for how people use it is that they are creating metrics, but they're
not data driven. I always felt this connection because you had the same
thought about data-driven investigations and researches, which is we combine
qualitative with quantitative. I personally really think that the only in
combination, they become powerful.

[00:20:19] I think that only qualitative isn't as powerful, only quantitative
can be extremely misleading. This is the metrics area that I'm talking about in
the critiquing so strongly. But I think that if we combine them, this can be
extremely powerful.

[00:20:34] In industry, it hasn't really landed. It's also quite complex to
combine that to have mixed research approaches. And behind the research
approach, there is also a hypothesis, questions that have to be tackled, and so
on.

[00:20:48] I'm consulting organizations, where we look at their data, because I
think it's so powerful, and it can help us guide and make decisions in this very
complex world. But I'm always missing this qualitative aspect that we actually
go and say, what does this mean? And so coming back to code reviews, it's
turnaround time, is on one hand super interesting metrics. On the other hand,
it's completely meaningless. If I take it as face value, if I built a dashboard
and I'm printing out turnaround time there, it's maybe meaningful for the first
week. It only becomes meaningful, if I do the qualitative work, which means that
now I'm digging deep, and I'm trying to understand what's happening here. Why I'm
seeing this number? Is this even a number that I should take at face value?

[00:21:36] **Dr. Michaela Greiler:** Probably not. Most of the time not. And I
wonder how can we bring that to industry? How can it be applicable and
manageable for industry? what's your take on that?

[00:21:50] **Dr. Margaret-Anne Storey:** Oh, that's such a great point. I think
that there are a lot of cases of industry that do use mixed methods and do use
qualitative data and quantitative data. I've seen some examples of this, and I've
seen some examples be used really, really well. I don't want to mention any
company or any person in particular, but I saw it with large companies.

[00:22:08] And I saw one colleague in particular. He went, and he sat, and he
watched developers to see what their pain points were, and that was incredibly
valuable to identify some really easy to solve pain points.

[00:22:21] **Dr. Margaret-Anne Storey:** Another example, this was more research
that I did with Microsoft, and we published this in our Tripoli software. One of
my student, Laura McCloud, she was looking, we were looking at the data and tools.
And she was going around and following, sort of jumping from office to office and
seeing what happened behind the scenes.

[00:22:42] The code review tools collect all of the telemetry of what happens
that the tool records, but it doesn't record the engineer jumping over to
somebody's office and saying, ah, by the way, I just tagged you in some code
that needs reviewing. Do you think you could do this quickly for me?

[00:22:58] Or, oh, I see that you submitted this code, and it's got this really
big problem with it. Do you want to fix it before you really send it to me to
review it? Because they don't want to embarrass somebody by finding a big bug.
So understanding what kind of happens behind the tools and behind the data is
really, really critical.

[00:23:18] Showing examples of this with companies and showing them why that's
powerful to have these rich quotes, these rich stories, about what's going on to
augment the data, to go hand in hand with the data, I think does shift how
people approach it.

[00:23:31] Data only tells us what's happening. It doesn't tell us the why. It
doesn't tell us what we should fix. It doesn't always tell us what is actionable
in here that we can change. So we may see over time that engineering
productivity, according to the activity metrics goes down, but that doesn't tell
us why it's going down, necessarily. We have to observe, talk to developers to
find out what's going on here. Why are you not committing as much code as you
used to? And then by talking to them, you can then get insights that help you
make changes, and then you can use your metric to see, okay, is there a change?
Do we see this change?

[00:24:13] **Dr. Michaela Greiler:** And I think especially with that one, it
could be just a change of how people use the tool. Maybe they squash commits, and
we are...

[00:24:19] **Dr. Margaret-Anne Storey:** Yes.

[00:24:20] **Dr. Michaela Greiler:** Counting commits, right?

[00:24:21] **Dr. Margaret-Anne Storey:** Yeah.

[00:24:22] **Dr. Michaela Greiler:** I think the biggest problem here also
is that okay, if you have one team, it's normally quite simple, but if you have
several teams, and they have very different work styles, then these numbers
really become meaningless.

[00:24:34] I would love to find more ways for organizations to bring that
insight. This ability to actually have metrics. But not only have metrics,
really have measurements. I distinguish between measurements, investigations,
instead of metrics. I define it once, and then, half a year later, they are
outdated. They're not reflecting reality, but I'm measuring, I'm having data,
I'm looking at data, I'm doing investigations. This investigation mindset. I
think that would be so strong for organizations. And the ones that I'm working
with, I see so many really good results. It's almost like enlightenment where
metric is a light somewhere making a little bit, in the dark, something visible.

[00:25:16] **Dr. Margaret-Anne Storey:** The other thing that I've come across
is that a lot of folks in industry think that interviewing or observing
developers is very time-consuming, and it doesn't have to be. You can learn a lot
from sitting with your team at lunch and asking them, what are your barriers?
What are the challenges that you face? How is your experience? And gathering
those insights just even once a month can lead to a lot of insights that you can
then use to make change, right?

[00:25:45] **Dr. Michaela Greiler:** I think one perspective that I also want to
add here is that this qualitative aspect that I'm talking about doesn't always
have to be talking to people or observing people. It could be that there's a
person that has this task, and they're going in, they're investigating, let's say,
50 pull requests. And they are writing down what's happening here. Or the last three
bugs, why did that actually happen? Some quality metrics. Or if you're thinking
about metrics again, metrics for me would be oh, line coverage. But then a
person really doing the investigation going and saying, why is this project so
different in line coverage than that project?

[00:26:22] Or why are people having those large pull requests over here and not
there? And very often, if we then do the work, and I call this also qualitative,
because you're not collecting data. It's not quantitative. You have to look at
it, you have to investigate, and you have to see, oh, actually this is very
coupled.

[00:26:40] This is the reason maybe there's a framework.

[00:26:42] And metrics, don't tell you this story. And I think that this is
really what's so important for engineers to improve the experience and to
improve their productivity, their performance. To reduce their pain points.

[00:26:53] **Dr. Margaret-Anne Storey:** Actually, you reminded me of one good
example when you talked about coverage. We did this study that I mentioned that
looked at the quality. How developers define quality, and how managers defined
quality. And we have this framework called TRUCE, which is the timely delivery
of robust features that delight users, support future collaboration and future
evolution of the product. This definition of quality came from the developer and
managers' words that they gave us in the survey we did. Again, there are five
dimensions. Quality you can think of according to these different dimensions,
and test coverage is quite interesting because that would fall under robustness.

[00:27:34] That you have really good tests for the code that you're delivering
so that it will potentially catch some of the bugs that you have in the code
that you push out today. But you might also have tests that don't necessarily
cover the code as it is today, but are there to support change in the future. So
they allow you to make changes in the future. Obviously, they cover the code
still, but they're more focused on not finding bugs today, but allowing somebody
else on my team to make changes in the future. So how do you tease that apart?
Understanding what it is that you're looking at is really, really critical.

[00:28:15] Metrics, if you use them or measurements, any measurements, if you
use them in a blind way, you're going to be missing that nuance, and they're
gonna get stale. And people will misuse them. And they'll be abused, and they'll
be gamified. So really bringing that nuance in is critical, and addressing the
misconception, I guess, that it takes a lot of time to bring that extra
information, and it doesn't. We need to think about it and build a culture that
it's important to ask these questions along all of these different dimensions.

[00:28:46] **Dr. Michaela Greiler:** I think there also have to be role models,
but I totally agree with everything that you said. I actually think we are at
the end. I'm so happy that you were here, and I definitely will invite you
again. So thank you so much, Peggy. Is there something that you think makes this
conversation a little bit more rounded that is still missing from this
productivity idea?

[00:29:08] **Dr. Margaret-Anne Storey:** I guess, just to sum up, if you're
thinking about developer productivity, also think about developer experience,
and also think in terms of quality, like product quality, and to really kind of
think about those three independently, and to think about if you make some
changes or you're making decisions, what are the dimensions of each of those
three things? What are those dimensions that you need to think about? And if
you're working with other people, find out what their assumptions are. If you're
talking in a team, and somebody is talking about developer experience, or
developer productivity, or software quality, just say: hang on a second, what does
that mean to you? Even if you do that, I think it'll shift the conversation in
the room quite a bit.

[00:29:54] **Dr. Michaela Greiler:** Unpacking their assumptions, this is so
powerful. So thank you, Peggy. Thank you so much for joining my show.

[00:30:01] **Dr. Margaret-Anne Storey:** Thank you so much. It's been great.

[00:30:02] ( _static noise_ )

[00:30:04] **Dr. Michaela Greiler:** I hope you enjoyed another episode of this
Software Engineering Unlocked podcast. Don't forget to subscribe, and please let
me know how you liked this episode by writing me on twitter se*unlocked, or
filling in my little survey in the show notes(??). And with this, I'll talk to
you in two week. ( \_outro music\* ) Bye! ( \_static noise* ) ( _clicking noise_ )
