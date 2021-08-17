# Episode 45 with Matt Biilmann

**Michaela:** [00:00:00] Hello, and welcome to the self engineering unlocked 
podcast. I'm your host, Dr.
McKayla. And today I have the pleasure to talk to Matt Billman. Matt is the CEO 
and co-founder of native guide, the modern platform for high-performance 
websites and apps that defy has around 150 employees and more than double digit 
dollar annual revenue. But that's not all Matt also coined the term JAMstack, 
which stands for JavaScript, API APIs and markup today JAMstack is even more.
It stands for collection of technologies and languages, including web oriented 
databases, frameworks, like next and next year, and even framework less 
approaches. So I'm super, super thrilled to have Matt here with me today to talk 
about his experience founding and running Netlify and also jam stag and  
self-insuring practices, admittedly fly. So yeah, I'm super surprised that 
you're here. Thank you so much for joining us. 

**Matt:**  [00:00:57] Thank you for having me. 
Yeah, 

**Michaela:**  [00:01:00] really, really excited. So how is that? I looked a 
little bit like a research you obviously a little bit. And so I started it's 
around, you know, seven, eight years ago that you, you for aided or you found 
that and Netlify how, how was that?
Is that. Or you have an idea and you do it, or what was the process like? 

**Matt:**  [00:01:23] It was a long, it was a long process that, that, that 
started way before Netlify itself. So. I I'm originally from Denmark, but spent 
seven years living in, in Spain, in Madrid, where I worked a CTO for a company 
that built websites for small to medium businesses, but at a very large scale.
So we would build something like a hundred websites a week, tens of thousands of 
sites in total. Right. And in. And I let the whole product and engineering or 
built the platform that all the designers would do the design with it, all the 
clients with useful content management that, that powered every single website 
from brief to production in.
And then, then I actually started a CMS startup in, in Madrid together with the 
founders of that Spanish. Is that up because we had just tried building sort of 
several iterations of this. Develop a platform in-house and we thought, okay, we 
can build a cloud hosted multi-tenant version that, that other agencies and 
other professionals can, can use to get a lot of the same efficiencies when they 
are building websites for their clients.
Anyway, that was sort of the first take on, like, how do you really remove all 
of that? The friction for web developers in, building deploying operators. With 
properties, but, but it was built as Hess as a traditional, like monolithic 
application. Multitenancy Amisu with database and template engine and all of 
that.
And I came to the, to the bay area and the whole tech scene here, working on 
that. But while working on that, I started getting this sense. But even if it, 
if it was a product that was, I was very proud of building. It had a lot of like 
early innovations in it that had serverless functions before. That was the thing 
you could write, like service side Java script to running in, in this case, 
within the JVM in isolates and so on.
But I got the sense that the fundamental architecture of this. This monolithic 
approach where data business, logic template language, front end code is all 
closely tied to gala was just not going to be long-term the real, like the few 
charts I could take chunks the way. Yeah. I was looking at lot at, at, in, at 
what was happening in the, in, in, in two different areas.
One was like the space of static site generators. Jake hill and middleman were 
at the time in the other ones, the whole no JSPs ecosystem and Beaufort was 
having what was happening there in terms of the early built tools and task 
runners like grunt and gulp, but also. The first sort of real full race into 
the, in, into the whole world of single page application with originality tools 
like sprout Cole or Andy and Leyda in birth in angular react to all of that.
Right. And I got this sense that. Pretty soon as browsers really started 
maturing, it would make much more sense to have an architecture where you try to 
decouple the front end web UI layer completely from the backend business logic, 
Leah, and the best back in business logic layer would likely Kelly split into 
all these different API APIs and services where someone to them, of course I, 
your own in Europe.
But a lot of them are other people's services, like Stripe oil, goldeo Twilio, 
and the like, and I also saw that if, if you could do that, you could sort of 
map that whole web UI there. You could map the workflow around that pretty 
tightly into the get centric workflow that developers were already working on, 
where in  pull request and merchants and so on.
Right? Like it was much more straightforward to. Map that whole process on twist 
StatePlus, UI Leah, then mapping it onto both the UI layer and the whole 
business logic data layer that tends to require all these kind of migrations and 
the settings and so on. So I got, I got the sense that that architectural 
approach would win out, but I could also see that there was just too many too, 
too much friction.
Standing in front of developers that wanted to go that direction and then 
actually building, deploying and operating with properties like that. So I built 
a small in VP of like, what's the smallest thing I can build that that's sort 
of. Aims at edit dressing the workflow for those kinds of web developers.
And the first MVP was this was a small service called bit balloon, where in the 
very first version, you could drag a folder with your friend  dot com and it 
would immediately go live on a, on a, on a URL. And then I edited some CLI 
tooling and some in API tooling around that. And, and quickly saw that it, that 
it resonated with the right kind of early adopters in the front end space and, 
and got very validated in the idea that this architectural shift was going to 
happen.
So at that point, I started to talking to one of my best friends back from 
Denmark, who Chris was my was my co-founder today. Him. He. We we've known each 
other all the way back from, from high school, which is sadly a long, long time 
ago by now. But while I, I spent seven years in Spain, he had built his own 
production company back in Denmark is specializing in like in very interactive, 
often video power websites typically built in flash for some of the largest 
brands in the world.
They won a bunch of international awards for its work there. And then sold that 
to a full ed foot, to a full service agency where he became the partner and the 
chief digital officer. And I started talking a lot to him about this 
architectural shift and what it would mean if you could sort of pre compile the 
whole UI and put it on a globally distributed network.
And then just talk to these different APS and services. How we could really 
fundamentally solve a lot of the problems around global performance, around 
scalability, around reliability, around security, in an, and even in the 
process, potentially really address to develop a practice city. And all of these 
areas were where areas that, that.
Like he, he knew from, from operating across like web properties from, from tons 
of different companies and running digital strategy for the sort of Walmarts of 
Scandinavia and the, like how, how big these problems were and how enhanced they 
were. Like how, how much worse the problems got as, as, as we also started 
having more and more people using mobile devices for the web and, and expecting 
a different kind of, of both pace and use experience.
But we could also just see again, how much friction there was. If a team wanted 
to adopt this architecture, suddenly they had to stitch together like CIC CD 
with object storage, with CDNs. They had to figure out cash perching rules and 
it's caching. They had to figure out how to connect to all these different API 
APIs and services, and typically had to pick out triggering, rebuild swings.
Content that data changed and so on. And there was just no viable tool chain for 
saying like, okay, we're going to do this. What do we do it with? So that became 
the core idea. We, we, we sat down and discussed and came up with from fo for 
Netlify and still the mission we're we're still working on, right?
Like how can we create a. At cloud platform for the collaborative work, where 
teams can really operate efficiently, where we can remove all the friction 
involved in going from pull requests to live code running in, in, in front of a 
real uses in. And yeah, we, we, we started out just bootstrapping the two of us.
Build on top of the, of the product I had already built and turned it into 
Netlify launched on air show. Heck a news post the in, in March, 2015. In, and 
by the end of 2015, we were still just two people bootstrapping a company, but 
we are serving around a quarter billion web requests a month out of our 
homegrown CDN for customers.
Like we work in Sequoia capital and the Molalla foundation and, and was 
realizing at that point that, okay, now, now we need to raise capital, build a 
whole team around this and, and really accelerate. Hmm. Ray cell first round of 
venture capital in the start of 2016 and hired the first engineers in March, 
2016.
And then, and then it, of course, it's been a really fast paced growth since 
then by now we've raised about \$107 million. From top tier find slack, 
Andreessen and Kleiner Perkins, Menlo ventures, EQT M we have for you onboarded 
more than 1.5 million developers onto our platform and, and, and sites are now 
like just, just the sites and web apps on our platform are reaching the close to 
700 million unique visitors every month.
It so. So, yeah, it's, it's been quite the ride so far. Yeah. Mine's lowing. 

