[00:00:00] 
**Dr. McKayla:** Hello, and welcome to the Software Engineering Unlocked 
podcast. I'm your host, Dr. McKayla and today after pleasure to talk to Avdi 
Grimm. But before I start, let me introduce you to an amazing startup that's 
sponsoring today's episode, Tonic.ai, the fake data company. So what does 
Tonic.ai do? I'm sure you know how complex and cumbersome it is to create 
quality test data.

[00:00:27] **Dr. McKayla:**  It's a never-ending chore that eats into valuable 
engineering resources. Random data doesn't do it and production data is neither 
safe nor legal for developers to use. What if you could mimic your entire 
production database to create a realistic dataset with zero sensitive data? That 
sounds amazing, right? Tonic.ai does exactly that. 

[00:00:50] **Dr. McKayla:**  With Tonic.ai, you can generate fake data that 
looks, acts, and behaves like production data because it's made from production. 
Yet, Tonic.ai guarantees privacy so your data sets are safe to share with 
developers, QA, data scientists, heck, even distributed teams around the world. 
Visit Tonic.ai to sign up today or click the link in the show notes to get a 
free two weeks trial sandbox.

[00:01:14] **Dr. McKayla:**  But now back to Avdi. Avdi has been a developer 
for over 20 years and runs, similar to me, a training and consulting business. 
The main difference is that he has been doing this already for over 10 years. So 
I'm super thrilled to pick his brain today around everything business-related. 
He's also a consulting pair-programmer and the author of several popular Ruby 
programming books and has several courses on this subject on his website, 
Graceful.Dev, formerly RubyTapas.com. So I'm super thrilled that he's here with 
me today. Avdi, welcome to my show. I'm very excited. 

[00:01:51] ** Avdi Grimm: **  Thank you so much. I'm excited to be here. 

[00:01:53] **Dr. McKayla:**  Yeah, I'm super excited. So I've been following 
your journey on Twitter and so on for quite some time. Very inspirational as 
well. And I have a lot of questions around how you run your business and why 
you're running the business and what we can learn from you, right, a seasoned 
entrepreneur and self-employed person to also maybe get a little bit more 
independence in our life, right? So this is probably the main goal for myself, 
for everything that I do is flexibility and independence. So why are you running 
your own business and how does this come about? Why are you not a software 
developer in a company somewhere?

[00:02:32] ** Avdi Grimm: **  Right, yeah. I mean, to some degree, I feel like 
it's almost an inevitable career arc for somebody in software. You know, I know 
people who have avoided it, but a lot of the people that I kind of looked up to 
over the years went through, you know, they went through the full-time 
employment phase and then they gradually kind of moved out to becoming 
consultants and having various other side businesses.

[00:02:55] ** Avdi Grimm: **  And, you know, come to think of it, I never really 
thought about this much before. I had the example of my dad who worked in 
software and hardware design, and he was an independent consultant I was growing 
up. So that was kind of normalized to me to, like, have your own thing 

[00:03:08] **Dr. McKayla:**  Yeah, for me was quite different. Yeah. 

[00:03:11] ** Avdi Grimm: **  I think that I, I saw that on the horizon maybe 
from earlier than some people do, just because it was, it was normalized for me, 
you know? And it just seemed like that's what a lot of my heroes did in the 
industry was eventually they became consultants. 

[00:03:26] **Dr. McKayla:**  Yeah. Yeah, it's good if you have like role 
models. For me, it was quite the difference. I always saw it that I will work at 
the company for a really long time and, you know, climb the career ladder 
somewhere. Actually, I started a family that I saw, oh, this is not working out 
as I expected. And as I would like it to work out, right? And so this was a 
little bit why I changed the thing. So you call it a banana stand. You don't 
call it like an enterprise or something. Why do you call it the banana stand? 
And what's your philosophy for your business? How do you run it? 

[00:04:00] ** Avdi Grimm: **  So, yeah., I've started using the term banana 
stand recently, especially as I've been kind of reflecting back on, you know, 
over a decade of doing this and, like, my style of, of running the business and 
writing a little bit more about that. So the, the term banana stand, it comes 
from, the show Arrested Development in which one of the characters says to 
another, this character is trying to save the family business and his dad who is 
in prison keeps telling him there's always money in the banana stand, which he 
completely misinterprets the message and winds up, burning down a banana stand 
that's full of literal money in the walls. I apologize if I've spoiled the show 
for you, but it's been out for a while. But you know, like, that phrase stuck 
with me. There's always money in the banana stand and that's kind of the way 
that I look at it.

[00:04:48] ** Avdi Grimm: **  So there's kind of two sides to this, this 
independent business for me. There's the consulting side. And then there's the 
product side, product being kind of a broad term for selling books, selling 
courses, selling workshops. It's kind of a loose definition of product, but it's 
definitely distinct from the consulting side of my business, which is more like, 
you know, hourly consulting on people's projects.

[00:05:12] ** Avdi Grimm: **  And I definitely look at the product side as a 
banana stand as like something that I kind of run casually, even if I'm putting 
most of my time into it now. I still run it kind of like lazily and you know, 
and it's my own banana stand to putter around in. I'm not, like, beholden to 
any, like, schedules and I'm not on any kind of like track of, I have to, you 
know, make this much money.

