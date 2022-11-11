---
episode: "Transcipt Episode 10: Suz Hinton"
permalink: /episode-10-no-corporate-games
status: publish
type: transcript
---

**Michaela:**: [00:00:00] Hello, and welcome to the software engineering 
unlocked podcast. I'm your host, Dr. Michaela. And today I have the pleasure to 
talk to **Suz:** Hinton. **Suz:** is a senior software engineer at Stripe. She's 
a full stack engineer that also loves tinkering with hardware and in addition, 
she regularly streams live coding sessions on Twitch.
She's involved in open source and is a recognized international speaker. 
Today,  she joins me to talk with me about her experience working at Stripe and 
her prior experience working at Microsoft. So I'm super thrilled. Thank you to 
that you are here with me today.

**Suz:**: [00:00:34] Thanks. I'm really happy to be here. Yeah. 

**Michaela:**: [00:00:36] Thank you so much.
So, so you recently started working at Stripe. Can you tell me a little bit 
about your role and what you're currently working on and what are your 
responsibilities? How does your day to day work look like?

**Suz:**: [00:00:47] I started at Stripe, I think about three months 
ago. And I'm a  Developer advocate, I guess, in a way.
Um, and so I work with basically a lot of people internally and also with the 
community and users of Stripe at large. Um, right now I'm actually focusing on. 
The terminal product offering that we have and terminal is an in-person payments 
product that we have. And so let's say you start out as an online business.
Um, a really good example of this is Glossier who has really awesome cosmetics 
and personal care items. And let's say you become successful, but you'd then 
like to go and open a physical retail store. Like we, we actually have a story 
there and we can basically offer you some pre-certified readers. Um, And we have 
some really nice APIs that are in line with our regular payment APIs in 
order to get started with that.
And so I focus on that particular product. I work directly with the product 
team. And so right now I'm working with the terminal product team and I'm trying 
to reduce the amount of time it takes for you to unbox a reader, to actually get 
it registered with your Stripe account, and then to start taking a test payment.
Right now, I don't think that time is as fast as it could be. And so making a 
lot of tweaks and changing some of our software and our documentation in order 
just to get people up and running as fast as possible. So it's a really a satisfying project 
that I'm on right now, just because you can act actively, feel yourself 
improving the experience.
And then that obviously has a multiplier effect to a lot of software engineers 
out in the wild who are actually using Stripe terminal. 

**Michaela:**: [00:02:25] Yeah, that sounds really interesting. And it also 
sounds like you have to understand the customer. So are you really in contact 
with the customers? 

**Suz:**: [00:02:34] Yeah, so Stripe does a lot of user research, um, and I 
don't necessarily have to always be out there sort of feeling the tough.
And rough corners of products that we have in order to do that. And so we 
regularly perform a lot of user research. Every time we change our APIs, or 
every time we notice that we have a really interesting new user who has a really 
interesting case. Study that we can sort of look at. We tend to reach out to 
them and we have a whole team that does that.
And we can invite along to those user research sessions as well for us to learn. 
Um, we also get a lot of feedback that, um, we solicit via online platforms and also just 
reaching out to people individually as well. So. I think that that's obviously 
one of the most important parts of my job is not just to see it from my 
perspective, but to actually understand how people use this every day.
Um, and to kind of challenge a lot of the assumptions that we might make and 
totally about things like API signatures, um, how, how you can actually, um, error 
check and handle errors, but also just, you know, Uh, people understanding how to 
use our software based on how we're actually presenting the documentation to 
them as well.

**Michaela:**: [00:03:46] Yeah. I find it really fascinating. So can you tell me 
a little bit about, um, how you really work with this UX researchers? So you 
said you can invite yourself to the studies then I guess that they also write 
down their findings in some sort of documents, or how does that really look 
like? How do you consume those information?