**Michaela:**  [00:11:26] Wow. Yeah. It's mind blowing. Yeah. And so for me, You 
were really very, very involved with the technology. And you had like this 
vision where it's going to go and it also went there. Right. So it was spot on. 
Do you feel like that you're still very connected to that?
Like, do you still feel like that you're so connected to technology or are you 
now more involved in, you know, you have to see overall. I am now a little bit 
more away from this technology side. And how is that for you? You, for me now, 
how you explained it and how much passion I could really see that.
Right. I can imagine that you have also like this passion for the role that you 
have right now. So you're probably extremely. Business oriented and you know, 
all these funds and you know, like where to raise money and how to acquire a 
company and all of that. Are you still very technical? Do you feel like you're 
as technical as you have been before?

**Matt:**  [00:12:24] I I'm obviously not as involved in building Nipsey five 
from writing code perspective at Southwest, right? Like the first version of  I 
built a CDN from there, from the ground up and the CSTD platform and the react 
UI that powered it and everything. Right. Like, and now I typically don't like 
by my working space, now it doesn't involve writing code file product eight.
Like. But in a curious thing about my background is that that while I've been 
programming as a hobby, since I was 10 years old, I studied the musicology and 
cultural studies in and was always more interested in how humans adopt ideas and 
make sense of the world and understand things. So, so I think some people are, 
need to feel very hands-on with the coach to feel that they are doing something.
I, I, I get a lot of joy also out of building the culture and the organization 
and the, and the engine that can build things without me. Right. And trying to 
understand both how, when we talk about something like the gem stake emerging, 
for example, and the shifts in technology. There's always a mixture happening of 
like the actual sets of technologies involved and, and the specific program 
languages and API APIs and infrastructure evolutions that we're seeing.
But in the end, technology is adopted by humans, learning about things and 
building things, right. And you can understand where technology is going, what 
will happen in an ecosystem? If you don't understand how humans adopt technology 
and why developers built with certain technologies at certain points in time and 
why you'll sometimes see technologies that are technically better loose out in 
the marketplace because their adoption path is harder.
Right? So for me, it I've always been a very curious person and, and, and, and 
like to understand. Both sides of that spectrum, both the lower details of, of 
how does technology, like how does that technology work behind the scenes, but 
also the details of like, how does human beings approach it and understand it 
and build with it.
And of course, as I been building this company and it's, I am building it right. 
The layer of where I operate them, we'll have to keep shifting. Right? Like in 
the beginning I had to be the one who just sat down and wrote the code. And then 
I had to be part of a team that wrote the code. And then I had to be more 
warfare at it, take lead for that team and guide them in the right direction.
And so. And now I have to build the right kind of organization and the right 
kind of organizational structure to allow our company to build the kind of 
product that. That we think we need to build. And that's that, that in some 
cases also requires finding the right partners to build it with in terms of fee 
investors or, or ecosystem partners in, or finding the right people to join our 
team and, and help build it.

