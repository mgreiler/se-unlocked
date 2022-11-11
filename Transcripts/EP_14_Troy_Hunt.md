---
episode: "Transcript Episode 14: Troy Hunt"
permalink: /developer-security-troy-hunt
status: publish
type: transcript
---

**Michaela:** [00:00:02] Hello and welcome, to the Software Engineering Unlocked podcast. I'm your host, Dr. McKayla. And today I have the pleasure to talk to Troy Hunt. But before I introduce Troy, let me tell you a little bit about myself. For several years, I've been working with Microsoft to help engineering teams be more effective and efficient.

I worked on solutions to improve, build, test and culture tools and processes at Microsoft. In fact, I worked with all major product teams such as Office, Windows, Visual Studio to help them get better results. Since 2018, I work with engineering teams all over the world through workshops and consultancy. 

In my code review workshops teams identify bottlenecks in the engineering processes and learn how to resolve them.

Everything I teach is based on proven best practices for code reviews that have to speed up code review turnaround times, but also increasing code review effectiveness. Given the recent events, all workshops are remote and are a great opportunity for team building and to strengthen the bond between colleagues. In our current stressful situation, such workshops can make a big difference and lighten up the mood.

If you want to learn more, have a look at my website at michaelagreiler.com/workshops or write me an email at michaela@michaelagreiler.com so and now onto Troy. Well Troy Hunt is a leading security expert. Through his online security workshops and his various online courses at Pluralsight, he has helped already hundreds of thousands of engineers understand the ins and outs of security.

He also developed the popular website, haveibeenpwned.com where you can easily check if your data has been exposed to a data breach in the last years. Well, I could go on and on, but just let me say that I'm super excited to have Troy here with me. Thank you, Troy, for being on my show. 

**Troy:** [00:01:46] Hey, thank you for having me here.

**Michaela:** [00:01:48] Troy, there are two very distinct topics that I want to talk with you about today. One is how you managed to become the leading voice in the security space and touch so many lives of so many people. And the other topic is: what do you think that, you know, what knowledge do software engineers actually need to posess about security?

What do they need to know about data breaches and attacks to the software system? So maybe I want to start with the data breaches. And there's, it's almost like every week there's a new data breach where millions of records of personal data are leaked. And on one hand that's super scary. But on the other hand, I also think because it happens so often.

People feel, I feel that people are getting a little bit blunt or debted by it. Maybe it's just me. It's almost like, well, it happened now for the fourth time in a row in a year, and nothing actually happened to me, for example. Right. So probably it's not that bad. What do you think about that? 

**Troy:** [00:02:47] Oh man, I wish it was only every week.

It is many times per day. At the moment. I just receive so much data that people are sending to me and it's just simply more than I can process. It's just untold numbers of individual breaches and of course a huge number of records in age. And then part of the problem too is that we only know what we know.

It's like that old quote about unknown unknowns in other, like there's so many more incidents out there that we've just simply never heard of, but, but have happened and are yet to surface and, and you're quite right that there is a degree of, of what I've often heard referred to as data breach fatigue.

So people just getting so used to seeing data breaches all over the place that they tend to sort of tune out. And, and what I, I sense has really happened over the last few years is we've sort of transitioned from people judging an organization harshly because they've had a data breach and now judging them more on how they handle the breach instead.

So if we think about incidents such as in 2017 there were a couple of big ones that were handled very, very poorly. Equifax was not a very well handled data breach. The, the Uber situation was not a very well handled data breach and they got, they got rather slammed by the public. But then I'll say in other organizations, had data breaches and handled them exceptionally well and actually come out of it looking pretty good.

So I think public sentiment has changed because it is happening so much. 

**Michaela:** [00:04:18] And do you think there is, you know, is that the right shift? Do you think it's just not preventable to have those data breaches or should organizations spend more and should technology be more involved to, you know, hinder data breaches or limit those.

**Troy:** [00:04:35] Well, the, the, the first thing is that they're all preventable. So every single data breach that I see has had a mistake somewhere. Someone who's got some poor coding and they've got a SQL injection vulnerability. Someone hasn't put a password on their publicly facing database and someone goes and siphons the data out.

So every one of these is due to a human error at some point. So yes, they are absolutely preventable. And I'd hate to sort of get to the point where we go "ahh , it's going to happen anyway." You know, I think we, we, we do need to continue doing our best to, to not make the mistakes in the first place, but then also plan for if they happen.

So, for example, password hashing is a really good example. Password hashing offers absolutely no security whatsoever. Until something else goes really badly wrong. So you've got to have a SQL injection vulnerability, or back your database up publicly facing and put it in the root of your website and someone downloads it.

And then password hashing is useful. So that's a good example of, of where we implement security controls in layers of defense. With the expectation that some of them might go wrong. 

**Michaela:** [00:05:39] And so you think that the attack surface has sort of stayed the same. It's just that 

**Troy:** [00:05:45] it's getting massively bigger. So, I mean, have a think about it, right?

Like we've all seen stats about how many different Mac addresses there are out there these days, how many different IP addresses there are these days moving to IPV6 and we've just got gazillions of them. And IOT is, is certainly a big part of this as well. I mean, IOT man. How badly are we messing that up.

There's so many connected things. It's just become a joke. I saw where I saw one last week I spoke about, which was a, an IOT candle. So there is a Kickstarter to have a candle that you can light with real fire remotely. Oh my goodness. I know. So I, I ordered one because I was like, I've got to see this.

You know, this is going to be amazing. Well, actually I was thinking, I'm going to take this to conferences. I'm going to talk about it, and it'd be really cool. But then I was like. Are you allowed to take that on a plane? I'm like, maybe I can't even put that on the plan. so that's amazing. Oh, well it's not just that, but you know, Hey, you're not meant to take like cigarette lighters on a plane. So I imagine it's similar to that. But, uh, yeah. Might find out soon. We'll see. Might have my candle confiscated. 

**Michaela:** [00:06:52] so. You have this website, where everybody can see if their email address was somehow connected to your data breach. It's called, have I been pwned? And I saw that. Well, one of the first steps that when you are a part of a data breach, what you do is you update your password, but what else would you recommend somebody to do?