[00:05:35] ** Avdi Grimm: **  I have to, like, make sure that my VCs get a 
payoff and stuff like that. It's just kind of like, you know, I get the putter 
around in the banana stand and work on whatever I feel like. And, you know, that 
phrase there's always money in the banana stand is kind of like that has 
informed the way I think about employment a lot, because, for me, if I'm in 
between jobs, I used to think of it as in between jobs, I don't think of it that 
way anymore, but if I'm in between jobs, quote, unquote, that's not like a time 
to panic and, you know, and, like, do all the interviews and freak out about how 
I'm unemployed. That's time to just focus on the banana stand.

[00:06:12] ** Avdi Grimm: **  And until something comes along, that makes sense. 
And I think that's been helpful to have that. And, yeah, that side of my 
business, really like, so we talked about consulting, but that side really came 
from early on, getting into e-book sales, which we can talk about how that story 
went if you want. 

[00:06:28] **Dr. McKayla:**  So if I understand that you would say there's the 
consulting, which is, you know, it's something that you have continuously to 
invest in and also make some contracts around that.

[00:06:37] **Dr. McKayla:**  I'm also doing some consulting, which means like 
now I'm dedicating, let's say 30 hours for this project for three months, right? 
And so you are more or less sold out for that time? 

[00:06:48] ** Avdi Grimm: **  It's kind of like a real job.

[00:06:49] **Dr. McKayla:**  Yeah. It's like a real job, only that you have 
all the risks as well, which is even worse.

[00:06:58] ** Avdi Grimm: **  But there's a lot more, even there there's a lot 
more independence. And honestly, you know, one of the things that I value on the 
consulting side is that, I mean, yeah, you have the risk, but there's always the 
risk. There are no guarantees in this industry. There are no guaranteed 
retirement plans.

[00:07:13] ** Avdi Grimm: **  And what I don't have to do is I don't have to buy 
into a lot of corporate mission and values BS that I don't believe in. 

[00:07:22] **Dr. McKayla:**  Yeah. So you have your consultancy and then in 
between those consultancy gigs, right, when there are no consultancy gigs, 
you're not freaking out, you're working on your banana stand and you grow that, 
right? And the good thing it's about the products and, you know, this mindset, I 
think, is that even a little bit of work on them pays off, right? So it's a 
little bit like an investment. So you create another free course, maybe, and you 
have like a, you know, a good lead magnet, have people that are interested in 
your work.

[00:07:53] **Dr. McKayla:**  Then you create a paid course when you have time 
and so on. And it stays, right? It's something that's there for longer, whereby 
the consulting, it comes, it brings normally quite good money, from my 
experience, right? In a very short amount of time, but then it goes away as 
well. While the banana stand, maybe it's a little bit, it's not this boom, now 
we have like all this money. But it's also not going away, right? Yeah, exactly. 
It's a snowball. It's a flywheel somehow, right? Yeah. 

[00:08:20] ** Avdi Grimm: **  Yeah. I mean, you know, a consulting gig is one 
big blizzard that, you know, that melts the next week and a banana stand is a 
snowball that you just kind of gradually roll over the years.

[00:08:32] **Dr. McKayla:**  And so how long did it take for you to have this 
banana stand where you could say, well, I have some predictable income that, you 
know, makes me sleep at night? . 

[00:08:43] ** Avdi Grimm: **  So actually I think, you know, my trajectory there 
probably was a little different from a lot of people's. I kind of, you know, I 
put along having the book, the e-book business on the side for a few years, and 
that really just fell out of speaking.

[00:08:58] ** Avdi Grimm: **  It happened because I was giving talks at software 
conferences. And I was pouring a ton of time and energy into researching these 
talks. And I was like, you know, I wonder if there's a way to kind of recoup. 
You know, I have all this material that I put together. I can't fit it all into 
a talk.

[00:09:14] ** Avdi Grimm: **  And I wonder if there's a way to like recoup the 
energy that I've been putting into this. And that was really the origin of the 
first book, which was Exceptional Ruby, which is about error handling and 
failure management and I made a book out of like the, all the extra material 
that I put together for that.

[00:09:29] ** Avdi Grimm: **  And that was that kind of launched things. And so 
that was kind of a side business. It was a nice little side business for a 
couple of years. And then what changed was I decided to get into screencasting. 
I've been doing the books, I've been doing some podcasting and this was around, 
you know, this was like 20, maybe 2010, 2011, 2012.

[00:09:52] ** Avdi Grimm: **  A lot of programming screencasts started taking 
off. And I decided to get into that business. And I had a vision of like, what 
if we did that only much shorter and more focused? And, you know, just do like 
five minutes or less. You know, get one idea across at a time. And so, unlike 
most banana stand efforts, that was really like a do or die, not do or die.

[00:10:13] ** Avdi Grimm: **  I don't like that terminology that was a go big or 
go home. That's the phrase I'm looking for, go big or go home because I knew how 
much energy went into video production and it is a lot. And so it was like, 
okay, this is a project that I'm going to test the waters. If it does well, I'm 
going to try, you know, the only way this works is if I can make it into my 
full-time job, otherwise I'll just stop. And yeah, I got really lucky. I was 
coming in at a good time. People really liked the format. And so within, I think 
around a year or two, I was able to say, I don't actually need other jobs right 
now with the RubyTapas screencasts. 