**Michaela:**  [00:16:01] So, this is really, really super interesting. Is it, 
is it for you all about the people or is it also about the structures and how 
people are working together? Do you see it as a system? Or, you know, like, or 
is it self forming, like is a company self forming or do you give it some 
structure? 

**Matt:**  [00:16:20] No. No, we, you, I believe in, in trying to, to, to.
Bring some structure along the way. I think both me and Chris have always fought 
that did that, that intentionally building structure and organization is really, 
it's really important for building a company that can, that, that can scale to, 
to become a really large company. Right. Like I think. If you, if you try to 
ignore the structure, you, you will hit a point where, where everything's that's 
is that's falling apart.
And it's very easy to hit points along the way that feels like that's happening. 
Of course, you're always a bit riding on a rocket that's slightly out of 
control. Right. But I think culture and structure and And value is a really 
important for how a company functions. And then of course, like you can never 
replace the, like, it's in the end, it comes down to actual people doing stuff.
Right. But the structure is important and it's important to be intentional about 
it. I think we've seen some companies that tries to build completely like say 
they built completely flat structures with. In any kind of structure to it. And 
that, that just means that as a leader, you're not taking any intentional 
decisions and route the structure, because your team is still going to have 
people that have more offices than other people.
And they're still going to have, it's just going to happen by politics and, and, 
and sort of maneuvering rather than by any intentional process of like how 
strict the structure. Do you see 

**Michaela:**  [00:17:51] like a parallel between like I texture, like software, 
I attacked her and technical debt and structures of companies.
Like where you say, well, we try to build the best system with the information 
that we have right now. Obviously also looking into the future, but then, you 
know, things evolve, things change. So we actually have to go back and change 
the architecture or change, reverse some decisions, you know? Remove some 
technical debt.
Do you see the same happens in company in your company structure? Or do you feel 
like, oh, this is for what we have foreseen, but now we actually have to 
restructure and re refined or redefine ourselves. 

**Matt:**  [00:18:31] Yeah. You absolutely see that happening. And of course it 
could be a useful metaphor too, to compare like your company through to the 
machine, building the thing and, and, and think of it as an architecture and 
that point.
Just also have to remember that Indian, the pieces of the machine. So not lines 
of codes that, that are predictable. They are people with goals and dreams and 
carry ambitions and interpersonal. Characteristics in. So you have to be aware 
of both, both sides of it. 

**Michaela:**  [00:19:07] So you're what you're saying is that technical debt is 
sort of peanuts, right?

