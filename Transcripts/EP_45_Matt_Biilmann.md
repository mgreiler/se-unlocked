---
episode: "Episode 45 with Matt Biilmann"
permalink: /bootstrapping-netlify
status: publish
type: transcript
---

**Michaela:** [00:00:00] Hello, and welcome to the Software Engineering Unlocked 
podcast. I'm your host, Dr. McKayla, and today I have the pleasure to talk to 
Matt Biilmann. The CEO and co-founder of Netlify.

But before I start, I want to tell you more about CodeSubmit - the best take-home 
assignment platform to streamline your tech recruiting! Yes, exactly. This 
amazing start-up is back sponsoring the podcast. And over the last month, they 
introduced a lot of new exciting features such as live coding with the full 
working IDE running directly in your browser.
CodeSubmit makes it really easy to recruit and hire amazing tech talent. They 
support 64 different languages and frameworks, and integrate seamlessly with git. 
Beginning of the year, when I was hiring engineers for a start-up, I used their 
tool during the interview process for all the candidates and I was extremely 
satisfied. 
Their mission: real tasks, not brainteasers, resonates a lot with me. So, I 
cannot recommend CodeSubmit enough. Please check them out at codesubmit.io. 
That is codesubmit.io.

But now, back to Matt. Matt is the CEO and co-founder of Netlify, the modern 
platform for high-performance websites and apps. 
Netlify has around 150 employees, but that's not all. Matt also coined the term 
JAMstack, which stands for JavaScript, APIs and Markup. Today, JAMstack is even 
more.
It stands for collection of technologies and languages, including web oriented 
databases, frameworks like Nuxt and NextJS, and even framework-less approaches. 
So I'm super super thrilled to have Matt here with me today to talk about his 
experience founding and running Netlify and also JAMstack and software engineering 
practices at Netlify. So yeah, I'm super super thrill that you're here. 
Thank you so much for joining me today. 

**Matt:**  [00:01:50] Thank you for having me. 

**Michaela:**  [00:01:51] Yeah, I'm really really excited. So how is that? I
looked a little bit like a research to you obviously a little bit. And so I saw 
that it's around, you know, seven, eight years ago that you, that you created 
or you founded Netlify. How was that?
Is that, was that you have an idea and you do it, or what was the process like?

