# Transcript EP-13 of the Software Engineering Unlocked Podcast Dan Abramov

**Michaela:** [00:00:02] Hello and welcome to the Software Engineering Unlocked podcast. I'm your host, Dr. McKayla, and today I have the pleasure to talk to Dan Abramov. Dan is probably the most well known person in the whole front end development online scene. Dan mostly works on React, a very popular framework for JavaScript. Dan it's also very vocal about JavaScript, React and development on his Twitter, as well as on his personal blog.

Den is also actively supporting diversity in the tech space and recently started a side project next to his day to day job at Facebook. So I'm super thrilled to have Dan here with me today. Dan, thank you so much for joining the show. 

**Dan:** [00:00:40] Thank you. Hi. 

**Michaela:** [00:00:42] So Dan, you're actually a software engineer at Facebook in London.

Can you tell me a little bit about what your day to day actually looks like? 

**Dan:** [00:00:49] Yeah. So I worked on the React core team. Even though most of the team is in Menlo park, in United States, but we do have a few people in London. So I'll work on React itself. Mostly the open source library that, so some of the listeners might be using most of the things like fixing bugs in it, deploying new versions and working on new features, sometimes writing documentation, figuring out the migration paths when we change API APIs and just general.

Kind of maintenance for the library. 

**Michaela:** [00:01:26] Yeah. So I actually read through your decades in review blog post, which I also link down in the show notes. And there you described how you interviewed for Facebook, and so you described that you were at a conference and you gave a talk and there were also people there from Facebook and one of the people from Facebook you knew already from online collaboration and through chat.

And this person asks you if you would like to interview right there at the conference in a hotel or something like that. And you spontaneously started to go through a whole interview loop right there in the hotel. So can you tell us a little bit more about the interview process itself? Which questions did they ask you and how does this experience compare to a regular interview process at Facebook?

**Dan:** [00:02:12] Yeah. so the interview process really depends on the exact role, and that's actually at least like at Facebook, that's a pretty important distinction, because if you apply for fontend engineer. That's an entirely different interview process from applying to your software engineer.

Even though internally these positions are exactly the same. So once you get in, it doesn't matter which one they were hired with, but the interview process is very different. So the one that I went through was front end engineer process, which is, it is, I find it to be a bit more practical in terms of like what questions get asked, because the regular software engineer process it, it is a bit computer sciency. and I'm like, I'm not super good at those questions. , but for, for the front end interview, we ask things that we think would be irrelevant to the actual, like application development, with JavaScript.

it's mostly, so in terms of length, I can say the exact length. it also depends on the office and the exact, like role title. But, I think it's something like four hours. So I think like the Yuto, interview processes. He, if first go through 'em. Kind of a screening interview that is, like a coding interview, but it's remote, that, because usually like, but we need to go through that first before we bring somebody onsite.

And then the onsite process is something like four hours and it's, easily three coding interviews, each, each interviews, but the different person, and the takes roughly 45 minutes. I think each. And, there is a, a couple of coding interviews, one interview about the past experience, in one interview that is more a kind of design architecture, kind of interview.

But all of those are tailored to, to fondant. so that's pretty much what I went through. And, in this case, I was just lucky that. There were four different people from Facebook at that conference, because there were speakers. and yeah, and we, we do use whiteboards, but we, at least in the front end interview process, we don't use the typical, like computer science, a wide questions.

So it's not about these in some weird data structures that aren't relevant in finance, but it's, it's more about things that you might encounter. and so we, we do use whiteboards in the sense that, we don't give you your computer to write code in, like, so you have to write on paper or on whiteboard.

but we also try to treat it like. Just as a draft. so I think it's good to practice with abide board. but it's, like sometimes whiteboard is annoying, right? Like, you can't copy and paste, and just stuff like this. but this is also why we try to keep the questions, relatively small. so we don't expect solutions to be more than like a 30, 40 lines of code for most questions.

so the whiteboard is also useful just to kind of communicate ideas and just discuss like trade-offs and what are the different things you could do, your different problems you might encounter with the solution. 

**Michaela:** [00:05:29] Yeah. Actually, I think vibe boards sometimes feel so intimidating because it reminds people, and, well, I'm generalizing here from myself, it reminds of a classroom setting, right?

So where you have like a teacher that asks you to be in front of the class and then you'd solve something, and if you can't solve it, it's very embarrassing. I think maybe that's the connotation that we have with bite boards because apart from that, I really love whiteboards. I mean, my office is full of whiteboards and I love to ride them them.

It's just that in the interview process where you're in a very vulnerable position, I think it becomes a little bit of an intimidating thing. But what I wanted to ask you, as well as, are you right now involved in hiring at Facebook? Do you, do you do interviews? And if so, what question do you ask and how do you determine if a candidate is a good fit?

**Dan:** [00:06:18] Yeah. so I J code in interviews. I don't want to experience her, architecture, indivisible is not yet. so it's, it's just code in, So, I obviously can keep the actual questions that we use. but I think in general, the things that I look for are, a solid understanding of the language.

that's fun. So, we expect that, people know JavaScript, people who apply know JavaScript pretty well. And, We don't actually test for any like libraries or frameworks. We don't ask react questions at all. we assume that if you know the language, you will figure out, like in your library, but if you only know the library, then you're going to struggle with like other libraries.

We're going to expect you to understand the language. so it's like, in terms of language, it's like things like understanding variables, closures, asynchronous programming, control flow, functions, and how all those things kind of work together. then in terms of data structures for funnel interview, and again, we don't.

Expect to you to like, understand any super computer sciency things that, that own the current front end. but some data structures do occur in front end. so like trees for example, you don't see, like, I dunno, red black trees or something like this, but, you do see Dom trees or like, react elementary is, and just understanding how to work with trees, like how to kind of traverse them.

What did you do with them? is, is important. and also just like, another example is like, a lot of interview training questions that you might see on the web are about what is the performance of this goat? What is the complexity? Like, is it like, Oh, F, N or O of N squared and so on.

