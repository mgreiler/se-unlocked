# Transcript Episode 30 with Ben Lesh


**Michaela:** [00:00:00] Hello and Welcome to the Software Engineering unlocked 
podcast. I'm your host, Dr. Mcayla. And today I have the pleasure to talk to Ben 
Lesh. Ben is a senior software engineer at Citadel Securities, Citadel 
Securities, a FinTech company in the market maker. They provide seamless trading 
experiences and tools for asset management, bankers, brokers, and many more.
Before that Ben worked amongst other companies at Google and Netflix, but it's 
also the project lead for our RXJS. And RXJs is a library for composing  and 
event-based programs by using observable sequences in general, Ben is active on 
Twitter and in the tech community and the big Edward kind of reactive 
programming and observables.
Well, I could go on and on, but let me just say to them Ben is on the show. So 
welcome Ben. 

**Ben:** [00:01:05] Thanks for having me. 

**Michaela:** [00:01:07] Yeah, I'm really glad you're here. So Ben, you have 
been working for some pretty large and precision corporation. There's a lot of 
folks want to work as well. Do you want to share a little bit with us, how you 
kickstart your career?
So can you walk me through  how you started, , and how, hi, you got the first 
job in, in 


**Ben:** [00:01:26] engineering. Okay. Okay. So, I've been doing this now for a 
long time. It's been almost 23 years. And, when I started the, the environment 
was quite a bit different. It was during the first.com boom.
and I was, I was actually a print designer, so I had dropped out of art school 
and I got a job as like a graphic designer doing like brochures and pamphlets 
and that sort of thing. And I helped out a little bit with a website that they 
had not very much just a little bit. And I thought, well, this is kind of fun.
And I had somebody teach me a little bit about it. and I applied for a job. It 
was a, it was a part-time job doing updates to a, very ancient e-commerce site. 
and it was, it was supposed to be four hours a day for one month was the 
contract. And it had been sitting there for awhile and there weren't a lot of 
takers because it's such a short contract.
I think at the time they wanted it, they wanted to pay a lot of money at the 
time for where I was, which was like $80 an hour or something like that. And I 
applied and I, of course, was not qualified on paper at all. not even close. And 
so I called every single day until finally someone asked me what they could, 
what they could do to get me to stop calling them.
And I said, well, if you get me in for an interview and they don't like me, then 
I'll, you know, I'll never call it's fine. And. They said fine. So they brought 
me in for an interview and, you know, they asked me questions and I maybe got 
half of them. Right. I didn't get all of the questions. Right. And I said, so, 
you know, we're going to ask you, I said, you're going to ask me, you know, why 
someone that's not qualified on paper as is applying for this job.
And I told them that, you know, it's, it's something that I really enjoy doing 
and I wanted to learn and do more. And I also told them that. I felt that it was 
going to be hard for them to find somebody that wanted to only work four hours a 
day for a month. And that I would work for $10 an hour instead of 80, just 
because I wanted the experience.
And, they, they said that sounded pretty logical. And so they decided to, and I 
even said that you could, even at that rate, you could even hire somebody else 
for the same money and like, keep me too. And they kept me for like three months 
or whatever, and they gave me a nice recommendation. And then after that, there 
was such a demand at the time.
But having some experience under your belt really helps you find another job. So 
that's kind of how I got my first, job in tech. And from there I worked through 
like a lot of consulting jobs and doing different types of, mostly front end 
back end sort of web development. And at some point years into I was a dotnet 
developer.
I did some, angular development and in order to learn angular because the 
documents weren't documentation, wasn't very good. At the time, I answered a lot 
of questions on stack overflow, because I felt like I was helping other people. 
And I also felt like I was learning. I'd find questions. I didn't know the 
answer to, and I'd try to figure out the answer.
So that way I learned things. And I got into just the right time. And like a lot 
of my answers tended to be more popular answers in stack overflow on that 
subject. And some folks that were working at Netflix, started building an 
angular app, which they ended up not making an angular app at all, but, they saw 
my name repeatedly and they thought, well, maybe we should, we should, try to 
get this guy to come in and.
I got an email and I thought it was one of my friends spoofing an email, right. 
Like why would Netflix be trying to recruit me? and so I said, Oh, you know, 
I'll talk to him on the phone. And then they said, Oh, we'll bring you out. And 
I thought, okay, well, I'll free trip to California at the very least I'll go 
out and do that.
And at the time I hadn't really traveled to California. So I went out and did 
that. And, then, you know, next thing you know, you've got somebody important 
walking you to like a VP walking to the door and you're like, okay. So it sounds 
like there's going to be a job offer, but there's no way it's going to be enough 
to move my family to the most expensive city in America.
And then, and then it was, so, but the, the real point is like the way that I 
got into like this Fang companies like Google and Netflix and those sorts of 
things really. a lot of my career has hinged on helping other people. Like if 
you are doing things to help other people in stack overflow, I did stuff to 
contribute on, get hub, and I, you know, tried to be as positive as I could.
getting a foothold contributing and get hub on like large projects is very hard. 
you have to be willing to, you're going to get, you're going to send something 
in. It's going to get rejected. You're going to have to state your case as 
clearly and plainly as possible and accept rejection. If it, if your PR doesn't 
land or whatever, and then not give up and try again.
And, but like people will see and remember positive interactions with you. and 
then, you know, when you get a chance to network with some of these people, You 
know, they, they remember that stuff. So a lot of like contributing to open 
source and answering people's questions online and trying to be a good citizen, 
you know, outside of just my office, like in the web community, has done things 
like it.
It's the reason I work in an RX. Yes. Right now, like I was asked to work on a 
rewrite of arcs. Yes. It's not something I just took upon myself. And I even 
told them that I wasn't, wasn't qualified to do it. When they asked me to do 
that. So, yeah, I would, I mean, people that want to get in at a company like 
that first and foremost, the easiest way to get into the car Google is to go to 
school, get a CS degree, and then, you know, study up on your algorithms and go 
through their whole recruitment channels.
but like, I don't have a CS degree, but I have a lot of experience. and. The 
route that I took to get in there. It was probably, it's probably more that I'm 
lucky. I'm lucky. That's probably a little bit more difficult, but like is, open 
source contribution and community interaction and, you know, trying to be a 
positive person and on the web, And those things can get you a long way, even, 
even in just to like a smaller community too.
Like if in a smaller city or a less tech centric city than, like say the Silicon 
Valley area or something like that. So I know I rambled there for quite a bit, 
but, 

**Michaela:** [00:07:31] , I think there are so many good things there because I 
know for example, the time that, so when I, for example, started working at 
Microsoft and we moved to the U S .
So I wanted to take my husband with me and, Well, he didn't get a visa in this 
year. So because they like had the lottery or something. and then, so he tried 
to find an apply for jobs that would sponsor visas. This means also that you 
have to get known by these larger corporations, right.
Because the smaller ones are not that likely to actually sponsor a research 
ships and things like that. And it was really hard to just be noticed. So even 
though, you know, he has a CS degree, for example, or, he knows algorithms and 
he studied a lot of algorithm because he wanted to make those, you know, yeah.
Make those interviews. it was just really, really difficult to get your foot 
into the door. Right. The people, even that, I mean, you're a, one of those 
thousand CVS that they are getting daily and, and, they did just go through, 
right. So he didn't even, he wasn't even, invited to make the first interview 
round.
 So there was this, there was this first step that was just so difficult to get 
in. that there was no, there was not even the chance to prove that, you know, 
your stuff or something. So I think that what you're saying, being. Online being 
not as well, having people remember you and know you, right, showing up in a 
different way is really something that compliments your chances 

**Ben:** [00:08:57] to, 

**Michaela:** [00:08:57] to be seen, right.
And also to kickstart your career. And it doesn't have to be like four days, but 
for many other things, also smaller corporations, smaller companies, consulting, 
gigs, everything I think will be, will be easier. If you are, if you're a little 
bit known, right? It's easier. You're trusting people more as well.
If you're seeing their work already out, out there, right. You can follow them. 
You see what they're talking about? It seems that you know them, even though you 
don't. Actually know them, 

**Ben:** [00:09:26] right? Yeah. So I mean, the way I got into both Google and 
Netflix were through recommendations. Right. and, Google in particular was from 
a recommendation from a Googler.
and you know, I wouldn't have that if I wasn't interacting with other people 
externally, th the truth of the matter is there are millions of people in this 
world that are smarter than I am, are better developers than I am. Like. I'm 
sure of it. I'm totally sure of it. the difference is in some cases that, you 
know, if, if I put my resume next to somebody else's, and there's a higher 
probability that they've, if they use ArcGIS or anger or something, like there's 
a higher probability, they've seen my name before.
and that, but that doesn't mean I'm better than the other person. That's just, 
it's just something that helps you out. But like that goes on a smaller scale. 
If you, If you're like again in a smaller community, you're active in meetups. 
That was I've, I've gotten jobs through meetups and like Pittsburgh and Columbus 
and those areas where, you know, I had a contract come up and I thought, well, 
you know, and now I've got to find.
Something else. And like immediately found something else because I had a 
network of other people. I knew they knew who I was that I had spoken at the 
meetups and, you know, they, they knew I kinda knew my stuff. So, you get those 
recommendations and, in my, in my personal opinion, Recommendations to get a job 
at a company hold more weight than a lot of the other vectors that are involved 
in hiring somebody.
I mean, they all, I mean, you're not going to get a job just based off a 
recommendation alone at most at any large company and most even small companies, 
but, you know, making sure that you're kind to other people and making sure that 
you speak up so people know that you're a smart person. Those are important to 
get, to getting jobs, getting promotions.
I, sometimes I see people are, I've worked with people that are brilliant, but 
very quiet in meetings. and it's their prerogative. I mean, I want people to be 
comfortable at work. I'm not saying that they should make themselves 
uncomfortable, but, you know, it's being when you're, when you're a smart person 
with things to say, being quiet in the meeting, doesn't do you any favors 
because then sometimes the important people that make decisions about who gets 
promoted or who gets.
You know, who they want to move to, what position have no idea how smart you 
are, because you know, you, you have to wait for someone else to advocate on 
your behalf, which I'm happy to, to, but, you know, that's, it's not the same as 
them seeing it for themselves. Right. So, the, the point is, is to try to be put 
yourself out there a little bit.
It's not without risk. You know, like I didn't really ever want so many Twitter 
followers for example, but, you know, it attracts some bad attention sometimes, 
and it attracts scrutiny that you might not always want. And that happens at a 
smaller scale too. The more you put yourself out there, you know, the more you 
end up it's possible, you could interact with someone who's a jerk.
It's possible that you can, you know, stumble over your own words and get called 
out for it or whatever. But, The important bit is if you, if you hide in one 
spot and you're complacent, then that's where you'll stay. If, if you put 
yourself out there, you increase your chances, a bit. And I mean, put yourself 
out there socially in particular, like that's.