So sometimes if, if there is not a lot of my other data, I mean, I cannot change where I live, right? So I will not move. Because of that. But for example, if there's credit card information, I would update my credit card. Is that justified or is that, you know, one step too far?

**Troy:** [00:07:27] Yeah. You know, like you just change your password, update your mother's maiden name, and change your date of birth.

It's, it's all fine. I mean, it's, it's an interesting thing, isn't it? Where we've got these pieces of static, immutable data, which we can never revoke. We can never change. And your birthday, mother's maiden name, perfect examples. And that, the interesting thing is, is that the way. This sort of data static KBA is still used for identity verification.

So there are still organizations out there who say, Hey, uh, you know, you want to say update something on your mobile phone account. Could you just give us your date of birth so that we know you are who you say you are. I was like, wow. Yeah. Like not only is that in all these data breaches, but also I put it on Facebook and I have parties and you know, now that piece of knowledge, identity verification knowledge is out there.

So that's a bit problematic that the credit card thing is interesting and honestly, like the, I think the piece of data I probably care about the least is my credit card. And, and the simple reason for that is that every time I have a credit card that's compromised and it has happened many times. I do travel a lot and I buy a lot of stuff online.

The bank normally calls me up and says, Hey, we're seeing some fraudulent activity on your card. Was this you? And you look at the transaction and go, no, it wasn't. And they go, okay, no worries. We're going to cancel the card. We're going to refund the money. We'll have a new one in the mail, it'll land in your inbox in a couple of days, your letterbox, it is like still a physical thing, right?

And then what you do is you go and update your direct debits or anything else that you have on file for your card, and then you get on with life. So I actually don't care too much about my credit card. I care a lot more about things like my passwords because they actually get you into my life. I care more about other personal attributes that could be used to prove identity.

And the only reason credit cards make such big headlines, and the only reason that they are constantly referred to and things like data breach disclosure notices is because PCI. Actually has the ability to effectively kill an organization. So every time a company's in a data breach, they're like, so you know, your email address and your password and your date of birth lists or stuff got exposed but good news, your credit card is fine.

"But that's the thing I care the least about!", Ahh but you've got to remain PCI compliant, so you're pandering not to the individual, but to the payment card industry. 

**Michaela:** [00:09:51] Yeah, that's exactly what I wanted to ask you, because every time I get an email about a data breach, it also suggests slightly that I might not be impacted.

So it never says you are not, or you are, it somehow, you know, it's between the line. It's like. Oh, there have been, you know, 300,000 records, but there are another 3 million that haven't been. And you know, it's more likely that you are not impacted. They're not. And so every time I get one of those, I'm like, probably it's not me, but I go and update my password.

But yeah, I think that this is probably a good strategy also to make people feel secure even when they are not. 

**Troy:** [00:10:31] Yeah, it's, I always wonder as well, how much of this is lawyers, right? And so I, I actually had a conversation with a company today that's got a very unpleasant vulnerability. And then the guy I was speaking to, he said, look, my, my legal counsel internally has basically said, don't say anything.

Don't do anything. And I'm like mate in this particular situation, if you don't do anything, you're going to have a really, really bad day. So lawyers. Very often I find really don't understand the industry and a lot of their guidance is out of step with reality. And yeah, a really interesting example of this is that so many times those individuals who break into websites, dumping data, redistributing it.

They don't care. They're anonymous or they believe they're anonymous, they don't believe anything bad can happen. So all the legal constructs in the world make absolutely no difference to them. And this is where I think lawyers tend to lose the plot a bit. 

**Michaela:** [00:11:25] So what are some of the steps apart from updating your password that you would say people should take action on?

**Troy:** [00:11:34] Well, firstly, if, if you ever say password in the singular sense, that's a problem. So if it is like, let me just update the one password that I use everywhere, well there's your first problem. So what we really want to see people doing here is doing what. I think most people know they should, which is having strong and unique passwords.

So never using the same password in multiple places. Always making sure it's strong and we've got to sort of be a little bit clear about those two things as well. Uniqueness is pretty obvious. Don't use the same thing multiple places because if somebody gets in one place, then they can log into your other things.

But strength is something that's, that's changed in terms of our interpretation of it. So in days gone by, we'd say, Oh, if you want a strong password, you've got to have upper case characters and lower case characters and numbers and symbols. And the original logic there was that that gives you a broader range of characters and the more characters you have in terms of length, and the more you have in terms of range, they multiply each other out and there's more possibilities.

The problem is, is that that's not really how humans work. And I do this really fun quiz. Every time I do a talk and I, I sort of travel around a lot and I get the same experience no matter where I am in the world. I say to people like, imagine if you had your favorite and it's all lower case, and you go to a website and you try to put that password in and the website says, no, you've got to have an upper case character.

What will you do? And everyone all over the world says, Oh, I just capitalize the first letter. And then everyone's like, Oh, hang on a moment. Why is everyone else doing the same thing? It's like, well, do you think maybe the hackers have worked this out? And then you go, okay, well you need a number. What do you do?

And everyone says, Oh, I just put a one on the end. So this classic view of what makes passwords strong is not really consistent with reality. So in a, in a perfect world, a strong password. If you want something that a human can actually type in is going to be something like a pass phrase, pick a few random words and combine those together.

Or ideally you have a dedicated digital password manager and you generate the password and it's just going to be 20, 30, 40 random characters, however many you set it as, that is a strong password, and that's going to be unique as well. 

**Michaela:** [00:13:47] So that's what I do. I have a dedicated password manager and I click every time I click the little generate button and something, you know, very unique and very obfuscated t comes out right?

But I'm still like. I, it gives me a little bit of anxiety because first of all, I have a master password for that one, which is now in, it's super, super secret. And then the second one is if that company gets into data breach or you know, what happens if, you know, I don't think, I don't know exactly what could happen, but I'm not completely at ease.

Do you think that I should just sleep very well? 

