**Michaela:** [00:00:00] Hello, and welcome to the _Software Engineering Unlocked_ podcast. 
I'm your host, Dr. Michaela. And today I have the pleasure to talk to Charlie Gerard.
Charlie is a software engineer and creative technologist. She currently 
works at Atlassian, the company behind the well-known software products such as 
JIRA, Bitbucket, or Trello.

Charlie works on the planning and backtracking software JIRA. In her free time.,
Charlie tinkers with electronics and build brain-control interfaces. I'm super 
thrilled to get to know her and to learn more about her work today. Charlie, 
thank you for being on my show. 

**Charlie:** [00:00:34] Thank you so much for having me.
I'm really, excited for this chat. 

**Michaela:** [00:00:38] Yeah, me too. Well, Charlie, so let's start at the beginning.
A little bit over half a year ago, you started working at Atlassian. What 
exactly entails your role? What are you responsible for?

**Charlie:** [00:00:48] Sure. So I'm a front-end developer on the JIRA product,
and, uh, my team is more focused on is around the navigation and 
what we call the — we're like the "findability" team,
so what that means is we're in charge of trying to make information more easily 
findable by our users. Cause we know that it's sometimes a bit hard for our users
to find what they're looking for inside JIRA. So my team is in charge of trying to
improve that experience and building features around the navigation and homepage to
allow people to find what they're looking for more easily. 

**Michaela:** [00:01:27] Is it also, has it to do with search? So, how you're
searching JIRA? Or is it mainly, really about how you display different informations?

**Charlie:** [00:01:35] So at the moment, what I know that I'm gonna be 
working on very soon is, when you load the first page of JIRA, 
there's like a "Your Work" tab. And what we want is, depending on 
your last activity in JIRA, we want to organize the homepage in a way that it 
will show you what you've worked on in the last few days or what you've searched.
So I'm not going to be working on specifically on a search bar, but we 
want to display the last information that you've been looking for, or the last 
projects that you've been looking at to help you remember what you've been doing 
in the last few days, because in general, we assume that if you have been 
visiting some some boards or some projects in the last few days, it is 
probably related to what you're working on right now.
So we want to make that easy to find when you load JIRA, the, you know, the homepage. 

**Michaela:** [00:02:22] Yeah, I understand. So it's really about the context 
that you have been in last time, and then you display information that's helpful for that.

**Charlie:** [00:02:30] Yes. Building features in a way that is easy to find for people, yeah.

**Michaela:** [00:02:37] That is really cool. So I know that within the six months,
a little bit over six months that you have been at Atlassian right now,
you already switched teams once. Um, have you seen differences between 
those two teams? How do you work? How they operate? What they, yeah. What 
software engineering practices do they have or has it been very streamlined?
Is it very streamlined at Atlassian? 

**Charlie:** [00:03:01] So, in terms of... well, the tech stack was the 
same and the process was the same because I was still on JIRA and I was still a 
front-end developer, but my previous team was supposed to be in charge of the 
analytics around the way people navigate JIRA, so understanding where people come from, where 
they go and to try and actually help redesign the navigation.
That was the purpose of the team. But then when I actually was in that team, we 
worked on something that was a little bit different. Sometimes it felt like 
we didn't really own a particular part of JIRA. So I think that's the main 
difference, whereas now, my work is a bit more clear, at least for me.
And so in the the team itself, my previous team was a lot smaller. We 
were around four people and we were only all developers, whereas now my team is 
a bit bigger. We're about maybe eight, nine people. And we have a designer with us 
as well that we didn't have before. So we're still a majority of developers, 
but, uh, now we have a designer, so I feel like we have more of a proper vision
of where we're going. So I think in terms of context of the team, it's a bit different,
but in the process of building software, we're all kind of doing it the same way. So that hasn't 
really changed. 

**Michaela:** [00:04:20] Okay. So it's interesting that you say that because you 
have different roles on your team—so for example, the designer—you have a more clear vision of where you go.
Is that because this other person brings on a different set of expertise that you 
normally lack, and now that you have access to that expertise or that input, 
you feel that that's making your journey more clearly, or...? 

**Charlie:** [00:04:46] Yes, definitely.
Because, well, now that we have a designer and maybe more product-focused 
people, we actually have a better idea of what we need to build or what 
our users would benefit from. I feel like when you have a team that's 
only developers, people might focus only on how to build the features, how to 
write the best code, not always how to actually write or build the right 
features for the end user.
So I usually like really to have people from different facilities because I 
feel like it brings different ideas. So having a designer is really 
important to me, because then we can have this person really think 
about the experience of the user, maybe get feedback before we actually build 
something.
So it is different in that way, meaning that I know that what we're building has 
been eventually tested with users, or we've actually been trying to think about 
what the users wants before going into building a feature. 

**Michaela:** [00:05:44] Mmhmm. And do you also have, like you said, product people, so 
do you have like product managers or product owners on your team as well?

