# Transcript Episode 3 with Leif Singer

**Michaela:** [00:00:00] Hello, and welcome to the software engineering unlocked 
podcast, where I talk to experienced developers from different companies about 
how to develop software. I'm your host, Dr. McKayla, and today I have the pleasure to 
be talking to Dr. Leif Singer, who is a software engineer at Automattic. I'm 
really excited to have Leif here today to hear how his life is at a fully remote 
company. Leif is like me passionated about improving software engineering, processes 
and tools. 
His specific interest is understanding how lightweight processes can help to 
collaborate better. He has a PhD in software engineering, but is also a science 
fiction writer and a musician. So I'm thrilled that Leif is here today. Leif 
welcome.

**Leif:** [00:00:44] Good morning, Mikayla. Thanks for having me. I'm good. 
Thanks. 

**Michaela:** [00:00:47] I'm glad that you're here. So life let's start at the 
beginning. We actually met when we both were working and living in well, 
beautiful Victoria in Canada, precisely at the university of Victoria, where you 
worked as a postdoctoral researcher.
Now we live in Germany and work as a engineers of engineer at Automattic. That's 
quite some change. So yeah. Why did you change from academia to industry and how 
did you start working at automatic? 

**Leif:** [00:01:13] Wow. Okay. You're you're studying with the tough question. 
Interesting. So do you know that, but not everyone might know that a postdoc 
position is a research position at a university that is supposed to prepare you 
for the job hunt for a professorship.
Right? So, um, I did the post doc because I thought I wanted to become a 
professor. But when I worked as a postdoc with, um, Two supervisors who were 
themselves already professors. I realized that academia was after all, not for 
me. The amount of time that I saw my superiors and my colleagues to put in far 
exceeded what I thought was reasonable.
So they, they, they loved their jobs. So they worked on weekends and things like 
that. Right. And I, as a father of a young family, I didn't see myself. Doing 
that regularly in the near future. And that was first thing that crossed my 
mind. And then a few other things came together with us living in a, in a 
different country, far away from home with no support network of our own with a 
small son.
And in the end, we decided to cut. Postdoc short at one year and moved back 
home. 

**Michaela:** [00:02:35] Okay. So it was actually supposed to go longer. Yes, 

**Leif:** [00:02:38] it was supposed to take two years, but I talked to my 
supervisor and she was all right with me. Cutting it short for one year. 

**Michaela:** [00:02:48] Thanks that you also addressed a little bit, was like.
That you were living in a different country. And I also traveled and lived in 
different countries over the time, but I always had the feeling that I couldn't 
choose it. But at the point that you so want to become a professor, it's somehow 
out of your hands a little bit. It's not like you can say, well, I want to 
become a professor in Germany.
That's really a very 