**Troy:** [00:14:24] Well, the question that normally gets posed is people say, what happens if someone gets into my password manager and there's a really easy answer, you're screwed. Like you're going to have a really, really bad day. Now that I think that the reasonable question to ask here is what is the likelihood, like we know the impact is high, what's the likelihood? And this really depends on a combination of the password manager that you choose and the practices that you follow. So I use the password manager Onepassword. And there's a few key things there that people need to understand. So first of all, my master password alone is not sufficient.

You need the master password and you need a secret key. And the secret key is a globally unique identifier. It's a great big string of characters. I have it printed out, physically stored in a safe. So someone with remote access that understands my master password, can't do anything. I also have two factor authentication, so even if you have those two things, you also need to have control of my authenticator app as well.

If someone completely compromises all of Onepassword. All of the passwords are encrypted on the client and then sent to Onepassword encrypted. So not only can an attacker not access the passwords, but Onepassword themselves can't access the password either. So the most likely scenario that I can come up with is someone would actually have to compromise the entire development life cycle pipeline.

Like they'd literally have to get into build servers or code level access, compromise the client, circumvent the client side encryption, or siphon the passwords off in parallel to somewhere else. But certainly as it stands at the moment, there's no way anyone can get into, can get anything of use if they actually get into the Onepassword environment or if they get the master password.

So with all that in mind, I feel a lot more comfortable that if I follow good. InfoSec hygiene. So not just my password, but also making sure I keep my operating system up to date cause I don't want malware running on my machine, which might then get access to the password manager. I'm very careful about the extensions I run in my browser, you know, all this sort of stuff.

**Michaela:** [00:16:22] Okay. Yeah, that sounds good. I should probably switch my password manager. Um, one of the things I wanted to talk with you about, again from a end user perspective a little bit is data privacy. So I know that you are sharing a lot of your life also online via Twitter or via your personal blogs. How do you feel about that?

What do you think, you know, is a good amount to share outside. are there some boundaries that you said. Did you say, well that's, that's something that I don't, you know, expose to the, to the outside world. 

**Troy:** [00:16:57] Well, I think the first thing is, is that it's a very personal thing. Privacy means very different things to different people.

Uh, I have friends that adamantly do not want any photo of the kid anywhere online. You know, even though they'll be at a friend's party, please don't take photos. My children don't put anything on Facebook. Now, I don't know exactly what they think will happen, but. Again, privacy is personal. They get to choose.

Uh, I know other people who at the other end of the spectrum where they, uh, they'll be like influencers as I want everything about my life on the internet. And then you're just looking at it going, Oh, I don't care about what your children are eating for breakfast. Like, why are you putting this on the internet?

So for me, I think I'm probably somewhere in the middle there where I share aspects of my life, a lot of my professional life, uh, online. Certainly I share bits and pieces of my kids normally related to things in the industry. In fact, I wrote a blog post with this only about a week ago. But there are other things that are, that are happening in my life, which, which I've chosen not to share, that are very personal.

Um, even maybe I'll share some of these things in the future, I don't know. But again, privacy is something that we all have to define for ourselves and then use the tools that we have appropriately in order to try and protect that privacy. 

**Michaela:** [00:18:10] Yeah. And is there something that you think makes you vulnerable more, you know, like for example, your address where you live or, you know, so for example I'm also thinking constantly about, especially my kids, right?

This is probably my biggest concern. You know, how much do I share online about my kids? And I'm not completely opposed to sharing anything. And there are pictures of my kids floating around on the internet, but still, every time it happens, I'm like. Am I okay with it? And it feels like I don't know exactly what, you know what could happen, and I feel probably nothing, but with AI and things like that, machine learning algorithms that are getting better every day, I'm not sure if I can predict the future enough, you know, to say, well, it's a safe choice to, to share, for example, pictures of my kids.

Do you think that that has some, some foundation this way of thinking, or is it just a panic. 

**Troy:** [00:19:07] I think the, the problem is, is that you represent that in a really binary fashion. Is it safe? Versus what? Like not safe. So if I put a photo of my kid on the internet, is everything going to be totally fine or is it going to be disastrous you know, is it going to possibly be somewhere in between?

And I think part of the challenges is what you've touched on, which is we just don't know in the future. What I do think is really interesting is the changing social tolerances that we have to online sharing. So I'm in my early forties I got to 18 before I saw the internet. I managed to make it to adulthood without having exposed myself in either the metaphorical or the literal sense, which often happens these days online. Like none of that happened. And the difference now is my kids are seven and 10 years old. So they've grown up in a time where they have never ever not known YouTube to exist or Facebook to exist, or an iPhone to exist and their social tolerances in as it relates to things like privacy.

Again, are going to be very, very different to ours. And I'll sort of lament a little bit when we, we look at privacy and we say, this is the way it should be. And it's usually those of us who've grown up in a time where we had a lot more of it and we project our childhoods and our held beliefs onto everyone else.

I think the reality of it is, is that as, as people get older and generations, uh, retire and then disappear and new ones come in and they've never known a world that's different, they're going to have a very, very different view of things. Up until that point my view of things is that I'm going to, I'm going to share what I feel is necessary and fulfilling to my life and my kids' life, and that's going to be a little bit different to what some other people do.

**Michaela:** [00:20:47] Yeah. Yeah. I think it's a good answer, and that's probably what I do as well because as I said, I share, but for each of the information that I share, I'm thinking. Should I or shouldn't I? Right. And I think it depends on the kind of information that, that you're sharing about your kids. 

**Troy:** [00:21:02] Well, I think conscious thought is, is a good thing, right?

Like the fact that you're thinking is this a good idea or not? Right off the bat is good. There's a lot of other people who are not giving it any thought whatsoever, and they're the ones I worry about a little bit more. 

**Michaela:** [00:21:18] Yeah. I'm, I'm evaluating on a case by case scenario.

**Troy:** [00:21:23] and you know, like this. Anyone listening to this, will go, that makes a lot of sense.

That's just a perfectly common sense approach. 

**Michaela:** [00:21:30] Yeah. So I would like to go a little bit away from the end user perspective and look at the tech behind. So, well, we touched a little bit already on what happened. If a company has a data breach, what are the common things there that go wrong? I would like to understand it a little bit better.