**Matt:**  [00:02:14] It was a long, it was a long process that started way 
before Netlify itself. So I, I'm originally from Denmark, but spent seven years 
living in Spain, in Madrid, where I worked as CTO for a company that built 
websites for small to medium businesses, but at a very large scale.
So we would build something like a hundred websites a week, tens of thousands of 
sites of in total, right? And I led the whole product and engineering or 
that built the platform that all the designers would do the design with, that 
all the clients with useful content management that powered every single website 
from brief to production.
And then, then I actually started a CMS startup in Madrid together with the 
founders of that Spanish start-up. Because we had just tried building sort of 
several iterations of this kind of developer platform in-house and we thought,
okay, we can build a cloud hosted multi-tenant version that other agencies
and other professionals can use to get a lot of the same efficiencies when 
they are building websites for their clients.
Anyway, that was sort of the first take on, like, how do you really remove all 
the friction for web developers in building, deploying, operating with properties. 
But it was built as a traditional like monolithic application, multi-tenant CMS 
with database and template engine and all of that.
And I came to the Bay Area and the whole tech scene here, working on that. 
But while working on that, I started getting this sense that even if it was 
a product that was, I was very proud of building had a lot of like early 
innovations in it that had serverless functions before that was the thing,
right? Like server side Javascript to running, in this case within the JV admin 
isolates and so on.
But I got the sense that the fundamental architecture of it, this monolithic 
approach where data, business logic, template language, front end code is all 
closely tied together was just not gonna be long-term the real, like the future 
architectures of the web. Yeah. I was looking a lot at what was happening in two 
different areas.
One was like the space of static site generators, like Jekyll and Middleman were 
at the time. And the other was the whole Node JS based ecosystem and Beaufort (??) 
was having, what was happening there in terms of the early built tools and task 
runners like Grunt and Gulp, but also the first sort of real for ease (??) into 
the whole world of single page application with originally tools like SproutCore, 
and later Ember, then Angular, React, all of that, right? 
And I got this sense that pretty soon as browsers really started maturing, it 
would make much more sense to have an architecture where you try to decouple 
the frontend web UI layer completely from the backend business logic layer. And 
the best backend business logic layer would logically split into all these 
different APIs and services where some of them, of course you own and you write, 
but a lot of them are other people's services, like Stripe, Algolia, or Twilio, 
and the like. 
And I also saw that if you could do that, you could sort of map that whole web 
UI layer, you could map the workflow around that pretty tightly into the git 
centric workflow that developers were already working on, where in work through 
pull request and merges and so on, right? Like it was much more straightforward 
to map that whole process on twist stateless UI layer, then mapping it onto 
both the UI layer and the whole business logic data layer that tends to require 
all these kind of migrations, and the settings, and so on. 
So I got the sense that that architectural approach would win out, but I could 
also see that there was just too many, too much friction standing in front of 
developers that wanted to go that direction and then actually like building, 
deploying and operating with properties like that. 
So I built a small MVP of like, what's the smallest thing I can build that sort 
of aims at addressing the workflow for those kind of web developers.
And the first MVP was this small service called BitBalloon, where in the very 
first version, you could drag a folder with your frontend onto bitballoon.com 
and it would immediately go live on a URL. 
And then I edit some CLI tooling and some API tooling around that. And quickly 
saw that it resonated with the right kind of early adopters in the frontend 
space and got very validated in the idea that this architectural shift was going 
to happen.
So at that point, I started to talking a lot to one of my best friends back from 
Denmark, who Chris was my co-founder today. He, we've known each other all the 
way back from high school, which is sadly a long long time ago by now. But while 
I spent seven years in Spain, he had built his own production company back in 
Denmark, specializing in like in very interactive, often video powered websites 
typically built in Flash for some of the largest brands in the world, won a bunch 
of international awards for its work there. And then sold that to a full at, 
to a full service agency where he became a partner and the chief digital officer. 
And I started talking a lot to him about this architectural shift and what it 
would mean if you could sort of pre-compile the whole UI and put it on a globally 
distributed network and then just talk to these different APIs and services. 
How we could really fundamentally solve a lot of the problems around global 
performance, around scalability, around reliability, around security, and even 
in the process, potentially really addressed developer proactivity. And all of 
these areas were where areas that he, like he, he knew from operating across 
like web properties from tons of different companies and running digital strategy 
for the sort of Walmarts of Scandinavian and the like, how big these problems 
were and how enhanced they were. 
Like how much worse the problems got as we also started having more and more 
people using mobile devices for the web and expecting a different kind of both 
pace and user experience.
But we could also just see again, how much friction there was if a team wanted 
to adopt this architecture, suddenly they had to stitch together like CI/CD 
with object storage, with CDNs, they had to figure out cache perching rules and 
its caching. They had to figure out how to connect to all these different APIs 
and services, and typically had to figure out triggering, rebuilds when content 
their data changed and so on. And there was just no viable tool chain for saying 
like, okay, we're going to do this, what do we do it with? So that became the 
core idea. We sat down and discussed and came up with form for Netlify and still 
the mission we're still working on, right?
Like how can we create a cloud platform for the collaborative work, where teams 
can really operate efficiently, where we can remove all the friction involved in 
going from pull requests to live code running in front of real users. 
And yeah, we started out just bootstrapping. The two of us.
Build on top of the product I had already built and turned it into Netlify 
launched on air, show Hacker News post in March 2015. And by the end of 2015, 
we're still just two people bootstrapping a company, but we are serving around 
a quarter billion web requests a month out of our homegrown CDN for customers.
Like we work in Sequoia Capital and the Malala Foundation, and was realizing at 
that point that, okay, now we need to raise capital, build a whole team around 
this and really accelerate. We've sell first round of venture capital in the 
start of 2016 and hired the first engineers in March 2016.
And then, and then it, of course, it's been a really fast paced growth since 
then. By now we've raised about 107 million dollars from top tier funds like 
Andreessen, and Kleiner Perkins, Menlo Ventures, EQT. We have onboarded more 
than 1.5 million developers onto our platform and sites are now like just, 
just the sites and web apps on our platform are reaching the close to 700 million 
unique visitors every month.
It, so, so yeah, it's been quite the ride so far. We only just getting started. 