**Matt:**  [00:19:12] Complicated. I just, it to deal with, with, with 
technology. It's a lot more predictable Indians than people are, but it, yeah, 
in the same way, it can also be a lot more fun. To deal with, with human beings. 
Yeah, 
obviously. 

**Michaela:**  [00:19:30] Yeah. Yeah. I'm, I'm super impressed. Like I can't 
imagine how much personal growth has to happen on a way from, you know, like 
bootstrapping something, then getting investors, you know, scaling probably if 
you get investors, you normally scale really fast really quickly.
And yeah. So th that's. 

**Matt:**  [00:19:53] Yeah. And it's also, I mean, it's also a choice you take 
when you go and raise venture capital that, that raising venture capital is only 
one way of building a business, right? Like the many other approaches to build a 
business. In, in our case, we felt that there was also the kind of market 
opportunity, right.
Because we really, from the get go belief. That there was a real opportunity to 
shape how the future of the web is, is going to be built and how it's going to 
function. But we could also see that, that making that big of an impact and 
getting there in time. And so. There was not something we could, we could have 
done if we had grown just organically based on our revenue.
Right? Like, so that's, that's why we, we went out and, and, and raised funds to 
be able to, to scale and grow much faster than we would be able to do 
organically. Right. And that, of course always didn't happen. Half the trade-off 
of like all the older challenges you get when you are trying to scale an 
organization very fast.
And it has like, you have to know what you're going into as a founder also, 
right? Like, as you say, of course, it's a, it's a learning curve and you have 
to be very okay with continuously taking things that, that you saw as quarter 
your role, like writing the code, building the technology. And then have other 
people come in and do them instead of you and step away from it.
Right. But if you do that, you'll also learn very quickly along the way. The 
more like that, no matter how much of your job you seem to delegate it at way, 
you only get more busy somehow.

**Michaela:**  [00:21:39] Yeah. So one thing that that would really interest in 
me is like you said, you wrote this little first version MVP of, of Netlify and. 
A lot of people adopted it. So it seems like you didn't really have to convince 
people about this solution or that there is a problem because sometimes like 
founders it's, it's hard.
Right. You think like, oh, I have this idea. And then is it too early? Do I have 
to convince people to have to explain it better? Do you have like to, do you 
think that this is, this is the right mindset or should people step away from 
something like where we have. Tweak one sentence to be really powerful and 
express like the pitch.
Right. Is that really too important? Or should we read our focus, our energy on 
finding the thing that people actually want? Even if you write a sloppy sentence 
about it, you know what I mean? 