[00:10:49] **Dr. McKayla:**  Oh, yeah. That's nice. 

[00:10:51] ** Avdi Grimm: **  Yeah. So that was, that was kind of like line goes 
up. That was less, you know, slowly rolling snowball.

[00:10:56] **Dr. McKayla:**  Yeah. And how much time did you spend in this 
line goes up phase? You know, because somehow when you're focusing on something, 
like doing the screencasts, you're not having an income, right? And then if you 
go to consulting, you don't have the time. So you have to switch between those 
boats of not having time or not having money. So how did you handle that at that 
time? 

[00:11:17] ** Avdi Grimm: **  I didn't sleep. I had at least one new baby at the 
time, too. And, like, I was working consulting gigs. I don't know. It's kind of 
a blur at this point. I don't think that I could do that kind of thing again, 
unless it was a great need. 'Cause I was also, at that point at the beginning, I 
was producing three episodes a week. 

[00:11:41] **Dr. McKayla:**  Wow. Yeah, that's a lot. 

[00:11:43] ** Avdi Grimm: **  Yeah. I was doing a lot at once and it was kind of 
nuts. 

[00:11:46] **Dr. McKayla:**  Yeah. And I actually really liked, with the whole 
style also, when I look through your blog posts and everything, right, you have 
your own style. You didn't call it like Professional Ruby screencast, you call 
it RubyTapas, right? And the tapas probably transport the message of it's small 
pieces of very digestible, tasty things, right? 

[00:12:09] ** Avdi Grimm: **  And I feel like some of that probably also fell 
out of just like the Ruby, like, the community has always been super whimsical 
and kind of silly. And so, you know, I can't take full credit for that approach. 

[00:12:22] **Dr. McKayla:**  Yeah. But recently, I don't know exactly when, 
but you rebranded your whole RubyTapas into Graceful.Dev, why is that? For me, 
it seems like it's now broader and there can be more happening, but what's your 
strategic vision behind, you know, going from RubyTapas to...

[00:12:40] ** Avdi Grimm: **  I do not do strategic visions. I used to, but, 
man, I avoid strategy as much as possible now. I mean, that's okay. That's not 
true. I do a little, I do a little. But I try not... 

[00:12:54] **Dr. McKayla:**  You definitely have some reasoning behind it, 
right? 

[00:12:56] ** Avdi Grimm: **  I try not to have five-year goals. Let's put it 
that way. I don't do goals. There's definitely some reasoning there. There's a 
direction there. I mean, the direction was one that I've honestly had in the 
back of my mind for a really long time. A lot of people don't know that, like, 
the same day in, like, 2011 or whenever it was that I registered RubyTapas.com 
and associated addresses. I also registered CodeTapas.com.

[00:13:20] **Dr. McKayla:**  Okay.

[00:13:21] ** Avdi Grimm: **  So like, you know, I never wanted to completely 
limit myself to Ruby, strictly Ruby content. You know, I've worked in, God, like 
a dozen languages over the course of my career. And Ruby was just an area that I 
wound up focusing on a lot and wound up making a lot of money in. And enjoying, 
I really, really enjoy the language still and the community as well.

[00:13:42] ** Avdi Grimm: **  But I always had in the back of my mind, you know, 
that I would expand, but, you know, I didn't wound up not using as you'll 
notice. I wound up not using CodeTapas as the branding 'cause I was really, 
like, moving in a different direction, broadening not just in, like, in the 
technologies that I want to cover, but also I just spend a lot more of my time 
thinking about broader topics like, the sustainability of the development that 
we do and systems thinking, understanding the systems in which we work and the 
systems that cause the work that we have to exist. And yeah, so just, for a lot 
of reasons, it made more sense to me. And in some of my talks, I've been really 
focusing on the concept of grace.

[00:14:21] ** Avdi Grimm: **  So it just made more sense to me to move in that, 
that branding direction. And then recently I had the opportunity to finally, 
like, do a lot of the heavy lifting of moving content over. And so I took that. 

[00:14:33] **Dr. McKayla:**  Where did this opportunity come from? 

[00:14:35] ** Avdi Grimm: **  Well, so I had a point a few years back where I 
was like, okay, you know what? I've been sort of off on my own, doing my own 
thing for a long time. I would like to get back into, like, the hustle and 
bustle of being part of a big team that's making something real in the world. 
And I spent, I don't know, a year or so interviewing pretty seriously at a bunch 
of different places. And that did not go as expected.

[00:15:00] ** Avdi Grimm: **  And I finally decided that I, wasn't going to 
focus on that anymore after all. And I was just going to get back to the banana 
stand 'cause there's always money in the banana stand. And that has been 
actually an immensely satisfying experience, kind of coming back to it with a 
fresh, fresh, like maybe this is my calling perspective.

[00:15:18] **Dr. McKayla:**  Yeah, I actually followed this journey a little 
bit on your Twitter, you were sharing it with us and also the hassle of the 
whole, you know, getting naked in front of strangers, you know, and really 
selling yourself. And I mean, you have been in the industry for so long, you 
have shared your learning.