So we don't expect people to like necessarily memorize those. but. To the extent that it is practical, like it's, it's valuable to know those things. so like a practical example, maybe, here's some code, that maybe it takes a, like a a hundred milliseconds, for like a thousand items.

But then if there's 10,000 items, then suddenly it takes like two seconds. so w what is the problem with the code and how do we fix it? And so. You can kind of like, even if you don't have full kind of theoretical, like if you don't know all the correct terms, but you have the right intuition about, where the slowness occurs and why, and what is the approach to fixing it and how to use like objects or a raise or appropriate data structures, to fix the problem, that's fine.

So that, that's what we're looking for. so it's a, it's kind of interesting because like in front end, It's very important that you care about user experience. Like that's, that's another thing we're looking for. but sometimes it does involve some of those fundamentals and we don't care that much that you're a great, at theory, but we want to see that he can apply those principles in practice.

**Michaela:** [00:09:19] So also what you mentioned in your blog post was that you were really nervous and that you had some difficulties actually swapping two items in an array, and somehow the interviewer encouraged you and she gave you the confidence that you could actually move on. So she helped you to move past. What I would call a little bit of a black bow.

Right? That was caused by a setting and your anxiety of the interview. And I find it really good that you are outspoken about that and that you say something like that openly. I mean, interviews can be nerve wrecking and they create unnecessary anxieties. I can totally relate to that. And I think one of the reasons why I'm self employed right now is because I don't want to go through any dreadful interviews.

That, how can we make the interview process less intimidating and remove some of the biases from the interviewers and make them also more inclusive? 

**Dan:** [00:10:09] Yeah. So I'm not, I'm not like an authority on the subject. and also like people, I've seen people get pretty nervous during the interviews. I think like one thing that helps is, that's why we have several.

Right. 

So, it's rare that everybody has exactly the same feedback. so this is my, we, uh, we keep it so that, they have multiple interviewers. Every interviewer has to submit their feedback before they see feedback from others so that their feedback doesn't get biased by what the other interviewers say.

you can't like change a decision. But then you also, like months, all the feedback is in, you also look at, look at it as a group and taught it big out similar themes like, Oh yeah, it seems like there is kind of a knowledge gap in this area, but maybe they age really well in this other area. And then it's kind of balance in like, do it ultimately what we want to figure out this, it's not like, is this person a great programmer?

but like other, again, to be successful, In this environment. And so sometimes, It may be that maybe the person's very good technically, but they don't communicate well. And so this is going to be a pretty big problem because we expect people to communicate a lot, especially as the like progress in their careers.

so, I think like another tip for interviews, at least like for Facebook, I don't know how people interview at other companies, but, We really care that he explained what to do and kind of explain your thinking process, that he listened to the hens. So like the interviewer is on your side. The interior wants you to do well.

and sometimes we kind of give him like, Hey, like maybe this is not the right direction. I'm like, are you sure about this? w what are the other things you consider? And. Sometimes people listen to them very well. And that, that gives us, if you learn that, yeah. Like this, this person is like in working in a team, they understand when, they, they had been asked to do something or they are, like they're being challenged.

And sometimes people just don't listen at all. And. It's like, okay, well what if there is a work problem and pretend to communicate something and this person doesn't hear us? so , that's also important is just to have a clear communication, clear thought process, and kind of both listen to the interview year and also explain the way you're approaching the problem.

**Michaela:** [00:12:35] So know that for many people working at Facebook, Google, and Microsoft is one of the big dreams. Was it also for you that it was a year long dream to work at Facebook? Did you think about that, or did you envision yourself, especially given that you were working with react, did you think Facebook would be a good place for you?

At least for awhile? 

**Dan:** [00:12:52] Yeah. so I, I think early on in my career I didn't really, like Pierre. About big companies as much. so I am originally from restaurant, so there was like a Russian company that I wanted to work at, which is kind of like a Facebook Sloan, but they had a really full, polished product.

And I think the thing that compelled me about it is that it's team was actually not big, so it was like 10 or 15 people who were actually working in the West side. I don't think I, I felt like. I really wanted to work as a big company at the time. and so I didn't really consider Facebook at all. and later on, so after I started like putting out some open source organ react echo system, I did get contacted by a Facebook recruiter.

and I did feel like I would want to work here. but then again, not because it's like Facebook, but because I knew people who were working here, right? Like Jane Chan, who was like one of my interviewers. and she's the person I met at the conference, but also like, a few other people who were on the react team.

and, like even today, I feel like, if I was not on the react team, like, There are things that are like about Facebook. There are things that I like less, like I don't like open floor spaces very much. although I can also see why Facebook is, is kind of doing that. but I think what really kind of keeps me here is just, there's so many smart people to learn from and to, like I, I feel like before Facebook, at least like in my career, I would always kind of max out.

Like, maybe started the company, I can reach some, well the thing that I'm doing and that I'm not sure what, what is the next, like how do I keep learning? I just keep doing the same thing. And at Facebook there's always going to be someone smarter than me or more talented than me or just somebody who, he just does things I haven't learned yet.

And so it's really, If you like learning, it's really fun to be around. 

**Michaela:** [00:14:46] Yeah. Yeah. I had the same feeling at Microsoft that there is always, I mean, at lunch you go a lunch with some of your colleagues and you could learn something, right? You're like, wow, I didn't know about that. Yeah. So, but what was also happening at Microsoft quite a bit, where reorganizations for examples and.

I was lucky that it wasn't really affecting me. So we were quite a bit, but it was always the whole team that bugs reorg. And suddenly we were, instead of research, we were part of research and development, and then we were a part of visual studio, for example. But somehow. They wait until the end. They, you know, they didn't take us apart or change our mission or something like that.

But it happened for many, many, many adult teams. And so is that also happening at Facebook? Are people reorg, you know, moved onto different projects without actually volunteering to do that? And what would that mean for you, for example? 

**Dan:** [00:15:42] Yeah, so that does happen as an annual large company. It's not super common, but it's also not super uncommon.