**Michaela:** [00:12:37] I think our humans are really just incredible social 
creatures. Right? So we, we like to relate to others who like to talk to others, 
we need to trust. Right. And we feel more, more willing to work with somebody 
that we know already what we get ourselves into. Right. So having a network and 
getting a recommendation is definitely extremely powerful.
I totally agree. so. Now you've worked with a lot of different corporations, 
right? So you're Netflix, Google now, Citadel securities. when you look at how 
the software engineering, practices are, right, the methodologies that companies 
are following, do you see that there's a big difference or is it all very 
similar?
Are people working in a very similar capacity at Google as they are doing it? 
Netflix or the company that you work right now? Or, yeah, where there are large 
differences. 

**Ben:** [00:13:28] Sure. I mean, there's, there's different camps. for all of 
these things, I have worked at like very small companies too. the, it depends a 
little bit on what you're working on and it depends from company to company.
So like for example, at Netflix, Netflix only hire senior developers. There's no 
junior developers there, which is it's, it's both good and bad. But like, so you 
have to have that in, everybody's kind of got one specialty and they, you know, 
you're, you're kind of tasked with coming up with a little bit, coming up with 
your own work.
Like there might be some direction that you're given as far as like, what way 
you want to go, but you're left, you know, to work amongst yourselves to figure 
out how you're all going to work together to solve problems. and, at Google, for 
example, it's, it's. There's a lot of junior developers, there's interns, 
there's, people at different levels, and you know, direction on what you need to 
do.
And this probably varies from team to team because it's a huge company, kind of 
comes down from the top and direction, how you need to do it, depending on the 
position you're in, can come down from the top. But sometimes you're in a 
position where you're a tech lead and that's your job to kind of do those 
things.
And some teams are more collaborative than others. But like there, I would say 
Google, they've got like internal tooling and everybody does things kind of one 
way. And it's this one it's like, internally I don't want to monoculture is a 
bad word, but like they've got a monitor repository. They've got like, 
everything is done in exactly the same way.
Even if various teams are working on different projects in different ways, 
there's style guides, and there's all sorts of very strict things. Netflix was. 
Every team had did things, whatever way, made them most productive. so they, 
they are different. Now. Citadel is, again, more of the environment of every 
team works in a way that makes them most productive.
it's like as far as testing and things go like it, Netflix, I worked on internal 
tooling that the idea was to kind of pivot it very quickly. And so. some of the 
tools or some of the stuff we worked on worked on that needed that were kind of 
rapidly developed. Didn't have a lot of tests, but again, they're internal 
facing only.
And then there were other tools that we worked on and developed, that had a lot 
of tests, that were, more production focused, pointing towards, you know, 
customer facing things. So, it all kind of just dependent on what team you're on 
and Citadel, again, like, right now I'm working on internal tooling.
So the focus is on, you know, rapid development and that sort of thing. So 
there's fewer tests than say, there might be for like, like Google would have 
for Gmail or something like that. Like there's not like a massive battery of 
thousands of tests. and of course there's like RSGS to which arcs. Yes.
It's used by millions of Delilah developers. So we have thousands of tests that 
we run against that. And as a utility library. So like it's the testing thing. 
It just depends like environment to environment, but the actual. Like what the 
cultural is, is like, I think kind of varies from company to company.
I feel like there's some similarities between say like Facebook and Google, 
maybe because they're large, companies at the same sort of structure internally, 
but, Netflix is much smaller, much, much smaller company. So they're run quite a 
bit different. 

**Michaela:** [00:16:41] And also the software and dam developing is quite 
specific.
Right? So you have real time on demand media streaming, right? I think it's very 
different. Like if you have like an email program or, I don't know what exactly 
now I introduced Citadel securities as a banking software, so like FinTech. but 
I was wondering what, what does this company actually do and what are some of 
the.
The programs and the software that you develop and what are you doing for the 
internal things, right? 

**Ben:** [00:17:09] They have, they have everything from, they have like 
quantitative researchers trying to like analyze markets and come up with 
algorithms for trading, to more like what I do, which is I work on internal 
tooling that can, in real time kind of show what's happening on all of the other 
services and stuff that the other teams have built and that are running in 
production.
So they have alerts that. Well, you know, the CPU load load gets too high or too 
low or too low or whatever. Like there's, there's different alerts that can set 
up and run through the system. And it's actually very similar to stuff. I worked 
on it at Netflix, but they're so Citadel, Citadel and Netflix have some 
parallels in that.
Said it all. they're dealing with, with, trading and securities and these sorts 
of like stock market focused sort of things. So they've got like, laser-focus on 
a product, like they're a set of products really, but they have all of this 
other infrastructure built around it. And Netflix was the same way where.
You know, they have there's Netflix, right? Like it's, it's a known product, but 
there's like, there's a breadth of stuff around Netflix. Like you would be 
walking through a floor and there'd be TVs torn apart there because there's 
someone working on, you know, interfacing with some hardware and some like 
specialized smart TV or, you know, there's people working on a windows thing or 
phone stuff for, you know, there's tons and tons and tons of metrics that they 
collect.
So all of the stuff around that, or maybe it's about importing assets for, you 
know, what. Cover art that you're showing to people in that sort of thing. So, 
but again, like there's, so there's all sorts of different jobs that people 
have, but they're all, you know, kind of focused towards one product where, you 
know, at a Google, like they have, I don't even know how many, probably like 
hundreds of products, thousands of products, something, and.
it's kind of just it's like there there's there's how do I put it? There's large 
groups of people working on a product probably, but they're, they're in a 
smaller silo than say the size of a Netflix and they're all kind of going one 
direction. but yeah, so different company to company. 

**Michaela:** [00:19:13] Yeah, true.
So one of the things that strike me, where, when you said, well, you have all 
seniors at Netflix, right? So, and there comes a different set of challenges. 
Can you go into that a little bit? What are the challenges? If you have like 
many senior developers and, you know, you said also, well, global, you have 
different levels.
I still imagine even Netflix, if you have like senior developers, they will be 
like the senior and then they will be the senior senior, like maybe it's the 
principal or the staff engineer or whatnot. Right. So you might have their a 
levels as well, or was it like really, if you're senior year equal altogether.

**Ben:** [00:19:46] So at Netflix, everything was equal. everybody's sr. to the 
point where it's almost an internal joke about how everybody was senior, this 
senior, that, and. There are people that fall into like tech leadership roles, 
but like, so on the, on the upside, all of the people that are senior very 
experienced and you have a high degree of confidence.
If you say, if someone says I'm going to get X, Y, Z, done. They're going to get 
it done. Like there's, there's very little chance. Cause if they couldn't, 
they'd be like, I don't know how to do that because they're senior developers. 
They'll just tell you, and then they'll tell you who they think can do that or 
how long it will take them to learn.
the downside though, the challenge to a flat or like that is when it gets large 
enough. Since everybody's vote is equal, it becomes easy for someone who is. 
Senior enough that comes in from the outside, that lacks context to downvote or, 
you know, put the kibosh on an effort that, they don't fully understand the 
history around or the context around.
and, and that was, that was something that I had seen and heard people complain 
about. and because it's like a growing pain for. For Netflix. So, so like when 
the smaller, they were the easier that, that wasn't as big of an issue because 
it's easy to come to consensus with a small group of people. But as the group of 
people gets larger and larger, especially if all of them feel as though, you 
know, I'm experienced, I know what I'm talking about here, inevitably, you know, 
everyone's wrong sometimes, but like, it's, it's a little bit more painful when, 
you know, it's like, It's you have, you have somebody with an equal voice that 
can kind of be like, Nope, sorry.
Cause you have no, there's not like one person kind of bring everybody one 
direction. Everybody can kind of go their own direction or make up, make a case 
and convince somebody that like the direction you're going is wrong or whatever. 
So it's, it's a, I think people, when you get a large enough group, there needs 
to be some sort of structure and leadership.
And I don't know, it's, it's been, it's been years since I've been there. So 
maybe that stuff has, has changed, but that was the only complaint and it was a 
very minor complaint, but it was the only complaint I had ever heard about the 
flat structure at Netflix. 

**Michaela:** [00:22:02] Okay. Okay. Yeah. And so is it more like, was it more 
collaborative or was it more competing like, 

**Ben:** [00:22:08] Oh no, it wasn't competing.
it was definitely collaborative, but. You know, sometimes people just straight 
up disagree. And when you both have the, when, when people, when, when two 
people disagree and neither one of them has authority over the other one, then 
you're at a, you're at a stalemate, right? Like then that's a problem where if 
two people disagree and one of them is the tech lead, then.
You know exactly wins. Like it's just how it is, whether it's right or wrong. 
It's helpful in keeping things going in a particular direction 