[00:15:38] **Dr. McKayla:**  You know, you have some portfolio online. It's 
not like somebody comes and has no idea about you, but still, it felt like at 
least what I got out of the tweets, right. What I read into them was that every 
interview was a little bit, it wasn't really like keeping your dignity, right? 
So you had really to get naked in front of them to do all these silly things.

[00:16:03] ** Avdi Grimm: **  You know, I wouldn't, I actually, I would argue 
that it's not, it wasn't really about being naked. It wasn't really being, about 
being transparent. It was about people wanting you to do a very special dance 
for them that strokes their ego and me being at a point in my career and life 
where I'm just like, I'm not going to do that. Why would I do that? Looking back 
I got some actually really nice offers from some, you know, well, large 
companies anyway, but in the end I was not comfortable taking any of them. And 
in part, because of what I saw during the interview process.

[00:16:39] **Dr. McKayla:**  Okay, what did you see? 

[00:16:41] ** Avdi Grimm: **  Well, you know, so actually, let me tell you about 
something I just heard recently from a friend of mine, because I hear the same 
story over and over again. Like my story, what I've realized is my story is not 
at all unique. So just the other day I heard the story again of like, basically, 
you know, an extremely senior well-respected brilliant engineer gets asked by a 
friend that works at a FAANG, you know, works at one of these giant unicorn 
Silicon valley darlings, gets asked to come interview there. It's like, we'd 
love, you know, I'd love to work with you here, which is basically what happened 
to me, a number of different places. And, you know, so they kind of go into the 
interview silo and then they go through this process where in, you know, in this 
particular case, like they got interviewed by someone who was totally unrelated 
to the group that wanted to hire them because this is the way the process works. 
You know, we don't want bias in the system. There's a lot in these processes 
that are supposedly about eliminating bias, it's actually creating it.

[00:17:42] ** Avdi Grimm: **  We can talk about that more in a minute, but, you 
know, was interviewed by someone totally unrelated to that team. And basically, 
they were like, you know, show that, you know, by heart, my favorite algorithm,

[00:17:55] ** Avdi Grimm: **  I happen to have a favorite algorithm. You're 
going to show me that you can, you can identify that I'm thinking of this 
algorithm and then you can write it by heart. And like that wasn't an algorithm 
that this engineer had used before. And so it wasn't one they thought of, you 
know, I've got a lot of stuff in my background where it's like, I know of 
algorithms that probably most engineers haven't heard of because they happen to 
be useful for networking middlewares and I hear this all the time.

[00:18:18] ** Avdi Grimm: **  Anyway, they got flunked out because they 
couldn't, you know, reproduce somebody's favorite algorithm from, by heart. And 
this is somebody with, like, close to my level of experience. It's nuts. And I 
keep hearing this. It's actually, you know, I've heard this from a lot of 
people, with my, lot of friends of mine, with my level of experience in the 
industry, that these systems, they're really tuned to find people that are 
exactly like the people who designed the system in as many ways as possible. 

[00:18:47] **Dr. McKayla:**  Yeah. 

[00:18:48] ** Avdi Grimm: **  Like, for me, I don't care. I am a white guy with 
plenty of opportunities and a banana stand. You know, I can fall out of a 
process like that and be fine. But what I'm seeing is that these processes are 
also, I mean, they're very gatekeep-y and they're very clicky. They're very 
in-crowd, they're very, very, like, we are expecting people that sort of show 
the secret insignia of a very select group of Silicon Valley insiders, 
basically. 

[00:19:18] **Dr. McKayla:**  I think one of the problems is also that they 
often require a tremendous amount of preparation, right? And if you think you 
are an experienced engineer, maybe at that point, you have a family, for 
example, around, right.

[00:19:33] **Dr. McKayla:**  And some other commitments, it gets really hard 
to study some, you know, lead code examples, just to be as fast as, you know, 
somebody else, right? And I think this is also something that I criticize a lot 
when I'm thinking, and then you don't even need that, you know, you don't need 
that knowledge. You could really solve real-world problems.

[00:19:51] **Dr. McKayla:**  You have some experience and background, right, 
that you have worked on. And it's probably also super challenging. So looking 
really at what that person has already achieved in the last, let's say 15 years 
would be, you know, and then really let them explain that in-depth, which shows 
that they probably can learn, you know, whatever problem or solve whatever 
problem you throw at them. It would be a much better way than, you know, getting 
back to bubble sort and, you know, and linked list or something, right?

[00:20:19] ** Avdi Grimm: **  And this, this is a big part of where the bias is 
in the system, and this is why I get sort of morally outraged by it, you know? I 
don't do well in these, you know, I might not do well in these because I'm at a 
point where I just can't be arsed to do that much homework of like learning 
somebody's arbitrary favorite algorithm.

[00:20:36] ** Avdi Grimm: **  But what they're implicitly biasing towards is the 
sort of stereotypical young white dude that has all the time in the world and 
doesn't have a family to support and doesn't have any disabilities. And, you 
know, I could list off a lot of, you know, a whole lot of privileges there that 
go into that sort of their really looking for that person who has nothing else 
going on in their life.