so we use a workplace as the primary means of communication. The workplace is like a, a version of Facebook, but for work. so we use, like most of the communication happens on workplace messenger and, and the groups, which is like Facebook groups, but again, for work.

And so, there is a group called, this week in reorgs, all the posts announced and reorg get reshared to that group. So this is, it's kind of funny. I mean, I think it's like one post for like three weeks, something like this, but it's a huge company. so this doesn't really happen like completely out of the blue.

So usually when there's reorg, it's because, something is not working and the chance to fix it by like shuffling people around, often teams around, maybe there is like a new director who wants to consolidate things differently. aye. I didn't expect the react team to suddenly become like reorg the way, because we, we actually have, like, there is actually a react org.

so this, this includes, management of, reacting really, like the team that's working on the new website. so Facebook is like rewriting the website and reacting really, And so , our org did get moved a few times. but that's actually, it's kind of interesting because it got moved from, It is to be closer to kinda Tulane. but it got moved to being closer to the application. and that does make sense because, it's a word called product infrastructure. And I think that's, that's a really important part of kind of Facebook approach to like UI to learn and react is, to keep it very close to actual, like developers using this stuff so that we don't kind of invent things in a vacuum and just like release it into the world.

But that we actually, like talk to people using this stuff. And if it's half working out, like it doesn't go through like five levels of, like management chain, but it goes directly to us. and that keeps us, that gives us a good reality check. 

**Michaela:** [00:18:05] Okay. Yeah. So, well, react, especially react 16 is now with the MIT license.

And so it's a proper opensource software. And do you feel that sometimes there is a balancing act between what you have to consider for, you know, the benefits of the company and then, versus the benefits of the community? Or are those interests really aligned and very easy to combine? 

**Dan:** [00:18:28] I think it depends on the, period and like, what do we want to do? I think, like one way, Tom, who's like my, Our current manager. So one way Tom has been, putting it is that you can imagine there's like a stack of things that are only important to Facebook. And then there is a stack of things that are only put into open source.

And then there is a third stack, which is like things that are important to both. And even if we just keep working on the third stack, like it just never ends. so it's like there is enough intersection that, We kinda, we can keep going. I think the beaker split is actually not between the Facebook and open source, but it is between serve in like legacy existing code versus, paving in the way for like improvements that are not incremental, and making sure that we don't get stuck in the past, because of the existing code. And like, we care about existing code a lot, but also at some point, like you need to make a choice that you, kind of move forward or, I stock during the same thing. And I think that is, that is kind of a bigger split.

Sometimes we have periods where we're all about maintenance, fixing bugs, improving documentation like Jane, all those things that serve existing user base and existing code. But sometimes we, we're going to focus on innovation. But then we tend to neglect, the, like the existing features a little bit, and it's just. We're going to switch between those cycles as as with Polish, new things and kind of get them out and then they all go through this same life cycle. . 

**Michaela:** [00:20:09] Yeah. Especially backwards compatibility can really bite you, right? 

Oh yeah. 

So I feel like you are really fundamental to the react community. Some people even believe you are the original creator of the react framework. Well, on your Twitter profile, the first thing that you stayed is, I did not make reacts.

So apparently you have to even, you know. Say it out loud. People don't project that to you, but still have the feeling that many people are projecting many different things onto you. Do you sometimes feel that there is too much way and responsibility on your shoulder, especially when it comes to the community and you know how the community behaves and things like that?

**Dan:** [00:20:48] Yeah. 

**Michaela:** [00:20:50] Do you have an idea how you got into that position? Why are people projecting things onto you and why do they think you are responsible? 

**Dan:** [00:20:58] I think it's, it's a bunch of things. so one is, I was there pretty early on, maybe during the year. Like, boom, off reacts like thousand 15. so I built a bunch of stuff for myself because I just, because it isn't, it didn't exist.

So like I, I helped, add some features to react harder. I helped like have a few libraries, worked on how to load in, which. Which is like a way to edit the page and see changes reflected in real time without like refreshing the application. So working on a bunch of things that people found interesting and I was working on them just because like nobody else was.

And it was still a very early time in the ecosystem. And so I also answered a bunch of Sacramento questions and I think people just saw. Like, it's when people come in a bit later in the ecosystem. They just saw my face everywhere cause I would just like because I was there early. I think that that is part of the reason, that the other one is just, I think I've worked on projects that, people found interest in, or like inspiring or eventually confusing, like with the Redux.

which was supposed to be a proof of concept for conference talk and not really like. The whole thing. but I think people like I, I'll take that I'm pretty good at making demos and, I'm not really good at like original ideas. So what I, what I tried to do is, I try to, find smart people with really good ideas. Who are struggling to kind of explain those ideas and by why those ideas matter.

And I try to popularize them because I think that these ideas deserve that. and I think people respond to that. So another part is just like, you remember who you learn from. Like I remember people I learned from like 10 years ago, even though they don't blog anymore, or like , I used to read like every Clippers blog on C sharp and like , I don't care about C-sharp anymore.

but like I remember him because I learned from him and I think people would tend to remember people they learned from. So I think that's, that's another reason. That people kind of remember me. 

**Michaela:** [00:23:13] I think also sometimes it's like the person who takes on responsibility is responsible.

And I have to feeling that if you see something is broken down, you are the person that takes action and the fix it. It are be part of the solution. And I think maybe that's also, well, one of the reasons why that's happening. I don't know. What do you think? 

**Dan:** [00:23:35] I dunno. Fix enough things. I kind of feel like lately in the last three years, I'm just, kind of goes then like I use the ice, the read, like all the notifications and like fix all the eaches in my libraries.

And for the past year I've completely unsubscribed from everything and dissolve reacts. I don't even check issues. Like, I felt bad about it for awhile, but then like, yeah, like I've done my work and I, I feel like I just can focus on these things right now and I need to cut them out and hope that somebody else will pick it up and I'll just work in the things that I think are important to me today, but not necessarily, be a good maintainer anymore.