**Charlie:** [00:05:52] So, I think our team lead has like a product mindset. So 
I feel like he's doing a bit of both. So we have proper tech leads in our team 
as well, but I feel like our team lead is more of the product person. So he's 
really focused on trying to figure out what we should build, what the roadmap 
should be. So I feel like it's a good mix of skills and of ideas as 
well.

**Michaela:** [00:06:14] Mmhmm. And so you said that the tech stack and the processes 
were the same because you have been on JIRA. So what is the tech stack that JIRA 
is built on? 

**Charlie:** [00:06:23] So, at the moment our tech stack is pretty modern 
actually, so we have React and Redux, like a lot of other products, but yeah,
so it's mainly React and Redux.
We are using Flow for the type system, but in some parts of the 
application, we also have TypeScript for our design system, so sometimes we 
have to switch between both. For testing, we use Cypress. We push 
everything to Bitbucket because we use our own products. And that's mainly it. 
Oh, we use Storybooks to make sure that our features, you know, we can see 
what they're supposed to look like.
Oh, and in terms of CSS, we use a bit of CSS-in-JS as well to organize our 
things into modules. And I think that's pretty much it. Like, we have a pretty standard 
tech stack, but it's quite modern, so that's nice. 

**Michaela:** [00:07:16] Okay. And so what about the processeses and engineering 
practices? So you talked about testing, so apparently you do automate the tasks.
Is there some rules about, you know, how much you should test your system? 
Should every unit have a unit test? What is going on there at Atlassian?

**Charlie:** [00:07:31] Sure. I think it's more about what you 
think is right to test. So, obviously we don't really want absolutely every 
function in your component to be tested.
It's more about what what is critical, what has a risk to break for example. 
Sometimes, for some components, we have some snapshots tests as well, but 
not all of them have it, cause sometimes it's not really beneficial. But 
it's more up to the developer developing the feature to figure out what they 
think is right to test. Personally, I like to test because it gives me a bit more 
confidence, but there is parts of the code base that don't have that 
much tests either because we had to deliver fast or because of the developer 
didn't think it was necessary.
I think it's more up to the developer. It's always better to have tests because 
we all review each other's code. So if I see that somebody added a feature
but they didn't test, then usually I comment on that PR and ask 
them, you know, maybe like, did you forget to add tests or maybe do you need 
some help to write some?
Because it's important to me, but I trust my colleagues to make the right 
decisions. 

**Michaela:** [00:08:41] Okay. So you said already code review. So code reviews is 
something that's standard in your development processes? Does this mean that 
every code change has to be reviewed? Are there some rules about how many people 
have to review that, or, you know, how many thumbs up you have to have, things 
like that?

**Charlie:** [00:09:02] So, I believe that every piece of code that we're 
about to merge has to be reviewed, from what I know of from what 
I've done so far, at least. And in terms of who gets to review it, 
personally, what I do is that if I am modifying a certain piece of code, 
I look at who was involved in the previous version of that component or in 
that part of the code and I'll try to add them in the pull request, because if
they've been working on that feature before, they might be the right person 
to understand what I've been modifying or what I've been trying to do.
But also, I'm always going to try to add somebody from my team, because if we're building
a new feature, people inside my team have the context about what I'm trying to change.
Usually, I try not add too many people, so I might need to add two or 
three, but then sometimes automatically Bitbucket is gonna assign more people to 
the PR depending on who modified the code before me. So sometimes I can add two 
of my team members and Bitbucket will see that I forgot somebody who modified the code 
before that might not be in my current team 
and it will automatically add these people. But in terms of approval, 
you need at least one person. If you have more, good, but it's not necessary, 
You need one person to approve to be able to then merge the PR. 

**Michaela:** [00:10:24] Mmhmm. And so I noted at Atlassian, you embrace Agile principles like 
continuous improvement and iterations and things like that.
Do you also strive for continuous integration and continuous deployment? And how long does 
code usually take from, you know, when you develop it—let's say you develop and test it on your machine—
how long does it take that it's really deployed in production and which steps are involved 
during that continuous integration or deployment process?