**Suz:**: [00:04:06] It's very much like what you said. Um, a lot of the time it 
can be just a Skype video call and we talk back and forth some specific 
questions. Other times we will run a workshop in person, um, which my team has 
actually been responsible for running recently. We will help people onboard who, 
a new Stripe product, let's say it's billing or terminal, or, um, just.
Just payments out of the box as well. And we will observe where they struggled. 
Um, we actually did this a lot in my previous job as well, which we're going to 
talk about about later and just feeling live and having to sort of point out 
things like, Oh, if you click on this link here in the documentation that will 
take you through, or, Oh, I've never seen that error before because you know, 
I've always.
Taking the happy path when testing out, you know, some of our API signatures and 
things like that, it can be really illuminating to just what someone's struggled 
with. Something that you thought was already a good experience. And so we do 
like to, um, not just get, uh, online form information typed out from people we 
do like to kind of have that personal touch where we're actually feeling the 
emotions and watching the pain that people go through.
So we will do in person and also remote interviews as well. 
**Michaela:**: [00:05:12] Yeah. I think that's a really a good approach to do 
that. And, um, I've done that several times as well. Yeah. How do you reach out to those 
customers? How do you reach out to the people and how do you, how do you get 
them to agree to spend the time helping you.
**Suz:**: [00:05:28] I've been surprised at how willing and excited people  
to talk to us at Stripe. Yeah. I think that even though our documentation 
is known to be very good, I think that everybody always is excited to talk about 
their business. They're excited to talk to us about how Stripe has really 
enabled them to take payments so easily and to be able to expand globally.
And so. I've been surprised and really delighted to, to find out since I've 
joined that people are very willing to talk to us. People are very willing to 
dedicate time to writing up a lot of friction points for them because they know 
that this is a company that cares very deeply about the user experience and they 
feel like the investment's going to be worth it a lot of the time.
Um, again, we might just spot. A lot of activity from a customer as they scale, 
just by looking at our internal metrics, which can cause us to reach out, or we 
even might bump into someone at a conference where they might ask us a question 
that's very interesting to us. Um, and then we will want to follow up with them, 
you know, um, via email, or via.
You know, video chat later on. I mean, even this just happened to me this week. 
I got to a question when I was at App developer summit, and now I want to 
actually follow up because it seems like they're having a slight challenge in 
PCI compliance. I'm retaining that, but also like migrating to, you know, one of 
our new APIs, which is super interesting.
So it tends to come up pretty organically. Um, but I do know that there are the 
user research team is actually actively, always trying to look at interesting 
businesses that, you know, a challenging out platform. 
**Michaela:**: [00:06:59] Yeah. So I was working with another company right now 
and they have some strugglers getting users, you know, to give feedback.
And I really think it has all to do with how are you providing value, as you 
said, I think people recognize that Stripe is providing value to them. And not 
only that, if they talk to you and tell you the friction points Stripe will work 
on those friction points and make the product even better. Right.
And if you can bring that message across, I think people are naturally. More 
willing to help. And, you know, it's a, it's a very, it's a synergy between the 
two parties. 
**Suz:**: [00:07:32] Right? Absolutely. Totally agree. 
**Michaela:**: [00:07:35] Yeah. That's really interesting. So, but how did you 
apply for this position? How did you decide that you want to work at Stripe and 
how did you apply?
How did you come across this position? 
**Suz:**: [00:07:44] It's interesting because initially it was Stripe who 
reached out. However, at the time I was working at Microsoft, I had been there 
maybe seven months, uh, which to me doesn't feel like it's quite enough time to 
sort of evaluate a job and sort of accomplish what you want to accomplish.
And so I did actually go into the office. I spoke at length with them, you know, 
I raised my concerns with leaving. I'm not leaving a company so early off to starting and 
things like that. So we decided to just table the conversation, um, and then, 
you know, pick it up at a later point. And so a little while later, I would say 
a year and a half later, um, I'd been at Microsoft for over two years at that 
point.
And so I reached out to them again because I felt that it was the right time. 
Um, I've always really admired Stripe because I used, uh, Stripe's API when 
I worked at Kickstarter, um, a while ago, because kickstarter actually uses 
a Stripe to take, uh, pledges from, um, from backers the projects. And so 
it was already familiar with how good the documentation was.
I was so inspired by that. It made me want to improve my own software and open 
source documentation. Um, and so it's always been a company I'd admired. It was 
more just that. I didn't think that I was, um, I guess like a good enough 
develop a quote unquote, to apply for a job like that. So when they reached out 
to me, I just thought it was this amazing privilege.
And so I really wanted to eventually come to work for the company and just had 
to wait for the time to be right. 
**Michaela:**: [00:09:12] So then you reached out and how, how did the process go 
done? What's the application process that you have to go through? True. When you 
want to work at Stripe. 
**Suz:**: [00:09:22] So I reached out to the original person who I had all of 
those conversations with all that time ago.
They were still at the company. Um, I asked them if they had head count for the 
specific role, which was to be in developer relations. And they said, yes. So I 
ended up applying by the official channels via the website. I submitted my 
resume and, um, that process. Because they were already interested in 
potentially hiring me.
I did skip the initial phone and technical screening. Um, but then I still had a 
take home coding challenge. So the first step was really just doing that coding 
challenge. Um, after speaking very briefly with a recruiter on the phone so that 
I knew what the process was. Um, I turned that coding challenge around in 
basically like the next day, just because I wanted to churn through it.
Um, and from there, um, We scheduled an onsite interview and that's very, a very 
similar, typical interview as far as, you know, it's a full day, you know, just 
like other large tech companies. Um, but it was done very empathetically. And so 
I was sent a giant document, um, basically informing me everything from what to 
dress, um, You know how to dress, which it wasn't telling me exactly what to 
wear.
It was just telling me in a very comforting terms, like what is acceptable and 
like what people tend to wear to the interview and to just be myself and like 
wear something that I'm comfortable in, which was really great. Um, but it also 
just. Explained what I can expect to be tested on technically. So what signs are 
they actually looking for?
So instead of walking in and feeling like you have no idea what they are, we're 
trying to, um, evaluate you on. Uh, I walked in feeling like I understood what I 
was supposed to be showing them, um, which was really, really great. Um, and 
every single interview was tailored towards the actual role that I was doing.
Um, so I did everything from like a live debugging challenge where I was 
presented with a repository of code to clone down that when you run the actual 
main script, it doesn't actually work. It explodes and you have to figure out 
why I had to give a. A spoken presentation, uh, for one of the interviews.
And that's because in my role, sometimes going to be speaking to customers and 
users at our user conference, which is called session. And then I spoke with 
marketing to try and segment different developers based on, you know, different 
ways to segments. Um, and then also just things like. Cultural questions and 
then more technical follow up as well.
For me to describe things from a systems point of view, what experience I had 
writing my own APIs, evaluating my own APIs and actually like improving the 
software that I'd written. That was, there was a really, really huge, um, 
concentration on that as a skill as well. So I really appreciate it. Just 
feeling like.
I got an idea of what the job was going to be like based on my interview 
questions. And they were also super open to me asking all sorts of honest 
questions too, which I really appreciated. And so that was pretty much Mo the 
whole process. Um, I came in very briefly to tour the local Seattle office just 
because that's not right interviewed and that's where I would be based and 
working out of.
Um, and after that, the same day, they ended up sending me an offer. 
**Michaela:**: [00:12:35] Okay, well, so actually it went quite quick. Um, the 
whole interview process, even though it's a very, very sorrow, uh, process, but 
the whole experience was quick and positive. That's how you would describe it. 
**Suz:**: [00:12:48] Yeah, that would pretty high touch.
Um, let's say if there were any delays in just, you know, there was a little bit 
of a delay between my onsite in San Francisco and coming onsite in Seattle just 
to, you know, speak with the site lead and things like that. There was a little 
bit of time in between that, but they were very good at being high touch and 
just keeping me updated.
Um, so I thought that was really nice. 
**Michaela:**: [00:13:08] Yeah, that sounds good. So a way back actually tweeted 
about leaving Microsoft, and I remembered that you expressed that the job that 
you had to do at Microsoft did not completely fit your personality. Can you, do 
you want to elaborate a little bit on that? 
**Suz:**: [00:13:24] I can definitely talk about that.
Um, I think that everybody's experience at Microsoft is going to differ. So I 
definitely want people to keep that in mind, you know, there's over a hundred 
thousand employees worldwide who work for Microsoft. So this is one tiny little 
grain of sand experience. Um, and it is very dependent on my personality as 
well.
Um, but I think that my journey at Microsoft was. Mostly a journey of 
frustration, but obviously I had a lot of personal growth from it as well. So I 
don't regret working for the company, but in a nutshell, um, I feel that the 
roles that I worked in at Microsoft, specifically, the teams were developed to 
basically run against the grain of a lot of other teams internally.
And what I mean by that is, you know, I was hired into a developer evangelism 
role, um, where I was working with customers and bringing product feedback 
directly back from the customers to the product teams. Um, and then I actually 
also worked in a role which was developed advocacy, which was more about trying 
to do outreach to users, improve, um, our samples, write demos, um, and go out 
to customers and actually give best practice talks about how to actually use our 
stuff.
So there were two very different sides to the actual job and. I think that in 
both cases, we were supposed to be challenging the designs of the Microsoft 
products we were focusing on. So was focusing on IOT, for example, and we were 
supposed to be saying, and pushing back and saying, I know that we released this 
specific feature, but it doesn't fit the customer at all and we really need to 
change it.
And here are the financial, um, you know, motivations behind it, changing this 
for this customer and I'm blocking them and things like that. And so you would 
constantly having to give quite critical feedback, um, and. Two teams who 
traditionally may not have necessarily had a team doing that in the past and 
having a mandate in to actually listen to our feedback.
And so when you're really stressed out on a product team and you're trying to 
ship a lot of features and you're running against these deadlines and someone is 
coming and trying to undo that work and telling you you're working on the wrong 
thing and telling you that this is broken, and this could be better.
Understandably, you know, you're going to get defensive about that. If you work 
on that product team and understandably, if you're the person giving the 
feedback, you can get burnt out very easily and you can feel like you're always 
the bad guy, you know, and you have to have, you know, a certain growth mindset 
in order for both parties to want to talk and work well together.
And that was just incredibly challenging for my personality. Like I learned how 
to be less conflict adverse. Um, but at the same time, That was something that 
was very tough on me. Um, and so that was one aspect of it. The next aspect was 
just that I learned very quickly and I was told by a lot of people that, and 
this again, doesn't necessarily apply to everybody, but.
In my experience, I was told that Microsoft is really just about playing a big 
game. Um, and that there was a certain hazing ritual you had to go through and 
you wouldn't understand how the company works for at least a year of working 
there. And then things would come into place and then you would build your 
network and then you would understand how to do your job.
And then you would start playing this corporate game to get ahead. And I just 
rejected that from the very first week and got very frustrated at people. 
Gatekeeping their networks and expecting me to prove it, why I deserve to have 
access to that, the networks internally, and just having to constantly prove 
myself, even though I wasn't interested in playing that game.
And so when I joined a company, I just want to. Do a good job. And I just want 
to, um, perform at the highest level I possibly can. And I want an environment 
that supports me to do that. Um, but I'm okay with just, you know, spitting by 
myself and being super motivated and ambitious and doing that by myself.
And I, I want my work to speak for itself and I don't want to have to play these 
really weird social games. And so I just felt like. Certain things were rewarded 
that shouldn't have been. And if I did something that I thought was low effort, 
sometimes people rewarded that in a very exaggerated manner.
When I just thought I was doing the bare minimum. Yeah. It was just a very 
scattered and mixed experience of trying to discover this weird board game that 
everyone else knew how to play that. I didn't know how to play. And that's when 
I figured out after two and a half years of kind of going against the grain, but 
also just like.
Not wanting to work within that culture and trying two different teams just to 
see whether I could sort of find a good place. That's when I knew that it was, 
it was time for me to throw in the towel. 
**Michaela:**: [00:18:18] Okay. So you actually worked at different teams during 
your time at Microsoft? 