**Michaela:** [00:24:18] Well, I don't think you have to make him life commitment out of everything that you do. And I mean, you are stepping away from something means that there is space that somebody else can fill up, which, you know, gives opportunities to others as well. So I think it can be a good thing as well. It's always how you want to see it.

**Dan:** [00:24:36] So it's a. Yes, but it's also kind of like a Tom Sawyer move where, you know, like when, when he says like, Oh, it's so amazing to paint this fence. and then like, he finds people to paint the fence for him, but it's still, especially like if those people are in the same position that I was, which is, like I wasn't working on this full time.

It's just like a side thing and I was, had a job. And so it's kind of like unpaid labor. And, if I get paid to the open sores and I hand off tasks to somebody who doesn't get paid to do that, then it's, it's like, sure. Maybe that will give them some opportunities to like, speak at meetups or like at conferences or like, Get a better job in the future with like improve their portfolio but also like, not necessarily, and they're not necessarily, you're going to be able to take advantage of it. And like the whole system where it got to have to do it is, well, when I have to pick up this optional work, just to kind of be competitive in the marketplace is also kind of weird.

So I dunno how I feel about that. 

**Michaela:** [00:25:40] Yeah, I am a mother of two and I know exactly what you're talking about. I know what it means that you cannot put in all the hours that you want, especially with the contributions outside of the regular work. There are just simple, plain limitations for some people on how much work they can put in and yeah, I really liked that.

You are so considerate of all the different aspects and everything that you said really makes sense. I think that there are many different angles to story and I think that people are free to pick up and make something good out of it for themselves. For example, I thought a lot about what it means to take responsibility of your own career, and I think I wasn't particularly good in the past of doing so.

I mean, I put in all the work. But I made also mistakes when promoting and showing off my work. For example, during my PhD, I blocked on the university website, which is the stupidest thing that you could do because I'm not owning the content. And you know what happened after a while, they just deleted it, right?

So they were like, Oh, she's gone now for a few years. Let's delete it. So everything that I ever wrote about the systems that are implemented, is not there anymore. The good thing, there are official publications and all that, but my point is that I could have, you know, advanced by career, definitely could have advanced my career if I would have been more.

No more caring for myself and thinking about making a more conscious decision that actually this should be on my own site. And similarly, during my time at Microsoft, I didn't let the outside world know what I was doing. I was very focused on their work inside. But after a while, you know. It's, it's not a good strategy because nobody actually takes care of you.

It's really your responsibility. And I think it's similar here, right? In open source software, there's so many different motivations for why you could pick it up. You can learn, for example, if you want, you can also promote yourself. but yeah, I, I see the negative sides to it, as well. So sometimes people feel.

Taking advantage of. And so I think that's why it's really important to step a little bit decide and really think about why are we doing that? What are the outcomes that we would like to achieve and how can we align that with what we are doing. Well, but, having said all that, I want to switch gears a little bit and talk about software engineering practices, especially at Facebook, because that's what I'm really interested about.

So I wanted to know if there are some company-wide practices and if you have insights into dad, for example, one of the slogans for Facebook is move fast and break things. And also one of the Twitter comments was that people actually mentioned that it has. Changed it a little bit. It's something like a more forest and break things, but have a stable infrastructure or something like that.

So do you have a particular way in which software is developed at Facebook and what do you think it means? Move fast and break things? What happens ed Facebook. And what's the impact of that slogan? 

**Dan:** [00:28:47] Yeah. Well, so the official answer is that, yeah, that we, we don't, we don't use that motto anymore. It works with a, some things, but it can have pretty bad consequences for other things.

I think, and I think it's true that it's, are there are parts of this mindset that as the left, and there are parts of this mindset, I think like, why this may not be a good approach is So one thing that we've started doing, I guess, like several years ago is, Like whenever you make change, that affects, like things like privacy or security. there is a lot of more, or even like accessibility. There is a lot more cross functional review that like in early days that wasn't the case.

Right? So like in the early days, they to exchange stuff and as long as like one engineer accepts it, it's live to production. so I think there is. Like, we've tightened that a lot. so it's harder to like make changes to those critical things without getting like a good review from like a policy and security and privacy and all of those orgs.

but fraternities that are like relatively safe, I think that mindset is still like partially leaves on. and the most kind of valuable part of the fit that I see is just,  if you don't have a strong, code ownership, process, so what that means in fact is, is that, if I want to fix something, Like a, maybe in a product that I don't own, right? Like maybe I want to, I see a blog, an Instagram, or like a see bog in workplace or just in common section and I work in a react team.

 I don't own any of the surfaces, but as long as I can get like somebody were necessarily like the owner, but like some other engineer, approve of my change. And as long as it doesn't like concern itself with things that are risky, like privacy or security, then I can, I can ship my fix.

And so, in practice, this means that people are empowered, to pick things up whereas like in, in some other companies. you have to get a review from somebody who is like in this file, like you have to get review for somebody in file called owners in this directory.

So we don't have that. we usually like, if, if the code is so, like fragile, that is so scary to change, then you should have better tests. And if, If you really want some team to kind of look at the changes, then you create automatic things. So you kind of add them as like optional reviewers or like it create things on top, but it's still, we kind of expect engineers, to rely on, I just social behaviors.

lot more. So for example, if I'm fixing a bug in the Instagram, I won't like just ask my coworker to stamp my change, but I will look at the blame for that file and I look at like the history and see, Oh, this, this person changed that line. They might have context on this. So we'll message them on the work release messenger and say, Hey, like I'm changing this thing.

 I think this is, the rye fee's going to take a look at it. And so it's expected that even though you. Like you are given a lot, more freedom. It is kind of on here to ensure that, like, to actually trust the change, to pick the right people, to review it and to, to commit it. And then, to just be there.

So we call it like support in your changes, which just means like you commit them and you. Watch the graphs, or  you notify the person who was on the call for this product. Hey, like, here's like a thing I changed just in case something blows up. Like, ah, I'm the person responsible for it.