**Charlie:** [00:10:54] Sure. So we, we definitely do have continuous 
integration and deployment. We deploy to production, I'd say, at least once a day, 
I wouldn't be exactly sure about how frequent, but I think we do it as 
frequent as possible because JIRA is a very, a big application. I think we have 
more than a hundred devs working on the front end of JIRA.
So it means that every time I work on my features, I actually have a lot of 
other developers working on their own brunches. So it means that when I try 
to pull from master before I actually create my new branch, I actually 
see all the other branches and pull requests that other developers have 
created while I've been working on my parts.
So we tried to actually deploy and merge as often as possible, because that will 
reduce the risk of us breaking something. And if it breaks, then it means 
that we don't have too many changes that we have to look at if we break 
something. So we're definitely trying to deploy as often as possible. And in 
terms of how long it takes for a feature to go to production, it really 
depends on what you're working on.
So for example, in my previous team, when I was working on adding 
profile counts in the front end of JIRA. So what that was is when you hover over 
the name of a user, you can see a profile card being displayed with the avatar 
and the name of the person and the email if you want to get in contact with them 
or something like that.
And that actually took us a few months because we had there was some 
legacy code that was there that we had to clean up, and we wanted to 
create this package in a way that it would be easily reusable across the 
application, and we wanted to provide an API that was easy for other developers 
to add it to that part of JIRA or later on.
So it was a bigger restructure than other features that we can work on. So 
that took a few months for us from start to finish, because we ran into a few 
issues as well, but more recently there's been some tasks that I've had to do 
that were just cleaning up some feature flags that hadn't been cleaned up in a 
while, and that can be merged to production in a day, depending on 
if the feature flag is dependent on another feature or something. 
If it's quite isolated, it's pretty easy to clean up and you can get it 
approved in just a few minutes and you can then merge that and it could be 
deployed by the end of the day.
So depending on the size of the feature, the cycle can be quite fast. 
Otherwise it doesn't, even if you have quite a lot of review on your PR or even 
if it ends up being a change that's longer, nothing stops you from actually 
starting another ticket while the build is running, for example, 'cause that can 
take quite a bit of time.
So it's sometimes up to you to try to close as many tickets as you can, and 
maybe while one is building and is taking more time, you can pick up a smaller 
one just to try to get things rolling, basically. 

**Michaela:** [00:13:58] Mmhmm, mmhmm. And so, you said the build takes a little bit of time. 
Do you have an idea of how long it takes?

**Charlie:** [00:14:05] Yeah, sometimes it is quite frustrating, I have to say. 
So I think... I would say at least 40 minutes sometimes, which I think it's 
quite long, so I don't know if, maybe in other companies, it's actually not long, 
but it can be sometimes quite frustrating because as the application is pretty 
big, you rarely run all the tests locally.
So you might run the test of your little package that you've modified and you 
check that these tests are, you know, passing, but then when you actually push 
and it goes through the pipeline and, you know, you're running the build, 
sometimes you only realize that at the end of the build that you broke 
something in another component.
So it means that you only know, eventually, 40 minutes later that you actually 
have to go back and modify something. So sometimes it can be quite 
frustrating when you're almost sure that you're ready to open 
your PR or that you think that you're done, you actually only know the 
issue 40 minutes later.
So I guess it's part of the work, but that's why sometimes, 
I said that while the build is running, you can pick up another small 
ticket if you want, just so you can keep going instead of just, you know, 
watching the builds for 40 minutes. 

**Michaela:** [00:15:21] Yeah, yeah. Sure. Yeah. I think it really depends on the size 
of the software. So Microsoft also quite some substantial software systems and 
the build can take also quite long. So yeah, I know that 
problem. Well, something that I want to talk about, which I think plucks into 
that as well is manual testing. Do you know if they are manual testers
or are people manually testing the Atlassian software as well?
Or is that something that's really replaced by automated tests right now?

**Charlie:** [00:16:00] So, I haven't worked yet with somebody who 
was only, like, a tester or a QA person, but so far, what we've been 
doing is that, every time that we're about to merge a pull request, we actually 
have a little QA session with somebody else in the team where we go manually 
through the feature, and we look at the change that we've been doing. So, on top of 
having a review of just the code in Bitbucket, we actually do a manual QA face-to-face
with somebody from the team, because if I work on 
something, I would have built something a certain way, but I need a colleague of 
mine to maybe come up with an idea of, like, "Oh, have you tried this?," or
"Would it break if you do this?," and things like that. So I haven't 
worked with somebody whose dedicated role was to do that. But I think we all 
are responsible in a way for the QA before we merge something. 

**Michaela:** [00:16:48] Okay. Yeah, that sounds reasonable. 
At Atlassian, I heard that you have something called the Team Playbook and it's 
sort of the best practices of Atlassian for building high-performing teams.
Have you heard of the Playbook at Atlassian, and do you know that some of your 
colleagues or your team is putting some of those plays, it's called in there, 
to make you work better?

**Charlie:** [00:17:21] So, I have heard of the Team Playbook, but right now,
actually, I actually forgot the rules that are inside, 
so I feel like the Team Playbook would be more of a guideline 
rather than, like, practices that you have to follow.
So I wouldn't remember exactly what we have in the Playbook, but I feel 
like, team-by-team, we would kind of pick our own practices. I think, 
maybe in the Team Playbook—I don't remember if it mentions some 
retrospective meetings where we talk about how we've been feeling in the 
team, not only about the work, but how we've been 
feeling, how we can do things better in the next sprint or, you know, is there 
any concerns? So I think team by team, usually the team lead decides the practices that 
we're going to have and team members can also propose things. So we 
often have sessions where every week we kind of have, like, a tech 
meeting where we show what we've been working on, because, as we don't really pair 
program, sometimes we don't have the time to see what other people in the 
team have been working on.
So every week we have a session where people are able to showcase what they've 
been doing to share knowledge within the team. So I wouldn't really 
remember if this is part of the Team Playbook, but I feel like every 
team would be picking whatever practices they feel more comfortable with, 
or they feel would be beneficial.