What should engineers know about, you know, software engineers know about data breaches, data privacy, security. So what, what should they know apart from, you know, very common things like SQL injection, cross site scripting, maybe failure to restrict access authentication and session management problems.

Those are the things that come to my mind. But is there something else? What are the fundamentals that engineers should know. Well, 

**Troy:** [00:22:12] probably the best place to start for engineers trying to figure out like what are the things that they need to look after. My applications is start with the OS top 10 so I was pissed.

The open web application security project, they're a not for profit organization and they produce a whole heap of really useful material and. They produce roughly every three years a document called the top 10 web application security risks, and I just brought up on the screen, so I remembered the right order of them, but there are things like injection such as SQL injection, broken authentication, lots of ways you can screw up authentication, XML, external entities, sensitive data exposure, broken access control, security misconfiguration, cross site scripting, insecurity to serialization, using component with known vulnerabilities and insufficient logging and monitoring.

And all of these vulnerabilities have really, really good explanations from OWOS quite critically are actually targeted at software engineers. So the targeted at the people building software, they're not written by security people for security people, and that's a massive, massive difference because there's so much material out there that just doesn't speak the language of people who are actually building the apps.

**Michaela:** [00:23:21] Yeah, I think so too. I know that document, and I use it actually in my cod review workshops to touch on the area of security reviews and code reviews with some, you know, security perspective. But you know, what happens very often is that I get some pushback from software engineers. They'd say, well, you know, it's really interesting, but I don't, I'm not in charge for that.

I'm not responsible. That's handled somewhere else. Or, you know. This is only relevant when I would access user data, which I don't. And then if you, you know, dig it a little bit deeper. We understand that we are accessing user data quite often, but what do you think about this mindset? Is that something that you encounter as well?

And how, how, how do you handle that in your workshop that are really focused on security? 

**Troy:** [00:24:07] Well, firstly, I've got a special place in HaveIBeenPwned for these people. I've got, I've got a lot of cloud space. Yeah, I'm, I'm fine. If people want to have that attitude, Hey look, I've made a complete career out of people having that attitude.

So yeah, I don't, I don't want to sort of kill my own job, but yeah, most seriously, I think that. There's a couple of issues there. So one of them is that just really demonstrates complacency. So a view that this just simply won't happen to us, or it's just not a serious problem. And it generally, when complacency is the issue, generally takes a serious data breach for, for something to change.

I also think that there's a little bit of a, uh, not my problem attitude there. And I've certainly seen cases where developers will say, look, there's this, there's what the security team does. I, I do the developing and the security team does security things. And really, security is a shared responsibility. We've got to get this right.

As a collective whole, we can't just say chuck it over the fence and someone else deals with it. And the third thing I think is really relevant here as well is that security doesn't necessarily have to be an impost. It doesn't have to be time consuming. It doesn't have to be costly. And if you look at something like SQL injection, that the difference in effort and costs between building code, which is resilient to SQL injection versus vulnerable to sequel injection.

It's the same. It is literally the same. There's absolutely no difference in the effort and in fact, I would argue that there are use cases where building resilient SQL injection code is actually more efficient if you're using object relational mappers or something like that. So I, I just don't see any good practical reason to have that attitude.

I only see ignorance. 

**Michaela:** [00:25:48] Yeah. Yeah, that's true. So I was thinking also about devops and now also dev-sec-ops, and it's more and more on the rise. Do you think that that's also one of the reasons why people have to know more about security than ever before, or does it stay the same? It's just a different mindset.

**Troy:** [00:26:08] I think it makes it faster and easier than ever to screw stuff up. I look a, I love the principles behind this. You know, the, I love so much of what we're trying to do in that area in the industry, it's just, it just makes sense that the, the challenge is, is that because of the rapid iteration of software and those rapid release cycles as well.

We, we do run the risk of circumventing what might've been a more formal security process in the past. Now, I think a lot of those formal processes have their own issues, but what it really does is highlight a shared responsibility thing again and say, Hey, you want to write software faster and release quickly?

You're really going to need to buy into this security stuff because we can't go and manually penetration test every single release anymore. 

**Michaela:** [00:26:54] Yeah, that's true. So if you are, I know you're consulting also with organizations, so what do you advise them about more formal strategies? What do you tell them?

For example, about code reviews or security reviews? What are your advices in that area? 

**Troy:** [00:27:11] So I look at it in a little bit of a continuum about where we actually want to implement the each part of this. So, for example, developer education I think is absolutely critical. Now I have a vested interest because I run workshops and I have courses and all that sort of thing.

But it just makes sense because it's such a cheap thing to do compared to all the other security things that you can spend your money on. So I would love to just start from the basis of high. Let's not try to screw this up in the first place. And I like, let's actually avoid writing bad code and we do that with education, but then we do have more formal processes that we can implement as well.

Now, they may be everything from code reviews to automated analysis. There are some great automated analysis tools out there for both static and dynamic analysis. I've written about them in the past as well. Things like, look, every night my build server is going to pick up whatever was coded during the day, build it, publish it to a staging environment.

I'm going to run all the automated tools over and have a report waiting for me in the morning. Fantastic. You can automate this stuff. And then I mentioned penetration testing before as well. Again, this is an important part of it to like build that into your life cycle at the right time because it is an expensive, very human intensive exercise, but that's great.

And if you build it on top of automated testing and you build it on top of educated developers, the hope is is that these really expensive penetration testers are not going to find much. And if they do, it's going to be something really, really good. 

**Michaela:** [00:28:37] Yeah. One of the things that, um, baffles me since quite some time now is we're testing and now you say penetration testing, but all kinds of men will test actually, when do they take place and where do they have space in this continuous deployment, continuous delivery life cycle. You said you have to think about when you do it because it's expensive, but when you think are a good times to do it, is it daily or is it weekly or you know, how do you figure out what a good cycle would be for that? 

**Troy:** [00:29:12] Well, ideally you want it to be a continuous process.

So, yeah, to my example before, things like dynamic analysis, it's machines doing the work, right? Like, let that happen on a nightly basis. Tell me if I've deviated from whatever baseline I expect to be there. Fantastic. Uh, I would definitely like to see things like penetration testing, manual penetration testing done at key phases of a project.