[00:20:59] **Dr. McKayla:**  Exactly. 

[00:21:00] ** Avdi Grimm: **  You know, so that they can then like induct them 
into the cult of your passion is your software career. And that bugs the heck 
out of me, you know, and I see this really like, you know, who is really hurting 
is people that come from backgrounds that aren't like mine and have other stuff. 
They have people that they're taking care of. They have kids, they have elderly 
parents, they have families that they're sending money to, and they can't afford 
a, you know, a break in their income while they spend six months, you know, 
doing nothing but the interview game. You know, there are so many things, and 
the people that are, you know, so many minorities in this country already have, 
in the world or, you know, minoritized people, I shouldn't say have so many 
other calls on their time because of the way society is already stacked against 
them. That it makes it impossible to jump through these. 

[00:21:48] **Dr. McKayla:**  Yeah, I totally agree. I totally agree. Yeah. 

[00:21:51] ** Avdi Grimm: **  Sorry, I get worked up.

[00:21:53] **Dr. McKayla:**  No, I want to come back a little bit to your 
banana stand again because this is the way out for, for you. And it's a little 
bit the way out for me as well, right? So with Graceful.Dev, I don't know if you 
had that before. You had RubyTapas and you had like the courses, but 
Graceful.Dev is now a full-fledged membership site, right? So you have different 
courses and you build it on top of WordPress. Why did you go this route? I mean, 
you could have like your courses on some third-party platform, right? From, I 
don't know, Teachable or whatnot, you know, many, many different PODR and so on. 
But you host it yourself and then you have the membership site as well. And you 
do that. Why does choice, like, I'm also thinking about right now, 
awesomecodereviews.Com for example, runs on, I switched from WordPress to 
Gatsby. So it's a static side and I'm thinking on how to give it a membership 
capabilities.

[00:22:49] **Dr. McKayla:**  And I looked at SurplusCI and so on, but why did 
you go for WordPress? And are you happy with it? And what's the philosophy 
behind it? What do people get from this membership? What do you want to build? 
Probably there's a community behind, right? And some, some visions that you have 
for that.

[00:23:06] ** Avdi Grimm: **  This is an opinion I've kind of come to over years 
of using many different systems. And there's continuum here because you know, a 
lot of people running, particularly running education sites for developers have 
rolled their own system from scratch. They've built their own servers or their 
own applications.

[00:23:26] ** Avdi Grimm: **  And so, you know, there's that continuum all the 
way from roll your own to, you know, use a completely hosted service, like 
Podia, Thinkific, whatever, you know, and I've, I've tried a lot of these 
different things. I started Ruby topis out on somebody else's platform.

[00:23:39] ** Avdi Grimm: **  And it was super limiting. You know, there would 
be things that people were asking for for years and they just, that feature 
wasn't a priority for the platform because you're competing, you know, you're 
competing with all the other people who use the platform. And for, you know, 
whose feature is most important.

[00:23:54] ** Avdi Grimm: **  So it was very limiting to use a hosted platform, 
and I've periodically I try them again and they're always, there's always like 
something pretty early on, it's like, wow, I really need this feature. And I 
don't have it. But I've also toyed with building my own. I did that for a few 
years and you know, what I realized was, if I did that, my show was going to 
become about building an app to support the show, because that's what I was 
going to be spending all my time on, because it's a lot of work to build.

[00:24:23] **Dr. McKayla:**  It's a lot of work, yeah. 

[00:24:25] ** Avdi Grimm: **  People don't realize, you know, how many features 
are expected in an application that sells content and serves content and keeps 
track of people's progress in the content, et cetera, et cetera, et cetera.

[00:24:38] ** Avdi Grimm: **  And yeah, I just, that was not the show that I 
wanted to be doing was, you know, I didn't want to be like here's videos about 
how to build a place that hosts these videos. So WordPress has turned out to be 
a really happy medium kind of between those two extremes. WordPress is just 
incredibly mature software.

[00:24:56] ** Avdi Grimm: **  There's a lot of people in, particularly, the 
developer world that are kind of biased against WordPress and sadly against like 
the PHP ecosystem entirely, which I think is really undeserved. There's a lot of 
really, really good people working in this space. And the ecosystem is just 
amazing because you can kind of build anything you want and you can get as 
little or as much support as you want.

[00:25:20] ** Avdi Grimm: **  You know, it's easy enough to build your own 
plugins for WordPress to just do a little tweak here, a little tweak there. You 
know, the architecture of it really supports the idea of exposing everything it 
does as hooks. And then you can hook your own stuff into those hooks, which is 
why it has this great plugin ecosystem.

[00:25:36] ** Avdi Grimm: **  But one of the really cool things about the plugin 
ecosystem around WordPress is A, there is a plugin for everything, like, 
anything you might want to do. Somebody has got a plugin for it. And B, usually 
they have, like, a premium version, which comes with support. And I have had the 
best experience with premium plugins for WordPress.

[00:25:55] ** Avdi Grimm: **  Like, you know, people just like being very 
responsive to the people that are giving them money and coming back and, you 
know, with bug fixes or like going into the, you know, going into your site and 
making, figuring out why it's not working. And so it's like, it's one of the 
rare places I've seen that people are putting out a ton of open-source software, 
but also getting paid for their work.