**Michaela:**  [00:12:16] Yeah. Yeah. Mind blowing. Wow. Yeah. It's mind blowing. 
Yeah. And so for me this, you were really very very involved with the technology 
and you had like this vision where it's going to go and it also went there, right? 
So it was like spot on.
Do you feel like that you're still very connected to that?
Like, do you still feel like that you're so connected to technology or are you 
now more involved in, you know, you have to see overall? I am now a little bit 
more away from this technology side? And how is that for you? You've, for me now, 
how you explained it and how much passion I could really see that, right? 
I can imagine that you have also like this passion for the role that you have 
right now. So you're probably extremely business oriented and you know, all 
these funds and you know, like where to raise money and how to acquire a company 
and all of that. Are you still very technical? Do you feel like you're as 
technical as you have been before?

**Matt:**  [00:13:16] I'm obviously not as involved in building Netlify from 
writing code perspective like as I was, right? Like the first version of Netlify 
I built a CDN from the ground up and the CI/CD platform and the React UI 
that powered it and everything, right? Like, and now I typically don't like my 
working stage now doesn't involve writing code file product, right?
But a curious thing about my background is that while I've been programming as a 
hobby since I was 10 years old, I studied the musicology and cultural studies 
and was always more interested in how humans adopt ideas and make sense of the 
world and understand things. So I think some people are need to feel very 
hands-on with the code to feel that they are doing something.
I get a lot of joy also out of building the culture and the organization and the 
engine that can build things without me, right? And trying to understand both how, 
when we talk about something like the JAMstack emerging for example, and the 
shifts in technology. There's always a mixture happening of like the actual sets 
of technologies involved and the specific program languages, and APIs, and 
infrastructure evolutions that we're seeing.
But in the end, technology are, is adopted by humans learning about things and 
building things, right? And you can understand where technology is going, what 
will happen in an ecosystem? If you don't understand how humans adopt technology 
and why developers built with certain technologies at certain points in time and 
why you'll sometimes see technologies that are technically better loose out in 
the marketplace because their adoption path is harder, right? So for me, it, 
I've always been a very curious person and like to understand both sides of that 
spectrum, both the lower details of how does technology, like how does that 
technology work behind the scenes, but also the details of like, how does human 
beings approach it, and understand it, and build with it.
And of course, as I've been building this company, and as I am building it, 
the layer of where I operate, they are all have to keep shifting, right? Like 
in the beginning, I had to be the one who just sat down and wrote the code. And 
then I had to be part of a team that wrote the code. And then I had to be more 
of a take lead for that team and guide them in the right direction and so on. 
And now I have to build the right kind of organization and the right kind of 
organizational structure to allow our company to build the kind of product that 
we think we need to build. And that's in some cases also like requires finding 
the right partners to build it with in terms of investors, or ecosystem partners, 
or finding the right people to join our team and help build it.

**Michaela:**  [00:17:01] So, this is really really super interesting. Is it for 
you all about the people or is it also about the structures and how people are 
working together? Do you see it as a system? Or, you know, like, or is it 
self-forming, like is the company self-forming or do you give it some structure? 

**Matt:**  [00:17:20] No. No, we, you, I believe in trying to bring some structure 
along the way. I think both me and Chris have always thought that intentionally 
building structure and organization is really important for building a company 
that can scale to become a really large company, right? Like I think, if you try 
to ignore the structure, you will hit a point where everything starts falling 
apart.
And it's very easy to hit points along the way (*laugh*) that feels like that's 
happening. 
Of course, you're always a bit riding on a rocket that's slightly out of control, 
right? But I think culture and structure and values are really important for how 
a company functions. And then of course, like you can never replace the, like, 
it's in the end, it comes down to actual people doing stuff, right? But the 
structure is important and it's important to be intentional about it. I think 
we've seen some companies that tries to build completely like say they built 
completely flat structures without in any kind of structure to it. And that just 
means that as a leader, you're not taking any intentional decisions around the 
structure because your team is still gonna have people that have more facility (??) 
than other people.
And they're still gonna have, it's just gonna happen by politics and sort of 
maneuvering rather than by any intentional process of like how should the 
structure be.  

**Michaela:**  [00:18:41] Do you see like a parallel between like architecture, 
like software architecture and technical debt and structures of companies like 
where you say, well, we try to build the best system with the information that 
we have right now. Obviously also looking into the future, but then, you know, 
things evolve, things change, so we actually have to go back and change the 
architecture or change, reverse some decisions, you know? Remove some technical 
debt? Do you see the same happens in company, in your company structure? 
Or do you feel like, oh, this is for what we have foreseen, but now we actually 
have to restructure and refined or redefine ourselves? 