So, for example, at initial release or major revisions. Now, your problem here is that you can make a very, very, very small change and that could be disastrous as well. So that certainly doesn't solve your problem, but that normally gives you a good overview of the whole thing. And then you can do the likes of a combination of dynamic analysis and integration tests to try and pick up those little changes that you might make that cause vulnerabilities as well.

But one of the principles that we've had a lot in the industry in recent years is this idea of shifting left. So if you pitch your software development life cycle and we go like all the way to the left hand side of the scale where like let's say the design phase, let's try and shift the security into design and get stuff right there rather than letting it filter through into build, deploy, sustain, all this sort of thing.

**Michaela:** [00:30:24] And how would it look like, for example, how would security take place during the design? What would you think about? 

**Troy:** [00:30:32] Well, I mean, a good part of that is actually having a security review of the design now, that's the sort of thing that I'd love to see security teams involved in. So if you're in an organization that's large enough to have a dedicated team, get their input on that.

So for example, are we storing passwords in what we now believe is the best practice today? Uh, are our password criteria. Correct. As per today's standards, that's something you can change at that design phase. What components are we going to use? Are we using any components with known vulnerabilities? I mean, that was one of the things in the OWOS top 10 how are you going to keep those components up to date?

They're good discussions to have even before a line of code is written. 

**Michaela:** [00:31:08] So one of the things that I wanted to ask you about is about sensitive data. So for example, a lot of the companies like Facebook, Google, Twitter, and they have like, tons of relevant and highly sensitive data about millions of people worldwide.

Yet, I don't see that they are regulated extensively, if they are even regulated. Right? It's a, it's minimal to non-existent regulations there. On the other hand, for example, the European union has regulated each small website to, you know, spam. I would say, spam, people about their cookies. Right? And I feel it's, again, what you said at the beginning, it's a little bit fatigue, right?

What our people are doing, are they reading? You know, what's actually stored there? It's more, what I see, People are just clicking, okay, you know about the cookies. It's okay. Yeah, I understand another cookie. Right? So do you think that those measurements actually make any sense? And then again, What does it mean for the larger good, right?

Because if, even if a website is tracking, I think a large amount of these little websites and many of the websites are run by small businesses, I don't even think that they are looking at the collected data. So the data again feeds back to the large organizations that you know, have, have the power over that.

What do you think about that? 

**Troy:** [00:32:28] Well, certainly one of the first things we gotta recognize when we talk about regulations in government, they're traditionally always behind the curve when it comes to technology, technology marches ahead at at an absolutely unprecedented price. And then government sort of tries to catch up and figure out what to do.

So that's, that's certainly a problem. Uh, things like, the cookie warnings, I think are a perfect example. I mean, every time I go to Europe, I just joke about it like, what are you guys do? Seriously? No one reads this. No one understands it. It doesn't matter. And by the way, even if you don't have cookies, you can still fingerprint browsers and track them.

And apparently you're not meant to do that either and this was part of the cookie warning, but I don't know that cause I don't read the warnings either. It's kind of doesn't make any sense on that regard. But having said that, like we do need regulation to keep organizations in check, and certainly the likes of Facebook are subject to regulatory controls and they have received some massive fines in the past.

Even very recently. And some people argue that, well, Facebook's worth a gazillion dollars. Say a fine of a hundreds of millions of dollars isn't that much, but that's still a very significant amount of money. So they are certainly subject to regulatory controls. I think the question then is, are the penalties sufficient in order to dissuade them from doing the wrong thing, or do they need to be higher?

And look, we've obviously got regulations like GDPR, which are designed to try and apply some pretty stiff penalties for organizations that do the wrong thing. And the question is how much that's actually being a preemptive control and stopping it from happening in the first place versus a slap on the wrist after that.

**Michaela:** [00:34:06] Yeah, yeah, that's true. Maybe I want to switch it a little bit gears again. I want to talk about your, your career as well. So I would like to understand that a little bit more, how, everything started? So can you bring me back to the time when you were not as security expert, not as solidly donor, but you are just at the beginning of your journey to become one?

Where were you in your life, you know, what was your, what did you think about, why would you do that and what were your first steps into that direction? 

**Troy:** [00:34:39] Yeah. So look, I started out as a developer. I mentioned earlier, I was, I saw the internet when I was eighteen in the mid nineties and I just wanted to build software for the internet.

And I, uh, I actually started out doing a computer science degree at university, realized that the internet was too new for universities. They didn't have any courses about it. So I did about 80% of the degree and then eventually just dropped out and went and went and just went, screw this. I'm just gonna do it myself.

So. Started going and doing a lot of software development and I freelanced for a while and then worked at a bunch of different companies, financial institutions, interactive TV, and then the, a large portion of my career was, I spent 14 years at Pfizer pharmaceuticals, uh, originally as a developer and then as a, as an architect.

And that was sort of the, that a big, big chunk of my career as it's been more than half my working life. And as I was in that job, in particularly towards probably the last five years that I was in that role, I, I just started getting very upset with no longer coding. I mean, there's, this, was this one of these sort of problems we have in this industry where a lot of organizations will say, Hey, if you're a developer, if you want your career to progress, you've got to stop doing that and do something else, which really, really super sucks if you actually like developing and would also like a career.

So I, I did the other thing, I did the architecture thing and I missed the development so much that I started blogging and I started writing a lot of blogs about software related things, and one of those things was security and security just got a lot of traction.

So every time I'd write about security, people like, Oh, this is amazing. You should do more of this. And I kind of know, okay, I'll do it a bit more of this. And I just found that there was a nation there which hadn't been met. 

**Michaela:** [00:36:29] Yeah. So it's really, you're, you're following what people wanted, wanted you to write about.

And so when did you make the shift from being an employee to being self employed and saying, well, now I'm going all in. Have you had your Pluralsight courses already? Or you know, how, how does that, how did the dad change happen? 

**Troy:** [00:36:51] So I've actually got a talk about this, it's a talk called hacker career. So if you do a Google for my name and hacker career, there's a YouTube video I've done a couple of times now.