**Leif:** [00:03:10] difficult. Right. You can't be choosy at that point. You 
have to just move where the jobs are. Yeah. And that was definitely part of our 
decision. 
**Michaela:** [00:03:18] I totally understand that. So then you made this 
decision and what happened next? What was the next thing that you went on to do 
after your posting?
**Leif:** [00:03:27] I didn't have a plan. So I looked for a job and I found a 
remote job at a small company called I done this. And it's a small app. When I 
joined, it was me and four others who are on that app was really small based, 
mostly in New York. I worked there for, I suppose, one and a half or two years 
almost when.
The founders at some point, decided that they want to sell the company. And 
that's when I started looking for a new job because the buyers didn't want to 
bind the team, only the product and the customer base. 
**Michaela:** [00:04:09] It's a bummer, probably if you put part of your heart 
in there. 
**Leif:** [00:04:12] Yes. Yes, definitely. It was a bummer, but in the end it 
turned out that automatic were some of our customers.
So I got an intro from our CEO to one of automatics, basic, basically the person 
who managed the automatic account. And that's how I even thought about applying 
an automatic until I find about this company. So in the end, it turned out to be 
a nice circumstance. So 
**Michaela:** [00:04:42] when you were interviewing Dan for automatic, did you 
have like the skillset that was needed for that position or did you have to 
adjust there?
**Leif:** [00:04:50] So automatic is the company behind wordpress.com. And as 
such, I externally I would have assumed that you need to know PHP and WordPress 
development. I had not developed a single WordPress plugin or theme before 
applying. I did have a few years of experience with PHP when I was doing my 
bachelor's at university, I basically worked on the side as a PHP freelancer, 
but when I went through my trial, automatic, you go through a trial over the 
course of one or two months where you work on.
Basically a real project. I worked on a react app that was not released at that 
time. It is now it has now been released as the front end or, well, the 
administrative backend for wordpress.com. So. Pretty much a replacement for the 
WP admin, part of things written in react JS with Redux, um, server side 
rendered with node, lots of buzzwords in there.
And I had never heard of anything from those technologies before I started 
working on that, but that was also part of the process. I believe of the trial 
process to see. How I learn how I adjust to new technologies and things like 
that. What kind of questions I ask? 
**Michaela:** [00:06:11] It's really interesting. So you started with this, 
maybe let us look at a little bit at this trial, because I think it's very 
specific to automatic how they hire, right?
Sure. But once you explained that, maybe look at that you actually started that 
without prior knowledge of the technology. I think that's really mind blowing 
somehow. I really liked that concept, but yeah, it can be frightening. I 
**Leif:** [00:06:32] can imagine. It really was. And actually, I don't think 
it's that common so I can see someone of what current trials are working on and 
it's much more.
Matched to their skillset. So I suppose I got lucky in an earlier time of the 
company where that was possible right now. I think we are trying to standardize 
a bit because we really need to scale up hiring. And that is much easier when 
you have one approach that works. 
**Michaela:** [00:07:04] So how does this such a trial look like at automatics 
right now, if I want to have a job at automatics, what do we have to do?
**Leif:** [00:07:09] Right. So at first you send an email, you, or it might have 
changed, actually, maybe you fill out a form, we're starting to use the tool for 
managing those applications as well. Anyway, you're right in with your CV and a 
cover letter. And at some point, hopefully soon you rear back with hopefully a 
yes, we'd be interested.
And then you do an interview over text. So. I believe we use Slack nowadays, you 
get invited out. Yes. It's a text chat. And you basically talk for, I it's about 
an hour where you're being asked about your career, about some technical things. 
So it's basically a screener where we try to figure out whether it would be a 
good match thinking wise technology wise, things like that.
If that chat works out well. You get invited to do a small project that should 
take, I don't know, the actual times right now, but I think it's about four or 
five hours that you need to put in over a week where you get a small piece of 
code that you are supposed to improve with specific instructions.
Hey, is this code secure? Um, what if we add this and that feature, could you do 
that? Things like that. And that's, I think we call that a code test. But if 
that works out also, then you get to do a trial, which can take anywhere from 
one month to two months. Some I've also taken longer. You get assigned a, a real 
project that we really want to use.
And sometimes you're part of an actual team. You get to know a few of your 
possible future colleagues. And we basically look at how you, how you write 
code, how you communicate, how you. React in the face of challenges, how you 
scope things, things like that. If you feel it's a very wholesome picture that 
began of the applicant, it is paid.
Add a flat rate of $25 per hour for everyone. It has no, it's no indication of, 
um, your future pay. But it's the same pay for every role at, during that trial? 
The trial should be doable well, putting in five to 20 hours per week, I 
suppose, I think I put in about 10 hours per week, which can be a challenge if 
you're working and maybe have children, we try to, um, accommodate as many 
people 
**Michaela:** [00:09:40] as possible.
Sounds interesting. So I'm working alongside the team that I will probably work 
afterwards. 
**Leif:** [00:09:46] Well, maybe, maybe it's not, that's not definitely, but you 
will work with other automotive or automatic employees. And 
**Michaela:** [00:09:57] then I will do daily tasks that are needed for a 
position actually at that team. Right. So I really do what day would expect 
**Leif:** [00:10:05] me?
Yes. And you will write code that if it works out well, will probably be used in 
production. Yeah, 
**Michaela:** [00:10:13] I see. Well, I actually used throw you a little bit in 
the deep end, right. With the whole hiring processes and things like that. And 
that's actually not your role, but I think it's always interesting to see a 
different ways of entering a company.
Yeah. 
**Leif:** [00:10:26] Yeah. I agree. And it's one of the, and it's one of the 
interesting, more interesting parts of the company where it can see how it 
scales. 
**Michaela:** [00:10:34] Yeah. Because it's very different, right? Yeah. Yeah. 
But yeah, coming back to software engineering, add automatic. So you talked 
about react and no Chaz and things like that.
What is the tech stack? So if I want to apply there, or what do you have to 
bring to the table to be able to, 
**Leif:** [00:10:53] it depends on the role. Of course, there's different still 
description and the different job postings generally. Um, for. Code it would 
help if you knew, um, PHP, WordPress, JavaScript react and yeah, pretty much 
that, but around that, there is always ecosystems of other technologies, edge 
adjacent technologies that will also be helpful or useful for you, you to know.
Right. So. For example, one project is based on GitHub and it's written in react 
JS. It's a huge app, um, uses redox as a store and we, um, we have proper, um, 
continuous integration there. We have unit tests and integration tests and 
Denton tests and whatnot. And then another project, um, uses, um, subversion. 
And PHP and WordPress, and that's pretty much it.
That's all the technologies you have available to you. So it, it can differ or 
it can vary a lot. So it helps if you come to it with a certain generalist 
attitude, I think. And if you can learn, then I think you already have the most 
important skill. So, 
**Michaela:** [00:12:22] what you're saying is also that you're maybe moving 
within the company.
So if I let's say I started, they get project that you just mentioned, and then 
it could be that I'm actually moved or I want to move. I don't know. What 
exactly happens to different 
**Leif:** [00:12:35] projects. So I started out working on the react app, which 
was very interesting with all those new technologies and everything right.
Using get is always very pleasurable experience and that is without sarcasm. But 
at some point I wanted a change of scenery. I wanted to learn other things that 
I had not learned about before. Um, so right now, um, How that works usually is 
huge. Just send a private message to Matt and tell him. I am looking to change 
teams.
Um, I'm interested in these, in these things. Can you take a look and then after 
a couple of days, he gets back to you and tells you that sure. We might have a 
position open and this team, what do you think? And that's how he started the 
process of switching a team internally. So now I work on the marketing team 
because I thought that being a developer and knowing something about marketing, 
that sounds like I'm like a super power combination, you know, like.
No, no. Knowing how to market a product that you can also build. So right now 
I'm really in the depth of that, um, specializing a bit now, um, I'm a project 
lead for affiliates and partnerships where we basically give people a commission 
if they refer customers to us. So that's what I've been doing. And the past 
months, I guess, 
**Michaela:** [00:14:03] I really find it an interesting approach that you send 
an email to all the CEOs 
**Leif:** [00:14:08] in an email, we don't use email pretty much.
So it's a Slack DM Slack message. 
**Michaela:** [00:14:15] And then he probably asks around for you or talks with 
leadership somewhere else. And you figure out where and how that could be. 
**Leif:** [00:14:23] Exactly. And he also talks to the hiring team because those 
are the people who naturally need to have good understanding of the open roles 
that we need to fill.
**Michaela:** [00:14:32] I guess that this process looks different from other 
companies because you are a fully remote company, right? So you can not bump 
into somebody at the water cooler and tell them, well, you know, actually I'm a 
little bit interested in changing 
**Leif:** [00:14:44] teams. Well, you can do that too. Um, so, so when you've 
worked on a few teams, you will know a few people around the company who are 
maybe not in your current teams.
So, um, so you can also use those connections, um, to figure out where there 
could be a good match for a new team. 
**Michaela:** [00:15:03] And, but how do you keep contact with those people? Do 
you use Slack for that or do you sometimes hang out somewhere in the cyberspace? 
**Leif:** [00:15:14] So we, we use Slack for the more synchronous communication 
needs.
Most teams have weekly calls. Most people will have a weekly one on one call 
with our lead. And those would usually be a video calls. We do have a, a company 
wide town hall once a month, where Matt basically hosts a huge call and talks 
about what's going on in the company that's month. And everyone can join from 
the 900 plus people.
Everyone can join that one call and ask questions through Slack. It would be. 
Pretty messy. I suppose if everyone was talking and then we have WordPress, of 
course we use a specific or a special theme called  that we use for project and 
team blogs. So every team and every project or. Larger projects will have their 
own blog, where we can post updates, questions, um, specifications, document, 
um, communications with outside vendors and stuff like that.
And that is pretty much all we use for communicating with each other. We do not 
use email at all. 
**Michaela:** [00:16:25] Wow. That's so different to my experience at Microsoft, 
where model we are fueled by emails, right? 
**Leif:** [00:16:32] So another big part of how we get to know each other and 
how we build up trust is meeting in person from time to time.
So every team meets about two times per year. And once a year, the whole company 
meets in one single place where we have one week of meeting each other, working 
on projects, learning things together and stuff like that. 
**Michaela:** [00:16:53] Yeah, that sounds really good because otherwise if you 
have never seen it person. 
**Leif:** [00:16:58] Yeah.
And it's also to be honest, it's, um, big perk of the company too, that you get 
to travel like two or three times to interesting places. 
**Michaela:** [00:17:06] Yeah. I always see your Instagram pictures, Dan, where 
you say like, what was new or something was the last time. No, 
**Leif:** [00:17:12] yeah, yeah. 
**Michaela:** [00:17:13] New Orleans, right? Yeah. Wow. It's amazing. I would 
like to be there as well.
Yeah. So when you look at it, so your company, is there something there's 
specific going on for the processes and tools that you use for an enormous 
software development? Well, really writing the code, building the code, 
deploying the code, testing, something like that. Is this something that you 
think is different from other companies and how does it look like in general?
**Leif:** [00:17:39] I don't know about other companies that much. Um, but I can 
say that because we have a bunch of different products and they are all 
technologically, somewhat different. The approaches we used to. So for 
continuous integration and for version control, for example, they can differ 
like by decades. So WordPress is on some version, right?
And we have a WordPress repose and we need to, to merge with the WordPress core 
project from time to time, or we have to merge the open source project into our 
repo from time to time. Right. And it also has our own modifications to it. So 
that project is on subversion and there is no GitHub for version, right.
The best or the next best thing that comes close to that would be fabricator, 
which is. Kind of like an interface on top of subversion repose, where you can 
also do things like pull requests and get reviews on those and stuff like that. 
And that system itself is also, again, we don't use circle CEI or Travis CEI or 
things like that on that repo because those systems assume get based repository.
So we use something that's called team city on that. So basically the parts are 
all the same theoretically. But in their manifestation, they differ. Like they, 
they will use different technologies. So we do use the version control. We do 
use code reviews. We do use continuous integration. We rewrite tests, all those 
things, but how we do that and how hard it is also will differ from project to 
project.
**Michaela:** [00:19:19] Yeah, that's really interesting. I mean, how big is 
automatic? Can you remind me again, 
**Leif:** [00:19:26] company? That's just 900 people, 
**Michaela:** [00:19:28] a hundred people. Okay. And how many engineers do you 
know? 
**Leif:** [00:19:31] It, it it's a rough estimate. I think like, I don't know if 
I recall exactly, but maybe about 400. 
**Michaela:** [00:19:37] Okay. So for 400 people, I think it's quite diverse, 
right?
I mean, we are dealing with all those different technologies. You're dealing 
with all those different tools. So also the knowledge that you have to have to 
know all of those really in and out of this. Quite scattered. Right. Is there 
some future goal of consolidating those different technologies? So like for 
example, porting the WordPress code base to get two huge thing to do.
**Leif:** [00:20:06] I think that's politically very. Heavy subject, because we 
depend on the WordPress open source project. Right. And it's an open source 
project. We don't get to dictate what they use, right. Or so we have a whole 
team who basically gets paid to work on the open source project, but they are 
trying really hard not to let company up decisions or influences, um, let that 
influence their open source work.
Right. So we really. Depend on the open source project for that. So if the open 
source project moves to get, we can move over to, 
**Michaela:** [00:20:43] I see. Okay. Yeah. I never thought about that. I mean, 
that's really an interesting aspect as well of working at automatic that you 
have like this, I call it now tension a little bit tension between open source 
and the commercial interests of a, of a company, right?
**Leif:** [00:20:57] Yeah. 
**Michaela:** [00:20:58] What are the benefits that the company gets out of open 
sourcing parts of their just software. But do you do that 
**Leif:** [00:21:06] open source company? The company is founded on the idea of 
open source basically, right? So we embrace it and I'm not sure if it's really 
about the concrete advantages of open source, but I think culturally, the spirit 
of openness of transparency, that's helpful in other areas too.
For example, if all the communication is transparent, And if decisions are 
transparent, that creates a vastly different company culture, and that might not 
directly affect codes or things like that. Right. But it will affect many other 
things. Yeah. And 
**Michaela:** [00:21:39] actually, I have to say that when I ask you to be on my 
podcast, it was quite a quick decision, right?
It's just send an email or almost not an email and message right. To one of your 
colleagues and they approved it. And I know that for several other interview 
participants, it's like weeks going on places to, for them to get well allowance 
to even talk. And some of them are just purely denied. It's like, no, you cannot 
talk on a 
**Leif:** [00:22:06] podcast.
So we have a Slack channel called PR for public relations where people talk 
about things like that. And I just asked the question there and by coincidence, 
the colleague who replied to my question was Matt. Okay. So I got official and 
official. Okay. From the CEO. Oh, 
**Michaela:** [00:22:26] yeah. Now I feel really at ease. Now I can ask all 
these tricky questions.
**Leif:** [00:22:32] Yeah, exactly. 
**Michaela:** [00:22:35] Yeah. Very cool. Yeah, that's really something. I mean, 
it's, it's a minor peek into your company, but for me it was very. Well, 
relieving Elsa. I asked you to ask for permission and you asked for permission 
and within a few minutes, you're coming back and saying, yes, I can talk on your 
podcast.
And that's, that's so nice, right? 
**Leif:** [00:22:52] I mean, we do have some, some back and forth too. We, we 
don't always have transparency, even if we want it, but the default is 
transparency, openness, low bureaucracy. So, so. We will never reach the ideal, 
but we're always trying to approximate it. Right? So, um, one, one guideline 
that Matt keeps on mentioning is to quickly make decisions that are easily 
reversible, you know, like don't, don't fret too much over making a decision 
that you can reverse within the matter of minutes.
Anyway. 
**Michaela:** [00:23:27] Yeah, that's really smart. So there's a lot about 
culture, right? How the culture of a company works and well, how long have you 
been now at automatic? 
**Leif:** [00:23:38] Oh, I am, no, I joined three and a half years ago. 
**Michaela:** [00:23:42] Okay. So do you feel that the culture, I mean, the 
company evolved and grew quite substantially. 
**Leif:** [00:23:50] Did the culture also 
**Michaela:** [00:23:51] change much during that time or did it stay the same?
**Leif:** [00:23:57] Both. I think so. I think when I joined who were about 300 
people now we're over 900. So it has tripled in size within three years. It 
would be pretty weird if that would not create friction, I suppose, especially 
with people coming in. Who might have worked in other contexts who might be 
further removed from the open source project, for example, they will carry 
different.
A different cultural inventory with them. I believe. So it's a constant balance 
that we're trying to strike between letting more diverse perspectives in, but 
staying true to the core of the company values. Uh, one thing that helps with 
that is that we have a creed. The automatic creed. Okay. What's that? So if you 
go to automatic.com/creed, C R E D, you will see a short text, which is 
something like the vision for the culture of the company in a nutshell.
And I'm going to read it to you. And the automatic creed says I will never stop 
learning. I won't just work on things that are assigned to me. I know there's no 
such thing. As a status quo, I will build our business sustainably through 
passionate and loyal customers. I will never pass up opportunity to help a 
colleague.
And I'll remember the days before I knew everything. I am more motivated by 
impact than money. And I know that open source is one of the most powerful ideas 
of our generation. I will communicate as much as possible because it's the 
oxygen of a distributed company. I'm in a marathon, not a, not a sprint and no 
matter how far away the goal is, the only way to get there is by putting one 
foot in front of another every day, given time, there is no problem that's 
insurmountable and that's the automatic creed.
And that is. Basically the, the gospel that we try to reference when we need to 
make decisions that we're not sure whether they align with company goals, 
company, culture, or values and things like that. And usually it at least gives 
us a rough direction to turn to. 
**Michaela:** [00:26:12] Yeah, I liked it. I liked it a lot. It sounds like a 
person spent a lot of time really thinking about the values of the company.
Yeah, that's nice. So I wanted to switch gears a little bit now and talk with 
you about the software engineering processes. So do you have similar guidelines, 
like the automatic creed for your development processes and how do you do 
things? Like, for example, how do you test your system? 
**Leif:** [00:26:38] So non end to end tests.
So all the tests that don't need a browser to run, I would say the developers to 
write themselves as part of their ongoing work, but for end to end tests where 
we use like a handle as right, or to actually use the site and buy things and 
sign up for that, we do have a specific team who works on that, just because 
it's a very specific niche technology and you have to develop a very.
Deep expertise to be able to automate all that and to, to know how to handle 
issues. For example, if you try to buy something and the test fails, why is 
that? Is that because maybe the payments provider was down or is it a problem in 
your code? And if you have many dependencies to other services, then it can 
become.
Pretty hairy pretty quickly. So it's nice to have a specific team for that. 
**Michaela:** [00:27:36] Okay. And do you have like something like code 
coverage? Do you track that? Is this something that's part of your daily 
**Leif:** [00:27:42] basis or not? No, I don't think we do that. No. Uh, I think 
we did discuss measuring something like code coverage at some point, but then I 
think we didn't want to focus too much on a single metric.
So we did experiment around that a bit. And I think what we ended up with is a. 
An integration on GitHub that posts a message to your PR. If the code that you 
add has code coverage lower than something, something like that. Something not 
too obnoxious, something. Kind of subtle. 
**Michaela:** [00:28:20] And now that you said, well, the whole landscape is 
very diverse technology wise, but also tool-wise.
Is, is that also something that's different for each of the teams and projects 
that you work on? Or is there some standard policy around testing, code reviews, 
things like that? 
**Leif:** [00:28:37] We don't have a standard policy written out anywhere. I 
think we do have guidelines in, so we do have a company. Handbook. So to say 
it's called the field guide.
It's just another blog. Everyone can edit it and you can find out pretty much 
anything you need to know about working here by looking into it. And it does 
have a few guidelines for how to, how to test the projects, um, how much effort 
to put into it. So you don't get derailed, but it's no, there's no hard written 
rules, I would say.
So usually you would. Look at the product that you're working on and figure out 
what the testing culture is on that product. And then basically blend in BB 
normal right. In that's project. 
**Michaela:** [00:29:24] Okay. But it can differ from project to project, 
**Leif:** [00:29:28] do stuff. Yeah. Especially because it's just different, 
very different technologies.
Right. 
**Michaela:** [00:29:33] Okay. So it's sort of technology driven, alignments. 
**Leif:** [00:29:38] Technology influenced, I would say. Yeah. And also, um, I 
mean, yeah, different products are obviously of different importance, right? So 
that will play into that as well. I would say so wordpress.com has, I don't, I 
don't know if I can say the number, but it's a lots of users and it would be a 
really bad if it would break.
So that would have different standards. Then say an internal app that we're 
developing for just for comfort reasons. 
**Michaela:** [00:30:08] Yeah, that makes sense. And what about code reviews? 
So, one of my topics that I worked a lot on was called your views and how they 
are used to improve the code quality, but also to share knowledge amongst 
developers is, is contribute something that you do at automatics and how are 
people perceiving it?
**Leif:** [00:30:27] I think it's changed over time. So when I joined, there was 
still a few people who would just cowboy code and commit, but that is getting 
fewer and fewer. It's been. Probably two years or something like that since I've 
seen anyone commit without a review. So every pull request or whatever you may 
call it, every change, um, will have been looked at by at least one other, yeah.
Colleague, if it's very sensitive stuff, like for example, payments code, then 
we would have two or three other colleagues look at it, depending on at what 
level we would feel comfortable. Right. We'd also reach out to experts on the 
subject matter. We. Are not experts ourselves. So that's yeah, I think that's 
really nice how it works.
I feel very happy with having everything reviewed. 
**Michaela:** [00:31:16] This gives you a good feeling about your own code and 
about the code from others. 
**Leif:** [00:31:20] Yeah. And generally I think it makes for a good environment 
where we all know about our own fallibility. Like, we all know that this is an 
obvious fix where famous last words.
Right? Like it's very hard if you work on something to really, really, really be 
sure that this doesn't break anything because you don't know everything. Right. 
And again, going back to the creed. I remember the days before I knew 
everything. So this sort of humility is kind of built in into the company 
culture.
So most people are very thankful for, for others, um, to look at their 
**Michaela:** [00:31:57] code. Yeah, that sounds great. Especially for code 
reviews, one of the bit falls or problems with it is that you wait very long for 
other people to look at your code. And I can imagine that the distributed 
company, while remote and distributed company with different time zones, that 
can be painful.
How do you mitigate that? 
**Leif:** [00:32:17] So many teams use, um, Trello. To basically move cards 
through this week in progress, in review and done. Something like that. And 
those changes will be posted to the team's Slack channels. So if I see a 
colleague move something into a review column on Slack, then I'll know this is 
ready for review.
I will usually not get to it immediately. But if it's, it has some time pressure 
behind it, then the colleague will reach out to me and ask me, Hey, do you have 
a minute today to take a look at this? I really like to deploy this today 
because that would really benefit our customers in X and Y. But there are also 
of course reviews that are neither important nor urgent, but we still are one to 
review that code.
Right. So, um, we do have a, it's a Slack app. We call it the stick and the 
stick. So I think it comes from being beaten with a stick. So it's like, it's 
not, you know, it nudges you to review. So it has like a conflict file where it 
can set up. Your teams and those teams, um, Trello boards. So it continuously, 
or once a day, it looks at your teams.
Trello board looks at all the cards that are in the in review column, and then 
randomly. Pinks people on Slack pay life. What about reviewing this one today? 
Right. So you get actual pings on Slack by the stick and depending on the 
person, I think very few people ignore it because a ping on Slack is kind of 
like, you know, um, yeah.
Yeah. It's a thing. Kind of should be doing okay. Yeah. And that's really helps 
keep that need three of you call him clean. 
**Michaela:** [00:34:12] Okay. So one thing that I wanted to ask you as well is, 
well, if you have this, do you have this review staff, but then how far are 
actually developers? Away from production. What I mean by that is, well, imagine 
you're making a new feature or back fix or whatever, what stabs are in between 
you saying, well, my code is done and having it in production, how much steps 
are in between which steps and maybe a roughly estimate of a time, if you can 
give it.
**Leif:** [00:34:42] So again, the specifics will depend on the project that 
you're working on because of the different technologies. But roughly if you have 
something that has been reviewed. Right. So you're confident that a sufficient 
number of reviewers have told you that this can be deployed, then you merge it 
and you deploy it.
We have a command to deploy, um, master branch, basically to production. And 
that's it. 
**Michaela:** [00:35:10] Okay. So you're quite quickly there and that's then 
really in production. Is there some staging happening before, or 
**Leif:** [00:35:17] we have a staging for at least one of the projects where we 
can try things out with the proper host names and everything, and with actual 
production data, but that's like only last check.
So you would spend maybe 10 minutes clicking around a bit. They are to see if 
really everything's really, really, really all right. But usually, yeah. Um, our 
development environments and our testing environments are close enough to 
production for us to be relatively, um, sure. That things will work the same.
**Michaela:** [00:35:51] And what about these testers that you said all of those 
tests are automatic tests that really end to end test, and those you would run 
before deploying to production as well? 
**Leif:** [00:36:02] Yeah, they could run automatically for every poll request. 
So if you create a pull request that has a label needs review, then that will 
automatically run all the end to end tests on it.
Cool. 
**Michaela:** [00:36:13] And what about technical dab? I mean, that's. A topic 
that's discussed hardly anything. It's well, it's a very fuzzy term as well, but 
I would like to talk with you about it, but role has technical depth in our edit 
to the medic. And how do you handle it? How do you assess it on a day to day? 
**Leif:** [00:36:30] Right. I mean, we definitely do have technical debt.
That's like, there's no way around that. Mostly because we try to move fast and 
we try to work only on the things that we really want to accomplish. And. That 
that that can be a aspect where, for example, future maintainability. Can become 
more difficult because you're trying to optimize for shipping customer value.
Right? One, once a quarter, we do have a week where basically every developer 
works on things like that. Either technical dab or also things like UX step, 
like where. Where flows don't match with each other, but it's not a priority for 
any team. So it kind of lingers in there. But once a quarter, we have this week 
where we address things like that.
And over, over the weeks, we, um, we collect tasks that we think would be a good 
idea for such a week. And during the week, we will then have like a pile of tech 
dev or UX step tasks that we can work on. Actually, we are in such a work. In, 
in such a week right now 
**Michaela:** [00:37:42] to then that's your main focus on your sole focus?
**Leif:** [00:37:45] Yeah. Yeah. I'm pretty much the sole focus. I mean, the 
things the lights need to be kept on, obviously. So you cannot 100% focus on 
that. Um, usually, but it's a large part of my day. If I'm not on a podcast, um, 
then I would usually try to work on those tasks just to win when the whole 
company tries to address tech dev and UX dev once a quarter for a whole week.
That means you get a nice case into it. You, you get into a rhythm where things, 
things aren't perfect at any one time. But they continuously get better. 
Step-by-step you know? Um, and I think that's how we try to address it. And then 
we can refactor things while we work on it. Right. So we try to build that kind 
of, um, maintenance into our daily work also.
But, um, it's not our sole focus, right? Like we, we try to optimize for 
shipping customer value. 
**Michaela:** [00:38:48] Yeah. Yeah. I liked it really scheduled and planned 
approach as well because otherwise people tend to work on things that are just 
more impactful or the D you know, like to work on tipping feature. Somehow 
always feels probably more urgent or more fun as well.
So it's sort of bookkeeping, right? So when tax season ends, you somehow have to 
do your taxes. Right. So if there wouldn't be a deadline, probably nobody would 
**Leif:** [00:39:15] do that. Yeah. Or documentation. I recently saw a talk 
where she discussed the incentives around writing documentation, and she said 
that nobody ever got fired for not writing documentation and nobody ever got 
promoted for writing documentation, which is probably roughly true.
So what incentive is there to do these things, right? But if you see the whole 
company turn towards this one goal for a whole week, then again, You want to 
behave as most people do. So, okay. Let's look at tech tab this week. 
**Michaela:** [00:39:48] Yeah. Yeah. True. Yeah. I also like that pick up the 
topic about promotion. So how, how do you think you're assessed?
How is, is there a form of process for, is, do you know how people assess you? 
What they look for? How'd you get promoted? What's the life there that 
automatic. 
**Leif:** [00:40:04] Hmm. So what's the promotion. So when you like a change in 
title or the change in the responsibility, 
**Michaela:** [00:40:14] the question maybe, I don't know, but very often I 
think is a change in title.
Yeah. Better compensation for what you do. 
**Leif:** [00:40:23] So, so a compensation is reviewed once a year. 
Automatically you don't have to do anything. And basically it takes into account 
the week you did the year before, and depending on how impactful you were on how 
much value you shipped to customers, basically your salary will get adjusted, 
buy more or buy less.
You'll never get a reduction. You'll always get a slight increase just to 
account for inflation, but that's all there is to compensation and automatic. 
Would you, how 
**Michaela:** [00:40:54] would you assess the quality that you shipped or the 
value that you ship to customers? I mean, that's not that easy to measure. 
**Leif:** [00:41:01] No. Sure. Um, so regularly your team lead will get a, a 
request for feedback and you will like.
Try to document everything that you saw about your report and report that in 
that request for feedback and the employee themselves will also get such a 
feedback request for self feedback, and they can also give feedback on their 
lead. So. And, and it can be anonymous if you want to, like, you don't have to, 
like, you can decide to share that feedback with a person, but you don't have 
to.
And that's how we get a constant stream of feedback about people, but on the 
formal side and on the career track side, we don't have any titles. Really. We 
can choose our own titles. Let me quickly look that up. Matt Mullenweg with, I 
looked that up in the employee directory, his title is C BBQ, T T, which stands 
for chief barbecue taster.
I think that, um, so it can be, um, the random can be fun, but it can also be a 
matter of fact. So some people will say senior developer and that's what they 
are so roll or. Responsibility, isn't tied closely to compensation. So if you 
become a team lead that we try to not consider that a promotion, um, there will 
be no change in compensation.
If you change your role, the incentives are designed in a way to optimize for 
people who really want to do the things that the role requires. So if you become 
a lead and your salary doesn't change, it's suddenly much easier. Just say, 
wait. Yeah, this is really annoying. Like I've given this a shot for a year.
Actually. I like writing code better and there will be no change in 
compensation, so you can do that. So, and that way we try to keep the people in 
the lead roles, in the management roles who really liked the management work 
right. At a traditional company, you would, I don't know, get like pay bum once 
you're a, like a manager.
And then you adjust to the new lifestyle and you can't go back and suddenly 
you're stuck with this role and that's something we try to guard against that. 
**Michaela:** [00:43:29] Okay. Yeah. I see dad. And so you said at the 
beginning, you said that you're striving for a lot of. Transparency and things 
like that. Is that also reflected, for example, in the, I mean, especially if 
you don't have those titles, I think on one hand, it's really good because it 
takes away though.
Things on the other hand, it's a little bit less transparent, right? 
**Leif:** [00:43:51] It's definitely a double edged sword. I mean, also just 
people coming in and it's not something that'd be advertised warning. We have no 
career titles here. Right. And that's something you definitely have to grow 
into. But to me it was, it is somewhat.
Freeing, you know where to realize that you don't have to follow this career 
ladder that someone somewhere designed at some point, but that, and basically 
make your own adventure right. And grow in ways that you think are interesting 
for you at this moment in time, it is a huge adjustment, but if you're still 
here or if you're still at automatic after two years, you will probably have 
adjusted to.
This way. And if not, then you might think about leaving because I don't know, 
you crave external, uh, career progression, more titles, more, maybe you're a 
very title orient per person, then that maybe not be a good fit because everyone 
into the random title. 
**Michaela:** [00:44:50] Yeah, I can see how that fits into the automatic 
culture and the idea of being humble.
Well, one thing that I wanted to talk with you about, and that I think fits a 
little bit into that topic as well, is diversity, how diverse is especially the 
technical workforce at automatic. 
**Leif:** [00:45:09] Um, so the tech industry in general is basically white 
dudes, right? And we are mostly that too. It's something we are trying to 
actively address by being more present at, at events where a much more diverse 
audience might be present.
We try to reach out proactively a bit more. We try to make ourselves available. 
We try to remove our own biases when hiring by for example, When we decided to 
hire a person, we have not have had a video chat with them. So you can go 
through the whole process before anyone sees your face. For example, we also do 
have an internal diversity and inclusion committee.
That meets regularly and tries to take care of where the whole company is headed 
regards to that, but it's not solved, right? Like it's very, obviously still a 
problem. And that's the case for us too. We're all very aware of it. And for 
example, the developer hiring is 50% or more than 50% females. And that that is 
really nice, you know, like, so the people who can make the decisions, the 
people who will impact what kind of people will join.
They're already, we at about 50% I believe. And I think that's a pretty good 
sign to have, like, they're kind of like the gatekeepers, right. Even though 
they try to be impartial and reduce their own biases. They, they are the 
gatekeepers. And it's nice to know that there is a, a larger number of 
perspectives in, on that team than there has been traditionally, you know, 
**Michaela:** [00:46:48] So, yeah, I can really see how that can impact the 
hiring decisions.
And I think it's a really good step forward. I wanted to thank you life for this 
awesome interview. It was, I think, very well rounded. We covered a lot of 
topics. Yeah. 
**Leif:** [00:47:03] What do you think? 
**Michaela:** [00:47:05] So thank you for being on my show and letting me know 
so much about your work life at autumn. 
**Leif:** [00:47:11] Yes. Thanks for having me.
Thank you life talk soon. Bye bye. 
**Michaela:** [00:47:15] I hope you enjoyed another episode of the sup 
engineering unlocked podcast. Don't forget to subscribe. And I talk to you again 
in two weeks. 
**Leif:** [00:47:26] Bye.