**Matt:**  [00:19:23] Yeah. You absolutely see that happening. And of course it 
could be a useful metaphor to compare like your company through to the machine, 
building the thing and think of it as an architecture in that point.
Just also have to remember that in the end, the pieces of the machine, so not 
lines of codes, that are predictable. They are people with goals and dreams and 
carrier ambitions and interpersonal characteristics. So you have to be aware of 
both sides of it. 

**Michaela:**  [00:19:59] So you're what you're saying is that technical debt 
is sort of peanuts, right? (*laugh*) That complicated for you, right? 

**Matt:**  [00:20:14] I just, it's a lot easier to deal with technology. 
It's a lot more predictable in the end than people are. But in the same way, 
it can also be a lot more fun to deal with human beings. 

**Michaela:**  [00:20:21] Yeah, obviously. Yeah. Yeah. I'm super impressed. 
Like I can't imagine how much personal growth has to happen on a way from, you 
know, like bootstrapping something, then getting investors, you know, scaling, 
probably if you get investors, you normally scale really fast, really quickly.
And yeah. So that sounds super awesome. 

**Matt:**  [00:20:45] Yeah. And it's also, I mean, it's also a choice you take 
when you go and raise venture capital that, raising venture capital is only 
one way of building a business, right? Like the many other approaches to build 
a business. In our case, we felt that there was also the kind of market 
opportunity, right?
Because we really, from the get-go belief that there was a real opportunity to 
shape how the future of the web is going to be built and how it's going to 
function. But we could also see that making that big of an impact and getting 
there in time and so on. There was not something we could have done if we had 
grown just organically based on our revenue, right? Like, so that's why we went 
out and raised funds to be able to scale and grow much faster than we would be 
able to do organically, right? And that, of course always didn't have the 
trade-off of like all the challenges you get when you are trying to scale an 
organization very fast.
And it has like, you have to know what you're going into as a founder also, right? 
Like, it's, of course, it's a learning curve and you have to be very okay 
with continuously taking things that you saw as core to your role, like writing 
the code, building the technology. And then have other people come in and do them 
instead of you and step away from it, right? But if you do that, you'll also 
learn very quickly along the way that the more like, that no matter how much of 
your job you seem to delegate it away, you only get more busy somehow. (*laugh*)

**Michaela:**  [00:22:31] (*laugh*) Yeah. Yeah. So one thing that would really 
interested me is like you said, you wrote this little first version MVP of Netlify.
And a lot of people adopted it. So it seems like you didn't really have to 
convince people about this solution or that there is a problem because sometimes 
like founders, it's hard, right? You think like, oh, I have this idea, and then, 
is it too early? Do I have to convince people to have to explain it better? Do 
you have like to, do you think that this is the right mindset or should people 
step away from something like where we have to tweak one sentence to be really 
powerful and express like the pitch, right? Is that really so important? Or 
should we read our focus, our energy on finding the thing that people actually 
want even if you write a sloppy (*laugh*) sentence about it, you know what I 
mean? (*laugh*)