**Michaela:** [00:22:42] in, in one direction. Yeah. Yeah. Yeah. Well, so, one 
of the things that, that came to my mind. As well is what about peer 
programming, for example, are you familiar with that?
Has that been, practice at Google at Netflix, at the company that you are right 
now at smaller companies? How do you think about it? How does it fit your style, 
your programming style, your work style, and, and. Yes, very often. I'm, I'm 
asked. So I'm, I'm mainly working with engineers to make their quality is 
better.
And I get this question really often, like, should we have like, and I just got 
that yesterday again. Right? So, when, when client and their whole organization 
wants to get rid of code reviews in favor of peer programming. Right. I have a 
lot of things to say about that, but I don't want to talk about it.
I want to know what you think about is, have you experienced pair programming? 
What's your take on it and, what's your take on. Code reviews. And how can we 
combine that? Or, you know, compliment, or I 

**Ben:** [00:23:42] think that pair programming and code reviews serve different 
purposes. so pair programming, I have taken part in it.
I've been, but usually it's, it's almost like a mentorship thing when it 
happens. Right? Like, so I've, I've been the mentee and I've been the mentor. 
and, so for example, when I joined the angular team, And this is, there's some 
interesting side effects of this is like I joined the angular team.
I was working on some internal stuff and they're rendering engine Ivy. And I was 
coming across things that I was like, man, this is really difficult. And my 
manager at the time, I think just couldn't understand why it was so difficult. 
And part of it, part of the difficulty was. you know, I wasn't particularly 
familiar with the internals of the Ivy rendering engine yet, but the other part 
of it was, there were things that were legitimately difficult and kind of there.
And, there was some back and forth on it. And finally we did some pair 
programming and he, he explained a lot of the stuff that was confusing to me, 
but then it was revealed that the stuff that I found difficult actually was very 
difficult. and we, we ended up kind of like after working, working, working on 
certain things, kind of walking away from the stuff that I was originally tasked 
with doing and working on other things, but like, it was, it was important for a 
few reasons.
One is, you know, it helped us understand each other a lot better too. It 
definitely it's, it's very high bandwidth to be sitting, talking to someone face 
to face while you're. Trying to figure something out. Like it's much higher 
bandwidth than sending a Slack and then getting a Slack back and then sending 
another one with a screenshot I'm getting on back.
Like you're, you're able to kind of solve problems very, very quickly. you know, 
and the downside to pair programming is if your personalities are incompatible 
or, You know, like maybe you've got, mental health issues that make you 
uncomfortable to have to sit next to somebody for a long period of time or 
anything like that.
Then, there's there can be some discomfort to having somebody sitting right next 
to you looking over your shoulder the whole time that you're doing something. 
you know, so if people do it, I do recommend not doing it like marathon sessions 
of it, but, as opposed to code reviews, code reviews are different.
Code reviews are something that, where you take a fresh set of eyes that have 
not looked at the code yet. I ideally, in my opinion, they're familiar with the 
code hopefully, but they haven't looked at the code that's already been written, 
so they have to go through and have to figure out, okay, so what is this doing?
And that provides opportunity to be like, okay, so I don't understand why this 
was written this way. Can you maybe add a comment or, you know, why aren't we 
doing it this way or whatever. it provides a lot of opportunities to spot things 
that you just, you know, we've all sat at a messy desk before and lost track of 
how messy it was.
Right. Because it just becomes part of the scenery. And so if you're working in 
code, you get the same thing where you work in some code and there's something 
there that's kind of crap and you don't really, really, you don't really think 
about it too much, but there it is. and, it's not really noticed until someone 
that never looks at that stuff.
It looks through and says, Oh, this looks weird here. So, you know, I, I just 
think they just serve different purposes. Now that said, I think that, code 
reviews are generally less thorough than paraprogramming because usually code 
reviews, people just will do it like on get hub or in Bitbucket or whatever, 
like on the web.
And they don't actually pull the code down and run it. And. Step through it and 
look at the diff and like try to figure out like, most people won't go through 
the effort to do that with a code review. which is unfortunate. They should. 
But, I dunno, the pair programming is probably got more value, but the fatigue, 
it puts on both developers involved in that process.
I don't think is worth making it. The only thing that you can do, like everyone 
pair programs, because we're not doing code reviews anymore or whatever like 
that. To me personally, if someone suggested that I'd be like, you're crazy. 
That's the craziest thing. Should we do more pair programming? Yes. Should we 
do, should we not do code reason now?
Like we should still do code reviews. 

**Michaela:** [00:27:46] Yeah. I also think that it's very complimentary. Right. 
And, as you said, I mean, the fatigue is real, right. I think in general, I 
can't imagine many people that would say they enjoy having another person like 
that clothes all over day and, and even the energy to do that.
Right. Even a very extroverted person. I don't think this is really what's 
happening here. and, and, you know, there's like the code improvement and, you 
know, working through. Two problems, but there's for example, just the bareness 
weed contribution, you have different purposes that you could have as well.
Right? The awareness, for example, that is much easier for pair program. If 
you're not doing more programming, there's one person that knows the staff as 
well for contributes, you could have like a little bit lighter version of this 
knowledge sharing, but a little bit more spread as well. but yeah, so yeah, it 
was really interesting to hear, how you think about this.
I would love maybe also to talk a little bit about testing with you. and so you 
had touched a little bit on, is that testing really depends on, you know, where 
you are. If you're doing rapid programming, you're not testing that  much , in 
depth, but if you're having like customer facing software, there are much more 
tests that you, that you're running.
so one of the things that I always want to know, and, maybe you can, we can talk 
about this for the different companies that you have worked on, but, Did you 
have like, they're like, like automated tests. I think as developers, the first 
thing that come to our mind is like, you need to test automated tests.
and then maybe we were thinking about integrating tests and UI tests. And the 
very last thing is like manual testing. Except for the manual testing that we do 
while we are developing the software. Right. but so how was that in Netflix? How 
is that a T two Dell? how is that? Is, at Google, are people still testing the 
software manually or, is that, you know, old school and not really done anymore?

**Ben:** [00:29:31] No. I mean, people definitely are. All right. If all you do 
is automated tests, then. I roughly guarantee you that you're missing stuff. 
Like you have to manually test your stuff either by dogfooding it yourself like 
using the latest version constantly or, but yeah, all that stuff, like actually 
a Google, there's a huge dog food program for like everything.
So if you're a Googler, you like every Google property that you're using, you 
have like this little dog pop in the corner and like you're, you're using. Some 
latest and greatest version, even if it's Android or whatever, before the public 
sees it, because they want to get, all the feedback on it.
But like, it's so important to do manual testing. Like you have to, you 
absolutely have to, now that the automated testing, the tolerance for like how 
much automated testing should be in place is going to vary wildly on a lot of 
different things. Right. if you, if you've got something like. A Netflix app 
that you're going to deploy to a smart TV that is never going to be updated or 
rarely going to be updated.
Then you better be sure that there's not any bugs in it, which means you're 
going to have to make sure there's a lot of automated tests and some manual 
testing, obviously before it goes out. because once it goes out the ship sail, 
most of these things can be updated now. but like, You know, if, if you just, if 
you just have apps that are very long lived, they go out any like, deployed like 
Android app or whatever they go out.
And they they're there for a very long time. you know, maybe people never update 
their Android app or something, then you need to be very, very sure that it's 
really well tested. If you have an app that's used by tons and tons and tons of 
users, and it's your number one source of, of revenue, then? You need to make 
sure it's extremely well tested in every possible way because it's, it's the 
important front, you know, that's funneling money into your company.
Now, if you've got internal tooling, you know, in my, this is my opinion, but 
like the more tests you have, the slower development can be depending on the, on 
the type of tests. They can save you a lot in cases where you need to rewrite 
things or something like that, because you can, you can rely on your test to 
make sure that your functionality is still the same after the rewrite, but the, 
the, you don't want to slow yourself down too much.
I'd say for internal tooling and other things, and this is true for most web 
apps, but the ability to deploy redeploy or roll back. Your software is like 
another level because testing is about safety, right? Like you're, you're trying 
to ensure that you don't break behaviors. You're trying to ensure good behavior 
with, testing.
And it's the same thing with TypeScript and, you know, type checks. Those are 
just, you know, safety checks at build time. And then you have safety checks at 
testing time, safety checks from Lindt and all sorts of other things. safety 
checks for manual testing and your ability to detect problems and, read of like 
deploy a new version or roll back to a previous version is another thing for 
safety.
So it's kind of like, you know, how well are you hitting on all of those meters, 
as long as those things meet your tolerance for those things, depending on the 
app that you're deploying, that's probably what's most important. So some people 
get really into like unit testing and stuff like that. and that's, I think most 
people now know that unit testing, like everything, you can get a hundred 
percent code coverage and nothing can be tied together.
you know, most people know that that's not great, but like, you know, you have 
to have some tests regardless of what you're working on, but your tolerance for 
how many tests that you need. Are going to very unlike, you know, what you can 
afford to do part of it, like, you know, are you a big wealthy company?
great. You can afford to test everything, or are you a small company that needs 
to work really fast? Well, then you need to in with you test what's important 
and, you know, try not to worry too much about minutia. 

**Michaela:** [00:33:29] Yeah, well, in general it's, I mean, the risks are 
always a really an important part, right.
That you have to consider, like, we want to be really sure that the payment 
functionality works very well. Right. And we don't care so much if maybe, you 
know, something visual on the website doesn't look that slick or something like 
this. 