[00:26:16] ** Avdi Grimm: **  Because all these plugins, like the base version 
at least, is always open source. And then basically you're paying them for maybe 
some premium features, but mainly for a support contract and, you know, and so 
people are making their living, creating open-source software. And I think 
that's pretty cool. And it's also, it also has done really well for my business. 

[00:26:32] **Dr. McKayla:**  Yeah, and it's true. And so when I'm thinking 
about your course software, did you get a plugin for that? Or did you have to 
write it yourself or do you have like a plugin and then extend that on your own? 
How does that work? You're hosting your videos, but then they're also like, you 
know, questionnaires, for example, some quizzes, you know, as you said, you see 
that people, you know, it somehow tracks the progress of the people. It has to 
know that you're a member that can access that course, the other course. All of 
that functionality, does it come out of the box with some plugins for WordPress? 
Or did you have to implement that yourself or was it a mixture that you're 
actually getting a plugin and then you can, you know, enhance that with your own 
code?

[00:27:15] ** Avdi Grimm: **  Great question. So, there are two to three 
categories of plugins that go into a site like this. I mean, my website has a 
lot more plugins than that, but there's sort of maybe three basic pieces. And 
one is  learning management system LMS, otherwise known as courseware. So that's 
a category of plugins I could probably reel off maybe six of them off the top of 
my head, I'm personally using LearnDash, which is one of the older ones and one 
of the more, probably the most popular one in WordPress right now. And it's very 
mature. It's a little clunky for me sometimes because it's really targeting in 
many ways, it's targeting like serious learning institutions where they have 
like accreditation concerns and certificates.

[00:27:59] ** Avdi Grimm: **  And like, you can't take this course until you 
take this other course, lot of stuff that I don't care about. On the flip side, 
it's very mature. They handle all the things that I might want to put into it. 
They just also, also a lot of stuff that I don't care about. And then, so you've 
got, like, there's learning management, that's one. There's membership, which is 
like another whole category of plugins, which are generally focused around, 
given this account, what material does this person have access to? And that 
includes courses, like what courses does this person have access to. 

[00:28:28] **Dr. McKayla:**  So they work nice together, LearnDash and the 
membership thing. 

[00:28:30] ** Avdi Grimm: **  Yeah, so generally what you see, so I'm using 
LearnDash on the LMS side, I'm currently using MemberPress, which is one of the 
more popular membership management plugins.

[00:28:39] ** Avdi Grimm: **  Generally these plugins, they work hard to work 
with each other, you know, different teams usually, but they work hard to work 
with each other because that's where a lot of the value comes from. And so they 
have explicit support for each other. And then the third piece often is like 
your e-commerce, how you sell the thing.

[00:28:56] ** Avdi Grimm: **  And that is often a separate plugin as well. Like 
in the WordPress ecosystem, it's usually WooCommerce. Sometimes it's EDD, Easy 
Digital Downloads. Now I've reeled these off like they are distinctly separate 
categories, but actually almost everyone in each of these spaces will happily 
give you like all of the above kind of in one.

[00:29:18] ** Avdi Grimm: **  Because they all kind of, they'd grow, all 
gradually expand out to include each other's features. So like LearnDash, you 
can do a pretty basic membership management using the groups that are built into 
LearnDash. You can sell courses directly. Like they have Stripe integration and 
stuff directly from LearnDash if you want to, it's kind of basic, but it's 
totally there.

[00:29:36] ** Avdi Grimm: **  MemberPress recently introduced their own 
courseware plugin for MemberPress. You can just like stick with that company if 
you want, as long as you're okay with like a more basic courseware offering. 
They also have the storefront part built in if you want to use it. So there's a 
lot of blur between these plugins as well.

[00:29:54] ** Avdi Grimm: **  Yeah. 

[00:29:55] **Dr. McKayla:**  Yeah. Okay, cool. And so are you then enhancing 
that, is that possible, especially if you have like the paid version, could you 
just write that? And then how do you keep track of your own changes and new 
updates that are coming from the team? How do you integrate those things? 

[00:30:09] ** Avdi Grimm: **  So one of the marks of a good industrial strength 
WordPress plugin is that they have well-defined hooks. You know, I was talking 
about like, WordPress is built on the concept of hooks. They have well-defined 
hooks that are documented. And so, like the ones that I work with do, they have 
good documentation sites and they have all these hooks that you can like, here's 
how you change this, you know, here's how you hook your own thing into this 
particular part of the interface or this particular process.

[00:30:36] ** Avdi Grimm: **  And then, so what I have is what they call a 
site-specific plugin that I keep under version control, and I have a deployment 
system for that pushes it out to my way. And my site-specific plugin, basically 
just very selectively has a few, there's a few hooks where I want to customize 
something in one of those other plugins.

[00:30:54] ** Avdi Grimm: **  And it just like hooks its own handler into just 
the, like the very specific hook that is one tiny piece that I care about 
changing. It's very small. The site-specific plugin is very small. I try to keep 
it very small and very focused. 