**Michaela:** [00:18:52] Mmhmm. So you worked, before joining Atlassian, you've worked 
actually at smaller companies first. What do you think are the differences you 
experienced in joining this larger enterprise? Do you see some differences 
how the organization operates, on how teams work together and things like that? 

**Charlie:** [00:19:09] There's definitely differences.
It's been really interesting to explore different environments 
because before Atlassian, I was working for a consultancy, so the nature of the 
work was quite different because instead of being really involved in one product,
I basically was assigned to a team every few months. Sometimes it was only a three-months project,
sometimes it was six, sometimes a year. It means that when you join a company to help 
them for a few months, you're not really part of their team. Like, you ended 
up being responsible for a part of a company's product, but you're not really, 
really part of the team. Like you help them only on the small parts.
So usually I worked on codebases that were way smaller. A lot of the times, 
we were sometimes starting something from scratch, which is very different 
from working on a codebase that has been there, you know, for more than 10 
years. And as a consultant, we were building teams that had 
sometimes more diversity in terms of roles.
So with the consultancy I was in before, it was rare that we only had one designer.
We usually had a couple of UX designers, we definitely had testers, we 
definitely had product managers, and the team was really diverse in terms of 
disciplines, whereas Atlassian is very often more technical.
But the main difference and the main challenge for me has been the size of the 
codebase.
JIRA has more than a million lines of code. So it's been quite different to go 
from a monolith front-end in JIRA or coming from more microservices when I was in 
a consultancy. So it's been really interesting to navigate these different 
spaces. But I like the fact that, in a product, I get to dive deeper into the 
codebase and be part of decisions that are supposed to be long-lasting, 
whereas consultancy, you try to help a company and you try to help them make 
long-lasting decisions when, in the end, they decide what they want to do. You're just here to advise 
them and do your best. But in the end, when you leave to go and help another 
company, they kind of decide what to do, and sometimes it feels like you 
don't really see the end of what you're building, because you're only here temporarily.
Whereas, at Atlassian, on a product, you know, you're supposed to 
make every decision knowing that you want it to last and you want it to be 
performant and helpful because it's going to impact the product in the long term. 

**Michaela:** [00:21:42] And so when you consulted those companies where you're 
sitting with the teams, would you go to Company A, for example, and then really 
sit with their team for a stretch of several months? Or would that be a remote consultancy
gig that you have there? How does that work?

**Charlie:** [00:21:55] So we were usually going into the 
company's offices and we were working with their developers and their product 
managers. So we were really with the team. So we were really trying to not only
build the software, but also understand their businesses and their, you know, 
their struggles and things like that.
So I think it was really interesting because it wasn't only coding. It was 
really being a consultant, so really trying to understand what pain points a 
company was having and how to solve that with software. And I 
feel like it has helped me. I think it's really quite beneficial to 
change environment.
So that's why I like it because then you really develop your 
communication skills because you probably write code maybe only half the 
time because the other time either you're upskilling the company's 
developers into a new tech stack that they haven't worked with before, or you're 
really trying to, you have to sometimes explain to people who are non-technical about why
maybe you're not shipping features as fast 
because you're making long-lasting changes. It's really been 
interesting because you're not only coding.
You're also advising people on their business and trying to make them 
understand the challenges of technology. Whereas at Atlassian, most of the 
people I talk to are quite technical, so the conversations are a bit different, 
but I do think that the background of having worked as a consultant is really 
helpful because it pushes me to really make sure that I explain things in a 
way that everybody can understand—that you don't have to be technical to understand what I'm 
trying to say. So I think that's a very important skill. 

**Michaela:** [00:23:40] Yeah, I think so too. So how come did you change 
from this consultancy to Atlassian? Can you tell me a little bit about why 
did you choose that company, about how did you apply and how did that interview 
process go?