**Suz:**: [00:18:21] Yeah, so I started as a technical 
evangelist and that's in the sales organization.
Um, and that's when I knew that they didn't really screen a lot for technical experize 
 and things like that. And I felt that I was being held back because 
when people see that you're in the sales org, they tend to not be as willing to 
engage with you from a technical point of view. So that's when a new team, um, 
spun up, which was in the engineering org.
So when that started, I waited a few months for the dust to settle and moved 
over to that team to see if I could get any further in trying to do quality 
work, um, on the engineering org, instead of on the sales org. 

**Michaela:**: [00:19:00] But your experiences were quite the same between those 
different orgs. 

**Suz:**: [00:19:04] I would say that there were just different games.
Um, and I would, I would say that I was rewarded for doing different things. I 
think that the second team in engineering was way better set up to succeed. Um, 
but that didn't necessarily mean that your relations with product teams were any 
easier to forge. If that makes sense. 

**Michaela:**: [00:19:26] Yeah. Yeah, yeah. Everything that you say.
I mean, I can totally understand that you wouldn't like to be in that position. 
I think few people, I mean, some of them might strive in such a setting, but few 
people would really strive in that setting. Um, from my experience working at 
Microsoft, I see that there is. A lot of diversity in teams. Like the culture is 
very different.
I worked with, with a lot of different product teams in the, obviously the 
engineering org, but even there, I could really see that. For example, the 
office engineering org is very, very different than for example, windows or, you 
know, visual studio, things like that. 

**Suz:**: [00:20:03] Yeah. So. 

**Michaela:**: [00:20:05] So that's really interesting to hear, um, your, your 
experience.
So looking back there, things, can you say that you learn something that you 
would do different and when you now decide to join a company, even, you know, 
when you decided to join Stripe, which signs and signals did you look for that 
you think, well, these signals, somehow, if you will fit there and if you will 
be happy and if you can strive there