**Ben:** [00:33:48] Right, right. 

**Michaela:** [00:33:49] yeah. Yeah, very well. So, maybe the last thing that I 
want to, you know, get some input from you because you're really the expert here 
is, maybe a little bit, let's talk a little bit about .
RX JS. And I have to admit that, well, the framework name is already 
complicated, right? So a lot of consultants and I always feel like this is 
really hard. Right. You just look at the name of it. And I was like, Oh my God, 
this is hard. I'm not going to learn this right. If it's called ponder or 
something, like, I don't know, a Bunda framework or something.
I'm like, Oh yeah, this is cozy. I can do it. so, and then I actually, announced 
it by saying something that it, how itself describes itself. Right. So as soon 
Kronos, you know, sequences with observables or something like this. Right. And 
so in general, so. How can we understand as entrepreneurs, even based programs?
Right. it sounds complicated, but what is it really? And what does it enable us 
to who should look into that? And I mean, it's not that new right.  It's been 
around for a long time, but it's still, there's still, people have maybe heard 
about it, but maybe are like me like saying like our exchange sounds really 
complicated.
but we should actually look into that and, yeah. Well 

**Ben:** [00:35:00] there's so there's two concepts it's inside of our stress. 
And the most important one is, this type called an observable. it's a lot like a 
promise, but a promise gives you one value, pasting asynchronously, and it's 
done. and a promise is eager.
Like you don't have to do anything to get that, to make the promise start doing 
work or anything like that. Something else is doing work and it's delivering the 
value through the promise. So that's, that's what a promise is. And I think a 
lot of people are familiar with that concept, but, and observable on the other 
hand is this type that is, it's a lot like a function it's it's, it doesn't do 
anything until you subscribed to it.
And then it gives you three callbacks, one for each one for when you get a 
value. And that's like the most important one. The second one for if there's an 
error, delivering values and telling you that it's done with an error and the 
third one for when it's complete, when it's, when it's done giving you values 
and it's was successful, there were no problems.
and it's just, it's just this really primitive type. And it exists all over the 
place in many different shapes. Like it's not just our X that has this concept 
of an observable. but the, I doesn't matter, I mean, many different shapes. 
They're all roughly the same shape, but like the same concept. and the idea is 
that if you have this, function that gets called with your values, whenever they 
happen and they can happen anytime, asynchronously, then what you have is, and 
you also know when it's done giving you this values.
Then, what you have is a set of events. So when you first subscribed to it, 
that's when the event set starts, and then it gives you events as it goes along. 
And then eventually it says I'm complete. And you know that you're done getting 
events. So you have events as a collection, as a, as a set or a collection of 
things.
And the thing that's interesting about it gets us to the second part of RCS, 
which is different operators and the operators are what I would tell most people 
not to worry about too much like observable itself. The type is what I most 
think everybody should understand. But the operators come from the fact that if 
you have a set of events or if you have a set of things, like say, I would say, 
give you a set of apples.
If I was to give you a basket of apples, You could count them and you could tell 
me how many apples there were. You could take all of the bad apples out you 
could, so you could effectively filter them down to the good apples. You could 
take them and combine it with a set of sugar and flour and whatever else I gave 
you and make it into a set of Apple pies.
Right? So the thing about a set is it can be transformed. It can be, it can be 
filtered. It can be joined with other sets. and all sets, arrays are this way, 
baskets of apples or this way, the universe just works like this with sets. And 
so if you have a set of events, you can do the same thing.
So you can take a set of events, say mouse clicks, and you can filter them down 
to the mouse, clicks that happen on a certain spot, or the mouse clicks that 
happen when you right. Clicked or whatever. you can take. A set of events from a 
WebSocket and filter it down to just the ones you care about, or you could count 
them all or aggregate them over time or what, what, whatever.
So that's what these operators are. The operators are these operations, you can 
perform on an observable, which is a set of events and it results in a different 
observable, which is a different set of events. So it's the same thing with the 
basket analogy. So if I was give you the basket of apples and you filtered it 
down to the good apples, now you have a basket of good apples, but you still 
have a basket that was the operation performed.
So it's, it's, that's the fundamental concept with our, yes, you have these 
observables, which are the most important thing to understand. And then there's 
all of these operators that can transform one observable into another one. 

**Michaela:** [00:38:44] so we were talking about mouse clicks, but the first 
thing that I had in mind when you were talking about observable is data 
pipelines.

**Ben:** [00:38:51] So this 

**Michaela:** [00:38:52] comes, you know, right. but so how can we use it? Like, 
do we use it only in the front end or can we use it in the backend, do we have 
like data pipelines that we can use? Like these observables, this is how we 
build, for example, our data pipeline, right. In, at Microsoft also with like, 
Observable.
And event-based things where we have like these, these events that are 
happening, if you're getting data right. And you're getting it real time and 
things like this, but, Our XJS. Do you use it only on the front end or yeah, on 
the backend as well, or which languages can be combined it, I read on the 
website with a lot of languages, but I'm just thinking, because it says GS it's 
like JavaScript only.

**Ben:** [00:39:26] So our XJS is the JavaScript version of reactive extensions. 
and actually it was born at Microsoft, from, kind of as a clone of Microsoft, 
our Microsoft's rx.net. So, And arcs JS can be used anywhere. JavaScript runs. 
when I originally worked on it at Netflix, it was being used in smart TVs and 
weird, weird JavaScript run times that, you know, were not V8 based.
They're not Chrome based or anything like that. They were like their own little 
custom JavaScript runtime. So it can be used in node. It can be used and it is 
used in node quite a bit. It can be used in, browsers and electronic, like it's 
used all over the place and it's very, very primitive. The observable observable 
type itself is extremely primitive.
you could use it to develop a promise, for example, it's like lower level than 
that. So, it can be run anywhere. Okay. 

**Michaela:** [00:40:21] What are some of the, what are some of the use cases 
where you say it's not a good option? You shouldn't use it. 

**Ben:** [00:40:28] Oh, no. There's there's. I mean, yes and no. So the thing 
about observable itself is it can re represent zero events or, you know, many 
events, that are either totally synchronous or happen asynchronously.
So you can use it to represent anything. Now that said, I recommend people ex 
exercise, restraint and judgment when it comes to doing these things because, 
our XJS as a library has all of these operators and they have operators named 
things like switch map, and merge map and concat map and all these things.
And I don't know, I don't expect just any random person to walk up and know what 
those things mean. And they're almost like a domain specific language on top of 
a JavaScript. So for, for dealing with these things, they're very, very 
powerful. you can accomplish a lot, in a very concise way, but you know, with 
that, you've got some abstractions.
So there's going to be a little bit of overhead for that. And we do the best we 
can on the team to make things as fast as possible and as small as possible. but 
also there's a burden on other people around you that have to know these things 
in order to interact with this, you'll have to add a lot of comments, that sort 
of thing.
do you need arcs, Jess for loading an Ajax request after you hit a button? No, 
probably not. That's silly. You don't even need a framework for that. That's 
just a button in a fetch, right? So, there's, there's a lot of places where I 
would say you probably didn't need it. Could you use it? Sure. but is it really 
helping you in certain cases?
Probably not. Where it's most helpful is where you have to do complicated event 
coordination. Or combining of different data streams, or maybe you have a data 
stream and you're filtering it and processing it in some way and coming out, 
like in the streaming case, if someone's doing like a lot of streaming data 
coming into like a node service or, like a it's, especially if it's push-based 
streams or they're just getting, here's a new, here's a new one, here's a new 
one.
or they're doing that in the web with like web sockets or whatever, server sends 
events, you know, if they're not using RX and. Especially, if they're combining 
streams, then I would be like, Oh, here's this other tool you might want to look 
into? Because I know firsthand from writing the library and writing other code 
that wasn't in our, that, you know, trying to write, event coordination between 
different streams, yourself, particularly trying to tear them down and stand 
them back up.
And all this other stuff is it's complicated business, and there's a lot of 
places where you can shoot yourself in the foot. So. that use it where it 
belongs, when possible, but it's not going to hurt you to use another place. 
Yeah. 

**Michaela:** [00:42:59] Yeah. So I have a couple of, so the question I actually 
asked you already were from Twitter, from some of the people that I asked or 
what they want me to ask you? And there are a couple of others. one question was 
what, what is your best advice for new developers? I get it very often and I 
think it's really interesting to see different answers from very accomplished 
developers. So what do you think is the best advice for new developers?

**Ben:** [00:43:22] I would say, you know, people that are new, I think a lot of 
times when I get people that ask that, like, I'll have someone message me and be 
like, Hey, how do I become a great developer? And I think they're expecting me 
to pull out, you know, a magic wand and be like, boom, you're a great developer. 
But like the truth of the matter is it's just about consistency and patience.
And, the best thing you can do is learn how to teach yourself stuff. I mean, 
that's true for anything. Like, if you can learn how to teach yourself things, 
then you are going to do much better than someone that has to have somebody else 
teach them something. because you're always available to yourself.
Right? So, so learning how to teach yourself things is super duper important, to 
being a software engineer and being a human being in general, I think, and, and 
also being consistent, you know, consistency is something I think people 
struggle with. that's why people have a hard time with a lot of different 
things.
Like. Exercise without consistency is just moving around a lot. Like there's, 
it's the same thing with any sort of mental exercise or anything else. Like you 
have to be consistent. And again, you have to learn about yourself. You have to 
learn what your limitations are. You have to learn how to teach yourself things, 
and lightweight where we were talking about earlier with, being like putting 
yourself out there a little bit, interacting with other people.
It helps you learn, right? Like interacting with somebody else. You're going to 
learn new things. So, I would make sure to, to try to get out there and network 
and meet similar minded people. And, you know, it's risky though, because 
there's some jerks out there for sure. but, you know, it's, it's worth the risk, 
in my opinion.