**Charlie:** [00:23:54] Sure. So, to me, the main reason was that, I think it was because as a 
consultant, I didn't really feel—I couldn't really know where my work ended 
because you know what you're doing for a certain period of time while you are 
with the company, but as soon as you go and help another company, you don't 
actually know if the company decided to rewrite the codebase or if they 
gave up on the project you were working on.
So I wasn't really able to say, you know, "I built this," or "I helped these 
people" because once you're gone, you don't always know what they 
decide to do. So in terms of knowledge, it was quite broad, so I experimented 
with a lot of different environments, but in terms of depth, I didn't really 
have the opportunity to go deep into a product and technology.
So that was my main motivation for moving on and going to product, because 
I know I knew that it would be an environment that wouldn't change. It 
would be more stable for me to go deeper in a code base and try to refactor 
or work with more legacy code and understand how to make more impactful changes.
And in terms of why Atlassian, it is one of the main tech companies 
in Sydney here, and I was interested in the fact that it is a product 
that is used by millions of people. So every change that you do, even small, 
is going to have an impact that is quite big. It also means that, in terms 
of challenges, every time, even if it is a small change, if you 
break something, it also has an impact.
So there is quite a lot of challenges in terms of performance, making sure 
that everything that you add on the codebase is not going to make JIRA slower 
than it is, for example. So that was really something that I was quite 
excited about, knowing that I would be really something that a lot of people 
use. And in terms of interview process, it wasn't super long. I think they 
shortened the hiring process because they're hiring a lot. And I think in tech 
at the moment, a lot of companies are trying to shorten to make sure 
that they don't lose the talents because, well, you know, you know how 
interviews go.
If a company is too slow, you might pick another job. But in 
terms of steps, it was a phone call with the recruiter—I think that is 
quite standard—but then instead of having a code test that you take home, 
you actually have to go to the office and you were live coding in front of 
somebody.
So I didn't know what the test would be before I went to the office, but so 
I went to the office and I met the developer that would be pairing with 
me. We're not really pairing, but he was available for questions. And then 
they show you the tests that you have to do, and you had an 
hour to go through tasks in a readme and code it live in front of the person.
And the developer that was with me was available to answer some of your 
questions if it wasn't really clear, and he was observing what I was doing, 
writing some notes and you have a few minutes at the end to explain what you 
would have done better because obviously in an hour you don't have the time to 
write the best code.
The goal of this interview was not to write the best code ever. It was just 
to see how you would go about solving a problem, and if you're then able to 
reflect on what you wrote and explain what you would have done better. So for 
the code test, that was that. And then if that goes well, there 
is a another technical interview where you meet with two 
developers, and it's more about talking about a project that you have worked on recently, 
where you were really involved in, so you can explain it quite deeply. 
So you spend quite a lot of time explaining what you were involved in,
the tech stack, the decisions that you made in that 
project, again, what you could have done better and things like that.
And then there's some, uh, what, for me, it was frontend technical questions. 
I think pretty basic interview questions. They were a bit more 
around React because they use React a lot, so the questions were React-related 
and there was also a very small whiteboard exercise, not at all algorithms 
and data structures, so it wasn't the scary things. But it was a JavaScript 
question where, you had to write a certain function on the 
whiteboard and explain what you were writing. And then finally, if that 
goes well, you have an interview with two managers of teams that are 
looking for people where you can get to meet your potential 
future manager, and it's more of a cultural interview where you get asked about a 
time where you had negative feedback and how you reacted or a time where you had 
to give constructive feedback and how you went about that, 
and what you like about technology, what you're interested in, and things 
like that.
And then you get to ask your questions as well about the different products or 
the parts of the teams that are hiring basically. And that was it. So it's kind 
like four steps.

**Michaela:** [00:29:09] And they are all in one day??

**Charlie:** [00:29:10] No, no, no, no. I mean, maybe you can do 
them in one day. I haven't tried that. It was pretty short. So I think I did them over a month,
so maybe once a week, because at the time when I went through the interviews, I had to work in 
another city, so I couldn't always physically be in Sydney, but I like to do 
interviews face to face. So I just asked them to sometimes delay some of the 
interviews so I could be in Sydney.
So I'm sure that you could do the interviews remotely—
I think they're hiring a lot of people in other countries that they then sponsor 
to come to Australia, so I think a lot of people do the interviews probably 
on Zoom or on Skype or something, but they're pretty flexible and they
go quite fast because I think they want to make sure that they don't miss out on talent.

**Michaela:** [00:29:56] Okay. So when you tell me about the live coding event, 
I get all kinds of anxieties, to be honest.

_[laughing]_

**Michaela:** [00:30:06] _[unintelligible]_ ...computer, and then somebody's looking 
over my shoulder with this, you know, I would probably forget where the different keys are on my
keyboard. So how was that for you?

**Charlie:** [00:30:18] So I'm very nervous as well when that 
happens, because I feel watched and judged and, you know, I'm like nervous, but I 
tried to switch the way I was seeing it,
and I tried to see it as a challenge for myself. I tried to forget that the 
developer was watching me, and I tried to calm down, and I tried to 
tell myself "If I don't get the job, it's fine. There's 
other companies and there's other jobs. It's not the end of the world. And if I 
can't do this contest, then it doesn't mean that I can't reapply later."
I tried to really downplay how important it was 
for me, the impact. Yeah, so I was fine, because then I could then focus on the 
code rather than focusing on how nervous I was. But also the developer 
who was with me was really nice and quite chill, so he didn't make me stress at all.
I think he even told me, like, "It's okay, take your time. If you have questions 
I'm here." He didn't make me stress out at all, so I think that definitely 
helped as well.

**Michaela:** [00:31:28] And so when you were coding that, would you be able to open Google 
and look something up or didn't you dare to do that or was it so clear that you could 
actually stay in your IDE?

**Charlie:** [00:31:43] I think I did Google something because I think I forgot how to, 
there was something quite basic that I forgot. I don't remember right now 
what it was, but I think the developer who was with me 
told me that I was allowed to Google. I think it was more about, if you Google 
something, maybe say out loud what you're Googling and why you're 
Googling it, because they know that, I mean, Google is something that we use a lot in 
our job. We can't pretend that we—I don't think I spend a day 
without looking at Google. You know, I probably look at Google every ten minutes. 
It's more of a understanding how you work. And I 
wouldn't want to pretend that I know everything because it's not true,
so I wouldn't pretend that I just wrote everything 
without looking anything up in a real-world scenario...