**Suz:**: [00:20:28] For Sure.
Um, I think the first thing that I learned was to ask really tough questions in 
an interview. I think that because the Microsoft door opening for me, it came so 
sporadically and out of the blue. Um, I always sort of just like really swept up 
in the excitement of the fact that Microsoft, you know, Actively reached out to 
me and that, that were excited about hiring me.
And I spoke to a few people on the team who had only actually been there for 
about three months. Um, so they were still obviously really excited to be there. 
And I think that it just didn't do my due diligence because I got too excited 
and I always feel like I don't have the power in that dynamic. And so I sort of 
realized that if Microsoft reaching out to me that.
Maybe I have safety and asking some of the tougher questions in the interview 
and not being afraid of asking them and just trying to find people within the 
company that are of a similar personality to me that I can talk to you. And I've 
definitely done that since, you know, I asked much more tough questions at 
Stripe.
Um, I, I also interviewed at Google and Amazon as well at the same time. And I 
asked. Very very, very specific questions and actually asked to speak to more 
people even after my interviews. So, you know, I wanted to follow up with 
someone who let's say works on open-source or Google in their spare time. And 
like, you know, what are the challenges behind IP ownership and things like 
that.
And so I tried to be a lot better at that. Um, this time around in doing that, 
given that I was in a, obviously a very privileged position, I was interviewing 
for a, you know, several large tech companies. I sort of sized up whether or 
not, you know, I was. In a position where I had the safety to do that, and I did 
this time.
So that was really good. Um, I think also just the signal to look for once you 
join a company, is, uh, people giving you weird advice. Like they're trying to 
teach you how to play a specific game. I think that's something that I was. Very 
frustrated upon running into it, Microsoft early on, but I definitely feel that 
maybe I stuck it out a little too long and didn't trust my gut.
Um, I think it's important to mention that changing jobs for me is not just. 
Sneaking out doing an interview and signing on the dotted line and giving my two 
weeks notice. I'm actually not an American citizen or an American permanent 
resident, but I do work in the United States. And so I required, VISA
sponsorship, which is a multi month.
Very stressful. Yeah. Very bureaucratic process. Every time I want to change 
jobs. And so I do tend to dig in a little longer, um, just because 
psychologically and mentally, it takes a huge toll and financially to take some 
massive toll on me to change jobs. Um, but I think, I think that that's just 
more important on me asking the right questions before I joined a company.
Um, and I think that that's actually been a really positive outcome. That's come 
from that. If that makes sense. 

**Michaela:**: [00:23:23] Yeah, I totally understand that I was also a US 
visa sponsor and I was always super frightened that one day I would get 
fired and I don't know what to do. 

**Suz:**: [00:23:33] Yes. I absolutely relate to that.

**Michaela:**: [00:23:37] I don't know, it wasn't very realistical event or 
something, but you know, if there were layoffs, I was like, completely shut 
down. I was like, Oh my God, the company is laying off people. And what happens, 
you know, if they would decide to lay me off. 

**Suz:**: [00:23:51] Yeah. Because it was terrible. Very 

**Michaela:**: [00:23:53] tricky. Right, right. Yeah.
It's tricky. It's not that easy if you don't, if you cannot just stay at, I 
don't know if I recall correctly, but I had in mind that within two weeks, I 
actually have to find a new job. That would fit to the visa that I had and 
things like that. 
**Suz:**: [00:24:10] So it's scary. 
**Michaela:**: [00:24:12] It is right? Yeah, it is. It 

**Suz:**: [00:24:14] is. That's really 
**Michaela:**: [00:24:15] true.
Um, so, well, can we talk a little bit about the software engineering process
at, as Stripe? Because I'm super interested in how either. Different companies
and different people, different teams developed software. And one of my 
favorite topics code review. So I would love to talk about code reviews with 
you.Um, what code you have your practices have you experienced during your 
career, the different companies and what stands out for you where you think 
well, that's really, that makes a good code review practice.