**Matt:**  [00:22:34] Yeah. I think, I think it it's never completely one or the 
Euler in, I think. You have to in like initially for example, the mental model 
we had around adoption was that for these kinds of technology products, if 
you're trying to build something that's in that the future of how things will be 
built, you would expect it to sort of grow in concentric circles where you sort 
of have these very early adopter technologies that are constantly.
Joking too, to broaden their horizon, then find new things that work and so on. 
Right. And, and, and you want this kind of product to resonate with them first, 
right? Like in the initial stages of this product, you wouldn't expect someone 
who was like aids. Are they working in a law long enterprise company?
Very focused on solving. Big picture of business problems, insight that for 
which assisting technologies to even be interested in your product, right? Like 
it's just not time, but you would expect like for a product like ours and, and 
early adopter of JavaScript frameworks or, or site generators to, to get 
interested in.
And then ideally like there's, there's two is essentially two different paths to 
building. Product companies, right? Like one of them is product led growth and 
the other is sales or marketing led growth. And not, there's not like one way is 
the right way for some products. If you have a product that requires in a whole 
organization to adopted horizontally before it really adds value.
Right. Build a product lead motion around that. You have to go build a sales lit 
motion where you first go and talk to executives and companies and pick out the 
needs and then solve their needs with a product. But if you have a product that 
can both be really useful to an individual engineer, into a small teams with 
engineer to a larger team of engineers into a whole organization, then you have 
the opportunity of building like a product led growth moment.
Motion. Where, the way you get into businesses is by individual users first 
adopting the product, and then, then it spreads from there. Right? And we saw 
the opportunity to build that kind of company. And when you built that, then it 
can't be like the cost sale doesn't depend that much. At first, unlike nailing 
there, the phrase on your marketing site or something like that, it comes on 
nailing the onboarding experience for how fast.
Can you get someone to land on your website and then be inside the product, 
doing something where they having a hard moment of why? Like, why is this 
product going to be useful to us? And for us, there was really about like 
landing on netlify.com and then having a web property running on a custom domain 
in a shorter time as possible.
Right? Like that was sort of the first iteration of, of, of that hard moment. 
And then knowing that maybe in, in, in 30 seconds, so minutes or something, 
right. You had gone from nothing to having a globally distributed website, 
running on a custom domain with a CSED pipeline plug directly into get right. If 
we could just make that motion, like something you could do in, in, in 30 
seconds or minutes at something like.
Then then we would drive that, that, that feeling of like, wow, this is, this is 
another generation of tooling. This, this is, this is just so different from how 
the world looked before and, and, and then build excitement with developers. But 
then in parallel with that, we will also positioning ourselves Hindu in, in the 
midst of like an architectural change of how are we going to build the web in 
the future.
And at the time when we started, there was just a lot of difference. 
Technologies that was making that happen. There was, as I mentioned, static site 
generators that were single page applications. There was a lot of talk of the 
API economy, some talk around like the programmable weapons, but there was no 
name for this architecture.
And that was something that, that, that, that Chris Sue, my co-founder 
immediately saw from his background. Like we need, if this is going to have him, 
we need a name for this category and this architecture, because otherwise, 
again, all of this happens because humans adopt the technology and humans goes 
in the direction and, and.
If you can't give people the vocabulary to talk about what they're doing, it 
becomes very hard for that idea to spread between groups and teams and people. 
Right? So that's why we ended up coining the term game stack. And it happened 
sort of in a very collaborative process with different people in the, in the 
industry.
And so on in an and the term started taking off because it was needed, right. 
Because it gave me. And nomenclature to start talking about things that before 
were seen as just separate movements, right? Like, okay. This, something 
happening about the architecture we use for cell phones, talking to API APIs, 
there's something happening or how this whole world of web API is exploding.
There's something happening around single page applications and something else 
happening around CDNs and site generators and stuff. And suddenly we had a 
nomenclature to say, oh, it's an architectural shift. It's a shift to watch the 
games deck. And that, that was really important to, to, to build the other part 
of like on the one hand, the individual product story and the developer story of 
like finding this product and instantly getting into ha moment and then connect 
them.
To a broader story around like a new architecture for the web emerging and, and 
the possibilities that that would entail and how not just individual developers, 
but large organizations could benefit from that change. So both sides are 
important, but in the end, if you're building a product led growth company, you 
have to be really obsessed is obsessive about the product itself and how.
That product that attracts Andy and convinces juices to, to, to work with it. 

**Michaela:**  [00:29:17] Yeah. The funny thing is that when you described the 
story off, you know, how a developer, you know, sees your side and tries it out. 
This is exactly how I felt when I tried it out. I was not an early adopter 
dough. Right. I try it out somewhere last year, but.
It wasn't exactly like this. I was like, oh, I have to reply this website. And I 
want to do it quick. And you know, like, let's, let's try that out. Right. 
Everybody is already on it. I'm like the late, late person too late for 
everything, but I went to it. Right. And obviously at that point it was fully 
baked fully in, but, you know, I was there and was like, wow.
Well, it's running, right? Like I was like, and as you said, right, this, like 
you push and then it's there.  I exactly felt what you were saying, but it was 
like last year.
How was Natalie fly when you say, well, let's go five years back. How was the 
experience? Was it similar? Like at that point, would you say. 

