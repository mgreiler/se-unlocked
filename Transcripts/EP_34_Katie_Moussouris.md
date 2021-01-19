# Katie_Moussouris_Ready


**Michaela:** [00:00:00] Hello, and welcome to the software engineering unlocked 
podcast. I'm your host, Dr. McKayla. And today I have the pleasure to talk to 
Katie Moussouris the founder and CEO of Luta Security. 

But before I start, I wanted to introduce you to ConfigCat - 
who sponsors today's episode. ConfigCat is a young startup that revolutionizes 
feature flag management, and met with one of the founders two weeks ago,
and he walked me through the main features of the tool. They are super 
enthusiastic about ensuring every company from small to large can release new 
features rapidly with less risk by using feature flags. ConfigCat lets you hide or 
expose features in your application without redeploying the code.
What's really cool is that it's designed for both developers and product 
managers. Also less tech savvy people are up and running within 10 minutes of 
training. 

ConfigCat supports, JavaScript, React, Python and Java. Well over 13 
different languages and frameworks. I have seen how seamless and 
effortless it integrates and how powerful the configuration management behind 
your flags is.
They offer an extremely generous free plan. And with each paid plan, they plant 
a tree. So, well, I can tell you I'm in love with this company and the product. 
So, I really hope you check them out at [configcat.com](https://www.configcat.com). 
But now back to Katie.

Katie is the founder and CEO of a new security startup company called Luta 
Security.
Luta Security specializes in helping businesses and governments work with 
hackers and security researchers to better defend themselves from digital 
attacks. Katie is also an expert when it comes to back bounty programs and also 
how you successfully prepare organizations to implement one. So I'm super 
thrilled to have Katie here with me, Katie, welcome to the show.

**Katie:**  [00:01:40]  Thank you so much for having me. I'm really happy to be 
here.

**Michaela:**  [00:01:43] Yeah. I'm also really, really thrilled. So 
Katie, can you tell me and my listeners a little bit more about security, 
vulnerability programs? What are those and why should we care?

**Katie:**  [00:01:53] Well, everybody has heard of, you know, security, 
bugs. They cause a lot of hacks, a lot of breaches, a lot of losses and you 
know, caused a lot of problems.
So why should we care? Well, it's because we run on a lot of software and 
hardware and all software and hardware contains bugs because it is designed and 
implemented by human beings. And we, we are flawed. And so, so why should we 
care about vulnerabilities? Because we should really care about the safety and 
security and privacy of the world we live in.
Yeah. 

**Michaela:**  [00:02:28] Yeah. And so what are when their ability disclosure 
programs in particular? So how can you imagine that is that, that I'm, you know, 
designing some processes so that other can report box, for example, that they 
find, or is that also something that happens internally? 

**Katie:**  [00:02:45] Well, vulnerability disclosure is a term that is used to 
describe, you know, letting somebody know about a vulnerability.
It was actually originated by the hacker side of the equation, security 
researchers, as, you know, some companies refuse to call them hackers, but I am 
a hacker, you know? And, and so the term itself was about how will hackers. 
Disclosed vulnerabilities either to the public to let them know that they're not 
safe and what steps to protect themselves or disclose the vulnerability to a 
software vendor, usually, you know, to tell them about it so that software 
vendor can fix it and then issue a patch or an advisory or something to tell its 
users what to do.
But the term vulnerability disclosure actually originated with hackers. It then 
became adopted by organizations who want to create a process to receive 
vulnerability reports. Or it's and then disclose, you know, the outcome right. 
Of their investigation, either nothing to see here, you know, this wasn't 
actually a bug or an actual software patch or, you know, were fixed and an 
advisory.
So that is the process of own disclosure. As we know it today. And 

**Michaela:**  [00:03:54] so I imagine I'm like a company and obviously my 
software probably has some security holes, some vulnerabilities. And so if 
people are coming and hacking my side, is that a good thing or is that a bad 
thing? So do I want people to come actually come and find issues on my side?
Or do you want them to stay away? 

**Katie:**  [00:04:14] Well, you definitely want a mechanism that if somebody 
notices something wrong with your site, you know, that you'd have some mechanism 
to receive a vulnerability report from the outside, but that should not happen 
before you've actually looked for vulnerabilities yourself.
And that is something that is. Hugely important and often overlooked. When 
people look at vileness Gaucher programs as sort of an end goal to their 
security, where once they do that, then they're, they're all good. And they'll 
just wait for the public to tell them about vulnerabilities. That's a very 
inefficient mindset.
So yes, you should have a way for people to report vulnerabilities to you from 
the outside. But if that's your primary source of learning about 
vulnerabilities, Then you are not a very secure organization and you have made 
very unwise choices and investments in what you've decided to do first. Yeah. 

**Michaela:**  [00:05:06] So, and if I'm, let's say I'm ordinary, maybe a little 
bit smaller company, maybe a young company, I don't know, you know, something 
like this and we have developed software and you know, this is what we mainly 
do.
We think this is our business goal, right. And we want to go to market. And so 
our main resources are software engineers that are working on our system. What 
would be some of the first. Steps. If we are in self note that we haven't 
invested enough insecurity, what should be our first step to make our system 
more secure and, you know, detect and close our own vulnerabilities.

**Katie:**  [00:05:42] Well, I think that it's super important to incorporate 
the principles of, of a secure development life cycle. Meaning you're building 
security in at every stage, starting with the design phase and architecture 
phase, and then going into, as you start to implement the code yourself, doing 
static and dynamic analysis.
Do you have any code reviews and making sure that you've left enough time to 
address any of those issues? I've seen organizations say, yes, we do a secure 
development lifecycle. Yes, we do. You know, static and dynamic analysis, pen 
testing, code reviews ourselves. But I see it so late in the process that 
there's really not enough time left by the organization to address any issues.
And they just released the software anyway. Knowing about serious bugs and just 
saying, they're going to, they're going to catch them in the next update or the 
next major release. And you know, so I think that organization is thinking about 
this as what should we do as our first step. It's always invest internally to 
try and reduce the number and the severity of vulnerabilities that even cross 
your front door threshold.
And then from there, you know, then set up, you know, a way to receive 
vulnerability reports for anything that you missed, but definitely don't leave 
it to the outside. That's according to NIST guidelines and documentation says 
that. It's up to 45 times more costly to address vulnerabilities after software 
has been released, as opposed to finding those flaws as early as the design 
phase.

**Michaela:**  [00:07:12] Yeah, and that's, that's really good. And so if you 
have like this software engineers, do we train them or do we hire, you know, 
specialists, security specialists? Do we outsource that? And what would be, you 
know, your procedure here? Let's say we don't have really a lot of security. 
Experts now in our 
organization.

**Katie:**  [00:07:31] Well, most organizations don't have security experts and 
that's a reality that we have to face as well. So I think that, you know, 
training them ideally is, is helpful creating, uh, software development 
environments. That have tooling that supports more secure engineering practices. 
You know, there's, there are things built into various SDS that make it harder 
for you to make certain types of coding mistakes.
I think that's important, but then I also think that it's important to bring in 
outside expertise. You are not going to have all of the internal folks knowing 
what, you know, a security expert of many years is going to know. So bringing in 
outside experts is super important. You know, even before you've released the 
software.
And before you look for crowdsourced help in the term, in, you know, in, in the 
form of vuln disclosure programs or bug bounty programs, you should actually be 
hiring professionals, professional pen testers, professional code reviewers, 
professional security, architects, and security architect, reviewers. And if you 
can't afford to keep them year round as full-time employees hiring them on a 
contract basis is absolutely essential before you go to market.

**Michaela:**  [00:08:40] Yeah. So actually one of the things that come to my 
mind is that very recently in one of the groups that I am in S uh, some, you 
know, startup group and so on, there was a question about, you know, how to do a 
pen test and how to get pen testers, and they actually recommended your company 
there. And then they decided, no, we are doing it.
In-house we will learn that. Right. And so it's like, One really not technical 
person and one engineer and it writes the whole software system, and now they 
are also doing the pen tests. And I think most of the pen testing was actually 
done by the non-technical person. Right. And, but I heard about it. I was like, 
yeah, I don't know if this is really something I would advise, but what's your 
take on that?

**Katie:**  [00:09:20] Well, I mean, I'm sure I'm sure they probably uncovered 
some yeah. Issues and it was a great learning experience, you know, and, and 
certainly that will strengthen the ability for those internal people to not make 
those precise same mistakes again, but you can't exactly, you know, just throw 
an anatomy book.
Into the woods and hope that surgeons come out, right. You know, you, you, you 
do need training and you do need expertise to get the most coverage. And I think 
that's, that's the most dangerous part of the scenario that you described is 
that they may feel like they, they did, they did the best, you know, their 
ability, but.
There's no guarantee there with non-expert sort of teaching themselves that 
they'd have the code coverage, that they need to be more secure. The confidence 
that their architecture review really took into account, true security threats, 
which over time, you know, as, as pen testers and reviewers, we, we know what 
these patterns are, you know, and everything.
And it's not going to be like a brand new problem every time. So while I commend 
them for using this as an opportunity to broaden the skills of their internal 
folks. And that's definitely the right thing to do on that front. It's 
definitely not going to be as, as effective at securing your products.
Then if you were to hire true experts to come in and do it for you. 

**Michaela:**  [00:10:38] Yeah. And so you were talking a little bit about 
cultural views and, well, when I was working at larger organization, we had like 
code reviews, which were done by software engineers. And they were mainly about, 
you know, obviously also a little bit about security, but it wasn't the main 
focus.
There was a lot about maintainability readability of the code, right. Also, you 
know, is this even the right feature that we are building? Right. So business 
aspects that we are having here, and then a lot of the code actually went 
through a security review, which was very separate step. Is that something that 
you see that's very common?
Is it something that you recommend or should it be security? Or if, if maybe as 
I said, there's a longer larger organization. If you're not having those larger 
organizations, do we have the security aspects in our daily code reviews? Or 
should we as a software engineering team, maybe set times aside and say, well, 
this is now a dedicated security review of a larger part of our 

**Katie:**  [00:11:30] organization.
Well, I've seen, I've seen different models work best because you are trying to 
balance, you know, getting, getting that software out to market what your 
internal resources are and what their skillsets are and what budget you have to 
bring in external eyeballs who are experts. And I think there's a lot of 
balancing going on with that.
But the scenario you described, you know, honestly, you know, I think that 
dedicated resources and dedicated steps. Devoted to security and security 
reviews are very, very important. And the sooner organizations build that type 
of, you know, dedicated security effort into their processes, they'll actually 
find that their code is more maintainable, that their code is more, you know, 
is, is more robust and efficient because, you know, as we know a lot of the time 
a security hole actually manifests.
As a crash with an unintended input causing a crash, that's a reliability issue. 
So if you know, orgs are really focused on reliability, when it comes to code 
reviews, it shouldn't be that much of a stretch to explain that if you dedicate 
specific time for security, you're not necessarily adding a lot of effort in one 
area that is disproportional.
It actually informs and, and assists in the efforts that you were already doing 
for other reasons. 

**Michaela:**  [00:12:50] Yeah. And so you were talking about some of the 
software engineering practices. You were talking about static analysis, dynamic 
analysis, right? Having your IDE configured in a way, you know that you cannot 
do some of the issues.
Maybe there are also like pots during the code review that tell you, you know, 
something is, is wrong here, but you were also talking about the. Design phase 
already. Right? So we are starting really from the beginning. And the security 
is part of our considerations, even maybe before we are building software.
Right. So how do we, how do security experts now interplay or collaborate with 
engineers? Are they there in a team? Do you like, for example, some of the 
engineering teams have like squats or packs, what they call right. Where we have 
different roles and responsibilities and expertise in one, you know, Autonomous 
cycle are where they can really do their, their, their thing independent of 
everybody else.
Or do you say, well, there's like in a security part of our company and that 
hops in from time to time or certain, you know, uh, steps or something like 
this. 

**Katie:**  [00:13:58] So. You know, the, your question to me comes down to, do 
you embed security into the product teams themselves shelves, or do you have a 
separate product security function, you know, in terms of reviews and approvals 
of from a security perspective, right?
There are pluses and minuses to doing it both ways, you know, you and I share 
some Microsoft DNA right in our past. Careers. And Microsoft actually developed 
an interesting way to try and divide who needs a full security review with 
dedicated security personnel versus who can sort of have, you know, essentially 
a security champion embedded within the product team that can do, you know, an 
appropriate level of security testing, review checking, running of tools, et 
cetera.
And I think the, the. The way that Microsoft used to fork these projects was 
having developers at the start of developing either a feature or, you know, even 
a brand new product going into internal tooling and essentially determining what 
the relative. Risks are for that component or that software. And if you do it 
based on this software or this component is going to be taking input from 
outside users or untrusted inputs, or it's going to be attached to the internet, 
or it has some other high value function.
Then perhaps those ones would benefit from a dedicated security review, as 
opposed to being just trusting it to the security minded folks who, who live 
inside that product team. Cool. And so one 

**Michaela:**  [00:15:32] other area that I wanted to talk with you about is 
because you said reliability and whenever I hear reliability, I think about 
data, right?
And so data breaches are, you know, everywhere. And somehow I also feel 
organizations don't really take our data. With a lot of, you know, they don't, 
they take it lightly, let's say right. If it goes, it gets out, it gets out, 
well, I'm sorry. You know, your credit card, your street address everything 
that's private to you to leave then is somewhere.
And then we pretend it might not be happening to you. Right. So it's only like a 
small percentage of, you know, our records, millions of records. It's only like. 
30% of our records that went out. So it's probably not user every time I get an 
email, I'm like, Oh, I think it's not me. So we are all a little bit more at 
ease again.
And we forget about these data breaches, but what can we actually really do 
about these data breaches? Are, can we prevent down, can we do something 
internally to really make sure the data is secured or you know, is safe? Or 
should we outsource that too? You know, some services, for example, that store 
the data.
What's your, what's your take on that here? 

**Katie:**  [00:16:42] I, I think that, you know, the, the most common it 
practices are what people are struggling with, but even as we've just seen with 
some of the targeted attacks that have been hitting the news this week, you 
know, you can do. As many of the best practices as possible.
And you know, if there's an adversary, who's determined they are going to get to 
you. Right. I think that we do struggle as an industry with, with nailing the 
basics. And it is often breaches are often not due to a software vulnerability, 
but actually due to fishing the human factor. So, I mean, I think there's a 
number of different technology things you can do, obviously encrypting your data 
at rest and in transit, limiting the number of people who have access to this 
data, limiting the API APIs that have access.
The system, that data is another overlooked area, you know, that often gets 
abused and, and results in some of these breaches. But, you know, I think it's, 
it's a really broad, broad topic. I, for one, you know, think that we're not 
going to get, we're not going to get, you know, one, one. You know, big umbrella 
answer that will stop data breaches.
I think that, you know, we'll, we'll, we'll always have targeted attacks that, 
that, um, end up being, being a big problem. And then, you know, for, for the 
majority of them, you know, still being because of phishing attacks that we see 
breaches and in fact, the. The Verizon, the Verizon breach report, you know, 
used to be a great kind of publication and tie, you know, fear, uncertainty and 
doubt publication because they had data on breaches and it was less than 1% of 
the breaches were typically due to a zero day.
Vulnerability. Most were either. Fishing next down from that are vulnerabilities 
that have been known and patched for a very, very long time. So the 
organizations just hadn't applied the patches yet, and the breach happened that 
way. So I mean, every organization is going to be different as to what their 
answer and what their key takeaways are for, you know, a breach that happen to 
them or a breach that they could potentially learn from, from the outside.

**Michaela:**  [00:18:43] Yeah, one, one, I actually watched a talk off you very 
recently at this conference called friends of Europe. And before your talk, 
there was actually one governmental person talking. I don't know exactly who she 
was. I forgot to be honest, but it was very, very interesting topic to me 
because I've never heard of it.
And this is that during COVID, there were a lot of attacks on, you know, 
hospitals, governments, and so on. Do you know about them and why is it have 
happening? Why are people, you know, I understand this idea of being a hacker, 
being, you know, a researcher to do that. And why would we attack for example, 
hospitals, or, you know, in, in, in such a very delicate situation, do the, do 
people want money or what do they get out of that?

**Katie:**  [00:19:30] Well, yeah, I mean, the, the attacks do sure seem to be 
ransomware related, but I remember at the beginning of the pandemic, actually 
some well-known ransomware groups said that they would not deliberately attack 
healthcare facilities, criminals have that code of honor though. And, and I 
think there was also a lot of unintentional targeting that that occurred, which 
is always the case when you've got a very big internet and these, these 
attacking groups.
We'll scan, you know, big subsets of the internet and wherever they find 
victims, they're not necessarily targeting the hospital, but they may get caught 
up in a broad un-targeted attack looking for malware victims. So I think that's 
really where, where at least some of the initial infections were coming from, we 
did see some of the criminal groups say, we promise, you know, we're, we're not 
gonna, we're not gonna lock up hospitals, et cetera.
And then some who, you know, Don't really care, you know, in particular. And 
also knowing that causing a disruption in healthcare facility has a very high 
chance of a ransom in a ransomware situation being paid for, to avoid loss of 
life. 

**Michaela:**  [00:20:44] So I know that you are working with governments, 
you're working with military, not only with businesses, and this is something 
that I find really fascinating.
And when I think about it, I imagined that it's extremely strict rather than 
military, very rigid and. It's almost a little bit frightening, but also I 
imagine that military systems are probably the most secure ones that, that you 
come by duty even need help from, from outside, from expert security experts.
And in which way is it different to work with them then, for example, with, you 
know, an ordinary business. 

**Katie:**  [00:21:16] Well, you know, in my work with the, with the us military 
over the years, they are moving towards embracing more of what private industry 
does. Right? The whole initiative of hack, the Pentagon was basically one of the 
first initiatives coming out of a new program at the Pentagon called defense 
digital service.
And I think that, you know, The desire to evolve and work with private industry 
and follow private industry, best practices is, is absolutely there. But I think 
it's a misunderstanding that, you know, military installations are going to be 
the most secure because there are a lot of different regulations and different 
rules about even how quickly they can deploy a patch.
Right. So, you know, if you think about it, availability from a military 
standpoint is. Probably going to take a lot higher priority than patching 
something that may or may not get exploited. Right? If you were supporting a 
military mission, you are not going to, you know, necessarily do a downtime 
maintenance window to get all of those patches out.
So. Does the military need help? Yes, absolutely. As all organisms patients do. 
And also something else to consider here is that we're at a global shortage of 
cybersecurity professionals filling open job roles that exist right now. I think 
when we get into the government space and military space, you run into issues 
of, you know, in the military, you're dealing with folks that are enlisted and 
trained or recruited and trained in how to do.
Cybersecurity, cyber warfare, et cetera. In government, you are dealing with 
government pay scales, not being anywhere near close to what a person could earn 
in cybersecurity in a career in private industry. So I think that there are a 
number of different factors that are involved in, in. You know, securing 
military organizations, government organizations, and they're not necessarily 
all the same or they're all in, they're not necessarily straight forward with 
the same issues that we see in private industry.
There are some overlaps, but there are different kinds of priorities and 
struggles. 

**Michaela:**  [00:23:31] Yeah. Yeah, I totally see that. And also I think if 
you are thinking about, you know, how many people there are in the government or 
in the military, and then, you know, compare that with the sheer amount of 
people and knowledge and brains and, you know, expertise that we have outside, 
if you can tap into that, uh, it's obviously extremely.
Valuable right. Also different experience, different backgrounds. Yeah. So 
Katie, I wanted to talk a little bit with you about your intrepreneurial journey 
because I know looter security now is like five years old. Something like 
this 

**Katie:**  [00:24:02] it's like four and a half years, 

**Michaela:**  [00:24:04] but yeah. Yeah. And so how does, how did that get 
started?
Why did you start doing your own thing? And was it hard at the beginning? 

**Katie:**  [00:24:12] It's, you know, it's hard and it's fun. It's both of 
those things at once. You know, I'm, I tend to be kind of a workaholic and it's 
really funny because at Luta I've, I've managed to not exactly break that habit, 
but at least confine it to 32 hours a week.
So, you know, in my entrepreneurial journey, I've, I've discovered that that 
actually working. Longer hour is not necessarily going to get me the same return 
as working more efficiently and trying to fit that in. But why did I start the 
company? Well, you know, there's the saying that entrepreneurs are insane.
And they're insane in a very specific way where they get irrationally upset 
about a problem that they are convinced that they can solve. And, you know, I 
think I've been irrationally upset at how poorly vulnerability disclosure has 
gone over the last like 20 plus years that I, you know, I agreed when I was at 
Microsoft to work on ISO standards.
Now, a hacker working on international standards. Creation just seems like the 
torture that it really was, you know, but, but it was important to spend that 
decade of my life working on those standards because you know, it enabled us to, 
to shape a different way for companies and governments to interact with hackers.
And one of my earliest goals for the first time I went to Def con back in 1999, 
Def con seven, as I watched my friends from health of the dead cow and, and. 
Throw, you know, USB stick or throw out copies of it was, it wouldn't have been 
USB sticks. It would have been CDs of back orifice back then, which was their 
hacking tool and realizing that, you know, In terms of our ability to contribute 
knowledge to the world.
You know, it was pretty much limitless, but we had to, we had to figure out a 
way to have the world hear us and not dismiss us as, you know, a bunch of cyber, 
you know, cyberpunks basically, so I think that, you know, from my 
entrepreneurial journey, one figuring out that. I, I knew a better way for 
organizations to interact with security researchers and outside reporters of 
security bugs, but also, you know, a way that kind of blends the world that 25 
years ago, I would have been punk rock rebelling against, you know, the 
corporate and military world of computing, but find a way to blend, you know, my 
hacker mindset.
And my desire to change the world in, you know, in a bigger way than one bug at 
a time is really what, what. Drove me to start my company. Yeah. It 

**Michaela:**  [00:26:57] sounds very exciting. And I think if you have like 
this mission and this passion for something, I mean, it can, it can only go in 
one direction. I think that that's, that's the good direction.
So another area that I wanted to quickly touch on before we are wrapping this 
interview up is what, what advice would you give to people that want to become 
Heckers right. So what are those first steps? Is this something that you can 
learn on a non-traditional path? Can you go online and read about.
Security is, can you maybe go into some of those security challenges, maybe be 
in a team that, you know, have different expertise and you can learn from, or do 
you think there is a specific way how you can become a hacker and also in a 
hacker in a very professional way, right? Where you can earn your, your you're 
living with it and, and, you know, positively contribute to our, our society.

**Katie:**  [00:27:48] Well, you know, when I had done some labor market 
research on the vulnerability economy and exploit market, I did it a few years 
back with MIT Sloan school as a visiting scholar. What we found is that hackers, 
their longevity of being sort of at the forefront of, of their profession 
hacking is about seven years.
Total. And the reason for that, you know, and I say this because you asked how 
do you become a hacker, right? What I'm saying is you can be kind of a hacker, 
but you have to think past what are you going to do seven years after that? 
Right. And that's not a very long time. The reason it tends to sort of do this 
bell curve of, you know, at the peak of your, of your hacking career, you know, 
it tends to be a seven year span is because technology changes.
Technology changes. It becomes more complex. You saw buffer, overflows, you 
know, very easy to find and exploit. Now, if you find a buffer overflow, there 
may be a number of different mitigations in place where you were lucky to find 
it, but good luck to you. And it's a different skill set almost in trying to 
explain it.
So we see hackers sort of spanning their hacking career part of their, their 
professional career of about seven years. So what I would say is. If you're 
thinking about making, taking a turn into hacking and have that be a chapter of 
your career as it has been for mine. Just think about what area are you the most 
interested in making an impact?
You know, several years back, a lot of hackers started looking at medical 
devices and the reason was because they wanted to make sure that, you know, as 
these things gained, internet connectivity and functionality, which they had not 
had before that, you know, We weren't exposing medical patients to something 
worse than having to install a software patch at an inconvenient time.
We were concerned about, about human life. And so if you're interested in, in 
these types of things, you know, there's a number of different. Online forums 
that you can, you know, that you can start reading. There are capture the flag 
competitions, you know, that provide a safe learning environment where you're 
learning how to not just think like a hacker, but actually try and gain access 
much like a red team or would.
And there's a lot of different jobs that are hacking related. And are absolutely 
essential to security, but don't require the hacker skillset per se. So I would 
encourage people who want to get a job in cybersecurity that don't just look to 
the hacker pathway that happened to be my pathway, but perhaps it's because I 
was not as good a software developer as I should have been.
Right. And that breaking code was easier. So maybe that was why. That's how I 
chose to contribute. So find your own path and be flexible with yourself. Always 
keeping in mind that seven years from, from whenever you've made it as a hacker, 
you may be desperately looking for something more stimulating or broader in 
terms of your scope and your ability to change the world.
Yeah. I, 

**Michaela:**  [00:30:45] I really like, and it very resonates with what, what 
resonates with me what you said, because what I always find really tricky is 
those labelings, right? So whenever I have to label myself what I am, right. Am 
I a software engineer? Am I a researcher? Right? Am I an entrepreneur it's 
really hard for me.
And I think maybe it's here. It's also a little bit more fluid, right? You're 
are, you could be security interested, right? You could work in a, you know, in 
a security related field. And I think it very much connects also to what we. 
Talked about that it beginning where we have like these different teams and 
where are the roles that people can take on right within the team or maybe in 
the security team.
And so I think maybe this can also be fluid. Maybe at first you are a software 
engineer and you are more interested or more passionate about the security 
aspects. And so. Yeah, probably it's, it's your passion, your interests, what 
you're learning, but also the opportunities that you get, right? It's not 
always, I mean, opportunities are not always handed out, especially for certain 
folks, right?
It's sometimes you're waiting and you don't get the opportunity. And so this, I 
think shapes also our paths and I liked that. You said, well, there are many, 
many roles that you can take on and maybe you're going, you know, not the 
straight line to. No I'm here and I want to become a hacker, but it could be 
that you're going a little bit around.
Yeah. Katie, I'm so happy that you have been on my podcast today. Is this 
something that you still want to say to my listeners, to my audience, that you 
want to, you know, leave them with a message somehow, if you think it's 

**Katie:**  [00:32:14] important. Well, I do think it's important to note that 
Luta security is tiring developers.
And I think that your audience is probably one of the best places I can make 
that request for, you know, for folks to check out Luta security.com/careers. 
And we'll be posting some developer roles up there shortly. But I think that 
that overall, you know, the, the, the, the only other thing I would say is, you 
know, if.
Folks are thinking about moving more into security as their full-time job, there 
is no limit, you know, and you can define your role and your job as you know, as 
you like it. I think that that's something that people overlook about 20 years 
into the professionalization of, of the security. Career set is that it's fixed 
in stone and that you have to go to school for it.
I certainly didn't go to school for it. I went to, I didn't even go to school 
for computer science. I went for molecular biology and mathematics. So you can 
come from a different background entirely. And I think the future. For us is 
getting people it's a lot easier to train a developer on security and secure 
coding and secure architecture than it is to train a non-developer on how to 
properly architect and fix those things.
So it's, it's easier to go from a different technical area into technical areas 
around cyber safety security. So I would just say that, you know, folks should. 
Feel confident in that nobody has a map that is going to work for everybody else 
and that you have to draw your own. 

**Michaela:**  [00:33:51] Yeah, I really liked it. I think this a wonderful 
closing words.
So Katie, thank you so much for being on my podcast today for spending those, 
um, minutes with us and sharing so much of your wisdom. Thank you so much. Thank 
you. Thank you for having me. Yeah, it was my pleasure. Bye bye bye. 

Well, before you go, let me tell you that my code review workshops are starting again.
So if you want to transform your code review practices from bottleneck to 
superpower, check out my training at 
[awesomecodereviews.com](https://www.awesomecodereviews.com). 

So thank you for 
listening to another episode of the soft engineering and unlocked podcast. Don't 
forget to subscribe and I talk to you again in two weeks. Bye.