[00:31:07] **Dr. McKayla:**  Okay. But so it has a valid defined API or hooks 
that you can really enhance. You're not going in and hacking in their, in their 
code base, right? So you're on the outside, whatever they allow you to change. 

[00:31:18] **Dr. McKayla:**  Yeah. And if you're going to really get into this 
ecosystem, that's one of the things you want to keep your eye out for is like, 
does it seem like these people are really supporting that kind of external 
hooks?

[00:31:28] **Dr. McKayla:**  Yeah, it sounds very interesting. And I know 
quite a couple of people that are running WordPress websites and have a lot of, 
you know, like you said, WooCommerce, or like a membership sites and they're 
very, very happy with it. Maybe my last question for you is around, you said you 
are not going to plan for five years and so on, right? But I think everybody has 
some, some vision you know, some, some reasons why you'd be doing things like 
transitioning from RubyTapas to Graceful.Dev, right? What do you see yourself, 
do you want to do, is there a possibility that Graceful.Dev is really your full 
time thing and that you're not doing any consulting or do you want to keep doing 
consulting on the side? Or, you know, where are you heading towards, what's your 
ideal case?

[00:32:16] ** Avdi Grimm: **  I wish I had a good answer for you. You know, I 
want to keep being able to do what feels right at the time, which is kind of 
what I'm doing right now. You know, Graceful.Dev is supporting me pretty 
decently along, you know, that alongside of my other, you know, other products 
and things. You know, I take consulting gigs as they look interesting.

[00:32:35] **Dr. McKayla:**  Yeah, and are you a solopreneur or do you have, 
like, a team that really helps you? 

[00:32:39] ** Avdi Grimm: **  Oh yeah. Good question. I don't have any full-time 
employees for years and years. I've employed people very part-time here and 
there, only ever like a handful only ever like maybe three to five at most, at 
any given time. Actually five is probably more than I have, but like I have 
somebody that's I've worked with for a long time, that handles kind of first 
line of support.

[00:32:59] ** Avdi Grimm: **  So support emails first go to them and then they 
escalate them to me. I have somebody I'm working with now who's doing a lot of, 
like, helping me with content, like doing video editing or fixing up blog posts 
that have become, like their formatting has gone wonky or is out of date or 
something like that. Yeah. So I have a few people that just like very part-time 
helpers.

[00:33:21] **Dr. McKayla:**  Yeah. I'm currently right now in this position of 
getting people and I find it really difficult finding the right people because, 
you know, if you're already in this, okay, I need help now. I don't know how you 
overcame that stuff, but for me, it's like, I need help now, and I can't grow, 
you know, without this help. But I also can't really make the time to find the 
right people and to teach them and do onboarding. 

[00:33:44] ** Avdi Grimm: **  And that is, that is the classic catch-22. And 
there's no easy way out of it. You know, the point where you absolutely don't 
have, like, you don't have the overhead space to train somebody, but you need to 
train somebody in order to get the overhead space.

[00:34:00] ** Avdi Grimm: **  Yeah, I wish I had an easy answer for that one, 
like that parts of slog. And eventually you kind of pull your head above it, but 
it's hard because, yeah, like the effort involved in like getting through that 
catch-22 is exhausting. I will say this about it. And, and this has informed my 
work for a long time.

[00:34:20] ** Avdi Grimm: **  This is the most important kind of scaling to plan 
for. I think a lot of people in software are completely focused on either 
financial scaling or on like user scaling, you know, the, your user base scaling 
up like our, will our code base support unicorn scale. That is by far like the 
least common form of scaling that you have to support.

[00:34:42] ** Avdi Grimm: **  The kind of scaling you need to plan for is 
devolving stuff from yourself. Taking, removing yourself as a bottleneck. That 
is the most urgent and immediate form of scaling that you're going to face. And 
so one of the reasons, I have a lot of reasons, but one of the reasons that I 
use WordPress is because it is the dominant player.

[00:35:02] ** Avdi Grimm: **  Like, it powers like half the web now, and there 
is this huge ecosystem. And if I need somebody to do like copy editing, I don't 
need to teach them how to use GitHub and like commit things, you know, I don't 
need to find a copy editor, but then teach them how to use my special, precious 
bespoke system.

[00:35:20] ** Avdi Grimm: **  They know how to use WordPress, whoever they are, 
they know how to use WordPress. And you know, if I need to get somebody, you 
know, if I want some help with my site because I don't have time to diagnose one 
particular bug, it's really easy to find WordPress consultants, and there's just 
so many things there where it's easy to find people that can do the thing that 
you need help with.

[00:35:44] ** Avdi Grimm: **  And that's just as a general kind of policy. 
That's one of my biggest considerations when choosing anything is not, you know, 
not is this going to scale up, but can I scale it away from me? Can, you know, 
can I remove myself as the bottleneck for this in the future? 

[00:36:00] **Dr. McKayla:**  Yeah. Yeah. That's such a good mindset. And I'm 
currently learning a lot with it and you know, it takes much more time and much 
more energy than I thought, but I also see that, you know, if you have already 
one person, right, so finding this one person, it means that you have to work 
with six different people. And then you realize, oh, it's, you know, it's, it's 
making more trouble that what I'm getting out of.