**Matt:**  [00:23:25] Yeah. I think, I think it, it's never completely one or 
the other. I think, you have to in like initially for example, the mental model 
we had around adoption was that for these kind of technology products, if you're 
trying to build something that's in that the future of how things will be built, 
you would expect it to sort of grow in concentric circles where you sort of have 
these very early adopter technologies that are constantly looking to broaden 
their horizon, then find new things that work and so on, right? And you want 
this kind of product to resonate with them first, right? Like in the initial 
stages of this product, you wouldn't expect someone who was at like day to day 
working in on a long enterprise company, very focused on solving like big picture 
business problems insight that for the existing technologies to even be 
interested in your product, right? 
Like it's just not time, but you would expect like for a product like ours and 
early adopter of JavaScript frameworks or site generators to get interested.
And then ideally like there's two ways, essentially two different paths to 
building product companies, right? Like one of them is product-led growth and 
the other is sales or marketing-led growth. And not, there's not like one way 
is the right way for some products. If you have a product that requires in a 
whole organization to adopted horizontally before it really adds value, right? 
Like you can't build a product-led motion around that. You have to go build a 
sales-led motion where you first go and talk to executives and companies and 
figure out the needs and then solve their needs with a product. But if you have 
a product that can both be really useful to an individual engineer, into a small 
teams of engineer, to a larger team of engineers, into a whole organization, 
then you have the opportunity of building like a product-led growth moment. 
Motion. Where, the way you get into businesses is by individual users first 
adopting the product, and then, then it spreads from there, right? And we saw 
the opportunity to build that kind of company. And when you built that, then it 
can't be like the core sale doesn't depend that much at first, unlike nailing 
the phrase on your marketing site or something like that. It comes on nailing 
the onboarding experience for how fast can you get someone to land on your website 
and then be inside the product, doing something where they have an a-ha moment 
of why, like, why is this product gonna be useful to us? And for us, there was 
really about like landing on netlify.com and then having a web property running 
on a custom domain in a shorter time as possible, right? Like that was sort of 
the first iteration of the a-ha moment, right? 
And then knowing that maybe in 30 seconds, or a minute or something, right? 
You had gone from nothing to having a globally distributed website running on 
a custom domain with a CI/CD pipeline plug directly into git, right? If we could 
just make that motion, like something you could do in 30 seconds, or minutes, 
or something like that, then we would drive that feeling of like, wow, this is 
another generation of tooling. This is just so different from how the world 
looked before and then build excitement with developers. But then in parallel 
with that, we will also positioning ourselves in the midst of like an 
architectural change of how are we going to build the web in the future.
And at the time when we started, there was just a lot of different technologies 
that was making that happened. There was, as I mentioned, static site generators. 
There were single page applications. There was a lot of talk of the API economy, 
some talk around like the programmable web, and so on. But there was no name for 
this architecture.
And that was something that Chris, my co-founder, immediately saw from his 
background. Like we need, if this is going to happen, we need a name for this 
category and this architecture, because otherwise, again, all of this happens 
because humans adopt the technology and humans goes in the direction and if you 
can't give people the vocabulary to talk about what they're doing, it becomes 
very hard for that idea to spread between groups and teams and people, right? 
So that's why we ended up coining the term JAMstack and it happened sort of in 
a very collaborative process with different people in the industry and so on. 
And the term started taking off because it was needed, right? 
Because it gave me an nomenclature to start talking about things that before 
were seen as just separate movements, right? Like, okay this. Something's 
happening about the architecture we use for cell phones, talking to APIs, there's 
something happening or how this whole world of web API is exploding.
There's something happening around single page applications and something else 
happening around CDNs and site generators and so on. And suddenly we had a 
nomenclature to say, oh, it's an architectural shift. It's a shift to watch the 
JAMstack. And that was really important to build the other part of like on the 
one hand, the individual product story and the developer story of like finding 
this product and instantly getting an a-ha moment and then connecting it to a 
broader story around like a new architecture for the web emerging and the 
possibilities that would entail and how not just individual developers, but 
large organizations could benefit from that change. So both sides are important. 
But in the end, if you're building a product-led growth company, you have to be 
really obsessive about the product itself and how that product attracts and 
convinces users to work with it. 

**Michaela:**  [00:30:08] Yeah. The funny thing is that when you described the 
story of, you know, how a developer, you know, sees your side and tries it out. 
This is exactly how I felt when I tried it out. I was not an early adopter 
though, right. I tried it out somewhere last year, but, it wasn't exactly like 
this. It was like, oh, I have to deploy this website. And I want to do it quick. 
And you know, like, let's try that out, right? 
Everybody is already on it. I'm like the late late person (*laugh*) too late for 
everything. But I went to it, right? And obviously at that point it was fully 
baked, right? Fully in, but, you know, I was there and was like, wow.
Well, it's running, right? Like I was like, and as you said, right? This is like 
you push and then it's there. I exactly felt what you were saying, but it was like 
last year.
How was Netlify when you say, well, let's go five years back. How was the 
experience? Was it similar? Like at that point, would you say it was similar? 