**Michaela:** [00:45:00] Yeah. Yeah, I think so. I mean, you can already start 
with,  asking questions, right? You don't have to provide answers. You can 
network and ask people like I'm now. I recently started my own business and so 
right now, I mainly, participate in founder meetings by asking questions because 
I don't know.
Right. How do you do sales? How do you contact people? Right. And you can do the 
same as a developer, right? Asking questions. And I think asking questions, even 
if you're a very senior developer is the right thing to do, because there's so 
much we can learn, right. on a daily basis that there are new staff and new 
concepts and new frameworks and technologies and things like that.

**Ben:** [00:45:36] Yeah, I was going to say there's the software engineers in 
particular very much like to be asked questions because they like to feel smart. 
So you can't go wrong in this group of people asking questions. 

**Michaela:** [00:45:52] Yeah. So, maybe the, the last question that I asked you 
just to wrap up this, this episode is what do you w where do you see the future 
of our exchange?
And I actually combine it with another question, which how does that actually, 
how does it integrate with the no-code movement? Right. So on one hand, you are 
the person, you know, that the driver is actually real. Hardcore libraries for 
developers, right. That are very, very technical. So you have to understand a 
lot of concepts.
And I mean, we are not talking about like, you know, web design per se, but 
we're really going into, well, we have to understand a little bit more and 
really algorithms and things like this, which I think is the opposite of this 
no-code movement, where you have like lower building blocks that you put 
together.
So, how do you see, how does, does this actually fit together? Because I think 
there is a relation between those two, but, what do you think about this? 

**Ben:** [00:46:46] Oh, sure. so there's two questions there. The first was 
about the future of RCS. feature of RCS is primarily just focused on making the 
library smaller, more efficient and kind of keeping up with changes and modern 
platform.
So for example, abort controller is now going to become ubiquitous. So maybe we 
don't need subscriptions anymore. We can use the abort controller and these 
sorts of things. so that's the future of RCS and it's it's, it is what it is. 
It's a utility library. Now, as far as its relation to the no-code movement.
I think that RCS is a solid fit for some of the internals of things that might 
be, tools that might be used in no-code. and the reason I say this, or not even 
just RCS, but reactive programming in general, the reason I say this is because 
reactive programming is based off the principle that, you can kind of piece 
things together like Legos.
So you can say, okay, well, I've got a stream of data of this shape. you don't 
know where it came from and you don't care, but the next piece is going to react 
to when that next bit comes in and do something with it and send it off. And 
then the next piece down the way, reacts to whatever that thing is that when it 
comes in, it doesn't know where it came from and it doesn't care.
So the thing about RX is it's, it's very, It's very composable in a way that, 
that like building blocks. So you can, you could in theory, make something where 
you could literally drag and drop shapes together. That declared how you're 
going to transform some streaming data. And then under the hood, it would build 
an array of operators in RX and just kind of apply them.
and so reactive programming as it stands. Like I actually don't even know. How 
you could go about developing something no-code without some form of reactive 
programming, not necessarily arcs Jess, but, just some form of, I don't know 
where this piece came from. My job is to transform it in this way.
cause I'm a blue Lego or whatever, and then I sent it onto the red Lego or 
whatever I do. so I think that it's got a strong future in the back of that sort 
of thing. And I actually liked that idea because one of the. Struggles that 
people have with RCS is just learning all of these operators. and if I could 
find a way to just abstract them stuff away from everybody, I absolutely would 
do that because, they're the most, they're the single most powerful piece of, of 
RCS.
not the most important observable, still the most important, but the most 
powerful pieces, these operators, but they're also the thing that confuses 
everybody. Because it is a bit mind bending to deal with this multidimensional 
problem of time and, and values. And, you know, when things happen here and here 
and here, and like, you know, even though you've broken it down into individual 
steps with reactive programming, you have to know like what a switch map is and 
so on and so forth and how it behaves.
So I think that, you know, building some sort of no-code thing on top of it is, 
is a fantastic idea. I don't really know that anyone's doing that, but. Or, or 
even anything like it, there's plenty of other, reactive programming paradigms 
or, or libraries and things that people can build no code on top of it's the 
same concept.
And in my mind, it's a win whether it's RX yes or not, like it's, it's reactive 
for a programming is important for this sort of thing. It 

**Michaela:** [00:50:03] could be very powerful. I think like just flexibility 
that no coder had with, you know, having that under the hood, just 

**Ben:** [00:50:12] that right. Yeah. 

**Michaela:** [00:50:14] Well, thank you so much, Ben, for being on my show, we 
talked about a lot of things and, I'm really happy that you took the time to be 
here with me today.
Is there something that you want my listeners to know? I will definitely link to 
your Twitter profile. Is there something else that I should put in the show 
notes or that you wanted to yeah. To say before we wrapping up this 

**Ben:** [00:50:33] episode? No. No, but I'm, I'm happy to hear that you're 
starting your own company.
Good luck with that, dude. I don't know what your, your company is though. What 
is your, can you tell us about your company really quick, 

**Michaela:** [00:50:42] but my company, yeah, I actually started it already. so 
I started, a year ago. so I left Microsoft in December, 2019 a little bit before 
the pandemic. and yeah, I'm, I'm giving quadruple workshops.
And I'm consulting with, with organizations that want to improve their 
processes. And right now I'm actually writing a code reviewing tool. It's not 
for code reviews, but it's for code review analytics. Right? So when I was at 
Microsoft, I was helping all the different teams. I was also for internal staff, 
right.
So I was responsible. I was in the tool tools, the software engineers. Team. and 
so we were responsible for the 40,000 engineers and that they are, you know, 
having a good experience for build test and code reviews. but everything that I 
did was data driven, right? So we had like all the events that we had from like, 
I'm doing a committed, I'm chatting here with another person.
And so we could use this data to inform actually transformation. So like for 
example, office would come and say, Oh, we have a problem over there. Can you 
help us? Right. And so I had all these data to help them, whatever the, the, the 
question was like, can we. split up the built graph to make the build faster, 
right.
Or can we make the tests more rebel liable because we have some problems here or 
can we make code review less painful for many reasons. Right. And so, um, so I'm 
doing the same thing now outside of Microsoft for different corporations, for 
different organizations, mainly focused on contribution. and yeah, and now I'm 
building my own tool to get that data.
because now I don't have the data anymore, like at my fingertips. And so yeah, 
this is what I'm, I'm doing. That 

**Ben:** [00:52:10] sounds really cool. 

**Michaela:** [00:52:11] Yeah. Thank you. Yeah. Okay. So thank you, Ben, for 
taking the time. Thank you so much for being here and have a good day. 

**Ben:** [00:52:19] All right. Thanks for having me. Yeah. 

**Michaela:** [00:52:21] Thank you.