**Michaela:** [00:32:41] You also would do that, right?

**Charlie:** [00:32:44] Yeah, yeah, definitely. And I think it's more about, well, if you want to 
solve a certain problem, what would you Google? And it's about, you know, 
seeing if you can efficiently Google maybe as well. But yeah, no, I did use Google.

**Michaela:** [00:32:56] Yeah. Okay. So, um, I know that besides the things that 
you do at the company, you also have quite a few side projects and they are in 
very interesting areas. I call them brain-controlled interfaces. I think you call them the 
same. And you're also tinker with various electronic devices, right?
So why do you do that? Why do you invest your free time in looking 
at something that's actually not one-to-one related to your current job and your 
career?

**Charlie:** [00:33:28] Well, first of all, I think it's 
because it gets me really excited. I am definitely very passionate 
about the way people interact with technology, and brain–computer interfaces is one way of doing that. 
But also, because I feel like I'm learning a lot while I build these side projects, and when I'm at work, 
I learn about certain frameworks or certain tech stacks or certain ways of building a website.
But I feel like technology is so much more than that, and in a way you don't really know where it's going. 
So I like exploring different parts of the tech industry, because, well, 
right now I'm building JIRA, but I don't know what's next. It gives me a better 
idea of what's going on or what the future might be as well.
And it's a field that is, well, to me so, so interesting. When we look at the 
way we usually interact, like the keyboard and the phone is so 
restrictive. It's like we've learned to type on buttons to do something, but 
there's probably so many different ways that we could interact 
with things that that could maybe be faster or be more intuitive.
And I feel like a lot of the times, we've had to learn how to use the 
keyboard, whereas technology could actually adapt to people in the natural 
environment and it would almost, you know, do things for you, 
but there is a way that you would forget that the tech is here, but it 
would just do things for you and make your life eventually better.

**Michaela:** [00:35:05] So I just said brain-controlled interfaces, but I watched some of 
your YouTube videos and I read some of your articles and what's actually 
happening is that based on sensors that are on your head, right, you can 
move for example, the mouse, or you could navigate a cube in space somehow, right?
How would you describe that, brain-controlled interfaces? 
What are those for you and where do you see them going? 

**Charlie:** [00:35:37] Well, I'm not actually sure where it's going, 
but what I think is that it is going to get a lot better than it is now. And I don't 
think it will take that much longer, but what I mean by that is, as I've 
been working on building some prototypes, I have a better idea of what is 
possible and what is not possible.
And at the moment, you can train some machine learning algorithms to 
identify patterns in your brain activity that you can then match to a certain 
thought. And then, using that thought, it's really up to you to build whatever 
interaction that you want. Like, if you train an algorithm with your own 
thoughts, then you can use that as triggers, but it could be moving a mouse,
it could be playing a game, it could be instead of using voice 
control, you would use thought control to start a playlist or post a 
YouTube video or anything. But at the moment, most of the experiments that I've 
seen have been using thoughts of a body movement. I feel like this is maybe 
where it's easier to identify patterns in info.
So the one that I've been playing with personally, like, I have to train an 
algorithm to recognize maybe a direction. So I was thinking about moving 
right or left, and then I was matching that with a motion on the screen as well, 
but recently, actually last week, I went to Mountain View for a 
Google Developer Experts Summit and I caught up with a friend who is the co-founder
of a startup called Neurosity, and they're building their own brain sensor as well. So it's a new 
one that will be available soon, and I tried it and it was really, really 
exciting. And I saw that what I trained with it as well was also body movement.
So I had to think about pinching my fingers or tapping my left foot on the 
floor, and as I was just thinking about these movements, I could then 
find patterns in the data and map that to something on the screen as well. 
So, so far I feel like what is doable is thinking about a body movement or
a motion in space, and that is easier to find patterns then, in the data. 
But what is, I think, not possible yet is to think about random things like a 
bottle of water or the beach. I think that these kinds of thoughts are not 
precise enough to be able to detect any kind of patterns. I might be wrong, though. 
What I've seen so far, it's easier with thoughts of movements,
but I feel like as the technology is going to get better in terms of 
hardware _and_ software, I don't think we are that far from being able to interact 
with interfaces using brain sensors. But I think that we have to be a 
little bit patient that we're not going to be able to detect everything.

**Michaela:** [00:38:30] It's really, really interesting. And the funny thing is 
that when you said, okay, you're thinking about something, a thought, and then 
you map that, right, to an activity and that will become your trigger. 
The first thing that came to _my_ mind is thinking about mice or elephants, you know?
And then you say, well, actually it has to do more with motions, right?
So I found that really, really interesting. I would like to learn more about that.

**Charlie:** [00:38:56] Yeah. 

**Michaela:** [00:38:57] I wonder if it has to do with the region of 
the brain that you trigger because maybe a mouse thought is somewhere else located,
than you're moving your hands or something. 