**Matt:**  [00:30:18] Yeah. So, so the expense involved in, and it will continue 
to evolve it as, as we also go for, broadening the experience and, and telling 
it different, like as a large and larger story through the product.
Right. So the very first story you would see was, was, was in bit balloon the 
predecessor to Netlify. Land on a website that just immediately on the front 
page, head like a drop soon in saying drag your web folder here. And there would 
also be a little download link where if you didn't have a website handy, you 
could download one and drop it there.
Right. And then you could just drop aside onto bit ballooned at com without even 
signing up or anything. And it, you didn't need to sip the files first, anything 
you just drag the actual folder onto a bit, little.com and boom. Now you would 
be live. We still have that done. If you go to app.netlify.com/drop, you'll get 
the same kind of experience that mimics, like what, what the very first version 
was like, of course, in the signed by me and not by actual designers.
Like it looks like today. So that was like the first simplest motion we could do 
right in. And then the next step was really to, to start, like after we had, 
after I had built out that initial version of just getting a site live and, and, 
and getting a custom domain connected to it, getting SSL set up and so on, then, 
then it was really the question of okay.
This is fine. If you're really just one developer by yourself, manually 
deploying, and we added a CLI where you could do the same from like writing it 
at for spit and native later, just Netlify deploy and immediately from the 
command line, deploy fault. That's fine. If you're really just one individual 
working, as soon as you're at team of people, that's not very useful.
Like you, you can't just random. You have people deployed manually at different 
time without structure and people get their structure from, from GitHub or 
GitLab or bit bucket. That's where developers collaborate on opening new pull 
requests and building new features. So. The next iteration of that on Netlify 
was really saying, instead of focusing on you deploying manually from a folder 
that solves the whole problem of you working in a good provider and getting that 
live.
So the next moment really became that flow of like calming. Tell us you'll get 
repository and we'll try to even guess what tool you have a framework you're 
using. And just say, okay, and now you're done, right? Like now you have 
something you live in. And, and now of course, with, without acquisition of a 
feature peak and that whole journey, we are going even deeper into that space of 
like, this is not just for single developer building.
On their own, like real projects, always built by teams with lots of different 
stakeholders and with several developers and one part of the processes it's 
writing the code. But another part of that whole process is that for every 
release, you have some feedback cycle where you have back and forth with product 
managers or designers or other developers or other stakeholders.
Before you take something live and now we're really sort of expanding that whole 
experience to drink fluid, that process and to sure how, how frictionless we 
can, we can make. The process of a team actually building releases together and 
taking them to the world. 

**Michaela:**  [00:34:21] So with, with this acquisition, somehow you have like 
this deploy previews feature.
Yeah. You know, my, my favorite thing are code reviews. Is that something that 
you think is part of the programming part or is it part of deploy? Is it, is it 
part of something that should be, should code reviews be somewhere in that 
picture or how do you see it? 

**Matt:**  [00:34:45] I mean, code code reviews are really important, but then 
there's also the, the step ahead that's like viewing their outcome of, of, of 
your current code.
Right? Like being able to just open a pull request and having that pull request 
running in the full production environment. Exactly. As it would look like if 
you were. That's that's really like, it doesn't replace the code review. Right? 
Like the developers should still work on the code review tools to make sure that 
the quality of the code behind that it's up to scratch and so on.
Right. But it does make the, the review, especially from. It QA testers, product 
managers to designers and marketeers to content editors or anyone else that's 
involved that will want to review what the output looks like. Hmm. It makes that 
process in much simpler. Right. And what we were seeing, like w w like we 
launched deploy previews in 2016, a long time ago, and we've of course been very 
big consumers of that whole workflow internally, ever since then.
netlify.com runs. And Netlify Natalie find that conference and identify all of 
our web properties up easily run on Netlify. And in that process of deployment, 
Completely essential to how our web teams work. We're constantly sharing URLs 
and so on. But the one thing we saw also when talking to clients and so on, was 
that when you share that URL, then.
The feedback cycle spec to the developers that happens all over the place. Some 
of it happens you're shared in slack and there's feedback in slack and more 
people open issues and get up or in JIRA, or they will piece two screenshots 
into documents and sent them back and forward for, at the mess attachments.
And, and for developers like the, the process. The process of, of that is as 
fragmented as the process of code reviews was before tools like get help and get 
lab integrated into the workflow. Right? Like before that happened, like there 
was no. You, you would sometimes have specific tools for code review, but mostly 
it would be processes of sending back and forth emails around the code, or 
simply just having to sit down at a laptop together or at, at this top bank at 
the time, and look at the code and talk through it.
Right. And get up with the pull request. Functionality really gave her home. For 
court reviews, right? Like in the game of place where, where now you no longer 
have to wonder, like where is it happening? And people commenting in all kinds 
of places and so on. Right. So what we're trying to do with collaborative deploy 
previews is in a similar way to give it a form for the,  feedback, not on the, 
on the input, which is the code, but on the output, which is the reason.
And make sure also that since every deployed review, it's a different URL. We 
don't, we didn't want to have a system where every deploy preview now has its 
own. Like you have to know it exists and go there and look at the feedback in 
order to take part in that process. Because like we had some initial prototypes 
integrating with tools like that, and it just attracted from the process because 
now.
Apart from checking the pull request to end a slack messages and the emails also 
I had to continuously try to figure out is people, are people now also 
commenting on the deployed from you? Yeah. So it's really important to make each 
deploy from URL. Okay. At checkpoint that that makes information flow into the 
original places.
So feedback that stakeholders make on the deployment of the will, will flow back 
into the poll requests. They'll take part in the comments there, or they can 
open tickets in whatever project tracking software you're using related to get 
Harper linear clubhouse for the like, and now it's really important for us.
Right. But again, it was this sense of like, Now when a developer, she is that 
deployed preview URL, the Isles are sharing how to give feedback and how that 
whole process operates. And we hope that can really, as I said, do do for this 
process, what, what pull requests themselves fit for them? For the code review 
process 