**Ben:** [00:53:12] Oh, okay. So, I've been doing this now for a long time. It's 
been almost 23 years. And, when I started the, the environment was quite a bit 
different. It was during the first.com boom. and I was, I was actually a print 
designer, so I had dropped out of art school and I got a job as like a graphic 
designer doing like.
Brochures and pamphlets and that sort of thing. and I helped out a little bit 
with a website that they had not very much just a little bit. And I thought, 
well, this is kind of fun. And I had somebody teach me a little bit about it. 
and I applied for a job. It was a, it was a part-time job doing updates to a, 
very ancient e-commerce site.
and it was, it was supposed to be four hours a day for one month was the 
contract. And it had been sitting there for a while and there weren't a lot of 
takers because it's such a short contract and. I think at the time they wanted 
it, they wanted to pay a lot of money at the time for where I was, which was 
like $80 an hour or something like that.
And I applied and I, of course, was not qualified on paper at all. not even 
close. And so I called every single day until finally someone asked me what they 
could, what they could do to get me to stop calling them. And I said, well, if 
you get me in for an interview and they don't like me, then I'll, you know, I'll 
never call it's fine.
And. They said fine. So they brought me in for an interview and, you know, they 
asked me questions, you got half of them. Right. I didn't get all of the 
questions. Right. And then when they said, so, you know what, we're going to ask 
you. I said, you're going to ask me, you know, why someone that's not qualified 
on paper is applying for this job.
And I told them that, you know, it's, it's something that I really enjoy doing 
and I wanted to learn and do more. And I also told them that. I felt that it was 
going to be hard for them to find somebody that wanted to only work four hours a 
day for a month. And that I would work for $10 an hour instead of 80, just 
because I wanted the experience.
And, they said that sounded pretty logical. And so they decided to, and I even 
said, you could, even at that rate, you could even hire somebody else for the 
same money and like, keep me too. And they kept me for like three months or 
whatever, and they gave me a nice recommendation. And then after that, there was 
such a demand at the time.
That having some experience under your belt really helps you find another job. 
So that's kind of how I got my first, job in tech. And from there I worked 
through like a lot of consulting jobs and doing different types of, mostly front 
end back end sort of web development. And at some point years into, I was a.net 
developer.
I did some, angular development and in order to learn angular because the 
documents weren't documentation, wasn't very good. At the time, I answered a lot 
of questions on stack overflow, because I felt like I was helping other people. 
And I also felt like I was learning. I'd find questions. I didn't know the 
answer to, and I'd try to figure out the answer.
so that way I learned things. And I got into just the right time. And like a lot 
of my answers tended to be more popular answers in stack overflow on that 
subject. And some folks that were working at Netflix, started building an 
angular app, which they ended up not making an angular app at all, but, they saw 
my name repeatedly and they thought, well, maybe we should, we should try to get 
this guy to come in and.
I got an email and I thought it was one of my friends spoofing an email, right? 
Like why would Netflix be trying to recruit me? and so I said, Oh, you know, 
I'll talk to him on the phone. And then they said, Oh, we'll bring you out. And 
I thought, okay, well, I'll free trip to California at the very least I'll go 
out and do that.
And at the time I hadn't really traveled to California. So I went out and did 
that. And, then, you know, next thing you know, you've got somebody important 
walking you to like a VP walking through the door and you're like, okay. So it 
sounds like there's going to be a job offer, but there's no way it's going to be 
enough to move my family to the most expensive city in America.
And then, and then it was, so, but the, the real point is like the way that I 
got into like this Fang companies like Google and Netflix and those sort of 
things really. a lot of my career has hinged on helping other people. Like if 
you are doing things to help other people in stack overflow, I did stuff to 
contribute on, get hub, and I, you know, tried to be as positive as I could.
getting a foothold contributing and get hub on large projects is very hard. you 
have to be willing to, you're going to get, you're going to send something in. 
It's going to get rejected. You're going to have to state your case as clearly 
and plainly as possible and accept rejection. If it, if your PR doesn't land or 
whatever, and then not give up and try again.
And, but like people will see and remember positive interactions with you. and 
then, you know, when you get a chance to network with some of these people, You 
know, they, they remember that stuff. So a lot of like contributing to open 
source and answering people's questions online and trying to be a good citizen, 
you know, outside of just my office, like in the web community, has done things 
like it, it's the reason I'm working on RSGS right now.
Like I was asked to work on a rewrite of arcs. Yes. It's not something I just 
took upon myself. And I even told them that I wasn't, wasn't qualified to do it. 
When they asked me to do that. So, yeah, I would, I mean, people that want to 
get in at a company like that first and foremost, the easiest way to get into 
the car Google is to go to school, get a CS degree, and then, you know, study up 
on your algorithms and go through their whole recruitment channels.
but like, I don't have a CS degree, but I have a lot of experience. and. The 
route that I took to get in there was probably, it's probably more, I'm lucky. 
I'm lucky. It's probably a little bit more difficult, but like is, open source 
contribution and community interaction and, you know, trying to be a positive 
person and on the web, And those things can get you a long way, even, even in 
just like a smaller community too.
Like if in a smaller city or a less tech sector centric city than like say the 
Silicon Valley area or something like that. So I know I rambled there for quite 
a bit, but, Yeah.
Yeah. So, I mean, the way I got into, both Google and Netflix were through 
recommendations, right. And, Google in particular was from a recommendation from 
a Googler. and you know, I wouldn't have that if I wasn't interacting with other 
people externally, I th the truth of the matter is there are millions of people 
in this world that are smarter than I am, are better developers than I am.
Like. I'm sure of it. I'm totally sure of it. the difference is in some cases 
that, you know, if, if I put my resume next to somebody, else's. and there's a 
higher probability that they've, if they use ArcGIS or anger or something, like 
there's a higher probability, they've seen my name before. and that, but that 
doesn't mean I'm better than the other person.
It's just, it's just something that helps you out. But like that goes on a 
smaller scale. If you, if you're like again in a smaller community, you're 
active and meetups, that was I've, I've gotten jobs through meetups and like 
Pittsburgh and Columbus and those areas where. You know, I had a contract come 
up and I thought, well, you know, and now I gotta find.
Something else. And like immediately found something else because I had a 
network of other people. I knew they knew who I was that I had spoken at the 
meetups and, you know, they, they knew I kinda knew my stuff. So, you get those 
recommendations and, in my, in my personal opinion, Recommendations to get a job 
at a company hold more weight than a lot of the other vectors that are involved 
in hiring somebody.
I mean, they all, I mean, you're not going to get a job just based off a 
recommendation alone at most at any large company and most, even in small 
companies, but, you know, making sure that you're kind to other people and 
making sure that you speak up so people know that you're a smart person. Those 
are important to get, to getting jobs, getting promotions.
I, sometimes I see people are, I've worked with people that are brilliant, but 
very quiet in meetings. and it's their prerogative. I mean, I want people to be 
comfortable at work. I'm not saying that they should make themselves 
uncomfortable, but, you know, it's being when you're, when you're a smart person 
with things to say, being quiet in the meeting, doesn't do you any favors 
because then sometimes the important people that make decisions about who gets 
promoted or who gets.
You know, who they want to move to, what position have no idea how smart you 
are, because you know, you have to wait for someone else to advocate on your 
behalf, which I'm happy to do, but, you know, that's, it's not the same as them 
seeing it for themselves. Right. So, the, the point is, is to try to be put 
yourself out there a little bit.
It's not without risk. You know, like I didn't really ever want so many Twitter 
followers for example, but, you know, it attracts some bad attention sometimes, 
and it attracts scrutiny that you might not always want. And that happens at a 
smaller scale too. The more you put yourself out there, you know, the more you 
end up it's possible, you could interact with someone who's a jerk.
It's possible that you can, you know, stumble over your own words and get called 
out for it or whatever. But, The important bit is if you, if you hide in one 
spot and you're complacent, then that's where you'll stay. If, if you put 
yourself out there, you increase your chances, a bit. And I mean, put yourself 
out there socially in particular, like that's.
Sure. I mean, there's, there's different camps. for all of these things, I have 
like worked at like very small companies too. the, it depends a little bit on 
what you're working on and it depends from company to company. So like for 
example, At Netflix, Netflix only hire senior developers. There's no junior 
developers there, which is it's, it's both good and bad.
but like, so you have to have that in, everybody's kinda got one specialty and 
they, you know, you're, you're kind of tasked with coming up with a little bit, 
coming up with your own work. Like there might be some direction that you're 
given as far as like what. Where you want to go, but you're left to work amongst 
yourselves to figure out how you're all going to work together to solve 
problems.
and, at Google, for example, it's, it's, there's a lot of junior developers. 
There's interns, there's, people at different levels, and you know, direction on 
what you need to do. And this probably varies from team to team. Cause it's a 
huge company kind of comes down from the top. And direction how you need to do 
it, depending on the position you're in, can come down from the top.
But sometimes you're in a position where you're a tech lead and that's your job 
to kind of do those things. And some teams are more collaborative than others. 
but like there, I would say Google, they've got like internal tooling and. 
Everybody does things kind of one way. And it's this one it's like, internally I 
don't want to monoculture is a bad word, but like they've got a monitor 
repository.
They've got like, everything is done in exactly the same way. Even if various 
teams are working on different projects in different ways, there's style guides. 
And there's all sorts of very strict things. Netflix was, every team had did 
things, whatever way, made them most productive. so they, they are different.
Now. Citadel is again, more of the environment of. Every team works in a way 
that makes them most productive. it's like as far as testing and things go like 
it, Netflix, I worked on internal tooling that the idea was to kind of pivot it 
very quickly. And so, some of the tools or some of the stuff we worked on worked 
on that needed that were kind of rapidly developed.
Didn't have a lot of tests, but again, they're internal facing only. And then 
there were other tools that we worked on and developed, that had a lot of tests, 
that were, more production focused, pointing towards, you know, customer facing 
things. So, it all kind of just dependent on what team you're on and Citadel, 
again, like, right now I'm working on internal tooling.
So the focus is on, you know, rapid development and that sort of thing. So 
there's fewer tests than. Say there might be for like, like Google would have 
for Gmail or something like that. Like, there's not like a massive battery of 
thousands of tests. and of course there's like RSGS to which arcs. Yes.
It's used by millions of developers. So we have thousands of tests that we run 
against that. And as a utility library. So like it's the testing thing. It just 
depends like environment to environment, but the actual, like what the cultural 
is, is like, I think kind of various from. Company to company. I feel like 
there's some similarities between say like Facebook and Google, maybe because 
they're large, companies at the same sort of structure internally, but Netflix 
is much smaller, much, much smaller company.
So they're run quite a bit different.
Oh, was. So they, they have, they have everything from, they have like 
quantitative researchers trying to like analyze markets and come up with 
algorithms for trading, to more like what I do, which is I work on internal 
tooling that can, in real time kind of show what's happening on all the other 
services and stuff that the other teams have built and that are running in 
production.
So they have alerts that. Well, you know, if the CPU load load gets too high or 
too low or too low or whatever, like there's, there's different alerts that can 
set up and run through the system. And it's actually very similar to stuff. I 
worked on it at Netflix, but they're so Citadel, Citadel and Netflix have some 
parallels in that set it all.
they're dealing with, with, trading and securities and these sorts of like stock 
market focused sort of things. So they've got like laser focus on op. For a 
product like there a set of products, really, but they have all of this other 
infrastructure built around it. And Netflix was the same way where, you know, 
they have there's Netflix, right?
Like it's, it's a known product, but there's like, there's a breadth of stuff 
around Netflix. Like you would be walking through a floor and there'd be TVs 
torn apart there because there's someone working on. You know, interfacing with 
some hardware in some like specialized smart TV or, you know, there's people 
working on a windows thing or phone stuff, or, you know, there's tons and tons 
and tons of metrics that they collect.
So all of this stuff around that, or maybe it's about importing assets for, you 
know, what cover art that you're showing to people and that sort of thing. So, 
but again, like there's, so there's all sorts of different jobs that people 
have, but they're all, you know, kind of focused towards one product where, you 
know, at a Google, like they have.
I don't even know how many, probably like hundreds of products, thousands of 
products, something, and, it's kind of just, it's like, there's, there's there's 
how do I put it? There's large groups of people working on a product probably, 
but they're, they're in a smaller silo than say the size of a Netflix and 
they're all kind of going one direction.
but yeah, so it's different company to company.
So it Netflix, everything was equal. everybody's sr. to the point where it's 
almost an internal joke about everybody was senior, this senior that, and there 
are people that fall into like technical leadership roles, but like, so on the, 
on the upside, all of the people that are senior very experienced and you have a 
high degree of competence.
If you say, if someone says I'm going to get XYZ done, They're going to get it 
done. Like there's, there's very little chance because if they couldn't, they'd 
be like, I don't know how to do that because they're senior developers. They'll 
just tell you, and then they'll tell you who they think can do that or how long 
it will take them to learn.
the downside though, the challenge to a flat or like that is when it gets large 
enough. Since everybody's vote is equal, it becomes easy for someone who is. 
Senior enough that comes in from the outside, that lacks context to downvote or, 
you know, put the kibosh on an effort that, they don't fully understand the 
history around or the context around.
and, and that was, that was something that I had seen. And. Heard people 
complain about, because it's like a growing pain for, for Netflix. So like when 
the smaller, they were the easier that, that wasn't as big of an issue because 
it's easy to come to consensus with a small group of people. But as the group of 
people gets larger and larger, especially if all of them feel as though, you 
know, I'm experienced, I know what I'm talking about here, inevitably, you know, 
everyone's wrong sometimes, but like it's, it's a little bit more painful.
When, you know, it's like, it's you have, you have somebody with an equal voice 
that can kind of be like, Nope, sorry. Cause you have no it's it's, there's not 
like one person kind of hurting and everybody one direction, everybody can kind 
of go their own direction or make up, make a case and convince somebody that 
like the direction you're going is wrong or whatever.
So it's, it's, I think people, when you get a large enough group, there needs to 
be some sort of structure and leadership. And I don't know, it's, it's been, 
it's been years since I've been there. So maybe that stuff has, has changed, but 
that was the only complaint. And it was a very minor complaint, but it was the 
only complaint I had ever heard about the flat structure at Netflix.
Oh, no, it wasn't competing. it was definitely collaborative, but. You know, 
sometimes people just straight up disagree. And when you both have the, when, 
when people, when, when two people disagree and neither one of them has 
authority over the other one, then you're at a, you're at a stalemate, right? 
Like, and that's a problem where if two people disagree and one of them is the 
tech lead, then.
You know, tech lead wins. Like it's, it's just, it's just how it is, whether 
it's right or wrong. It's helpful in keeping things going in a particular 
direction. yeah.
Sure. I think that pair programming and code review serve different purposes. so 
pair programming, I have taken part in it, on I've been, but usually it's, it's 
almost like a mentorship thing when it happens. Right? Like, so I've, I've been 
the mentee and I've been the mentor. and, so for example, when I was joined the 
angular team, And this is, there's some interesting side effects of this is like 
I joined the angular team.
I was working on some internal stuff and they're rendering engine Ivy. And I was 
coming across things that I was like, man, this is really difficult. And my 
manager at the time, I think just couldn't understand why it was so difficult. 
And part of it, part of the difficulty was. you know, I wasn't particularly 
familiar with the internals of the Ivy rendering engine yet, but the other part 
of it was, there were things that were legitimately difficult and kind of there.
And, there was some back and forth on it. And finally we did some pair 
programming and he, he explained a lot of the stuff that was confusing to me, 
but then it was revealed that the stuff that I found difficult actually was very 
difficult. and we, we ended up kind of like after working, working, working on 
certain things, kind of walking away from the stuff that I was originally tasked 
with doing and working on other things, but like, it was, it was important for a 
few reasons.
One is, you know, it helped us understand each other a lot better. To it 
definitely it's, it's very high bandwidth to be sitting, talking to someone face 
to face while you're trying to figure something out. Like it's much higher 
bandwidth than sending a Slack and then getting a Slack back and then sending 
another one with a screenshot and getting on back.
Like you're, you're able to kind of solve problems very, very quickly. you know, 
and the downside to pair programming is if your personalities are incompatible 
or, You know, like maybe you've got, mental health issues that make you 
uncomfortable to have to sit next to somebody for a long period of time or 
anything like that.
Then, there's there can be some discomfort to having somebody sitting right next 
to you looking over your shoulder the whole time that you're doing something. 
you know, so if people do it, I do recommend not doing it like marathon sessions 
of it, but, as opposed to code reviews, code reviews are different.
Code reviews are something that, where you take a fresh set of eyes that have 
not looked at the code yet. Ideally in my opinion, they're familiar with the 
code hopefully, but they haven't looked at the code that's already been written, 
so they have to go through and have to figure out, okay, so what is this doing?
And that provides opportunity to be like, okay, so I don't understand why this 
was written this way. Can you maybe add a comment or, you know, why aren't we 
doing it this way or whatever. it provides a lot of opportunities to spot things 
that you just, you know, we've all sat at a messy desk before and lost track of 
how messy it was.
Right. Because it just becomes part of the scenery. And so if you're working in 
code, you get the same thing where you work in some code and there's something 
there that's kind of crap and you don't really, really, you don't really think 
about it too much, but there it is. and, it's not really noticed until someone 
that never looks at that stuff.
It looks through and says, Oh, this looks weird here. So, you know, I, I just 
think they just serve different purposes. Now that said, I think that, code 
reviews are generally less thorough than paraprogramming because usually code 
reviews, people just will do it like on get hub or in Bitbucket or whatever, 
like on the web.
And they don't actually pull the code down and run it. And. Step through it and 
look at the diff and like try to figure out like, most people won't go through 
the effort to do that with a code review. which is unfortunate. They should. 
But, I don't know. The pair programming is probably got more value, but the 
fatigue, it puts on both developers involved in that process.
I don't think is worth making it. The only thing that you can do, like everyone 
pair programs because we're not doing code reviews anymore or whatever like 
that. To me personally, if someone suggested that I'd be like, you're crazy. 
That's the craziest thing. Should we do more pair programming? Yes. Should we 
do, should we not do code reason now?
Like we should still do code reviews.
No. I mean, people definitely. Alright. If all you do is automated tests. Then I 
roughly guarantee you that you're missing stuff. Like you have to manually test 
your stuff either by dogfooding it yourself like using the latest version 
constantly or, but yeah, all that stuff, like actually a Google, there's a huge 
dog food program for like everything.
So if you're a Googler, you like every Google property that you're using, you 
have like this little dog pop in the corner and like you're, you're using. Some 
latest and greatest version, even if it's Android or whatever, before the public 
sees it, because they want to get, all the feedback on it.
But like, it's so important to do manual testing. Like you have to, you 
absolutely have to, now that the automated testing, the tolerance for like how 
much automated testing should be in place is going to vary wildly and a lot of 
different things. Right. if you, if you've got something like. A Netflix app 
that you're going to deploy to a smart TV that is never going to be updated or 
rarely going to be updated.
Then you better be sure that there's not any bugs in it, which means you're 
going to have to make sure there's a lot of automated tests and some manual 
testing, obviously before it goes out. because once it goes out the ship sail, 
most of these things can be updated now. but like, You know, if, if you just, if 
you just have apps that are very long lived, they go out any like, deployed like 
Android app or whatever they go out.
And they they're there for a very long time. you know, maybe people never update 
their Android app or something, then you need to be very, very sure that it's 
really well tested. If you have an app that's used by tons and tons and tons of 
users, and it's your number one source of, of revenue, then? You need to make 
sure it's extremely well tested in every possible way because it's, it's the 
important front, you know, that's funneling money into your company.
Now, if you've got internal tooling, you know, in my, this is my opinion, but 
like the more tests you have, the slower development can be depending on the, on 
the type of tests. They can save you a lot in cases where you need to rewrite 
things or something like that, because you can, you can rely on your tests to 
make sure that your functionality is still the same after the rewrite, but the, 
the, you don't want to slow yourself down too much.
I'd say for internal tooling and other things, and this is true for most web 
apps, but the ability to deploy redeploy or roll back. Your software is like 
another level because testing is about safety, right? Like you're, you're trying 
to ensure that you don't break behaviors. You're trying to ensure good behavior 
with, testing.
And it's the same thing with TypeScript and, you know, type checks. Those are 
just, you know, safety checks at build time. And then you have safety checks at 
testing time, safety checks from Lindt and all sorts of other things. safety 
checks for manual testing and your ability to detect problems and, read of like 
deploy a new version or roll back to a previous version is another thing for 
safety.
So it's kind of like, you know, how well are you hitting on all of those meters, 
as long as those things meet your tolerance for those things, depending on the 
app that you're deploying, that's probably what's most important. So some people 
get really into like unit testing and stuff like that. and that's, I think most 
people now know that unit testing, like everything, you can get a hundred 
percent code coverage and nothing can be tied together.
you know, most people know that that's not great, but like, you know, you have 
to have some tests regardless of what you're working on, but your tolerance for 
how many tests that you need. Are going to very unlike, you know, what you can 
afford to do part of it, like, you know, are you a big wealthy company?
great. You can afford to test everything, or are you a small company that needs 
to work really fast? Well, then you need to in test you test what's important 
and, you know, try not to worry too much about minutia. Yeah.
Okay.
There's so there's two concepts inside of our stress and the most important one 
is this type called an observable. it's a lot like a promise, but a promise 
gives you one value. Async asynchronously and it's done. and a promise is eager. 
Like you don't have to do anything to get that, to make the promise start doing 
work or anything like that.
Something else is doing work and it's delivering the value through the promise. 
So that's, that's what a promise is. And I think a lot of people are familiar 
with that concept, but an observable on the other hand is this type that is, 
it's a lot like a function it's it's, it doesn't do anything until you 
subscribed to it.
And then it gives you three callbacks, one for each one for when you get a 
value. And that's like the most important one. The second one for if there's an 
error, delivering values and telling you that it's done with an error and the 
third one for when it's complete, when it's, when it's done giving you values 
and it's was successful, there were no problems.
and it's just, it's just this really primitive type. And it exists all over the 
place in many different shapes. Like it's not just our X that has this concept 
of an observable. but the, I doesn't matter, I mean, many different shapes. 
They're all roughly the same shape, but like the same concept. and the idea is 
that if you have this, function that gets called with your values, whenever they 
happen and they can happen anytime, asynchronously, then what you have is, and 
you also know when it's done giving you this values.
Then, what you have is a set of events. So when you first subscribed to it, 
that's when the event set starts, and then it gives you events as it goes along. 
And then eventually it says I'm complete. And you know that you're done getting 
events. So you have events as a collection, as a, as a set or a collection of 
things.
And the thing that's interesting about it gets us to the second part of RCS, 
which is different operators. and the operators are what I would tell most 
people not to worry about too much like observable itself. The type is what I 
most think everybody should understand. But the operators come from the fact 
that if you have a set of events or if you have a set of things, like, say, I 
say, give you a set of apples.
If I was to give you a basket of apples, You could count them and you could tell 
me how many apples there were. You could take all of the bad apples out you 
could, so you could effectively filter them down to the good apples. You could 
take them and combine it with a set of sugar and flour and whatever else I gave 
you and make it into a set of Apple pies.
Right? So the thing about a set is it can be transformed. It can be, it can be 
filtered. It can be joined with other sets. and all sets, arrays are this way, 
baskets of apples or this way, the universe just works like this with sets. And 
so if you have a set of events, you can do the same thing.
So you can take a set of events, say mouse clicks, and you can filter them down 
to the mouse, clicks that happen on a certain spot or the mouse clips that 
happened when you right. Clicked or whatever. you can take. A set of events from 
a WebSocket and filter it down to just the ones you care about, or you could 
count them all or aggregate them over time or what, what, whatever.
So that's what these operators are. The operators are these operations, you can 
perform on an observable, which is a set of events and it results in a different 
observable, which is a different set of events. So it's the same thing with the 
basket analogy. So if I was to give you the basket of apples and you filtered it 
down to the good apples, now you have a basket of good apples, but you still 
have a basket.
That was the operation. So it's, it's, that's the fundamental concept with arcs. 
Yes. As you have these observables, which are the most important thing to 
understand, and then there's all of these operators that can transform one 
observable into another one. I go ahead.
Sure. Yeah.
JavaScript version of reactive extensions. and actually it was born at 
Microsoft, from, kind of as a clone of Microsoft, our Microsoft's rx.net. So, 
and RX JS can be used anywhere. JavaScript runs. w when I originally worked on 
it at Netflix, it was being used in smart TVs and weird, weird JavaScript run 
times that, You know, we're not V8 based, they're not Chrome based or anything 
like that.
They're like their own little custom JavaScript runtime. So it can be used in 
node. It can be used and it is used in node quite a bit. it can be used in, 
browsers and electronic, like it's used all over the place and it's very, very 
primitive. The observable observable type itself is extremely primitive.
you could use it to develop a promise, for example, it's like lower level than 
that. So, It can be run anywhere. what was the second part of your question?
Oh, no, there's there's I mean, yes and no. So the thing about observable itself 
is it can re represent zero events or, you know, many events. that are either 
totally synchronous or happen asynchronously. So you can use it to represent 
anything. Now that said, I recommend people exercise, restraint and judgment 
when it comes to doing these things because, our XJS as a library has all of 
these operators and they have operators named things like switch map, and merge 
map and concat map and all these things.
And I don't know, I don't expect just any random person to walk up and know what 
those things mean. And they're almost like a domain specific language on top of 
a JavaScript. So for, for dealing with these things, they're very, very 
powerful. you can accomplish a lot, in a very concise way, but you know, with 
that, you've got some abstractions.
So there's going to be a little bit of overhead for that. And we do the best we 
can on the team to make things as fast as possible and as small as possible. But 
also there's a burden on other people around you that have to know these things 
in order to interact with this, you'll have to add a lot of comments, that sort 
of thing.
do you need RHS for loading an Ajax request after you hit a button? No, probably 
not. That's silly. You don't even need a framework for that. That's just a 
button in a fetch, right? So, there's, there's a lot of places where I would say 
you probably didn't need it. Could you use it? Sure. but is it really helping 
you in certain cases?
Probably not. Where it's most helpful is where you have to do complicated event 
coordination. Or combining of different data streams, or maybe you have a data 
stream and you're filtering it and processing it in some way and coming out, 
like in the streaming case, if someone's doing like a lot of streaming data 
coming into like a node service or, like a it's, especially if it's push-based 
streams, are they just getting, here's a new, here's a new one, here's a new 
one.
or they're doing that in the web with like web sockets or whatever, server sends 
events, you know, if they're not using RX and. Especially, if they're combining 
streams, then I would be like, Oh, here's this other tool you might want to look 
into? Because I know firsthand from writing the library and writing other code 
that wasn't in our ECS that, you know, trying to right, event coordination 
between different streams, yourself, particularly trying to tear them down and 
stand them back up.
And all this other stuff is it's complicated business. And there's a lot of 
places where you can shoot yourself in the foot. So. use it where it belongs, it 
when possible, but it's not going to hurt you to use it in other places.
I would say, you know, people that are new, I think a lot of times when I get 
people that ask that, like, I'll have someone message me and be like, Hey, how 
do I become a great developer? And I think they're expecting me to pull out, you 
know, a magic wand and be like, boom, you're a great developer. But like the 
truth of the matter is it's just about consistency and patience.
And, the best thing you can do is learn how to teach yourself stuff. I mean, 
that's true for anything. Like, if you can learn how to teach yourself things, 
then you are going to do much better than someone that has to have somebody else 
teach them something. because you're always available to yourself.
Right? So, so learning how to teach yourself things is super duper important, to 
being a software engineer and being a human being in general, I think, and, and 
also being consistent, you know, consistency is something I think people 
struggle with. that's why people have a hard time with a lot of different 
things.
Like. Exercise without consistency is just moving around a lot. Like it's the 
same thing with any sort of mental exercise or anything else. Like you have to 
be consistent. And again, you have to learn about yourself. You have to learn 
what your limitations are. You have to learn how to teach yourself things, and 
lightweight where we were talking about earlier with, being like putting 
yourself out there a little bit, interacting with other people.
It helps you learn, right? Like interacting with somebody else. You're going to 
learn new things. So, I would make sure that to try to get out there and network 
and meet similar minded people. And, you know, it's risky though, because 
there's some jerks out there for sure. but, you know, it's, it's worth the risk 
in my opinion.
So.
I was going to say there's the software engineers in particular very much like 
to be asked questions because they like to feel smart. So it's it's you can't, 
you can't go wrong in this group of people asking questions. I mean, you can, 
but.
Oh, sure. so. So there's two questions there. The first was about the future of 
RCS. A feature of RCS is primarily just focused on making the library smaller, 
more efficient, and kind of keeping up with changes and modern platforms. So for 
example, a board controller is now going to become ubiquitous. So maybe we don't 
need subscriptions anymore.
We can use the abort controller in these sorts of things. so that's the future 
of RCS and it's it's, it is what it is. It's a utility library. Now, as far as 
its relation to the no-code movement, I think that RCS is a solid fit for some 
of the internals of things that might be, tools that might be used in no-code.
and the reason I say this, or not even just RCS, but reactive programming in 
general, the reason I say this is because reactive programming is based off the 
principle that, you can kind of piece things together like Legos. So you can 
say, okay, well, I've got a stream of. Data of this shape. You don't know where 
it came from and you don't care, but the next piece is going to react to when 
that next bit comes in and do something with it and send it off.
And then the next piece down the way, reacts to whatever that thing is that when 
it comes in, it doesn't know where it came from and it doesn't care. So the 
thing about RX is it's, it's very, It's very composable in a way that, that like 
building blocks. So you can, you could in theory, make something where you could 
literally drag and drop shapes together.
That declared how you're going to transform some streaming data. And then under 
the hood, it would build an array of operators in RX and just kind of apply 
them. and so reactive programming as it stands. Like I actually don't even know. 
How you could go about developing something no-code without some form of 
reactive programming, not necessarily arcs Jess, but, just some form of, I don't 
know where this piece came from.
My job is to transform it and this way, cause I'm a blue Lego or whatever. And 
then I sent it on to the red Lego or whatever I do. so I think that it's got a 
strong future in the back of that sort of thing. And I actually liked that idea 
because one of the. Struggles that, people have with RCS is just learning all of 
these operators.
and if I could find a way to just abstract them stuff away from everybody, I 
absolutely would do that because, they're the most, they're the single most 
powerful piece of, of RCS. not the most important observable, still the most 
important, but the most powerful pieces, these operators, but they're also the 
thing that confuses everybody.
Because it is a bit mind bending to deal with, you know, this multidimensional 
problem of time and, and values. And, you know, when things happen here and here 
and here, and like, you know, even though you've broken it down into individual 
steps with reactive programming, you have to know like what a switch map is and 
so on and so forth and how it behaves.
So I think that, you know, building some sort of no-code thing on top of it is, 
is a fantastic idea. I don't really know that anyone's doing that, but. Or, or 
even anything like it, there's plenty of other, reactive programming paradigms 
or, or libraries and things that people can build no code on top of it's the 
same concept.
And in my mind, it's a win whether it's RX yes or not, like it's, it's reactive. 
A programming is important for this sort of thing.
Sure. Yeah. Yeah.
No, no, but I'm happy to hear that you're starting your own company. good luck 
with that, dude. I don't know what your, your company is though. What is your, 
can you tell us about your company really quick?
That sounds really cool.
All right. Thanks for having me.


