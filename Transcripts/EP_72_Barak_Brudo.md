---
episode: "Transcript Episode 72 Barak Brudo"
permalink: /software-bill-of-material
status: publish
type: transcript
---

[00:00:00] **Michaela:** Hello and welcome to this Software Engineering Unlocked 
Podcast. I'm your host, Dr. McKay, and today I have the pleasure to talk to 
Barack Br. 

But before I start, let me tell you about an amazing opportunity that allows YOU, yes, YOU to earn additional income! 
Do I have your attention? Yes? Great. So, [User Interviews](https://www.userinterviews.com/hello) is a company that connects 
researchers with study participants. And they especially are looking for developers 
that share their feedback on products. 

Share your opinion with top brands such as Sporify, Adobe, Amazon and many more, and get paid. 
Most studies take less than one hour to participate and pay over \$60. 

So, sign-up today - It’s free - apply to give feedback for products that interest you, and make a 
nice side income. Additionally, you help to shape the future of the tools we als use. 
What’s not to like, right? So, hop over to [userinterviews.com](https://www.userinterviews.com/hello)
That is [userinterviews.com](https://www.userinterviews.com/hello).


But now back to Barak. Barak helps organization secure the 
software supply chain.

He works as a developer relation advocate at scribe security, and Vela will tell 
us today all about why we should care about acronyms such 

as e o 14 zero uh, 28 s, SD f and s b o m. So welcome to the show, Barak. I'm so 
curious what this all means, . 

[00:01:05] **Barak:** Well acronyms are very common in, in the land of cyber in, 
in general.

Uh, They're just because there's so many words that it makes much more sense to, 
to shorten them into acronyms than to say the whole thing over and over and over 
again. There are actually so many acronyms that you could get confused, cuz some 
of them just mean different things depending on the context.

But for this conversation, all of these acronyms are centered around one main 
thing, which is the software supply chain. The software supply chain represents 
essentially all the bits of software. that end up in your software, your code, 
whatever, because you see these days almost nobody writes a piece of software 
completely from scratch.

It's hardly ever done because there's so many building blocks already available 
in the open source. But if you follow the same train of logic to its source, you 
see that if you use building blocks that are written by other people, Then those 
building blocks also use building blocks written by other people and so on and 
so forth.

It could go on for a very long time. So if you end up using some of these 
building blocks, you really don't have a very clear notion. Of everything that 
is included in your final product, that means that you have a higher chance of 
including something that might be bad for you. Just like if you're allergic to, 
for example, olives and you eat something, but suddenly, oops, you're not 
feeling well.

Maybe there was a trace of olives in there and you just didn't know. So the 
whole point of these various acronyms is to help. Or help the, the industry at 
large, figure out what's in your code, what's in everybody's code so that 
everybody can know where or what everything is. That transparency should help 
everybody be more secure, more safe.

At least they'll be informed, which is the first step. So we started with EO 14 
0 28. That's the number of the executive order from the Biden administration in 
the United States. It came out in May of 2020. Following the very massive, very 
famous public pack of SolarWinds in the late 2020. The executive order is, is 
very long, very comprehensive.

Section four of that executive order speaks specifically about the securing the 
software supply chain. It numbers various ideas, various strategies among other 
things that charges nist which is the national infrastructure. Organization 
there to write a framework for securing the software supply chain.

It also mentions the sbo, the S B O M by name. Specifically the SBO is the 
software bill of materials. Just like any bill of materials or a list of 
components, it does exactly that. It's a list of components for your software. 
Um, Because it is supposed to be, at least in theory, comprehensive. It doesn't 
only tell you you have fragment or library A.

It tells you everything in your software, even things you didn't know you had. 
So instead of just saying, this is library A, it tells you this is library A, 
and it relies on library B, C, and D, and those libraries rely on those if these 
are the connections between them. This is everything in your 

[00:04:18] **Michaela:** software.

So it's like a dependency graph of my. , 

[00:04:22] **Barak:** it's more than in dependency graph because dependency is 
only one of the types of relationship that you can find between mm-hmm. 
different libraries. But it is the most common. But there are other types of, of 
relationships that you can describe. For example, this file was created as a 
result of a test on this file.

These two files joined together, then we're deleted in the compiling process, 
creating this file instead there the description of the. Standard for Sbam 
describes I think over 43 different types of relationships. I don't remember 
them all, but yes, dependencies is the most common. And again, you can describe 
dependencies in a graph, which is very helpful.

But an ESBA is so much more because it is has other uses. For example, each of 
these open source libraries has their own license. some of these licenses. There 
are many different types of licenses. Some of these licenses say that if you 
include that, that library in your product, it has to be open source.

You can't use it if you're using it for something that is proprietary. If you 
don't follow the chain of, of let's call a chain of dependency all the way 
through, you might inadvertently. Such a piece of license in your software, and 
suddenly your IP is meaningless. Everything you do becomes open source.

It's called licensed. Yeah, it's called licensed poison. Okay. And a lot of 
people that are let's call it legally minded, spend a lot of time and effort to 
make sure that everything that is included in enterprise software does not 
inadvertently somewhere include one of these licenses. That's just one of the 
uses that you can use an SBO for.

Some other examples is once you have a full list of everything in your. A full 
list makes it a lot easier, first of all to search for vulnerabilities, to 
search for exploits. It also enables you to take the whole list, plug it into a 
database of vulnerabilities and give back a full list of everything that might 
be a problem, including where it is in your software.

You need to remember that software is a very, very dynamic thing. It also gets 
old, very, very, So if you have a legacy system that the people who wrote or 
developed are no longer with you, maybe on old servers, having an SBO for those 
systems make it so much easier to suddenly tackle known and, and very, very 
rapidly becoming a problem.

New vulnerability, for example, to log four j instance late last year in 
December was a huge problem, still is for a lot of. Mainly because they weren't 
sure if they had that particular problematic version. And even if they did, 
where exactly was it? Remember that a certain piece of software or library could 
be included numerous times in various places, locations.

The fact that you possibly may have found it once doesn't mean that you're now 
free and clear. So having an sbam that tells you exactly where everything is, 
including. Relative path of various libraries, including the exact version, 
including the exact license. It tells you basically everything you need to know 
about your software.

Very handy. Okay, 

[00:07:29] **Michaela:** so you made a lot of arguments for such a as bomb 
thing, right? So we need it because obviously we are depending on third party 
libraries and you know, we don't know where it is. So now, , when I think about 
a list of all the software that I'm using, first of all, as you said, it's 
dynamic. So it's changing a lot.

And first of all, creating it will be definitely quite tedious. So how, how I'm 
going to work with such a sbo? Is it, is it something that's extracted from my 
software? And then updated automatically? Or do I have to write that by, you 
know, by hand? How, how does it work? 

[00:08:04] **Barak:** Well, The reason that the executive order and, and the 
SSVF and other let's call it people of conscience are, are saying to use it, is 
that it's not the responsibility of the user to produce this list of components.

It's actually the responsibility of the producer. So the idea is that everybody 
who produces software will include in their pipe. a little piece of software 
that produces an sba. Obviously the SBA needs to be recreated every time you 
recompile your software. Mm-hmm. . Now, if you are using third party software, 
then you need to request an ESBA with that piece of software too.

The thing is that like you said, some people already recognize the importance of 
escom and they wanted to run the, the program that creates it themselves on 
their own software. But some people let's call. , very, very zealous for their 
IP rights, are worried that if you break open their software to look what's 
inside, to see what's under the hood, you may discover some things that they 
don't want you to see, for example, that they're using very old libraries, 
unpatched un unmitigated with, with, even, even though they have known 
vulnerabilities, just because a lot of.

Value the concept of if it's not broken, don't fix it. And it saves time on 
development and saves time to go to market. So they are, they're actually, yeah, 
they're actually rules. I don't know if they're, you know, fully legal now, but 
there are rules, just like the old rule of don't remove the tag.

From a mattress or don't open a laptop yourself because you void the, the 
warranty there rules that if you run an SBO creating software on a closed piece 
of software, you're basically voiding the warranty or doing some other, you 
know, very, very bad thing. So the idea is for the software producers to create 
the esba and supply it.

with every with, with their piece of software so that you're not only getting a 
black box, that you have no idea what's in it. You're getting the black box and 
you're getting the full list of everything in it. So the ingredients, if you 
have, yeah, if you have a problem, if you're allergic to a certain library, a 
certain certain ingredient in that software, you now have the ability to look at 
the, the list and see that you don't really want to.

Well, you might, 

[00:10:19] **Michaela:** yeah. But as you said, I mean, now let's think about, 
okay. It's a very nice idea, right? And you know, but as you said, some 
companies, and they think quite a large majority of their companies, they have 
real problems with it. And this is not just, they're not making things up. 
Right. It's, it's not, they cannot, similar to j Lockford J right?

You cannot just go and say, oh, I'm spending a day and I'm, you know, now 
removing the dependencies. It's a lot of work, which sometimes is just not 
possible. So if I would show that I'm using those old unpatched versions of 
something, I cannot change it from one day to another. And if I would expose 
that, I mean, it's not that.

It's not that I'm secure because not of exposing it, but I'm definitely more 
unsecure if I'm exposing, you know, that I am relying on those. Like, it's, 
it's, it's open to every hacker, you know, in the world. , that wants to destroy 
me . So I'm not going to release it. I would not release it. I would say yes.

Nice idea, but , 

[00:11:21] **Barak:** yeah. Yeah. It, it's just that you, you are thinking of it 
from the point of view of the producers. Mm-hmm. , which is fair enough that a 
lot of people would. But you need to think of it from the point of view of the 
users. Let's say that we're talking about a critical piece of software in a 
critical piece of hardware.

Let's throw in 

[00:11:37] **Michaela:** something really important. I think most critical 
pieces of software rely on the mostest pieces of software. . 

[00:11:43] **Barak:** Well, that's my, which I said I wanna take a really, 
really like extreme example. Yeah. Pacemaker. 

[00:11:49] **Michaela:** Yeah. Or an insulin pump. Yeah, 

[00:11:51] **Barak:** yeah, yeah. You really don't want the software in there to 
be.

When, when you include an , sure. You're basically giving the consumer the power 
of choice. You can say, okay, look, I may be using legacy code, I may be using 
old you know, old libraries, but in, in, you know, as, as sort of, not really 
compensation, but the, the, the trade tradeoff is you can get the, the software 
faster and it's a lot cheaper.

But this, the consumer can say, okay, yes, yes, it is cheaper and it is faster. 
I know about these 15 vulnerabilities. That might mean that somebody who doesn't 
like me would now stop my insulin or stop my heart, and I think the trade off of 
paying a bit more is worth it. Giving the consumers the power to make that 
decision knowingly, I think is better.

And also if that S one is. Open to review. The consumer can't say sorry, the 
producer can't say, but I didn't know. Nobody told me I didn't do the tax. I did 
my due diligence. If something bad happens, now they are liable. And liability 
is very important because that's the sort of world we're live in these days 
with, with massive hacks.

Software supply chain attacks, and, and hackers from nations even who do bad 
things just to disrupt their circled enemies. And then people who are out there 
just to make a. if the, the producers of software are not held responsible for 
whatever it is they're producing. nobody is, and people will 

[00:13:20] **Michaela:** just keep on.

Yeah. I totally agree with you. I'm totally on board with you. I'm just talking 
from a practical perspective, you know? Mm-hmm. , how, how we, how are we 
getting there? Because I remember, you know, I remember back when the pandemic 
started, there was this, oh, I can't, I probably, it's good that I can't rem 
remember the name of the company, but they advertised for the ventilators.

And they said something like, oh, our ventil ventilators are with 8 million 
lines of code. And everybody was like, oh my God, like the, the software. Oh my 
God, this is the worst advertisement you can then do, right? Like mm-hmm. , 
it's, it's the, the more lines you have, the worse it actually is, right? So, I 
would argue that pacemakers or you know, hearing aids or ventilators, a lot of 
software in the hospital, maybe banking, we don't want to know really what's 
inside, right?

So how can we, how can we come from a state that we are right now where we say, 
well, , right. You know, running such a software and getting an SBO from my 
software is probably a real bomb . I don't want to, you know, release it. I 
don't want to show it to the world to something where we can actually do it.

[00:14:34] **Barak:** Well, this is where I think that the US did something 
right for once the executive order. Instead of making this a regulation with 
audits and codifying into into law, they went in a slightly different route. 
What the executive order says is, , if you don't follow these new rules, we just 
won't buy from you.

We won't do business with companies who are not proven to follow the new 
regulations or you know, let's call it best practices cuz they're not actually 
regulations, the new best practices for securing supply chain. And, and the 
other you know, that's just section four, but, and all the other sections, all 
the other requirements and suggestions that we made to.

Software security or cybersecurity more important. Now, you might think, okay, 
how many companies could possibly be selling to the US government can be that 
many, right? I mean, we're, we're talking about military suppliers and then 
really like car suppliers, but they can't be that many. But here's the beautiful 
thing.

If we go back to what I said at the beginning, about companies who use pieces of 
software being written by other people also, that's true for, for hardware. So a 
lot of the, those people who sell to the US government are just aggregators. 
They're just taking bits of hardware and software and putting them together.

And if they need to be liable to the US government and, and prove that they're 
following these new press practices, that is not their responsibility solely 
because they're going to roll it down. They're going to require all their 
suppliers to follow regulations so that they can prove it. Cuz otherwise you.

Nothing there. And if those suppliers, which are obviously again aggregators 
themselves, need to be held accountable, they're going to roll it down and roll 
it down and roll it down. And eventually this goes everywhere because this 
involves money and contracts with the US government, which are extremely 
lucrative.

I think it has a better chance of following through, of making these let's 
follow changes or require. A thing of reality then, had they said, this is just 
a new regulation, I can't tell you because I'm following the subject that as of 
March this year, the omb, which is sort of like the US administration for 
purchasing things already issued, already issued a a statement or, or an 
instruction for all us all the us.

Departments that are relevant to start following the S sdf. I didn't mention the 
S SDF so far. The SDF is a software. Security sorry. The Secure Software 
Development Framework. Mm-hmm. Like I said, making, making it an acronym is so 
much easier than saying the whole thing once over again. . It was written based 
on the requirement of the executive order, and it's, it's, it's not that long, 
it's about 30 pages, but it does give a list, very comprehensive list of best 
practice ideas and suggestions so that no matter what your business is, if you 
follow all these suggestions, your software will be more secure, which is, The 
object here.

Yeah. So, and another very nice thing they did was we are not going to start 
checking you. We're going to take your word. If you tell us that you are secure, 
that you follow the Ss d F, that you have the evidence, we're going to believe 
you until something happens. And then we're going to ask to see the evidence.

And if you don't have it, then you've been lying to the US government and there 
are punishments for that. You can't just go around lying to the US government. 
So I think most people, if they want to do. Business with companies who do 
business and so on and so forth, down the chain, they're going to start to have 
to rely and generate these types of evidence and will all be better for it.

Yeah. 

[00:18:05] **Michaela:** So the sbam is probably only one thing. What about code 
use? Yes. Does it mention code use somewhere in there? Definitely. What does it 
say? 

[00:18:12] **Barak:** Yes, it does. Code review is, is essentially one of the, 
well, very, very strong suggestions in the s sdf. Mm-hmm. Because we don't want 
Programmers to just push changes through without anybody looking at them over.

Sometimes a code review is being done automatically, but the s SDF recommends 
that at least two people would, or at least two, I, I wouldn't know, wouldn't 
necessarily say people two eyeballs or, or two sources would look at code before 
it's being pushed through. So one of these could be an automated test, but the 
other should be human person.

Just like code review, for example. Two FA is also mentioned. Automatic testing 
on the pipeline as mentioned. Having people in charge of, of thinking about 
security from the minute you're designing a product and up until the moment it's 
no longer viable and you need to inform people having a plan in place to what to 
do if something bad does happen.

Who do you tell? How do you inform people? When do you inform? All very 
important. A couple of really bad examples. Some, there's a lot of companies who 
are being hacked left and right everywhere. Some of the news that are coming out 
of it are more than six months later. You get a piece of news that six months 
ago this and this company was hacked, and, and consumer information was stolen 
and then used, and they only inform everybody six months later, what, what does 
that.

everybody who could have used that information already did. If your identity was 
going to be stolen, it already was your social security number, your credit card 
number, assuming it was part of the information, is already out there for six 
months, so knowing six months later doesn't gonna help anybody.

[00:19:48] **Michaela:** and also they give us, did they give a concrete 
timeline when you have to inform everybody or is it very vague? Normally all 
these things are very weak. Yeah. S 

[00:19:58] **Barak:** SDF is, yeah, the SSD F is vague on purpose cuz it's 
trying to be true for everybody. Mm-hmm. . But I think CISA has recently, I, I 
think last week.

As is starting to work on a new timeframe, I think that between 24 and 48 hours 
timeline to inform everybody is, is what is correctly suggested. We have to 
remember that if you were affected by some sort of hack or ransomware or 
something, the faster you inform other people, the easier it would be for those 
people to create a defense or be prepared or not fall for the same trick if you 
wait six months just because you want to look good.

Shareholders, you're basically just perpetuating the same problem and the bad 
guys just have an easier time doing the same trick over and over for everybody. 
Yeah. But you 

[00:20:42] **Michaela:** also need time to fix it, right? Like if it's a, if 
it's a real vulnerability, you need time to fix it. And I think 48 hours is very 

[00:20:50] **Barak:** unrealistic.

You don't, no, no. You don't have to fix it immediately, but you need to inform 
it. Again, you don't necessarily have to inform the public in 24 or 48 hours 
mm-hmm. , but you do need to inform let's call it the relevant. Groups. Cisa, 
for example, is not just saying, tell us and we'll do nothing about it.

Tell us, and we might be able to help you. Let's all share the information even 
if you don't tell the public, because sometimes the public has a right to know, 
but even if you don't at least tell us we have more resources. You're not alone 
in this. We all want to make ransomware and hacking more problematic for the 
people who practice it less profitable.

And we can all share resources of this. This is a, a national. Especially if the 
hack that you think is nothing, just to steal some, I don't know, some user 
emails might be from a nation state, might be somewhere down the line. A matter 
of national security. You might not have all the information. So share with us.

We have more resources we can call on additional help. We can all work together 
to make not just your hack, but everybody's hacking. Less profitable, less, more 
time consuming, more problematic for. It's, it's a, a new idea that might be 
familiar to something what's called cooperation and working together.

I really appreciate the new head of cisa, who's really working hard on, on 
creating the connections with the right communities. She recently visited the 
Black Hat Con Conference and spoke on stage. She said that humility is very 
important. She's not there to tell them what to do, but she is there to.

That they work together, the request that they cooperate, that they share 
information because again, the more they cooperate Seesaw hackers, the, the 
civilian market companies, the more all of them work together, the harder it 
will be for the bad guys to succeed. Yeah, 

[00:22:36] **Michaela:** that's true. I totally agree. And maybe you can tell 
me, but if I would be in, let's say, maybe.

unexperienced, C E o or cto, right? And something happens like you probably 
completely freaked out and then reaching out to other people. And in a 
capitalistic world, I can't imagine that somebody is helping us for free, right? 
So if you are telling me that a lot of organization that seem very impressive 
will now start to do.

I see our ship sinking much faster than if I would just shut up my mouth, which 
obviously is not, you know, not what I recommend, but I'm just talking about how 
you might feel, right. You might feel intimidated that such a large organization 
somehow now looks on your fingers, maybe once you know, consultancy fees that 
you can't pay and so on, right?

I don't. What's going to happen? Is it all for free? Do we get for free help or 
? 

[00:23:31] **Barak:** It is. It is for free. Congress has approved the gigantic. 
Budget for this. There. The White House even has a, a ready room for, for, you 
know, taking care of hacking as far as I remember. And the White House, I think 
earlier this year even had a special conference day for helping secure open 
source the uh, Google, Microsoft pledging millions of dollars working with very 
well known bodies like the Limits found.

To I think that the project is called the Alpha Mega Project, working to secure 
open source projects because, again, open source projects could be maintained by 
a single person, and if that package is extremely useful, well known, well 
downloaded, and suddenly it has a vulnerability. , there's nothing you can do 
about it.

So the idea is to secure the open source packages that they're sourced to help 
the maintainers and, and the people who work on this to be more secure, both in 
the development and in the final packaging of those libraries. Uh, And millions 
of dollars are going into this so that whatever it is you end up using, if it's, 
you know, popular enough, they can't do everything, but they're starting 
somewhere.

And if those packages are popular enough and, and merit the intervention of the 
Alpha Omega project. , you will, you will get to know that. And, and they 
actually published a call for both people and companies who want to help. They 
have meetings. It's all very transparent. I highly recommend that if our 
listeners are interested, they should go and look it up.

The Alpha Omega project. Mm-hmm. . It's, it's an interesting project for 
securing open source. And again, the, the idea is that because these problems 
are not unique to a single company or even a single sector, they're everywhere. 
if people don't work together, they just make it easier for the bad guys to 
succeed.

[00:25:14] **Michaela:** Yeah, I mean, I recall when there was the Lockford J 
thing and then people shitting all over the open source maintainers while, you 
know, large organization making millions and, you know, are using that software 
without ever contributing back, right? Mm-hmm. . So yeah, I definitely see how 
that can work.

But you were only mentioning open source. What if I'm the CTO of not an open 
source thing? Because probably if I'm a cto, I'm not an open source thing. so. 
Some software that I'm selling mm-hmm. . And we are running into troubles, 
having some vulnerabilities. Can we also expect some help? 

[00:25:48] **Barak:** Or yeah, if you, you can at least inform, even if you 
don't request the help, which you don't have to, it's your software, it's your 
company, but you could, you should at least inform CISA of what happened so that 
they can add it to their database.

especially because some of these are not merely technical issues. They're 
relying more and more on human engineering. And the, the more those techniques 
are being published and known, the harder it is to use. I've recently read about 
a technique which was used to penetrate Cisco, which is, you know mm-hmm.

a security company. The technique is very simple. It's called two ffa. Fatigue. 
The, the bad guys are basically finding somebody who they think is susceptible 
and they keep sending them messages of two f a authentication over and over 
again via email, via phone. They just bombard them with messages.

Please authorize the two F. You need to authorize it. We need to authorize it. 
There's a problem you, some unknown has used. We need you to authorize, we need 
you to authorize eventually. sha sheer fatigue. They just click it and authorize 
it because they're tired. And at that moment they gain access. Yeah.

They bypass to put the two, eight, because they just got the authorization from 
the people, the person who's holding the code and they get in. Yeah, they, they 
only need a single person in your organization to fall for this, and they're now 
in your network. They can escalate the the permissions and do whatever it is 
that guys do with, they're in your network, which is usually some stuff that you 
wouldn't agree with or, or condone.

So yeah, as soon as people hear about this, they're like, Hmm, if I get a lot of 
messages, I should be suspicious. One of the fishing spearfishing is called that 
I myself have experienced and I, I know better, so I, I. I didn't fall for this. 
My CEO was in a conference in a different country, and I get an email early in 
the morning from supposedly my ceo, Hey, I need help.

I wanna buy something. And my credit card has been, Canceled. Can you please use 
your credit card by it? I'll, I promise you, I'll reimburse you. And this email 
looks suspicious because you know he's the ceo, he has his own credit card. Even 
if he can't use the companies, why would he be calling on me? And looking at it 
closely, I see that the email is not my CEO's email, it's just a random email.

They just changed the name to look like my ceo, and they must have seen from his 
LinkedIn that he's elsewhere. So they know I can't contact him because of the 
hour difference. So they use his name, supposed email and contact. , obviously I 
informed the company and realized that on the same day, probably the same guys 
have used the same trick on five or 10 different people in the company, the 
exact same email, and they're like, please help.

It's important. It's for the company. Don't tell anybody. I want it to be a 
surprise. Yeah. They're all these kinds of human engineering sort of, of tricks 
that once they're known once. You know, once you tell people about this, they're 
like, huh. It's obvious. If I, now, if I get an email like this, I'll be 
suspicious.

I don't know what to look for. But until you do, you might easily fall for this. 
It's early in the morning, you're still groggy. You just woke up, you know, your 
CEO is in the conference. It might be important you, your first instinct is, you 
know, if you care about the company, let's, let's help them out. It might, you 
know, it'll benefit the company.

I'll be praised. I'm helping, and you're just, you know. In this case, it would 
just, I would just be giving my, my credit card information. It could have been 
something else. It could have been. Please send me, you know, I don't know our 
list of clients. Please send me to this email. An un unlocked version of our 
source code.

I don't know, something like this because I wanna show an investor, whatever. It 
could be anything if you fall through. You've just put your old company at risk. 
Yeah. And this is exactly the type of stories that need to be out there, that 
people need to know about. And if you keep it quiet because you are embarrassed, 
because you know you wanna keep your profits, because it doesn't matter if the 
information leaked, as long as nobody knows about it, you're fine.

It's good in the short term. Everything comes out in the long run, you'll just 
look worse. . Yeah, 

[00:30:01] **Michaela:** probably . . I know that, you know, from a moral 
perspective, I totally understand and I also think everybody should share their 
thing. I just, you know, from a realistic standpoint, I'm, I can see how people 
not share it.

You know, they don't, they want, don't want to look bad. So maybe it would be 
cool if you could do that anonymously. Would that be an option? 

[00:30:24] **Barak:** You could, you could, yes. Yeah, you could inform them 
anonymously, because getting the inform. is better than not getting it at all. 
Yeah. They do accept anonymous you know, tips and they keep updating their 
vulnerability database.

They keep updating their exploit database. They have a webpage, cisa, I mean, 
they have a webpage full of tools that you can use to help secure your software. 
They're trying to be as helpful as possible. It's their job not just to secure 
the government's framework or network. Yeah. But secure the nation's you know, 

[00:30:57] **Michaela:** So probably it's also a trust issue, right?

Mean I'm in Europe. Definitely. So if you tell me about all these organizations, 
I'm like a little bit . I'm like, can I trust them? , excuse maybe the us you 
know, people are a little bit more have a bigger trust in, in, no. Okay. Nope. 
So I'm not alone cause I'm like, I'm getting a little bit stressed out if you 
tell me to tell somebody that I don't know.

And they seem like so. Big, important, you know, like intimidating. So I think 
that I definitely would I, I recall that you should do that and I probably will 
do it. I will do it, but it, it's not an easy call for me. You know, like if I 
would mess up, it's definitely not something that I think, oh yeah, I'm going to 
tell them.

It would probably take a lot of courage for me to think, yeah, let's do the 
right thing. Right? And I'm saying Big Brother to everybody do it. Big 

[00:31:47] **Barak:** Brother is always Big, brother is always watching. Is is a 
concern. Everybody, especially in your cybersecurity, which is exactly why the 
whole philosophy of shifting left exists in the first place.

The whole philosophy of zero trust don't trust people, so you don't end up 
having to call people you don't want to for help. And that circles a stack to 
where we started. , having more visibility into whatever it is you're doing, 
having more trust in whatever it is you're using should help. It won't eliminate 
the risk, but it should help minimize it to a point where the cases where you 
will need to call for help.

are smaller and, and further, you know, yeah. Further between again, using an 
SBO will give you more visibility into what you're using. Asking for SBOs from 
your third party suppliers would, you know, again, increase the, the visibility 
and use. There are multiple other tools which you could employ, like integrity 
verification reports digital signing to make sure that whatever it is you're.

Originated from the person that you're taking it from. Lots of different types 
of tools that can be employed to make sure that eventually what you're using, 
you have greater visibility and greater trust into the components. Yeah. So 

[00:33:00] **Michaela:** what's your, what's your take on all these automatic 
scanning tools?

Right, like I have static analysis that tells me. I, I've run that on all my 
repositories. That tells me if I'm using an unsecured version of some software 
mm-hmm. Obviously, probably there are some boundaries to, you know, how much 
that can help me. But maybe it helps me more than having an SBO that I have to 
manually look for.

[00:33:23] **Barak:** I don't know, like, you don't have to manually look for an 
. That's the beauty of the thing. The whole idea of using an SBAM is that it's 
standard. There are standards for creating. Several right now, but they're all 
still standard. And once you have a standard type of file, essentially adjacent, 
you know, with a standard structure, yeah, you can use automatic tools to scan 
it.

There are already automated. So open source tools for taking an sbam and telling 
you what vulnerabilities are in it, because again, it's a list. It's easy to 
scan the list and compare it to a database of vulnerability so you don't have to 
manually look at it if you don't want to. And 

[00:33:56] **Michaela:** second of all, yes, so is it already used?

Is that aspo? Maybe. Maybe that's my tools are already using. 

[00:34:02] **Barak:** Unless they tell you the, they might and they might not. 
SBO is relatively new and there's a big push to, to get it to, to more and more, 
to be more and more in circulation and use the, the key here is to get people to 
ask for it. 

You want your DevOps who work on the pipeline to make sure that no breaches 
happen in the middle of the pipeline at the end of it. And you want that when 
you end up delivering that software, either via a website, a server, a cloud 
service, or just putting an image on a repository, you wanna make sure that 
whatever it is you got, Is exactly what you indebted it to be, that nobody 
swapped it or changed it or modifying it unintentionally, or, you know, with 
intention, usually a bad one.

The more of these steps and, and protections you take, the better you are. 
Obviously if you can show them to people. , if you can say, yes, I'm secure. 
Here's a document that shows all the tests and they're signed. Here's an SBO m 
with my final product, and it is signed as well. So you can verify that I am the 
one who produced this SBO m and nobody else did, so that you know that it wasn't 
modified.

Again, the whole thing is there to give the people who were going to use that 
image, the security, that it is legit, that it is fine. And that is exactly the 
type of confidence of security of, of trust. That is the one you mentioned is 
missing. Cause right now there's not a lot of automatic trust anywhere, 
especially the way the world is today.

[00:35:28] **Michaela:** Yeah, yeah. You just created four new positions, at 
every company. , every single company. No. Yeah, I totally agree. My whole 
point, maybe for the whole thing, It seems very overwhelming. Right? And as an 
expert, you know that we are far from what you are describing. So what are the 
first steps that I can do?

Like say I'm this startup. You know, we have a couple of people we are, you 
know, still thinking about, you know? Yeah, yeah. Can we even add that one more 
position? So what's the first You don't 

[00:35:58] **Barak:** even have to have any positions. You don't even have to 
have any positions because just like anything else, a lot of the tools that I 
described, you can get a proprietary version obviously.

Open source is there for the rescue. There are open source tools for generating 
ASBOs. There are open source tools for scanning ASBOs for vulnerabilities. Those 
are the two. You know, from my perspective, two of the things that you can I uh, 
implement in your pipeline immediately, even if you're a single developer, even 
if you're just building a P O C in your mom's garage, your basement, why not use 
them?

It's fun to play with these things just to see the usability and I'm pretty sure 
that once you input an sbam, any sbam, even if it's not yours, if you input an 
sbam into the tool and, and check out the list of vulnerabilities, you're like, 
Hmm, this is really useful.

I should input that in my own pipeline. 

[00:36:45] **Michaela:** Yeah, yeah, exactly. So I will definitely try that out. 
I can see the usefulness. So yeah, thank you so much for explaining everything 
to us today, and I will link the tools that you just mentioned, you know, not by 
name, but that one that you have in mind.

So I will link them in the show notes and so everybody can try them out. Yeah. 
Thank you so much Barrack, for being on my You're welcome. Show today. Yeah, 
very welcome. Okay. Have a good. You too. Bye bye. This was another episode of 
the Software Engineering Unlocked Podcast. If you enjoyed the episode, please 
help me spread the word about the podcast.

Send the episode to a friend via email, Twitter, LinkedIn. Well, whatever 
messaging system you use, or give it a positive review on your favorite 
podcasting platform such as Spotify or iTune. This would mean really a lot to 
me. So thank you for listening. Don't forget to subscribe and I will talk to you 
in two weeks.

Bye.