**Charlie:** [00:39:09] I think, yeah, I think it has to do with the amount of 
focus that you need as well for a certain thought.
Definitely the part of the brain that, let's say, you know, lights up when 
you think about when you think about movement, but it's—I read something a 
while ago, but I wouldn't be a hundred percent sure, but I think that it's 
because the region of the brain that is in charge of thinking about movement 
creates patterns or activity that is more similar between people than our random thoughts,
because maybe if you think about an elephant or a mouse, you might be attaching 
some kind of feeling or memory or experience to that particular thing that 
you're thinking about. Whereas a movement, I think is more selective, like you're only 
thinking about that movement. I don't think there's any other thoughts 
that you are doing at the same time. When I tried the Notion—so, the Neurosity headset—
it was quite difficult for me to focus and to train it because we 
were in a room where people were having lunch,
and I had two people on my side who were having—so, my friends were having a 
conversation while I was trying to train the patterns, the thoughts,
and it was actually quite difficult. So I think, even if I was 
thinking about motions that are quite specific and selective, I still 
had all this noise because I was listening to conversations from my friends,
so it was very hard for me to focus. So I think that's also one of the 
limitations that we have at the moment with brain sensors, is that when you train 
them, usually you have to be in a quiet environment when you can focus on that 
particular thought of movement. That's why sometimes when I was demoing
things on stage, it's very different than when I'm at home, because when I'm 
at home, no one is watching me and I can just focus on that.
Whereas on stage, I have other thoughts that go through my mind, like "Everybody's 
watching me." And every time you have only one 
second of silence, it just feels like forever. So yeah.

**Michaela:** [00:41:10] Yeah, I can, I can see that. I also read that, for 
example, the brain part that's responsible for the motions is actually one of the 
most powerful ones. So for example, the geniuses that can calculate and count up or
have a square of an unbelievably large number and do that in their head, they 
actually calculate with a different part of their brain than we normal people do, right? And 
it's connected to the movement part.

**Charlie:** [00:41:41] Oh, wow!

**Michaela:** [00:41:43] So they can calculate with that part of the brain.
Yeah. Anyway, so that's why I find that really, really interesting. I have to 
look that up more, read more about it. Yeah, I really see why you deep dive 
into that during your free time.

So, one thing that you also said that I wanted to pick your brain. You talked 
about the Google Dev Summit, and I know that you are a Google Developer Expert
and you're also a Mozilla speaker.
And I would love if you could share with me and also our listeners, obviously, 
what it takes to become one or the other. I know there are two different processes,
so maybe let's start with the Google Dev Expert. How can someone become a Google Dev Expert?
What does it take?

**Charlie:** [00:42:24] Right. So, to become a Google Dev Expert,
you first have to be referred by somebody who is already an expert.
So there's kind of no way to get in it if nobody refers you. But once you are referred—
so if you go to an event and you meet another Google Dev Expert and you can ask them to refer, you. But what it takes to become one is that you have to be able to show certain activities that you've done for the community.
So that could be the number of blog posts that you've written 
or it could be that you're running a podcast. That's a community activity.

**Michaela:** [00:43:03] Oh, yeah! Good for me! Yay!

**Charlie:** [00:43:09] It could be the talks that you've given, or if you ran workshops
or if you're a coding teacher or something. So any way that you can show that you've 
shared knowledge with the community counts as activity that they can take into 
consideration to know if you're going to be a Dev Expert or not.
So, yeah. So you'll have a first interview where you talk about your activity 
and you have to kind of fill a form where you add everything that you've done.
And the second step is an interview with a Google employee 
where they ask you a bit more questions about your activity and also some 
technical questions related to the field that you picked as a Google Developer Expert.
So my field is web technologies, but there are 
experts in Android, IoT, machine learning, Angular specifically. So, when 
you apply, you can pick the field that you want and your interview will 
have questions related to that field. So there's only two steps of interviews:
one more related to your activity and one with questions related to the topic 
that you picked, and once that's done, then you join the program and 
you're going to be part of mailing lists and yeah. Things like that.

**Michaela:** [00:44:23] Okay. Cool. And then also a Google  Developer Summit
where people get together. Is that per continent or per city, or how frequent
are those summits and where are they located?

**Charlie:** [00:44:33] So the summit I just went to, I think it's a yearly one,
and I think it is always in Mountain View cause it's in the Google offices. 
And it was people from around the world, but I don't think it is every expert.
I think this time we were about 450 people and I think everybody gets an 
invite, but then, you know, people can't come that weekend, so you know,
not everybody will be there. But it is experts from 
different disciplines as well. So this time, there was a 
lot of Android experts. There was quite a few web technology experts. I 
don't think there was any IoT experts, but there were some machine learning 
experts.
And, in this summit you have talks from both Google employees and also other 
experts. So as an expert, you have a chance to actually share your knowledge 
with other people from around the world as well. 

**Michaela:** [00:45:33] Yeah, that sounds really nice. And what about the 
Mozilla speaker that you are? 