**Suz:**: [00:24:49] Most of the code review practices I've been through at 
companies have been pretty similar to each other. Um, I think that the first job 
I worked in there was actually code review because that wasn't always a thing in 
my career. Uh, somebody would write an entire feature. They would take maybe 
three months to write this too.
Um, and sometimes in isolation, because if you're working for a startup, 
sometimes you're just owning the entire product and. Before bundling up to 
deploy the, basically like the highest ranking person in engineering within them, 
would sit down with that person and just go through it together, which to me is like 
incredibly laborious and isn't necessarily productive to catching easy things 
that could have been caught early on.
Um, and so I saw like a lot of major refactors being needed, um, at that time. 
And so as I've sort of worked at a variety of places, the most common approach 
to this, which is very different to that is to. Look into continuous deployment, 
which means that you're actually just bundling up a couple of different commits, 
whether that's in git or.
You know, another source control method. Um, usually you just bundle up 
something small, something that's sort of self encapsulated, and then you ask 
for at least one person to review it. So Stripe is no different from that. Um, 
Stripe deploys, lots and lots of times a day. Um, and they have a lot of 
different engineers actually working on the like, you know, the same service 
slash services.
And so, um, It's the same kind of mentality. So you work on something, it 
doesn't necessarily yeah. To be the full feature, complete you, right. Open a 
pull request and you assign a specific person. And then we have a bunch of Gates 
in the way, um, such as automated testing and also, you know, human reviewers in 
order for that to then become mergeable and then deployable out to production.
**Michaela:**: [00:26:40] And the Stripe have any guidelines or real policies 
around at least one person of that team or with that expertise has to look 
through, or is that your diligence to, you know, select the right reviewer for 
your code piece? 
**Suz:**: [00:26:57] So we are pretty strict about requiring at least one 
person to look at it. And part of that is just the nature of the payments 
industry, um, when you're handling people's money and when you're writing 
software in order to do that, um, there are certain requirements and compliance.
Requirements that we need to actually satisfy in order to keep our code secure 
in order to keep people's information secure. And so just as a general rule, we 
always have at least one person, um, looking at the code that someone else wrote 
just to remain compliant with those requirements. Um, beyond that, though, you 
are allowed to choose who you think is the best.
Person to look at something, um, it's, it doesn't necessarily fall down to this 
mandatory hierarchy and you are trusted to choose the correct person, you know, 
with the right knowledge. Um, but also with the right amount of fresh eyes, to 
look at something that you've written, um, in order to gauge whether or not, you 
know, everything seems to check out.
Okay. So I really liked that. I think that's very empowering and also it's a 
really nice opportunity to pair with people and learn from other people. And 
given that, you know, we always require that out of the gate. 
**Michaela:**: [00:28:02] Yeah. So one of the topics that I wanted to talk with 
you about is mentoring junior developers.
And I know that you, you do that. Um, can you tell me a little bit about how you 
do that and what you focus on when mentoring junior developers? 
**Suz:**: [00:28:19] So I definitely got into mentoring accidentally, and I 
still feel that I still do that. Um, what I've found is that. You know, I've 
been a senior engineer for a number of years now, you know, this is my 15th year 
in the field and that.
That industry that we're in has just changed so quickly in that amount of time. 
Um, and I think now that juniors who are entering the field have to know a lot 
more than I did when I first got started. I think that, um, back in the early 
two thousands, it was a lot more scrappy. Uh, there was no concept of cloud 
computing.
There was no real JavaScript on the front end because it wasn't performance. Um, 
and things like that. There were just so many. I guess like extra things that I 
just didn't have, have to learn that people have to learn these days. So I have 
a lot of empathy for Juniors entering the field. I would say that there are at 
least two to three times more qualified to, um, to not qualify because that's 
kind of like a judgy thing, but yeah.
But just the, the two or three times more knowledgeable entering the field, um, 
compared to when I entered. Right. Um, and so I think that that's something to 
be respected and also they're probably feeling very overwhelmed because they 
also, even though they know a lot more, they also know how much more they need 
to know.
So a lot of the time, you know, I would see juniors get hired into companies 
that I've worked at. And then I would come in on their first day and I'd be 
like, Oh cool. So where are they going to sit? And then I would find out nobody 
had. Assign a seat to them. And then I would say, Oh, okay. So like, who was their 
buddy?
And they'll be like, Oh, it's like, it's Steven over there, but Steven's 
actually in meetings all day. And then I would just start tearing my hair out 
because I thought, Oh, if, if that was me starting, I would just feel so 
unwelcome. And so just like left in the deep end and I would feel a lot of 
imposter syndrome and things like that.
So it came out of just like, Heart ache and a bleeding heart to just help smooth 
over that experience. But I found that a lot of other senior engineers who I 
worked with were not actually super stoked or, you know, to mentor or if they 
did put their hand up, they didn't really understand what the commitment was.
So it came out of an arrogance on my part of I can do better than this, and I 
really, really want to make their experience a lot better than it is. Um, and so 
usually I would voluntarily reach out to someone and say, Hey, I know that 
you've got. X person that you're studying with, or I know that this person 
onboarded you and that onboarding is now complete, but would you like to have 
someone going forward, who you compare with, you know, maybe at a minimum of two 
hours a week, but if you wanted to bug me for questions, you can also do that.
And my prerogative was to mentor them technically. Which then kind of bleeds 
into helping them level up their career and learn how to work with teams and 
things like that. I think if you start with the technical call, it sort of fans 
out to them. So asking other questions about how their career relates to the 
technical side of what they're learning as well.
And so it just came out of an, a want to make other people stronger in order to 
make my own engineering team stronger. And also, uh, I have a teaching 
background, so I do miss teaching a little bit. Um, and so it kind of helps me. 
Express that as well.
**Michaela:**: [00:31:27] Yeah. I mean, when you explain that, like that, 
I feel like, Oh, I want to be a mentee.
It sounds really cozy and dinner. I would have, if 
somebody reaches out and offers, you know, to, you know, answer some questions, 
I actually didn't experience that in my career. It felt like, Oh, I can go 
there. And. It would have helped so much and still worked. Right? I mean, right 
now, actually I'm seeking out mentors a lot more pro actively, but I've never 
had a person come up to me and say, Oh, you know, do you need some help?
**Suz:**: [00:32:03] yeah
**Michaela:**: [00:32:03] So right now I'm really seeking out mentors and, you 
know, proactively approach people and ask questions. I don't think that they 
think they are my mentors. I feel they are my mentors, but yeah, I totally, you 
see the value in that. And I think it's so wonderful that you do that. And so 
you also said that you're starting with the technical side, which I like a lot, 
because that's concrete.
Right. That's, you know, you're sitting down, you're looking at the piece of 
code, they have questions, you know, about 
**Michaela:**: [00:32:30] how to do  something. Yeah. And yeah, it's, it's, it's very 
concrete and it's very clear. And then it evolved into something more. So you 
also said that you're helping them advancing their career.
So, um, how do you do that for yourself? How do you develop your soft skills, 
communication, conflict management, empathy, and also, you know, fitting into a 
team and things like that. 
**Suz:**: [00:32:55] I actually find this side of. Engineering really, really 
challenging. And so you discussed before how you didn't really have any mentors 
in your career so far, and you've only just started doing that.
I didn't have a single mentor until I actually started at Microsoft and the 
person they paired me with was just. Like so incredibly the same as me, which 
was very helpful. Um, and so I would say that developing those skills for myself 
was a lot harder and came a lot later in my career. And so that mentor, because 
I knew that there were a very similar personality to me, but they'd been at the 
company a year and a half and in had enjoyed quite a lot of success.
I knew that if it was possible for them to achieve success, even though there 
were different things at play, for example, uh, Uh, this, this mentor was a man, 
I'm a woman. And so obviously we have different sort of cultural things that we 
can, uh, different cultural challenges we can run into. I figured that if they 
were able to be, um, successful with their mindset and their approach to things, 
then maybe I could be successful too.
So I just tended to ask them a lot of questions. I, I tended to interrupt them a 
lot and say, hi, I've run into this challenge where I want to work with X 
person, but it seems like they're not. Super willing to work with me. Have you 
bumped into that before? And how did you solve it? And so it was a very slow 
process of me just saying, do you ever feel like this?
And they'd be like, and I'm like, well, how did you solve that? Um, mostly 
because I think that I've gone through. Like a huge chunk of my career being the 
only developer or the only front end developer or the only technical person in a 
company, you know, that was my first seven or eight my career. And so landing on 
a team when you wrote that many years into your career is incredibly 
challenging.
And I really just had to bunk it down, observe people, try and mirror the 
behaviors until I figured out enough to be competent. And then from there, I 
could sort of ask some of the harder questions. And so it definitely just, if 
you don't have a mentor trying to kind of model yourself after others, you 
admire can be a very effective way of sort of upgrading your skills, so to 
speak.
**Michaela:**: [00:35:03] Yeah. That's what I'm doing now a lot. And so, and so 
have you ever thought about, you know, becoming a leader manager thing like 
that, or do you want to stay in the individual contributor role? 
**Suz:**: [00:35:19] Yeah, this is a huge challenge in my career. I think just 
given that there aren't, there aren't actually that many women who I encounter 
very often now who have been yeah.
And the industry, as long as I have. And, um, there, there are like quite a few 
don't get me wrong, but you just don't encounter them very often. So sometimes I 
feel alone in this, but I've been a tech lead twice. That's the closest I've 
gotten to management and I've had people unofficially reporting to me.
Before bed, it's been more of a mentoring role and it's not like a pay grade. Or 
official title. It's more just that, Hey, this person really likes learning from 
you. So can you just check in with them and do one-on-ones every week, but I'm 
not actually doing their expenses? Um, I think that's the closest I've ever 
gotten.
It's not something that I'm interested in, in the slightest. I love sitting down 
and just coding every day. I mean, in developer relations, you don't get to code 
like, you know, for the entire eight hours, but I still get to ship stuff. I 
still get to focus on. APIs. And I still get to like sit around and mess around 
and Docs seeing if I can, you know, make an experience better.
And, and I still get to actually open PRS and look at other people's code and 
talk to people and have those technical conversations. Some managers are able to 
juggle a little bit of both. Um, but I just don't think that I'm the right 
person for that. I think that I still would need to work on my conflict 
resolution skills, um, and things like that.
I just don't know that I have the right stuff, but I'm also not super interested 
in becoming so good at this stuff. That being a manager would be easy. Um, I 
would rather just be. Really good at working with other engineers, really good 
at talking to the business and really good at coding. If I could just have that 
lovely trifecta stay in individual contributor and keep shipping things, that 
would be my perfect balance.
And so I've definitely turned down almost every management role or anything that 
looks like management. These days. I tend to run away from just because my 
tech lead experiences weren't particularly, uh, fulfilling either. 
**Michaela:**: [00:37:23] And do you have the feeling that at Stripe you can 
stay and progress as an individual contributor?
I know that at Microsoft is individual contributor path can really, you know, 
you can advance your career and really become a thought leader in the company. 
Right? So it's something similar happening at Stripe. Do you see that? 