**Matt:**  [00:31:10] Yeah. So, the expense involved in, and it will continue 
evolve as we also go for, broadening the experience and telling it different, 
like as a large and larger story through the product, right? So the very first 
story you would see was in BitBalloon, the predecessor to Netlify where you would 
land on a website that just immediately on the front page head (??), like a drop 
zone saying drag your web folder here. And there would also be a little download 
link where if you didn't have a website handy, you could download one and drop 
it there, right? And then you could just drop aside onto bitballoon.com without 
even signing up or anything. 
And it, you didn't need to zip the files first or anything. 
You just drag the actual folder onto a bitballoon.com, and boom. Now you would 
be live. We still have that on, if you go to app.netlify.com/drop, you'll get 
the same kind of experience that mimics, like what the very first version was 
like, of course, designed by me and not by actual designers (*laugh*), like it 
looks like today. So that was like the first simplest motion we could do, right? 
And then, the next step was really to start, like after we had, after I had built 
out that initial version of just getting a site live and getting a custom domain 
connected to it, getting SSL set up and so on.  
Then it was really the question of okay, this is fine if you're really just one 
developer. By yourself. Manually deploying. And we added a CLI where you could do 
the same from like writing, at first BitBalloon, and then later just Netlify 
deploy, and immediately from the command line deploy a folder, right? That's fine 
if you're really just one individual working. As soon as you're at team of people, 
that's not very useful. Like you can't just random, you have people deploy manually 
at different time without structure around. And people get their structure from 
GitHub or GitLab or Bitbucket. That's where developers collaborate on opening new 
pull requests and building new features. So. The next iteration of that on Netlify 
was really saying, instead of focusing on you deploying manually from a folder 
that solves the whole into problem of you working in a git provider and getting 
that live.
So the next moment really became that flow of like coming. Tell us your git 
repository and we'll try to even guess what tool or framework you're using, and 
just say, okay, and now you're done, right? Like now you have something you live. 
And now of course, with, without acquisition of FeaturePeek and that whole journey, 
we are going even deeper into that space of like, this is not just for single 
developer building on their own. Like real projects always built by teams with 
lots of different stakeholders and with several developers and one part of the 
processes is writing the code. But another part of that whole process is that 
for every release, you have some feedback cycle where you have back and forth 
with product managers, or designers, or other developers, or other stakeholders 
before you take something live. And now we're really sort of expanding that whole 
experience to include that process and to show how frictionless we can make. 
The process of a team actually building releases together and taking them to the world. 

**Michaela:**  [00:35:12] So with this acquisition, somehow you have like this 
deploy previews feature.
You know, my favorite thing are code reviews. Is that something that you think 
is part of the programming part or is it part of deploy? Is it part of something 
that should be, should code reviews be somewhere in that picture or how do you 
see that? 

**Matt:**  [00:34:36] I mean, code reviews are really important, but then there's 
also the step ahead that's like viewing the outcome of your current code, right? 
Like being able to just open a pull request and having that pull request running 
in the full production environment exactly as it would look like if you merge, 
that's really like, it doesn't replace the code review, right? 
Like the developers should still work on the code review tools to make sure that 
the quality of the code behind that is up to scratch and so on, right? But it does 
make the preview, especially from QA testers, product managers to designers and 
marketeers to content editors or anyone else that's involved that will want a 
preview what the output looks like. It makes that process in much simpler, right? 
And what we were seeing, like we've, we launched deploy previews in 2016, a long time ago, and we've of course been very big consumers of that whole workflow 
internally, ever since then app.netlify.com runs on Netlify, all of our web 
properties up and run on Netlify and that process of deploy preview is completely 
essential to how our web teams work. We're constantly sharing URLs and so on. 
But the one thing we saw also when talking to clients and so on, was that when 
you share that URL, then the feedback cycle spec to the developers that happens 
all over the place. Some of it happens you're shared in Slack and there's 
feedback in Slack and or people open issues in GitHub or in JIRA, or they will 
paste the screenshots into documents and send them back and forth for, add the 
message attachments, and for developers like the process of that is as fragmented 
as the process of code reviews was before tools like GitHub and GitLab integrated 
into the workflow, right? Like before that happened, like there was no, that you, 
you would've sometimes have specific tools for code review, but mostly it would 
be processes of sending back and forth emails around the code, or simply just 
having to sit down at a laptop together, or at this top back of the time, and 
look at the code and talk through it, right? And GitHub with the pull request 
functionality really gave that home for code reviews, right? Like in the game 
of place where now you no longer have to wonder, like where is it happening? 
And people commenting in all kind of places and so on, right? So, what we're 
trying to do with collaborative deploy previews is in a similar way to give it 
a home for the feedback, not on the, on the input, which is the code, but on 
the output, which is the result.
And make sure also that since every deployed preview is a different URL, we 
don't, we didn't want to have a system where every deploy preview now has its 
own, like, you have to know it exists and go there and look at the feedback in 
order to take part in that process because like, we had some initial prototypes 
integrating with tools like that, and it just attracted from the process because 
now developers apart from checking the pull request to end a Slack messages and 
their emails also had to continuously try to figure out is people, are people 
now also commenting on the deployed preview URL. So it's really important to 
make each deploy preview URL at checkpoint that makes information flow into their 
original places.
So feedback that stakeholders make on the deploy preview will flow back into the 
pull requests. They'll take part in the comments there, or they can open tickets 
in whatever project tracking software you're using relate to GitHub or linear 
Clubhouse or the like. And that was really important for us, right? But again, 
was this sense of like, now when a developer shares that deployed preview URL, 
they are also sharing how to give feedback and how that whole process operates. 
And we hope that can really, as I said, due for this process, what pull requests 
themself fit for the code review process. 