so it's like the chicken, people that here is, like you have a lot of freedom, but you also have this accountability. And that's something like, at first you're going to miss up and you're gonna like, maybe not take the side down, but maybe like. Yeah. Are you might, like mess something up. hopefully like automate the system, sketch it before it goes out to all the users.

but we also expect the, just the kind of learn to be responsible with your changes and learn how to be there and to build those connections. And then the thing is. That actually, and the courage is a law of more collaboration, the future. Because like the next time, maybe you want something from like Instagram, you can message that person.

We'll review the change and say, Hey, like, maybe you can help me with this. Oh, like, so you, you built all those, like social connections within the company and then, it's a lot more efficient than always go in through like. Posting and in groups or like official channels is everyone is encouraged to create their own kind of network within the company.

And I think that's, that's actually pretty cool. 

**Michaela:** [00:33:29] Yeah. well, so you mentioned testing a little bit, so I would like to know how does testing work at Facebook? Do you have like one company wide strategy or does testing depend on the kind of part of the software that you are testing or maybe the team that you're working with also?

are there some manual tests happening or penetration tests happening in Facebook? And if so, how does it look like. 

**Dan:** [00:33:52] So it really depends on, yeah, on the product. And the, again, like there's like things like security or privacy that are parents separate and there are like teams, we're actively, I tried to break it.

 we have this, shifting left, which is, like if you, if you draw kind of a graph of like, At different stages where you just may care. So it's like, there is like code review, there's like automated static analysis and like Lynn Lynn's checks and then there's like code review and then there's like out to a subset of users out to all his ERs.

And then like the further you go to the right, kind of the worse it is. So like this, they just have to be to discover the issue, right. And like, the worst one is like when people actually find it so it's, it's like the scale and the, the thing that like those teams are trying to do is shift the outcomes to the left. So like, figure out, okay, we didn't catch this thing, but how do we catch all the things of this class the next time?

And how do we catch something that was caused only. After the commit by tests, how do we change it so that it would have been caught before the commit? Or like how do we make sure that this, this whole pattern is impossible because the API doesn't allow you to do a bad thing? 

there are like things like security and privacy where like those mechanisms and various tricks. But then, for like a lot of just regular product development, individual teams have, like a lot of freedom with how data stuff. so some companies do have very strict policies on like test coverage and like component unit testing.

Like every component should be in a tested. We don't believe in that. because like in a lot of cases, bath tests actually slow you down more than my product issues. And they also, for example, like you do some internal refactoring of some component and it doesn't affect the behavior though, but a bunch of tests break because they assume.

That whatever the shape was, it doesn't change. And so that, that's like an example of a bad test. And so we try to minimize those and we try to make sure that our tests are mostly kind of end to end. We have a few custom frameworks around making that easier and like making those tests less flaky. but we're trying to make sure we test the actual behaviors that people experience and not like internal implementation details because we are really care that it's easy to change, that there's lot of plasticity in the product code and bad tests really hurt.

That was the dissident.

 **Michaela:** [00:36:27] So I did a study, probably, I thought about it yesterday, I think it's almost 10 years ago, and it was about testing and how eclipse, not only the IDE eclipse, but the whole ecosystems of plugins and plugins systems. Well, how people would test those modular systems. And at that time, a lot of the people were focusing and advocating for unit tests and integration tests and system tests.

And especially UI tests on the other hand, were often seen as . Bad thing. But over the years, especially the last few years, I see more and more people actually shifting their mindset again and now people advocate and implement more end-to-end tests. And I think it's because the better answer, many of the problems you've just described.

So do you see this shift also happening for testing at Facebook? Yeah. 

**Dan:** [00:37:14] I think like we even had the same problem with the react where we were, we're basically rewriting react at some point. that's already done. That was react 16, pretty much almost fully backwards compatible rewrite, which is like not, not very common.

but, We had a bunch of tests that were testing internal modules. So like one, problem is like when we talk about unit tests, then people have very strong opinions, but what is even the unit like that's such a meaningless term. Like you can say anything is again that, so like is reacts itself a unit or like is one more one file in react a unit or like a group of files?

I don't know. And so, but what we found is that. If listen to this rewrite, we, like we actually had to replace most of the implementation completely. So it was like written from scratch, entirely different architecture internally. And so. That's that were written against specific files, and it was like testing the internal API of that module.

They were useless because they didn't actually correspond to anything that the user would see. And also, if you read it like three years later, you're like, okay, I understand what this test is destined for in terms of this module, but Why is this the behavior? Like what does it, what is, what is the problem it was trying to solve?

Why was this behavior added? And so you still have to find in my good Blaine, here's the political events that added this test and this behavior and here's the actual issue was trying to solve. And so the problem is like maybe there's another solution to this issue.

But even if you solve it in a different way, that test won't tell you that. and so we had to rewrite a bunch of tests to only use public API, which, like in many cases just look like the original reports that like reported the issue. They had examples. Here's the thing that's broken. And so we turned that into a test.

And so now we know that. Whatever the solution we have, if we change it to some other equivalent solution that also solves this problem, that task will still pass. And that's. Let, like, that's our aim is to be able to, to throw away the implementation, completely rewrite it and still have the test Fasten.

Or another thing we do sometimes is we have two copies of the implementation. So, and that's also what we did at Facebook. We were doing with these branches. like not, we don't use long in branches. We use branches on the for like just. Just to get something reviewed like 300 lines, but then they merge it.

And so we, we rely extensively on feature flex, the enable and disable functionality or the switch between different implementations. So we might have like some module version one and some . What's your version two you checked in. And we have a dynamic chat that says like, if it's like maybe it's out to like 1% of users and then 50% of users, and we'll see if there are any progressions and metrics.

And then when we're confident that the fix actually works and it doesn't make anything worse, then we'll switch it over to 100% and delete the ultimate limitation. But the one, the tasks to. To be able to test both at the same time. So that's why like we try to not include implementation details in, in this tests.

**Michaela:** [00:40:31] Yeah. So it's really about writing robust tests that are, well, as you said, implementation independent. Yeah, I really like that. so one of the other things I wanted to talk with you about is your new side project, because you started something, it's called just Java script. Right? And it's an email sequence, at least that's my latest information.