**Michaela:**  [00:39:23] feature peak, which basically is part of what you're 
just describing right.
Of the functionality that you're describing. As I understand it. Is it a company 
that you acquired? So I would like to understand the process around that a 
little bit. So you have this vision, obviously you seem very vision driven, 
right? So you have this vision and then you see that there is no place for that.
But how does that work? Like, and then you find a company or, you know, like it, 
because you're, you're obviously. Yeah. Having your eyes out on the space and 
under companies, and then you see a company that works in that space and you 
think, oh, they're going to the right direction. And then you contact them.
Or how does that, like how, how can it be such a good match and why not do that? 
In-house and you know, like how does this whole process wig? And what's your, 
what's your mental model behind it? 

**Matt:**  [00:40:12] Yeah, let me, let me tell them, so let me take a step 
first bank and just to the listeners shit like yesterday, we announced a big 
feature for us called collaborative deploy previews that allow other 
stakeholders to give feedback in the process of, of, of reusing and going from 
pull requests to release.
And behind that feature launch was an acquisition of. Affair venture funded 
company called feature peak that was backed by Y Combinator and matrix venture 
in that joint Netlify and integrated that product into the core of our product. 
And the whole, the whole process started in a way back into, in our all hands 
meeting at the very start of 2020, where in memory.
So was a UX researcher on, on, on our team. Yeah. Brought up the, it like 
brought up the initial idea that take it. It would really add so much value to 
the other stakeholders. If there was a way of bringing feedback and commenting 
to to deploy previews. And based on that, we started at first in prototyping 
with a couple of different tools that already existed in the space for.
Full commenting and annotating on websites. So we integrated one of those tools 
through it, built, pluck in and started testing it out internally. And we 
learned there that if the commenting was something external to the current 
process, our developers cut more frustrated than helped by it. Like they quickly 
felt like, okay, now, now I'm just getting.
At pod from all the meals and slack messages in this year's I get, I'm also now 
getting comments in a different place. Right. So after testing that for a while, 
we found out that, okay, that's that's not going to be the right approach. It's 
the right idea. It's the right problem with tackling, but it's not the right 
solution in.
So we think it, that, that we would have to do something that tied into the 
process that developers will already working in. And that tied into the pull 
request process. And we did start in building our own. We built first, a quick 
prototype that I went to celebrate experienced team built in. To be able to take 
that to our user researcher and then put it in front of a bunch of our clients 
talk through like, what would this do for their workflow?
What are they currently doing for their workflow? And started all to really 
understanding like the set of tools that, that our customers were working with 
and how they were already solving this problem. Because obviously like, It's not 
like this is something that everybody already doing in some way. No, no one are 
building software just by having developers write the code and then launch it.
Right? Like there's always a process of write the code, show the output, talk 
through it, do testing, validate the result, give feedback, iterate on it. And 
then you launch it. Right. But often that process is just a lot of screenshots 
and PowerPoints and emails and slack messages and stuff. And we could see that, 
that, that if we could make that flow back into the poll requests, that would 
help.
But it wouldn't be enough. Like when we tried just that with our first 
prototype, we saw like just full requests, comments. It's not enough. Like 
people are also using is your track or some project management software. And we 
had to figure out how can we integrate into those pieces as well? So this was a 
long process and we built several internal prototypes and did some.
Kicked off some real development. And in the process we kept looking at, in any, 
any company, they was trying to take a listen to the market. The end, the one of 
them that started to really stand out was, was west feature peak. So we reached 
out to them and, and asked to meet. And they came to us and, and had at the time 
actually started working on it on a nearly fight integration through our built 
plugins layer and.
Yeah. I was in Nicole together with a, with,  Jessica, one of product managers 
with the two founders of feature peak. They gave us a demo of, of what they had 
been working on in the integration. And as the demo progressed, I would say like 
our jobs got closer and closer to the, to the flow of because yeah, it, was 
really far ahead of anything else within this space.
And more than that, It, it was as if they had been reading all of our use of 
research, like building exactly the kind of product that, that I wanted to build 
in that we were dreaming about. Right. So we very quickly figured out that, 
that,  between us and, and the, and the Fiji peak founders, we really shed a 
vision of like, what can you do in this space?
And what can you build in? They had already built a product that, gets a lot of 
things. But we could also like, just, just talking through food, future 
potential. We could see that we were so aligned in like, what could this turn 
into? And as we started to talk more, it was also pretty obvious that they could 
build a great integration on top of Netlify and here's how our integration layer 
for that.
But it would still just be an add-on. It would still just feel. Like something 
you could add and that would be bolted on, right. It would have its own like 
separate sort of dashboard and lock in. And the integrations would be only on 
there and not on our end and so on. That would not really be a good way to 
integrate the whole feedback cycle as a first-class citizen throughout our whole 
product journey.
It would be feeling like it just,  to pluck in just an add on, right. And we 
felt. Between all of us that if we really wanted to do this, integration had to 
be much deeper. It heads to be much tighter. And we would only really be able to 
do that if we were one company. So then we started talking about what if we 
joined forces?
What if we, what if we built something together, then build something in, in two 
different silos ended and ended up agreeing that, that that was the right way to 
go. 