**Michaela:**  [00:40:13] So, FeaturePeek, which basically is part of what 
you're just describing, right?
Of the functionality that you're describing. As I understand it. Is it company
that you acquired? So I would like to understand the process around that a 
little bit. So you have this vision, obviously. You seem very vision driven, 
right? So, you have this vision and then you see that there is no place for that.
But how does that work? Like, and then you find a company or, you know, like it, 
because you're, you're obviously having your eyes out on the space and 
on the companies, and then you see a company that works in that space and you 
think, oh, they're going to the right direction. And then you contact them.
Or how does that, like how, how can that be such a good match and why not do 
that in-house, and you know, like how does this whole process wig? And what's 
your, what's your mental model behind that? 

**Matt:**  [00:41:03] Yeah, let me, let me tell those. So let me take a step 
first back and just to listeners share, like yesterday, we announced a big 
feature for us called collaborative deploy previews that allow other stakeholders 
to give feedback in the process of reusing and going from pull requests to release.
And behind that feature launch was an acquisition of a venture funded company 
called FeaturePeek that was backed by Y Combinator and Matrix Venture in that 
joint Netlify and integrated that product into the core of our product. And the 
whole process started in a way back in our all-hands meeting at the very start of 
2020, where Marissa was a UX researcher on our team brought up the initial idea 
that it would really add so much value to the other stakeholders if there was 
a way of bringing feedback and commenting to deploy previews. 
And based on that, we started at first prototyping with a couple of different 
tools that already existed in the space for commenting and annotating on websites, 
so we integrated one of those tools through it, built plugin and started testing 
it out internally. And we learnt there that if the commenting was something 
external to the current process, our developers got more frustrated than helped 
by it. Like they quickly felt like, okay, now I'm just getting a part from all 
the mails and Slack messages, administer git, I'm also now getting comments in 
a different place, right? So after testing that for a while, we found out that, 
okay, that's not going to be the right approach. It's the right idea, it's the 
right problem we are tackling, but it's not the right solution.
So we figured that we would have to do something that tied into the process 
that developers will already working in and that tied into the pull request 
process. And we did start in building our own, we built first a quick prototype 
that our developers experienced team built, to be able to take that to our user 
researcher and then put it in front of a bunch of our clients talk through like, 
what would this do for their workflow?
What are they currently doing for their workflow? And started all to really 
understanding like the set of tools that our customers were working with and how 
they were already solving this problem. Because obviously like, it's not like, 
this is something that everybody are already doing in some way. No one are 
building software just by having developers write the code and then launch it,
right? Like there's always a process of write the code, show the output, talk 
through it, do testing, validate the result, give feedback, iterate on it, and 
then you launch it, right? But often that process is just a lot of screenshots 
and PowerPoints and emails and Slack messages and so on. And we could see that 
if we could make that flow back into the pull requests that would help, but it 
wouldn't be enough like when we tried just that with our first prototype, 
we saw like just pull requests, comments, is not enough. Like people are also 
using issue trackers and project management software. And we had to figure out 
how can we integrate into those pieces as well? So this was a long process and 
we built several internal prototypes and did some, kicked off some real 
development. And in the process we kept looking at, in any company, they was 
trying to tackle list in the market. And one of them that started to really 
stand out was FeaturePeek. So we reached out to them and asked to meet. And they 
came to us and had at the time actually started working on it, on a Netlify 
integration through our built plugins layer, and yeah.
I was in a call together with Jessica, one of our product managers with the two 
founders of FeaturePeek. They gave us a demo of what they had been working on 
in the integration. And as the demo progressed, I would say like our chores got 
closer and closer to the flow of because it was really far ahead of anything 
else within this space.
And more than that, it was as if they had been reading all of our user research 
(*laugh*), like building exactly the kind of product that we wanted to build in 
and that we were dreaming about, right? So we very quickly figured out that 
between us and the FeaturePeek founders, we really shared a vision of like, what 
can you do in this space?
And what can you build in? They had already built a product that get a lot of 
that, but we could also like just talking through future potential. We could see 
there we were so aligned in like, what could this turn into? And as we started to 
talk more, it was also pretty obvious that they could build a great integration 
on top of Netlify and use our integration layer for that.
But it would still just be an add-on. It would still just feel like something 
you could add and that would be bolted on, right? It would have its own, like, 
separate sort of dashboard, and login, and the integrations would be only on 
there and not on our end, and so on. That would not really be a good way to 
integrate the whole feedback cycle as a first-class citizen throughout our whole 
product journey.
It would be feeling like just a plugin, just an add-on, right? And we felt 
between all of us, that if we really wanted to do this integration had to be 
much deeper, had to be much tighter. And we would only really be able to do that 
if we were one company. So then we started talking about what if we join forces?
What if we, what if we built something together, then build something into 
different silos? And ended up agreeing that that was the right way to go. 