**Suz:**: [00:37:42] I've looked at the engineering ladder is there's a slightly 
different engineering ladder for develop relationships just because we're not 
just sitting around shipping stuff all day.
Right. So you have to show leadership and not just writing good code. Um, and 
obviously engineers have to also show good teamwork skills and technical 
leadership skills too. I'm not discounting that. Um, but yeah, we do actually 
have different career ladders, even just within engineering for different roles, 
which I really like because that's tailored towards, um, Making it clear what's 
required and making it clear what your opportunities are.
So in a lot of the engineering letters that I've read internally at Stripe, 
there are actually focused in the road where you can go towards the manager 
track, or you can fork off the other way. And the manager track is kind of seen 
as a, is more treated as a career change as well, which I really liked just, 
just from a cultural perspective.
Um, and so I think that that's been a really. Good thing to give me the 
confidence that I'm going to have long-term success here, because I can already 
see examples as well on different product teams and engineering teams of people 
who have succeeded at that. And people who I can talk to in order to find out, 
you know, like what was successful for them to reach that level.
**Michaela:**: [00:38:51] Yeah I really like those career change mentality that you think 
a management is a career change and isn't the progression, right? And if you are 
not becoming a manager, it means that you somehow stack which. Is somehow 
implied that some companies, but I see more and more companies that really have, 
as you said, these career change mentality where just, you know, can go on with 
what you're really passionate about.
And, uh, well that's technology, right. And thinking with your code and things 
like that, then that's what you become an expert on. Right? 
**Suz:**: [00:39:24] There's also another distinction within the, I guess like 
the individual contributor track, which is, there are certain career levels 
where you can communicate that you don't want to proceed to the next level.
Does that make sense? And so for a lot of people, that sounds counterintuitive 
and it sounds really unambitious, but I don't. Necessarily think that's the 
case. And so you can reach a certain level where you can just say, I would like 
to stay on this level now for X amount of years, or I would like to stay here 
forever, or I would like to stay here until I changed my mind.
And what that means is when people have different abilities, different 
capabilities, different thresholds, for things they might just. Really, really, 
really, really love the work that they are expected to do on a certain level. 
And they don't want to give that up. And, and, you know, they don't want to feel 
pressured to move to the next level of taking on things that aren't necessarily, 
um, something that they would really want to get up.
Out of bed in the morning to do, I think that's an enormous privilege to have in 
a company where you're, you know, where a lot of the time, the mentality, you 
always need to be like being the absolute best, you know, but that's a really 
subjective term because moving up levels doesn't necessarily mean you right.
Actually improve at what you do. It just means that yeah, you satisfied certain 
requirements or you got really lucky and got a really large responsibility 
project and, you know, The, the CEO noticed it in, you know, thought that that 
should be recognized. I think it's really wonderful to just say no, actually I 
think I'm actually really good here right now.
And that can be really supportive as well for people who may not be in a certain 
situation in their life where they can take on that extra challenge either. And 
I just, that was something that really stood out to me when I started at Stripe 
where you can actually. Um, opt to stay at a certain level.
Once you've gotten to a certain competency within the company, 
**Michaela:**: [00:41:10] I really loved it because, um, there is there, I think 
it's a comic or something where you see that people, you know, they always 
progress to the next level until they are completely out of their competency. 
Right. So they're incompetent in what did you and yeah, you're, you're totally 
right.
If you are good at what you do, right. And you love what you do have a passion 
for it. Why change. Maybe sometimes, and maybe it's for a several years, maybe 
it's for half a year or whatever. Right. It's just right to be where you are. 
And I think it's really about seizing the moment and it doesn't have to always 
be the change that you're striving for.
I really like if you can have both, right. So I know that there are some 
companies that when you're hired into it, it's expected that you always stay in 
that. I don't think that's really a good thing,  but. 
**Michaela:**: [00:42:00] I love that if you have, if you, if you can choose 
right now, I'm feeling that I can do something else I can take on a new 
challenge.
Or as you said, I am staying where I am, because I'm actually doing really good 
work right now. And I like it. 
**Suz:**: [00:42:14] Yeah, I think it gives people space to do that best work. And 
sometimes their best work is not necessarily going and learning something new. 
You know, sometimes it's just that they're just going to be so ultra valuable on 
something and, and, and an Alliance so well with the team and, and them as well.
And I think that's a wonderful thing to celebrate and something that tends to be 
judged as being on ambitious. And I think that that's the wrong way to think 
about it