In fact, I was looking at it just an hour ago for another blog post I was writing and I was this, I think this is my favorite talk. Yeah. It's the only sort of soft skills talk I think I've done before, but it's, it's my favorite talk. And, and in there I talk about how I started to eventually hate my job.

So this is now sort of 2014 era. Ah, I've got a new boss. The new boss really didn't understand what I did. He was in the Philippines. I was in Australia. Big cultural differences. My Ozzy honesty and directness probably didn't go down very well with him, which, if I'm being honest and direct, I didn't really care about.

And, um, you know, we, we really didn't see Ottawa and I was just hating the job. And, I eventually had the very joyful opportunity to take a redundancy, and so they, they ended up making four different roles that were based out of Australia, but worked across Asia Pacific, redundant. We were in a part of the world where we were sort of the most expensive market looking after the cheapest market we were contracting, they're expanding.

It just didn't make sense. And that the joy of a redundancy is the company sort of saying, look, it's, it's not you, it's me. Right? Like they're going, yeah, you're fine. We just don't need the role anymore. And as such, we need to pay you a lot of money to go, which is good. So I got paid, I think it was almost like a couple of years worth of pay to go.

And I managed a, at that time, my Pluralsight courses were going really, really well. So I just went and started doing that. And then. Heaps of other things on top of it. 

**Michaela:** [00:38:31] Yeah. I think that's a really good start. Many people would wish for. So there are actually several things. So your, your topic was being picked up by folks around the world.

They found it interesting. You were already doing Pluralsight courses and then you are not happy with your day job and you get this opportunity. What do you think how, Yeah, I have like some ideas. How would a person that isn't, you know, in that particular position, how would kickstart a transition from employment to self employment?

**Troy:** [00:39:03] So the first blog post I ever wrote, I think summarizes that really well, and I didn't know it at the time, but it actually turned out to be kind of insightful. So the very first blog post was why online identities are a smart career move. And when I wrote that blog post. It was partly because I was interviewing people at the time for developer roles and I'd interview them and they'd say, you know, here's my CV.

My CV says I'm awesome, and I'm like well of course it says you're awesome, like you wrote it. It was like, what else was it going to say? And again, and they went like, go and speak to my referees, you know, like, here are my references. Give them a call, you know, they'll say, I'm awesome too, and I'll sort of go, Whoa, well you chose them.

Of course they're going to say you're awesome. Like, what do you expect? There is absolutely no independent verification of who you are or what you do or anything like that. This doesn't make any sense at all. And what was happening is I'd go and try and find information about these people online. So it's like, all right okay, I'm going to take this guy.

I'm going to, I'm going to Google the person, and then I'll find their LinkedIn profile, their StackOverflow information, some blog posts. Maybe they've commented on a forum, and I'd find absolutely nothing about the person, and I found that really fascinating that there was sort of no independent verification of identity and role and history.

So my theory was that if I was to start to carve out a bit of an online identity, and there was something there that other people could then look at and say, Hey, this is, this is troy. Look, Troy's got this history, he's done all of these things is what he's been up to. Then that would, That would hold me in high regard later on. And, at the time when I wrote the blog post, I sort of said, look, I don't know how long it will be before my employer doesn't like me, or I don't like them, but what I know is that if I get to that point later on and then I decide I want to do this, it will be too late.

You know? It just takes a long time to do. And I think it worked out to be about four, four years after I wrote that, that I was pretty sick of the job. And by that time I had that identity and I was able to go out and do independence. So that I think that the big sort of suggestions for people here is you've got to start planning this way, way, way in advance.

And one of the things that's really struck me, particularly over the last year for various reasons, is that to, to have great success at a lot of these things really, really requires a lot of, a lot of hard work with little return in the immediate term in order to get the longterm gain, and there's not a lot of people that actually want to go through that and put up with a lot of the things that I'll put up with, especially lately in order to try and get that good outcome.

**Michaela:** [00:41:51] Yeah, I totally agree. And I think also, for example, when I did my PhD, I was blogging, but I was blogging on the university website. And in hindsight I'm like, yeah, this was super stupid because I didn't own the content. And now that I'm gone for several years, they completely scratched the website. There isn't any blogpost of me anymore.

There is no information about the tools that I have developed and, um, the things that I've written just don't exist anymore. So I should have owned that content and I should have put that on my own website. But yeah, it was a lack of awareness. I wasn't completely aware that I should do that. And so, yeah, I think that for many people.

Even if you do test a little bit as you're sad, it takes a lot of time, but maybe you don't have to produce each month a blogpost, but maybe you write something every half a year, and if you do that over a long time, it will come bound to a substantial portfolio that people can look at it and say, well, you did that.

What do you think about that? 

**Troy:** [00:42:47] I think that the real key thing here is to, to have autonomy from your organization. Now that this doesn't have to be in conflict with your organization, whether it be a university or job you go to day in and day out, certainly doesn't have to be in conflict. It can be very complimentary, but you've got to think of yourself as an independent individual and an identity who's going to a job and one day it might be a different job, and if he can't do that, I think you really, you really carry forward, too big risk. An interesting story about this is that when Pfizer made these roles redundant, the, the way they did it is a week after Christmas in 2015.

There was a meeting scheduled and there must've been about 12 or 14 of us in the room in the technology department, and it was just a meeting with a really interesting mix of people that just didn't make sense to have them all in the one room at the same time. And then the topic of the meeting was something like, updates, and when I got it, I was like, I wonder, I wonder if you know, and because by this I was so keen to leave and I was just waiting for that redundancy.

Yeah. I went to the room and the most senior person, there was a lady who'd been with the company for more than 20 years and she was crying and I thought, ah, this isn't going to be very good.

There was a meeting scheduled and there must've been about 12 or 14 of us in the room in the technology department, and it was just a meeting with a really interesting mix of people that just didn't make sense to have them all in the one room at the same time. And then the topic of the meeting was something like "Updates", and when I got it, I was like, I wonder, I wonder if you know, and because by this I was so keen to leave and I was just waiting for that redundancy. Yeah. I went to the room and the most senior person, there was a lady who'd been with the company for more than 20 years and she was crying and I thought, ah, this isn't going to be very good.