**Charlie:** [00:45:40] Yeah, it feels weird that I'm part of both,
but I actually went through the process at the same time, 
so I didn't actually plan on doing both. I mean, I'll probably get one of them 
and I got both, so yeah. But the process for the Mozilla Tech Speakers is,
there is actually an application. So you don't need to be referred.
I think once a year they open up applications. I think usually they tweet about 
it. They say, "Oh, if you want to be part of the program, fill that form," 
and then they select people, again based on your activities. So 
I think you have to also report what you've been doing and also why 
you want to be an expert because it's not a job, you're not paid.
It's really just about if you are passionate about being with 
a group of people who love the same things as you, and who are as 
passionate about sharing knowledge as you are, then, you know, this is a good 
group for you. So you fill a form and then you either get selected or not.
And if you do get selected, there is a little training program with people from 
the same region. So when I got selected, we had a few people in Australia and Asia as 
well. We were on the same call where you had current Mozilla Tech Speakers 
telling you what the program is about, and you had a bit of homework 
where you had to write a draft of a talk that you might give, and then everybody gives 
feedback to each other.
So that was really nice because it was just kind of, like, showing you how to 
write a proposal for a talk, and then you get feedback by different people. And I 
think it was over a few weeks—I forgot how many weeks exactly. But you just had 
to make sure that you could join that call. And if you couldn't, it was fine
and you were not kicked out of the program.
But it is better if you join the call so you get to meet people 
already and you get to share ideas, and then we know we're all part of a 
Telegram channel, you know, the app on your phone. And we get to 
chat quite often. And so the process was a bit different. It wasn't 
truly interviews. It was more chats. So yeah, basically that was it. 

**Michaela:** [00:47:50] Yeah. So one of the things I wanted to process if 
you're now in Sydney, but I know that you have been living in Paris as well. So 
how comes that you are 
**Charlie:** [00:48:00] in Sydney? Um, it's much better. It's
so well, I moved to Sydney about eight years ago. Um, so that that's been quite 
a while now. Um, but I think so at the, at the time I was not in tech, I was in 
marketing. I was finishing my master's degree. And as part of, um, as part of 
that degree, I had to either do an internship in an agency in Paris or a 
semester abroad in a university that was partnering with my school at the time.
And I had done internships before because, um, In France. I didn't really do 
uni, but I did more of a school that was, um, like we had to do internships 
quite, uh, quite often to build that kind of like a professional, um, portfolio 
kind of thing too, then get hired 
**Michaela:** [00:48:53] dead, like a Polytechnical. 
**Charlie:** [00:48:54] Um, so it was. It's I think it works differently between 
different countries.
So I wouldn't really know the equivalent in other countries, but it was a mix of 
lectures and a mix of actual professional, um, experience. So, so I had done, 
yeah, I had done internships before, so I was thinking, well, if my school is 
willing to send me somewhere, then yeah, I think that opportunity. Yeah. So, um, 
I totally get it.
So I decided to, um, to pick Sydney because it was really far, uh, and I wanted 
to go quite far
it's on songs like that, but, uh, I, I just, yeah. See the other side of the 
book. I just mean it. I might not have the opportunity, you know, to go. Um, to 
Australia every day. Um, so I picked that and then I love, and I basically 
started working here and yeah. 
**Michaela:** [00:49:52] Yeah. That's really interesting. Yeah. I can see it. I 
mean, I did, um, during my masters, I also did.
Yeah. An Erasmus was called Erasmus term. So I went to London and based on that 
I had experience, I traveled the world because I also want 
**Charlie:** [00:50:07] to see everything 
**Michaela:** [00:50:09] that's out there so I can see. And so now you're 
feeling that you are, that you are going to stay in Sydney or are you going to 
come back 
**Charlie:** [00:50:16] to Europe at one point?
Yeah. At the moment, I'm not. I'm not sure because you know, after eight years, 
sometimes things. Uh, like, you know, what you want in, you know, in your life 
or things like that change. So I'm, I'm actually not quite sure at the moment. 
I'm actually thinking about what I want to do with my life, you know? 
**Michaela:** [00:50:34] Yeah.
It's a constant Todd 
**Charlie:** [00:50:38] that I have 
**Michaela:** [00:50:38] every morning that I wake up. 
**Charlie:** [00:50:40] It's like, Oh yeah. 
**Michaela:** [00:50:43] Yeah. 
**Charlie:** [00:50:44] Well, so. 
**Michaela:** [00:50:46] Charlie. I think we covered a lot. Is there something 
you want to talk about that we haven't covered yet? 
**Charlie:** [00:50:53] I don't think so. I think we did cover a broad range of 
topics. It was, it was really cool. It was really interesting.
Yeah. 
**Michaela:** [00:50:59] Yeah. I really enjoy talking to you. Thank you so much 
for being on my show. 
**Charlie:** [00:51:03] Thank you so much for having me. 
**Michaela:** [00:51:04] Yeah. Thank you. Bye bye. 
**Charlie:** [00:51:06] Bye. Bye. 
**Michaela:** [00:51:08] I hope you enjoyed another episode after sup 
engineering unlocked podcast. Don't forget to subscribe and I talk to you again 
in two weeks. Bye.