And I'm actually subscribed to this email sequence, and this little email course is directed at people that have JavaScript knowledge but aren't feeling super confident with it. And so the emails have information about fundamentals of the language and you help people correct some of the misunderstandings they have about how Java script actually works.

Well, I, I find this project really fascinating because it serves a niche in a market that isn't saturated right now. For example, also on Twitter, somebody asks, how do you fill gaps and holes in your knowledge when you're no longer a beginner, but you haven't quite reached the intermediate stage? So I'm reading her comment right now.

she says there are so few resources aimed at that level. Well, and I think that just JavaScript is somehow an answer to that need, right? So there are tons of resources out there for starting a Java script or I don't languages. And they tell you, for example, what is the very able and how to assign something.

And so very basic things. And then when you are moving on to more advanced topics, there isn't, there isn't so much information anymore. And it's really hard to get this very deep understanding. There was also another person on Twitter asking, for example, what are some of the architectural patterns that you should use for react?

Well, react isn't a Java script, but it highlights the same need and information need about answers to question that are not easily found on blog posts or somewhere else on the internet. So is that exactly what you want to do? Fill those holes for intermediate developers.

**Dan:** [00:42:24] Yeah, that's pretty much how I described it.

There's like a few different ways. The pitcher, so like one way to pitch it is that indeed there is a lot of. Beginner resources, that are like, oversimplifying things because they, they want to kind of get to, like excited about the language.

They want to kinda get it started. So they, the charter, trying to make it a bit simpler than it really is. And then there is a lot of misleading there. It's, it's sad. Like if I tweeted, then people would be like, wait, what? Why don't you fix it? Well, that's what I'm trying to do, right? So there's a lot of misleading information.

If you just read like stack overflow questions about JavaScript, like every time I read them, I just get really sad because it's, there is so much wrong info, and I'm not saying this to promote my chorus, but like, just watch out if you're reading psycho Ruffo. Unfortunately, it's like questions from 2007 when like

It was a wild West in JavaScript. And a lot of answers are either misinformed or they're just not, not the way to do things. It's just they happen to work by accident. and it's, it's just so much work. Like I, I just give up, like I do have like moderator privileges on stack overflow, so I can actually edit some of those, but I just give up every time I look at those, cause it's, it's just so bad.

And so there are some high quality resources for like advanced developers. but I feel like, yeah, there, there is a gap and, Like, I imagine my target audience as a, like a person who has maybe just graduated from a code in bootcamp and they were taught, Java script in three weeks, react in three weeks, no JS in three weeks.

And they're like, okay, now you're ready for a fun and job. And maybe it, like, they, they do have some knowledge, obviously, if they are given a Kobe's and the relative, the scope task, they would probably be able to complete it and figure it out, but some guidance or mentorship. but the thing is, if they don't have a very strong mental model of how the code works,  they probably do have is like a mental model that's off in a few places.

That's like not entirely correct. it's just like, if you. Add more things to your shaky foundation. Like everything kind of falls apart. And I see this a lot with react where people like, I don't want to send react. And if you if you keep asking them, okay, well what is the problem you run into that are like, Oh, this thing doesn't behave as I expect.

Like this thing does not react. This thing is JavaScript. And they will sometimes say, Oh, react is just JavaScript. And that's. It's kind of annoying too. Like I can see how this can be seen as like demeaning and kinda, if you struggle with JavaScript and you're told, Oh, it's just always going well that that wasn't helpful at all.

Like, that's actually like really, really annoying to hear. but I, I still wanted to use that name to kind of reclaim it for, yeah, it is a bit.  confusing if you come from a different language or if you were taught in a way that doesn't actually match how JavaScript works, but this is something we can fix because it's a, it's actually not.

That's complicated. Is it just you need the ride structure. and I think I'm, I'm taking some liberties with this course. So it's, it's really opinionated, not in terms of like what features they use, but more in terms of how I presented. I put a lot of, a kind of emphasis on the idea for a mental model.

So  when you read the code. I don't, I just wanted to understand things in theory, but I want you to kind of feel the go to like, to see the same connections that an experienced developer sees when they read the code and to kind of operate them in the same way that, Like can experience person would operate. And so the focus of the course is really to, to help you kind of see this mental models that are inside like an expert's had, but they're. Opaque to you. And so that my, my job is to extract them and to, to kind of help you see them. And the first form with like emails is just benefit proof of concept.

But I want to make it a lot more interactive where you actually like interact with those mental models as like things you can touch and kind of play with, and get a sense of, Oh, so here is what JavaScript is really like in the conceptual sense. 

**Michaela:** [00:46:46] Yeah. That sounds really fascinating. I mean, I have so many questions now popping up in my head that I want to ask you.

so let's start with one of the last things that you just said, which is you want people to be able to touch the thing, which creates a very visual picture of your course. In my head, and one of the first emails, you talked about boxes and you ask if I ever thought about the variable as a box, which I never thought about it like a box, but somehow that stuck with me.

So now I'm thinking, how can a variable be a box. And, if it is, how can you move it? What would be the properties of that box, right? And yeah, and do you do with the box and things like that. So will there be some visual aid for the course? Will there be a screen, for example, and will I see things and will I be able to interact with those?

And what will be the visual way for me to learn about Chavez crypt? Or what else did you mean by interaction. 

**Dan:** [00:47:34] Yeah. So the, the funny thing is, we're actually not going to use boxes. so a lot of people were Tod boxes and like universities and stuff for those could do dude have like a classic computer science education or like some courses also do that.

but I've made a explicit decision to kind of do it. Completely differently. And, some people are not happy about it, especially like people with like 15 years of experience. so they are the ones who I messaged and they, Oh, this is a completely wrong way to teach people. Like whatever. I 

**Michaela:** [00:48:03] like that.

I think that if people are, you know, opposed to it, then your drinks and things like that. Yeah. 