You know, when you go to a meeting already crying, the outcome's probably not going to be favorable for that person. And then as the penny dropped and it became clearer for people, there are just many ashen faces, many people very worried about what was going to happen to them. And, and I remember me at one stage, I literally said, can we just... because it was the way they were doing.... they were saying "here's the org chart now", and there's all these names right in, in the boxes. And then they're like, here's the org chart in the future and there's just titles and there's less boxes than there are names. And they weren't really saying it. And, and I was getting quite excited cause I'm like, Oh this is it.

I'm going to get up. And I remember saying like, can we just stop the bullshit and someone just psych? Clearly are you making jobs are done. Cause I'm quite okay with that. You know, I just want you to be honest about it. But I'll always remember how worried most of that room was because they didn't have that plan B. Their job was their life, and that to me, that Dutch has taught me a massively valuable lesson.

**Michaela:** [00:45:06] Yeah, yeah. I was definitely that person. You know, they're just very, very focused and dedicated to one thing and somehow blindsided. Right? On one end, because I don't think that this dedication is from Marshall sites. Especially for lateral organization. Right. So, yeah, I think that's a very valuable obsession. Yeah. 

**Troy:** [00:45:26] No, you're, you're, you're right. And, and look at it, it might be that your boss loves you, right? Like the, you could have a fantastic relationship, but your boss is another individual within a larger organization that in certainly in a case like Pfizer might be making decisions multiple levels up the chain on the other side of the world, based on numbers in a spreadsheet.

And it doesn't matter how much you love the place or how much you think your boss loves you. That is not going to save you when an accountant does the numbers and decides that they need to cut heads. 

**Michaela:** [00:45:53] Yeah, and it also doesn't, you know, you have no influence over what your boss is going to do. Right? Maybe your manager is leaving, going some Burrell's being pre placed their reorgs.

There is so little control that you have over what's actually happening, but I think people should be more prepared for that. I see so many, I mean, even in my very. Close, you know, a network. I see people really dedicated to their job and not, you know, putting enough effort also to really care and prepare them for themselves.

So I think that's really a really good, really good lesson. So are you, you're still doing a Pluralsight courses. There are many other platforms, course platforms out there. How would you make a choice, if you are a new trainer, a new teacher, how would you make the choice nowadays to think about where should I put my courses?

How did you make your choice back then? 

**Troy:** [00:46:47] Well, I made that choice back in 2012 and the way I might it was was pretty simple. I read a news article about another author who was doing exceptionally well. He was making like $1 million a year out of Pluralsight courses, and I saw that and I went, Oh, that might, that sounds good.

I'd love to do that. Like I'd love to make $1 million a year out of Pluralsight courses. And I had a friend who was an author, so I asked him for an introduction and, and the rest is history. But you're right, it's a landscape that changes quite a bit. And certainly even within Perl site, it's changed. And, and I haven't actually done many courses lately.

I haven't done any courses for at least a year. And in fact, I had a meeting with them just the other day and we were chatting about more and, and what I'm trying to do is sort of find where the, the highest and best use of my time is. And one of the discussions I had with them as well, what's really different for me now as compared to 2012?

Is that a lot of my value now sits in, in the fact that people know me and I have by some miracle of the universe, a profile and, and some fame. And that is actually more valuable than just the technical knowledge on its own. So for me, that has sort of changed over time in, in terms of it making less sense for me to sit there for hours and hours and hours editing content with Eastern, it makes more sense to do things that are much more visible, but there are a lot of different other platforms that are popped up that have different mechanisms of the way they recruit authors.

The way they publish content, the way they monetize a Pluralsight worked well for me because they've paid royalties based on how much your content is watched. Turns out my content was popular so that that kind of worked well. There are a lot of other situations where you'll be paid or say a one off payment for your content or where it might be a different monetization strategy.

You've got to sort of think about, do you want to be on a tech platform or do you want to be on just a, just a massive e-learning platform of which tech is one thing . So there are lots of different decisions for someone to make. And of course there's always the route of self publishing and then there's all sorts of other things you can do independently of courses and videos as well.

**Michaela:** [00:48:48] And do you think it's still a very viable career choice to do that, or is the market somehow saturated with online courses because 2012 I think it looked quite different on, you know, the amount of courses that there were and the impact that you could have with creating one course or five courses. 

**Troy:** [00:49:07] I think it would be hard to do the same thing today.

So it even, for me, I think, I think it'd be hard if, if I was, yeah, let's say I was eight years younger and I was just starting this now as opposed to in 2012 I think it'd be much, much more difficult for my content to rise above everyone else's, which is what's kind of needed in a royalty based model.

And the, I guess the only reason I sort of hesitate is that no matter what the industry is as one opportunity declines, there are always others that emerge and there are lots of other ways of making money online, becoming independent, getting your content out there. There are a lot of other ways today than what there were before.

There's probably lots of things that I haven't even thought of as well. So I don't think that the way I did it in 2012 is the way to do it today. But that's not to say that there's not still great opportunities. 

**Michaela:** [00:49:55] And do you have some idea of what are the, in your mind, the best opportunities that are right now there for people?

**Troy:** [00:50:03] Well, that would be giving my secrets away.

It does really depend. So obviously I think a lot about what makes sense for me. Uh, you know, one of the biggest opportunities for me in terms of a combination of the effort required and then the exposure, and then the return on the effort is the workshops. Because I've just, I've created the content, I don't do any preparation,I turn up in a bank for two days. I talk, I leave, I send a bill job done. 

It's actually super, super easy, but that's something which is going to be a lot harder for some other people to do the conference speech. I do a lot of commercial conference talks these days because there are companies that run events that, That a commercial in nature and they want someone who can keynote and scare people about cyber things. 

And that, you know, that seems to be something I can do these days. So everyone's got to sort of find, not so much what, what the thing is that that works across the board, but what's the thing that leverages their expertise. 

I found that, that my expertise was around how I communicate and present, and that's worked really well for me. Other people's expertise might be around the, the depth of their technical knowledge, you know, like find the thing that works for you. 