**Michaela:**  [00:47:26] And so now, you acquired them this week? And are you 
going to develop something now or is it already developed? Or, you know, like 
how does that process would like?

**Matt:**  [00:47:38] So, we did the acquisition in about three months ago and 
behind the scenes that their whole team and our team have been working really 
hard on integrating their technology really deeply into Netlify. 
So Netly, so yesterday we didn't just announce the acquisition. We also 
announced the full product launch with all of these collaborative features now 
available to all Netlify users from yesterday on.

**Michaela:**  [00:48:09] Very cool. Very cool. So you took the code base that 
they had, and then it, it's not a complete rewrite, it's just that you plugged 
in what they had, you know, got rid of some, you know, functionality because it 
was a plugin first and now it's, you know, it's part of Netlify. So you, took 
the part of the code base and integrated it? Or how does that work?

**Matt:**  [00:48:33] The team that has like they both whom rewrote parts of 
their code base to integrate it into our code base directly for the whole co-API 
functionality. I think our team together with their team built three new 
micro-services to power like identity for cross integrations, for uploads and 
so on. And they updated the whole UI to be in line with how we built Netlify's UI 
and to feel integrated into that process. But I have to say was like an incredible 
job from the whole team, executing that in just three months and taking it to 
market. 

**Michaela:**  [00:49:20] Yeah, I can imagine. Yeah. Yeah. Well, it did. So I 
have 1000 more questions, but we are on time. So (*laugh*) I will just, I would 
just say thank you so much for sharing everything with me and with our, you know, 
with the listeners and with us. It's like, yeah. As I said, I just have so many 
more questions. I could talk for hours, but you maybe I'm inviting you again.
Maybe you have time to spend a little bit more talking with me about all of 
those things and I can give you more questions. But yeah, it's, I'm really impressed. 
It's a, it sounds really fascinating and really cool. Is there something from 
your side that you want to share, like with my listeners that you want to give 
them on the way I will obviously link everything in the show notes, but is there 
something that you want, especially for people that are, you know, like love 
technology, software engineering, and also maybe want to become founders or, you 
know, do their own thing?

**Matt:**  [00:50:20] Yeah. I mean the first thing I would say, if you think 
all of this sounds interesting and you would like to be part of it, we are 
very actively hiring. So check out our careers page and if you don't find anyone, 
anything there but think you could be a great part, then we always have your 
dream job position that you can write in for, so that would be the first part. 
And the other part, I would say is that as this whole shift from big monolithic 
applications having to modern architecture with it, decoupled frontend and all 
these different APIs and services. There's also a lot of opportunity for founders 
to build new interest, new interesting pieces that fits into that developer workflow.
And I'm always happy to spend time with founders in that space that are building 
something new or interesting. So, feel free to reach out or Twitter or email 
or the like. 

**Michaela:**  [00:51:25] Wow. That sounds really nice. Cool. Thank you so much, 
Matt. For being on my show. It was really a pleasure. Byebye.

**Matt:**  [00:51:45] Thank you for having me. Bye.

**Michaela:**  [00:51:37] I hope you enjoy the another episode of the Soft Engineering Unlocked podcast. Don't forget to subscribe and I talk to you again in two weeks. Bye.