**Dan:** [00:48:10] It is controversial, but I. I'm going to see, I think there is some sense in what I'm teaching so. Yeah. So there is a, in the current kind of provoke concept stage, there's, like there's pictures and there's animations.

So Maggie Appleton is a co creator of the course, and she's a, as soon as an illustrator. So we meet with her and like, we sketch things out together and she, she makes those Voges animations and illustrations for the chorus. so it is pretty visual in many ways.

 so in the, in this first situation is just like, animations and, , diagram exercises. But I really envision it as a much more interactive thing in the future. So I'd like to to move the exercises into the lessons, which she can't really do with emails, but you could do with web pages. So I'd like to them to be a part of the lessons rather than something at the end of the lessons. And I like them to actually be interactive in the sense that you don't like just look at the animation, but you actually like you drag things, like you kind of connect them together.

And there's this translation layer where like it says, here's the code, do the thing. To this, to this life thing, like do whatever the code says, and you're, you're, Oh, okay, here's, here's what assignment operated. Does it like the next day things together. I like, here's what this thing does. And so it's like.

It's really like translate into learn in way to translate from code to this visual environment and then back and eventually get on need the visual environment because it's, you just understand the mechanics and the mechanics become like a part of your mental model. so that's, that's kind of what I'm going, I don't know.

That's it. That's going to work out, but I hope so. 

**Michaela:** [00:49:57] Yeah, it really fascinating, especially when you said that you present knowledge to somebody that isn't as experienced, that normally only a very experienced developer has. Right? So I love teaching and right now I'm giving code review workshops that I totally enjoy, but I also taught at university and community college.

And even though I have been happy teaching for several years of my life, I know that the most challenging thing is to extract. Tactic knowledge, so knowledge that they are really, really familiar with. And then to, you know, put it. Yeah. Put yourself in the shoes of a beginner and help them to understand it.

And I think, as you said at the beginning, some of the JavaScript courses I abstracting things, they leave concepts out or hide something or they're not explaining everything because they're aimed at making it easy for the person to start understanding. And I also recall the time at school. Well, I actually graduated from art school before I started to study computer science.

And the first six months they were really difficult because I didn't have any mental models about computers. And you know, how programming works and how things interact with each other. And it really took me a very long time until, yeah. Things fell into places, right. And so before I, I understood what's actually going on.

I was just doing the exercises or without understanding them. Do you know what I mean? Like for example, I was writing Java methods without understanding why it's working. I just did. And it worked. And I was bustled and you know, piece by piece, it started clicking. But right now, I wouldn't be able to, for example, reverse engineered that process.

So it would be hard to be that person again and, and to know what I actually struggled with. So how, how do you do that? How do you extract your tactic. Knowledge. And how do you know which holds people half. and which concepts they may be misunderstood and, how do you know how to correct their mental models?

**Dan:** [00:51:54] So I wouldn't say that I really have the answers. I think like, because I didn't have any formal kind of teaching experiences, I, I feel like I'm qualified to do it, but I still try to do it. I'm kind of, I do my best. I know what people don't know just from experience.

So I, I try to. Kind of think of knowledge as a tree of ideas. And, there's like, with dependencies between them. So like, do you understand this? To really understand this, you have to understand like, this and this and this. And so, like I, I have this kind of mental, like, mental model of mental models, a meta mental model of what, like the tree of JavaScript knowledge is like.

with this course, I kind of lean back on the fact that I expect the person to kind of know JavaScript already, so I can take shortcuts and like, I can use a function before I really explained, like, I don't have a chapter on the functions yet, but I kind of use them in simple ways.

As semen, that the person kind of knows what a function does. but like if I had to design this course for a complete beginner, it would have been like, designed very differently. And that's a lot harder. Like, I'm not qualified to do that. Yeah, definitely. but one thing that, that, that I've noticed is that,

like, you need to really let go for assumptions. this is very similar to kind of profile in code when, you're trying to figure out why the code is slow and you think it's like, Oh, I need to optimize this, this, and this. But if you run it through the profiler, it's actually somewhere you did not expect.

Like that's the bottleneck. And I think with learning, it's kind of similar in that you might think that here are the things that the person is understands, but there's actually something that you completely missed and like it may be very fundamental. So I found that. Every time I thought, Oh, this is obvious.

Everyone knows that you test it on people. No, they don't. 

That's why I have this like exercises and like diagrams, so I can get a sense of did people get like whatever I was trying to show, like can they make those connections themselves? And like if, if it seems like it's working, then I'll keep building on top of that.

And that's also why it's been amazing to work with Maggie. Cause so she's an illustrator and she doesn't have like a JavaScript background.

She does a little bit of JavaScript, like to the point that. Like shadows, write code. but she doesn't have a deep knowledge. So it's been super helpful to kind of bounce ideas off of her and kind of ask like, what do you think this go does? And then see, Oh, this is your mental model 

 one way I've been thinking about it this, especially for people who already kind of know stuff, it's like, it's a, it was like a decision tree where it's like they learn all these concepts and then.

There's like, there are forks in the road where you can misunderstand something. In my one of three ways, like it's usually not many ways to misunderstand something. It's like maybe they misunderstood this, maybe this, or maybe this, or maybe they're right. And so for each of those forks, again, to have come to different combinations of like incorrect understanding.

And then if you're at least aware of like each of those forks and each like how those misunderstanding will manifest themselves. So you can test them. So you can make, like, it can make an exercise that, that shows whether the person understands that particular thing or not. And then if you run it on like enough people, you just gain enough insights to see where those forks are.

And then those are the things they're supposed to teach. 

**Michaela:** [00:55:20] Yeah. Yeah. I really like your meta mental model of mental models, so I think you are really onto something here, and I'm definitely looking forward to reading more of that email course. And also. I'm looking forward to the course that will come out of that prototype.

So one of the last thing I wanted to ask you, if your thoughts on improving diversity and inclusion in tech, I know we are switching gears completely right at the end, but I would like to know, what would you advise to somebody that wants to do some impactful actions to make tech more inclusive and diverse?