**Michaela:**: [00:42:37] yeah yeah, I agree. So one of the things that I want to talk 
with you about is the regular live coding events that you have on Twitch. So, 
first of all, can you tell me a little bit more about that I've coding and also 
to the listeners as well is live coding.
Why do you do it? How did you start? You know, everything, we want to know 
everything. 
**Suz:**: [00:42:57] So live coding tends to fall into two different tracks. Um, 
I'm on one of them, there's the track that you actually perform at a, like a DJ 
and new live code visuals and things like that. So sometimes I can get con 
people can get confused about the two definitions.
So that's one definition. I have friends that do that. The other definition, 
which is. Probably like a more recent one is the phenomenon of, um, of coding, 
but then sharing yourself, coding live via the internet. So that's usually 
sharing your screen. Um, sometimes it's sharing your webcam as well and your 
voice, and then people can just watch and listen to your process, um, and 
actually see that live via a video stream, essentially.
Um, and so that's what I do every Sunday. I've been doing it for around three 
years. Um, I take breaks if I need to travel or if. Or whatever, but it's 
usually almost every single Sunday and we just sit down for two hours and I 
explain some pull requests that I'm looking at to potentially merge, or I'm 
preparing a demo for a talk that I'm giving, um, that's coming up or just really 
anything that I need to get.
Done on that Sunday that I'm going to enjoy working on. Um, you know, I like to 
kind of show that and I think it's, it's fun for people to learn from, but it's 
also fun for me cause I learned from other people as well. And it just provides 
me with a little company while I'm working on something. 
**Michaela:**: [00:44:17] I imagine it's super stressful, to be honest.
I mean, I'm very afraid of interviews for example. And it also, if somebody 
looks over my shoulder that I'm not very familiar with. I mean, if it's a 
colleague that I trust that's okay. But so some stranger, for example, looking 
over my shoulder, I sometimes forget where the keys are on my keyboard someday.
I can't type anymore. So, how do you deal with that? Do you enjoy it? Do you 
enjoy it from the beginning? And that people actually see what you do? Do you 
get nervous? And if I would like to do that, what would you advise me? How can I 
go get over my fear of being observed and judged and things like that? 
**Suz:**: [00:44:59] I think this is a very valid concern.
And just for the record, I still perform super badly in interviews, especially 
white boarding interviews and things like that. Like if you ask me the question 
casually, when I was in my house, I would be able to immediately solve it. Um, 
but if. You put me on the spot in a power dynamic where someone is literally 
judging me on my abilities, and has something that I want to such as I would 
really like this job and impressing this person relies on that.
Then I completely fall apart. I forget basic programming concepts. I just don't 
know what it is. And I've tried to overcome that for years with live coding. It 
felt very similar at first. So you're not actually wrong likening that. Um, and 
I used to rehearse what I was going to do the night before, which meant 
essentially I was doing double the work because I would basically type it out, 
see where I was going to get stuck.
And then the next day I would do exactly the same thing, which, which, which is 
very counter intuitive. And you could tell at first I was trying to impress, but 
I was also trying to provide a really good experience for other people. It was 
more about them than it was about me, even though it was also about me trying 
not to look like I.
Hadn't you know, trying not to look like I'd forgotten how to program. Um, but I 
eventually became comfortable just because you start out with a really small 
audience when you live code, because not. Not a lot of people know what you're 
doing. You don't even have to tell anyone what you're doing. And you could just 
sort of like very slowly ease into it and get used to that's the technique that 
I used, you know, I, for the first month I rehearsed every single project I was going 
to work on and also just didn't really tell anyone about it.
Um, then I started watching my videos back, looking at what, you know, issues I 
was running into and things like that. Gaining the confidence, looking at what I 
actually liked that I did. Good. Um, and gaining confidence through that. And 
then I just slowly kind of stopped caring about it. Um, And, and I actually 
couldn't live code on stage much easier now, too, if I'm doing a demo or 
something, I think for me, it's when people are looking at my fingers, I forget 
how to type I'm exactly the same as you.
Um, but on the stream, they can't actually see your fingers. They can see how 
slow you're typing, but they can't necessarily see your fingers. The, the one 
thing that I will say, though, is. When you're coding by yourself and you're 
listening to the perfect music or you're listening to silence or whatever, 
you're always going to be very productive compared to when you're on the stream.
You know, I'm looking at the chat, I'm trying to talk aloud while I'm 
programming, I'm running into bugs. And again, I'm feeling those judging eyes on 
me when, when I run into bugs and I do the exact same thing in interviews where 
my mind goes blank. So. It's going to happen and you have to be comfortable with 
the fact that some people are gonna think that that's literally your coding 
ability and you can't do anything about that.
But I tend to try these days to communicate and defend that live coding is much 
harder than it looks and you will never, ever be as smart and fast and 
productive as you are when you're alert. 
**Michaela:**: [00:47:52] Yeah. I mean, I have two kids and if they make a scene 
in a wild and then all the other parents look at me and I feel super Josh,
this reminds me on that. Oh my God, I'm not that bad parent. You know, it's 
just, it looks like. 
**Suz:**: [00:48:13] Exactly. Yeah. I actually spoke to a young parent who she 
said the same thing to me this week and she's a programmer as well. And it was 
funny that we were comparing. 
**Michaela:**: [00:48:22] So, um, why do you use Twitch and not YouTube?
Um, there's is there something like a streaming community on YouTube as well, or 
is Twitch the platform, if you want to do that, 
**Suz:**: [00:48:32] there is, it's kind of odd because I think that 
conceptually YouTube makes more sense because YouTube is a variety platform. Um, 
whereas Twitch is more geared towards gamers. I think the difference is that 
Twitch started out as a streaming platform like live streaming and YouTube has 
more sort of expanded into that offering.
So I think that Twitch has a better foothold and a better and deepest story 
about the nuances of how different live streaming is to prerecorded videos. I 
think that YouTube is catching up, but I find that. The discover-ability of live 
streams on Twitch, based on categorizations and things like that. And then also 
just the different and very nuanced moderation tools on Twitch.
Also just better in general, even though it's designed for gaming platforms and 
it can be a very strange phenomenon of weird cultures of remotes and, you know, 
Different ways of getting streams, his attention and things like that. I think 
that it's just a more mature platform is to knowing what stream is need and the 
tools that they need in order to get the job done.
**Michaela:**: [00:49:43] So I watched some of your past streams because they 
are actually on Twitch as well. And you can go there and you can just replay 
one of those. And they started, well, there's a lot of chat going on and I've 
wondered, how can you even, you know, how can you not only chat? I mean, there 
are several people, I mean, a hundred people.
Writing to you and your one person that has to respond or read every comment, 
and then you have to do the other task as well. So do you, do you do that on 
your own or do you have another person that actually looks at, because I know 
for example, for webinars, do you sometimes have a team then, you know, you're 
giving the.
 talk. And if I, for example, have a webinar, they teach something. 