[00:36:23] ** Avdi Grimm: **  Yeah. And I should say here, like, use my bad 
example for learning. I hit a crash at one point where I really wasn't like I 
was, my outgo was bigger than my income. And a big piece of that was that I had, 
I had tried to devolve too much of myself. You know, I tried to become too big 
and pay too many people to do too many different things.

[00:36:45] ** Avdi Grimm: **  And the funny thing about what was happening there 
was that I was still swamped. I still had too little time. And it was because I 
had basically, you know, installed myself as a manager and I was spending all of 
my time helping people get unstuck and managing things. And so, yeah, it's 
really easy, like once you, once you kind of start going down that delegation 
road, it's really easy to go too far. 

[00:37:10] **Dr. McKayla:**  Yeah. Yeah. I think, I think one step at a time 
and keeping the focus like I really would like to create more content, have more 
of this really quality time doing what I love to do like teaching, thinking 
about content, writing blog posts, right?

[00:37:25] **Dr. McKayla:**  This is really what gives me energy and less 
about the administrative stuff. But then, as you say, I have to be real careful 
not to get people adding to my administrative stuff. So, yeah. But yeah, very, 
very good.

[00:37:38] ** Avdi Grimm: **  I think it's important to always know that like 
you can do the thing. One of my personal policies is like, anything that I'm 
thinking of delegating or automating, always do it manually first and do it 
manually for a while first and get a really good idea of what it is that I'm 
either delegating or automating.

[00:37:55] ** Avdi Grimm: **  And usually what I discover is that I can automate 
less of it than I was planning. And it's enough. Or I can delegate less of it 
than I was planning and it's enough, but yeah, as it's always very tempting to 
be like, man, there's this one aspect of my business. I just don't want to think 
about at all. And so I want to delegate, delegate that part of it.

[00:38:13] ** Avdi Grimm: **  And I think that's really dangerous though, that 
leads down that road of like now I'm just jammed up managing everyone and paying 
too much, you know, not balancing my books. 

[00:38:22] **Dr. McKayla:**  Yeah. I think that's true. 

[00:38:25] **Dr. McKayla:**  Do the thing the hard way for a while, figure out 
the smallest piece of it that you can automate or delegate.

[00:38:31] **Dr. McKayla:**  Yeah, cool. So Avdi, thank you so much for 
sharing all your insights. Is there something like, if there are developers out 
there that think, oh, I would like to have some side hustle, you know, get a 
little bit more independence or maybe even go full in, what do you think what is 
a, is a good strategy nowadays?

[00:38:50] **Dr. McKayla:**  You know, when there are already so many, 
screencasts, when they're already, you know, so many other things, so many blog 
posts, so many podcasts and so on. What do you think? How should people start 
doing it? Is a blog still a good first outlet? 

[00:39:04] ** Avdi Grimm: **  There's no going wrong with blogging. Honestly, 
like, it really doesn't matter like what your plan is. Get good at writing about 
things. Like, practice writing. It's just that I feel like that skill has 
informed, has improved so many other aspects of my business and of my career. I 
mean, writing about what you learn is such great practice for even if you just 
stay a regular developer, you're going to be a better developer because you are 
better at explaining and documenting your work to other developers. And so like, 
yeah, there's just no downside to getting in the habit of writing all the time 
about the work that you're doing. 

[00:39:46] **Dr. McKayla:**  Yeah, that sounds good. Yeah, I think so too. I 
think that's a such a good advice. There's I think there's so many positive 
things that can come, be that job opportunities or maybe you have to jump on, 
you know, you get better as, as you said, in your communication skills, better 
at communicating with your colleagues and so on. So yeah, I think this is a 
great, this is really a great insight. Thank you so much, Avdi. 

[00:40:09] ** Avdi Grimm: **  Oh, I have one other thing on that, on that note 
that I should include. Start building your, your mailing list now. 

[00:40:16] **Dr. McKayla:**  Mailing list, yeah. Good idea. Independent 
mailing list, I would say.


[00:40:20] ** Avdi Grimm: **  You know, do that blog thing and then slap, you 
know, go with ConvertKit or something and slap a mailing list, subscribe on that 
thing, and just start collecting that snowball now, because that, it takes a 
long time, but oh my gosh, the opportunities that come out of having a good 
mailing list. There's nothing else like it.

[00:40:38] **Dr. McKayla:**  Yeah, that's true. Yeah. I think that's a great 
add, great addition to what you said before. So Avdi, thank you so much for 
taking the time and talking with me and sharing everything with my listeners and 
yeah, have a good day.

[00:40:53] ** Avdi Grimm: **  Thank you so much for this. I really enjoyed it. 

[00:40:55] **Dr. McKayla:**  I enjoyed it too. Thank you so much. Bye bye. 

[00:40:58] **Dr. McKayla:**  This was another episode of the Software 
Engineering Unlocked podcast. If you enjoyed the episode, please help me spread 
the word about the podcast, send the episode to a friend via email, Twitter, 
LinkedIn, well, whatever messaging system you use. Or give it a positive review 
on your favorite podcasting platforms such as Spotify or iTunes. This would mean 
really a lot to me. So thank you for listening. Don't forget to subscribe and I 
will talk to you in two weeks. Bye.