What do you think? 

**Dan:** [00:55:55] So I think if, that person Isn't the pirates of like minoritized groups that like, we want to include them, they can step away and try to amplify the voices of those people who are part of those groups because, and that's actually something I haven't been very good at.

I think in a lot of cases, It's tempting to kinda like , if you're like white male, you're gonna want to see yourself as a good guy. Like, Oh, I'm gonna, I'm gonna help all those people or whatever. But really it's just your presence and your, taken up of the resources that.

Like makes it more difficult for other people who don't have your network yet. , we don't rely on your connections, who don't have the kind of support  in terms of hiring where we hire people who we know, and in many cases, we know people who we know, like socially and we know people socially who kind of.

Like we do things together with, so in many cases, they kind of look like us. Or, they're like part of connections. that is, like this is creating this effect where,  if you start with some advantage, then it has this cumulative effect. So, I'm not saying like that every guys would like, disappear from the internet.

That's not what I'm saying. but I think that is some misguided, but if knew that, the best thing you can do is like, do something. Whereas I think in, in some cases, it's like, it's more about stepping away and, given other people the spotlight that they deserve and, helping them kind of make connections with each other and, figuring out where it is that he, that you reinforce the existing structures and how you can like, avoid doing that.

**Michaela:** [00:57:35] Yeah. Yeah. I like that. I like, especially the last one, which is, again, it's a little bit about how we think about things, right? Extracting and reverse engineering, what's actually going on. And I think that especially what you said about amplifying, for example, is something that can be done quite easily and could have a big effect.

So it's just something that we haven't covered in that interview that you think we should 

**Dan:** [00:57:58] touch on. I dunno. There's been so, so many topics. I feel like. I discovered there was gonna fall in my mind. I don't know unless there's something that you're so curious about that you want to talk about. Yeah, 

**Michaela:** [00:58:13] no.

Yeah, you're right. We've covered quite a big, well, one thing that I think many listeners would be interested in is your opinion on the future of reactive Redux, and we haven't really touched ad, so maybe if you want to cover that for a few minutes, what do you think? Where is everything heading towards?

To. 

**Dan:** [00:58:30] Yeah. Well, I, I don't have a magic crystal ball, so I can't really answer that. I, I always find it confusing when people ask me, like, what is the feature of, ah, I don't even know if I'm like, we're going to be alive tomorrow, so how can I know the future? But I think people underestimate how, Unpredictable things are, like, I would, I guess I would be confused if somebody was confident. Well, was going to happen. But I think like for react where we've tried to be like as transparent as we can be about what are we building and why.

So there's like, if you're curious about those things, and I always go to react blog. So that's, we actually as the.org/blog, we try to post about all big updates or like upcoming features . I guess the big one is, building support for concurrency interreact and that, that means a lot of things and it's still not quite ready.

So we don't talk about it a lot, but there's a few talks from Rhea County that, again, you can find on the blog at the talk about this. but I think the overall kind of big picture of what we're trying to do is, like the big idea of reactors. That here you want to describe things declaratively and, with the full power of the language that he gives in. And I think in that sense, react has been hugely successful because it's not just react like the adoption for ads itself or like even the react native. But, all the next generation libraries like Swift UI in iOS and Jetpack compose for Android.

they're following not exactly the same approach, but they embraced this declarative, user interfaces, which was a very controversial, like five years ago. So I think react has largely succeeded at that. And the thing that also differentiates react from other libraries, like, I don't, want to name, them, So that people , don't find me on Twitter, but I think an intentional design choice of react is that we embrace JavaScript and we embrace the host language in the sense that if you want to have dynamic logic, in Java script saying like, if this condition then show this thing, or like operate on UI as a value, as a first class citizen and say, here's like three things I want to render, like map them and like use the expressiveness of Java script to do that. And we let you do that and we don't just let you, this is the way to use react. We don't have like a separate template language that is like less expressive. So I think that's another choice that react makes, which some people agree with, some people disagree with.

but you can see that like Swift UI and compose are also making that choice. So maybe there is something there. So I think that those are the areas in which react has been successful. But,  one downside of this paradigm is that it's very developer centric. So , like sometimes, when a user goes from one page to another page, you don't want to immediately switch it because it's a bit Chiron to like see a blank screen for a split second and see things kind of fill up.

And. It's just like, it's not very pleasant. it might be easier to wait a little bit, , for the user so that it's not as Jerin, but the react program and the model kind of, not just you two always express changes as like, what should be on the screen at this moment. And so it's, it doesn't really give you any control over time.

And so you end up flushing changes as soon as they happen and does not always the best experience. And this is also related to animations, like sometimes. You click on something, you want to see something different, but you want to like the previous thing to kind of animate gracefully before you transition that, because the react model is like, if this show this, otherwise show that, then it has to kind of jump and implement an animations is a bit annoying and it doesn't match the paradigm exactly.

So I think that's like the next stage of react is just giving him more control over time and maybe not even necessarily given the developer Mark control, but, being more considerate of when we show things on the screen and why and how does that, match the human computer interaction research that shows us that.

So in too many things, like too many things, flashing is bad. Like you want to kind of batch them together and, you want , try to use animations where appropriate. And, how do we make the library, of still keep the declarative paradigm? but. Operate on time in a way that matches how humans perceive time and how to make them like have a nice experience.

He's in their product. And so that's what this like work on concurrency and react is all about. 

**Michaela:** [01:03:17] Okay. Yeah, it sounds really exciting and, and it also answers one of the questions people wanted me to ask you, which is when not to use react. So yeah, your answer has been very insightful. That actually brings us to the end of the show.

I really want to thank you for taking the time to talking with me about so many different topics and sharing your ideas and your thoughts. Then, thank you so much for being on my show. 

**Dan:** [01:03:41] Thank you for having me here. you asked really good questions, so I appreciate that. Yeah, that was a, that was a really nice interview.

**Michaela:** [01:03:47] Yeah. Thank you. Thank you so much. Bye. Bye.

 