Then I have a team. Maybe that's handling the questions with the audience, but 
for that, it looks like you do everything yourself.

**Suz:**: [00:50:33] It's so hard. It is really hard. And this is 
where I come back to. You just become the worst programmer in the world because 
you're basically.
It's like, it's like people dancing in front of you and like, and like asking 
you questions about every character you're typing to get work done in an 
office that was like that where everyone it's like yelling at you all at once 
while you're trying to type something. Yeah. So you are correct. And I have 
between 250 and 300 people, every stream that watch me.
And on average, I have around a hundred people in the chat. So you, you are 
correct that it is really hard. Um, I try to just sort of. Subconsciously have 
like a time box where I'll code them. Talk for a bit, then I'll look at the 
chat. Maybe I'll have to scroll up a little bit. Cause it was too much activity.
And then come back at the, you know, sort of answer the questions, come back and 
then keep coding. Um, you'll, you'll notice. And that when I watch my own 
streams back, just for analysis, you'll see that there are some questions where 
I'm like, Oh, I missed that question. Or she ignored that person. So, you know, 
there's no way to do it perfectly.
Um, but I found that. After I've made some of my, my regular viewers who are 
really, really. Good community members. I've made the moderators a lot of the 
time, I will answer questions that have very common that come up such as what 
font is that in your terminal? Or are you using theme or, you know, like what 
project are you working on right now?
So we have chat, command, chatbot short cuts that can help answer some of those 
common questions, which leaves me more time to kind of look at some of the more 
meety questions, but I don't have a. Perfect answer for this because it is 
actually really hard. I just trained myself to, after a certain amount of time, 
just, you know, feel like, okay, I should look over him and have a look at it.
But yeah, it is, it is, it does feel like a one man band a lot of the time. Um, 
even though I do have moderators that helped me out with some of the most simple 
stuff. 
**Michaela:**: [00:52:24] And so why do you do Don? Why do you do live coding? 
What, what do you get out from out of it? Yeah. What motivates you to do that? 
**Suz:**: [00:52:31] I think initially I was feeling frustrations with, um, a 
few things, which was why I started the first thing was like, when I mentored 
people one on one that didn't scale very quickly.
Um, and I felt that. People kept, I guess, putting me on a pedestal because of 
the open source work I did because it's like hardware and IoT related, but they 
didn't understand no matter how many times they tried to communicate it that 
well, if you want us to contribute to this project, you don't necessarily have 
to have.
Any electronic knowledge, because I am still coding it all in JavaScript. So if 
you know JavaScript, then there is still, you know, a lot of areas of my 
software where you could improve certain patterns or you could help me update 
dependencies, or you could fix documentation, or you could just, um, You know, 
refactor small parts to a more modern version of, you know, um, the JavaScript 
language, you know, because I have a lot of stuff that I wrote in the  ES5 
that's all we had back then, you know?
And so I try to convince people of that and they just sort of smiled and nodded. 
Um, and so I sort of sort of thought, well, I'm just going to show people. And 
I'm also going to show people that I'm not some hardware wizard that gets 
everything perfect. Every time I do make mistakes. And you know, I want people 
to see why I enjoy working on open source.
In my spare time as well. And maybe people will be less afraid of contributing 
and maybe I'll be able to make some more friends via open source, you know, that 
way.  
**Michaela:**: [00:53:59] And do you feel that you made some friends in that 
community now on Twitch?
**Suz:**: [00:54:03]  Definitely. In fact, in, I think just over a week's 
time, I'm going to meet two of them in Europe, which I'm really excited about 
it.
There are two people who, uh, have been contributing to one of my projects for 
almost. I think a year and a half now. And they're just the most wholesome, 
wonderful people, uh, who turned up in my stream a lot. Uh, they're both 
moderators as well. They helped me, you know, moderate, any bad behavior I have. 
And.
Honestly, the project is so much better as a result of contributions from not 
just those two people, but a lot of other people. And so it's, it kind of is 
this reminder every Sunday that there are nice people on the internet. And I 
think that. In enough is a reward to me knowing that yeah, there's people out 
there who understand why I'm doing this.
You understand that I'm trying to create nicer communities and are willing to be 
part of that and help me defend that community. 
**Michaela:**: [00:55:04] Okay. That sounds really nice. So Twitch is really a 
cornerstone for you to build your community, to make open source, more welcoming 
showing, you know, show you to the people, communicating on a on again.
I think it comes to me back to how you mentor, right? You start, you said you 
start with code. You're actually start with the problem with, with the hard 
facts. Right? And if you are. Using Twitch and is showing how you code, how you 
approach problems. You're again, back at the very basic of what programming is 
about.
Right. Well, even though you said you started three years ago, I think it's a 
very new phenomenon. And, um, it's just getting, it's just starting to get 
traction all over the place. What do you think what's the future of live coding? 
**Suz:**: [00:55:52] Yeah. I mean, there were people before me too, such as 
handmade hero and, um, phlegm Flamborough game studio.
But I think that now people are starting to actually understand why it's 
beneficial. Um, and I think that a younger generation who loves to learn from 
videos is definitely, you know, rising up into our field. And, and, and, and so 
it's gaining a lot of relevancy from that too. So yeah, I think this was an 
insightful chat about it.
**Michaela:**: [00:56:17] Well, thank you so much for joining me today. I think 
we've talked a lot about very different topics areas. So if we want to reach 
you, we can go on Twitch. Well, how do I find you there? 
**Suz:**: [00:56:32] Yeah. So in most social media, my, um, username or handle 
is NoopKat or new Paquette. You can pronounce it any way you like, and that's 
N double O P K a T.
Um, and so I am twitch.tv/noopkat. And on Twitter, I am twitter.com/noopkat as 
well. 
**Michaela:**: [00:56:51] Yeah, I will link everything in the show notes so that 
people can find you. Thank you so much for showing me, you know, your work and 
also, yeah. Getting me some insights into live streaming. So thank you so much 
for joining my show.
Thank you so much. 
**Suz:**: [00:57:06] Thank you. 
**Michaela:**: [00:57:07] Okay. Bye. Bye. I hope you enjoyed another episode 
after software engineering unlocked podcast. Don't forget to subscribe. And I talk to 
you again in two weeks. 