**Michaela:** [00:51:18] Yeah. I think also you are in really different place right now because I'm being, you know, a thought leader already.

I don't think a paid speaking gigs are a big opportunity for others. Right? So very often I even read online on and Twitter's that people have to, you know, pay for going to conferences, having to pay their accommodation there or things like that. Right? So I think there, there are really worlds between you and others right now.

**Troy:** [00:51:46] And let, let's be clear, cause you, you've used that term a couple of times now, the thought leader thing, like I didn't sit there, uh, 10, 11 years ago and I started blogging and getting out. I want to do, I want to be a thought leader, you know, like I started doing other things and then this followed. So I think if people sort of sit there and they master plan this whole thing out too much and they have this end goal in mind, I, I, I suspect that that is probably going to lead to a lot of disappointment as well.

So that I strongly believe the reason it all worked out so well for me is that I started doing this at a point where I didn't have to do it, and then I just adapted and I did what felt right and I changed on a very, very regular basis. And I still do that today. In fact, I was just thinking the other day, look, I've actually got to sit down and plan things out a little bit because the only thing that I've ever done is just reacted to the environment at the time.

**Michaela:** [00:52:38] And I think that's a very good strategy. So because you said thought leader, do you feel, do you feel that you are a thought leader? Is that something that when you think about yourself, do you think about a thought leader?

**Troy:** [00:52:48] It's not sort of a front of mind thing. I mean, I'm, I'm conscious of it in so far as if I put messaging out there positively about something, negatively about something that influences people's perceptions.

Uh, I'm conscious that I've got, uh, a platform and a bit of a megaphone now. So, for example, if an organization does a bad security thing, I know that I can, I can sort of shame them a little bit and usually get results. And that's, that's something which, uh, it's, it's almost like with, with great power and responsibility, so on, I'm very, very aware of that.

Uh, some people are very unhappy actually, that I, that I have the ability to do that, that they get upset with for shame. But, uh, I've got a blogpost that I don't really care about that .

**Michaela:** [00:53:33] I will link all the progress you mentioned in the show notes. 

**Troy:** [00:53:35] So I actually think that having a platform and a voice and then being in an influencer position, it can really allow you to do some pretty awesome things.

So I think about examples where organizations have been doing some fairly woeful security things, and I've been able to write about it or tweet about it. And get it changed in ways where someone who didn't have that following or profile wouldn't simply because the organization gets shamed, they get negative press, and then they're like, Oh yeah, we better not do that anymore.

**Michaela:** [00:54:03] Yeah. So one of the things that really interests me is how do you get that information? How do you get information about the data breaches? How do you get information about those companies? Is that like some, you know, some informants give you the data and the numerously or something like that, or how can I imagine that.

**Troy:** [00:54:20] Well for things like data breaches, people always send it to me. It's just constantly sending it to me. So even if I look at my inbox at the moment, I, someone here, I won't say their name, it's a, the title is new data breach. And then there's the name of a website here I have not even looked at yet. And the CA.

So here's, here's the data. The data is from this website. Uh, this is a server that does something very particular. I'm very confident about legitimacy. There's breach since it contains my own personal information. So yeah, uh, good on him. Other individual and could have the bridge manager be security conscious as myself.

So I thought it would be worthwhile having an included, never been paid. And this one's only got about 7,000 records or something in there. So I might not even be able to justify doing anything with it, which is a really kind of sad thing to say, but it all is inbound, so it's always people popping up, sending me DMS or sending me emails or encrypted chat messages going, Hey, here is more data.

**Michaela:** [00:55:15] Okay. And then do you pointed to a server where you can, for example, download the data or how does that work? 

**Troy:** [00:55:20] Yeah, so very often, and as I've done a number of talks where I explain and show this, but very often people will do things like put it on Mega.nz. So, Mega.nz is a really great file sharing platform though.

They'll drop the data in there and then they'll send me a link and then I'd download it and verify it. And if it's all legit, load it up. 

**Michaela:** [00:55:39] Okay. Yeah, that sounds, sounds interesting process. So there's also a lot of manual actually work involved from your side too, to have that website running. Is there, do you have any plans for that backside point of future?

**Troy:** [00:55:54] Yeah. You know, the, the biggest day of head was about a year ago, had 10 million people in a day come to the website. So, yeah, that was popular. I actually announced in, in April, I was going to look at, uh, finding another organization to acquire it. And I started, in fact, I announced it in June. I started the process in April.

And, uh, I wrote about that at the time, and literally today have been writing the blog posts, which will announce the outcome of that. So I really hope in the next week or two I can get that out there. And that is, yeah, it's just been an interesting year.

**Michaela:** [00:56:33] Yeah it's true. So, um, I think for my side, especially because we are running out of time, we, uh, I would like to wrap up the interview. Is there something from your side that I haven't, you know, haven't asked you, where you think that's an important message that you have and that you want to share with my listeners?

**Troy:** [00:56:51] Oh, look, I just think it's been a really interesting set of questions around both of the security side and the career side of things. And I guess if, if nothing else, I'd just suggest that people really sort of think about where they want to go with their career and, and take control of it. There's, it's just such an amazing industry.

In fact, I read a blog post, the blog post for everything you can clear this one, which was around, uh, in fact, I wrote, I think it was the last day of 2018 it was around fundamental financial tips for technology professionals, a bunch of stuff in there. All right, cool. So that, yes, man, every time I do something of like a soft skill nature, people find it really interesting.

So maybe there's a lesson there for me. Um, so I would encourage people to read that, think about what they're doing in the industry and the amazing opportunities they get working tech. 

**Michaela:** [00:57:37] Yeah. Yeah. That's, I think that's a very good, clear thing. Things. Um, I read that blog post, it was amazing. I will also link it down there.

So thank you Troy for being on my show today. It was really a pleasure.

**Troy:** [00:57:47] My pleasure to be here. Thank you.  

**Michaela:** [00:57:51] Yeah, thank you. I hope you enjoyed another episode after stuff engineering unlocked podcast. Don't forget to subscribe and I talk to you again in two weeks. 

**Troy:** [00:58:01] Bye.

 