**Michaela:**  [00:46:35] And so now, You acquired them this week. And are you 
going to develop something now or is it already developed or, you know, like how 
does that person?

**Matt:**  [00:46:46] So, , we did the acquisition in about three months echo 
and behind the scenes that their whole team and our team have been. Working 
really hard on, on, on integrating their technology really deeply into Netlify. 
So Netflix too. So yesterday we didn't just announce the acquisition. We also 
announced the full product launch with with all of these collaborative features 
now available to all Netlify users from Friday.

**Michaela:**  [00:47:19] Yeah, very cool. So you took the D the code base that 
they had, and then it w it's not a complete rewrite, it's just that you blacked 
in what they had, you know, got rid of some, you know, functionality because it 
was a plugin first and now it's, you know, it's part of Natalie fly. So you, 
part of the code base and integrate the data.
How does 

**Matt:**  [00:47:40] that. The team that has like they both whom re rewrote 
parts of their code base to integrate it into our code base directly for, for 
the whole coy API functionality. I think our team together with their team built 
the. Three new microservices to power, like identity for cross integrations, for 
uploads and so on in.
And and they updated the whole UI to be in line with how we built Netlify UI and 
to feel integrated into, into that process. Eh, But if, but I have to say  an 
incredible job from, the whole team, executing that in just three months in and 
taking it to them. 

**Michaela:**  [00:48:29] Yeah, I can imagine. Yeah. Yeah. Well, it did.
So I have 1000 more questions, but we are on time. So I will just, I would just 
say thank you so much for sharing everything with me and Medalla, you know, with 
the listeners and with, with, with us, it's like, yeah. As I said, I just have 
so many more questions. I could talk for hours, but you maybe I'm inviting you 
again.
Maybe you have time to spend a little bit more talking with me about all of 
those things. Yeah. Can you have more questions, but yeah, it's, it's, I'm 
really impressed. It's a, it sounds really fascinating and really cool. Is there 
something from your side that you want to share, like with my listeners that you 
want to give them on the way I will obviously link everything in the show notes, 
but is there something that you want, especially for people that are, you know, 
like love technology, software engineering, and also maybe want to become 
founders or, you know, do their own thing.

**Matt:**  [00:49:28] In. Yeah. I mean the first thing I would say, if you think 
all of this sound sounds, sound interesting and, and you would like to read the 
part of it. We are very actively hiring. So check out our careers page and if 
you don't find anyone, anything there. Think you could be a great part, then we 
always have at your dream job position that you can write in for in.
So that would be the first part. And do the other part, I would say is that it S 
this whole sheet. From big monolithic applications having to to, to modern 
architecture with it, decoupled front end and all these different APIs and 
services. There's also a lot of opportunity for founders to, to build new, 
interesting, newer, interesting pieces that, that fits into that developer 
workflow.
And I'm always happy to. To, to, to spend time with founders in that space that 
are building something new or interesting. So it feel free to reach out or 
Twitter or email or the like, 

**Michaela:**  [00:50:36] wow. That sounds really nice. Cool. Thank you so much, 
Matt. For, for being on my show. It was really a pleasure. 

**Matt:**  [00:50:43] Thank you for having me.
Bye.


