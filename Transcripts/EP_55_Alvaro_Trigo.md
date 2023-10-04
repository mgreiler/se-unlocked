---
episode: "Transcript Make money with open source software"
permalink: /money-open-source-software
status: publish
type: transcript
---

[00:00:00] **Michaela:** ( *intro music begins* ) Hello, and welcome to the 
software engineering unlocked podcast. I'm your host, Dr. Michaela. And today 
I have the pleasure to talk to Alvaro Trigo, a web developer, who enjoys 
learning every day. But before I start, let me tell you about an amazing 
startup that is sponsoring today's podcast, Codiga. Codiga is a code analysis 
platform that automates the boring parts of code reviews and lets you merge 
with confidence on GitHub, GitLab and Bitbucket.

I've worked at Codiga for around one year now and I love how it guides me in 
discovering and improving, well, the not so nice parts of my codebase. But 
there is more. Codiga also has a coding assistant that helps you write better 
code faster. Find and share, safe and reusable blocks of code within your 
favorite IDE on demand while you're coding.

Codiga has a great free plan. So, ( *chuckles* ) there's nothing that stops you 
from giving it a try. Learn more at [Codiga.io](https://www.codiga.io/?utm_source=podcast&utm_medium=social&utm_campaign=se_unlocked). That is [Condiga.io](https://www.codiga.io/?utm_source=podcast&utm_medium=social&utm_campaign=se_unlocked).

But now really back to Alvaro ( *intro music ends* ). Alvaro created his first 
website at the age of 16 and did not stop learning and perfecting his craft. 
One day, he started to make JavaScript plugins and well again, to learn and as 
an experiment.

And three years later, he earned enough from his experiment so that he could 
quit his job. When I last looked his library had 21,000, I think downloads per 
week on NPM. And today I'm super, super excited to talk with him and learn how 
he actually makes money with open source, how he could, write 
something on the side so that he can quit his day job and become free and 
independent. So hello, Alvaro to the show. Welcome. And I'm really excited that 
you're here!

[00:01:47] **Alvaro:** Hello, Michaela. I'm happy to be here. 

[00:01:49] **Michaela:** Yeah. So the last time I looked and this was 2020. 
Right? The tweet from 2020, it said like 21,000 downloads on NPM what is it 
now? Like? It must be even higher. Right?

[00:02:02] **Alvaro:** Well, to be honest, I'm not sure I haven't checked in 
awhile, so I don't know exactly, but it would be similar I guess, I'm not very 
sure if the NPM stats are very representative anyways, but I think it's just a 
way to, to show that, you can have quite weight broadcasts, if you do 
something, by yourself in your own house, nowadays is quite easy to 
reach so many people and to influence people in some way. Right? Or companies or 
whatever. So I think it shows a bit the power of open source sometimes. 

[00:02:30] **Michaela:** Yeah. Yeah. So this is exactly what I want to deep dive 
a little bit into the power of open source. Right? I think the power of remote 
work. Yeah. It's something that I'm very fascinated with and with the pandemic, 
I think a lot of people now really understood what's going on here, but what 
about open source?

So, how did you even come up with the idea and maybe we should also explain my 
listeners, a little bit what you were building, it's called 
[fullPage.js](https://alvarotrigo.com/fullPage/). Right? And as I understood it, 
it's like a webpage that goes over or a website that goes over the full page and 
it's easy to set up. And?

[00:03:03] **Alvaro:** Yeah, it's a component that allows developers to create 
these kinds of websites, where you have like a full screen kind of slider that 
snaps to each of the sections. So when I created that, the page wasn't very 
popular yet it became very popular because I realized that almost at the same 
time that Apple released the page for iPhone 5C. The iPhone 5C website 
was using these kinds of effects. So I think then people started searching for 
these kinds of effects and, and they were able to find my component.

So, how did they come up with the idea? Well, I, I didn't actually think too 
much about it. I wanted to create a component just to learn by myself. I wanted 
to keep on practicing jQuery at the time because the first version was a jQuery 
plugin. It wasn't vanilla JavaScript. And well, I just came up with this idea 
that I thought it was cool because I was making a website in my company.

At the time, my boss told me, I want kind of like a very simple website, kind 
of like a PowerPoint presentation. And then I, I researched a bit and 
then I came up with this idea that, I took from different websites. And 
then after creating the website, I thought, well, this was quite difficult 
for me. I was trying to find for a component to do these kinds of websites 
and it doesn't exist.

So it might be a good idea for me to create the components and see if other 
people find it also interesting, because it would save them lots of time. And 
that's what I did. And then it started getting some traction on GitHub. I 
remember one day checking in and seeing that it had like 500 more stars on 
GitHub and I didn't even push it too much. I was quite surprised and then, 
just kept moving.

[00:04:35] **Michaela:** Cool! And so did you, because I, I looked on, on your 
GitHub profile and saw it's now, GDPL/GPL. Right? Was that the initial 
license also that you looked up and you thought this is the right thing. 
Did you already think that you want to commercialize it a little bit?

Did you want to make money by having people that use it commercially? 

[00:04:57] **Alvaro:** No, not at all. My whole purpose was just to, to keep on 
learning and at the same time to get the motivation for myself to, to, to keep 
on learning, to do something useful for others and that, well, 
makes you very excited about that and initially it was under the MIT License. 
Because that's what most open source kind of use. Right? In JavaScript spectrum. 
And later on, when I decided to start commercializing it is when I made 
the change to GPL version 3, because I thought it was going to be more 
suitable. 

[00:05:26] **Michaela:** Yeah exactly. It's also my license, like it's the 
Apache like years before it was the Apache.

And now it's always the MIT that I, that I use for open source to give a lot of 
freedom to the user. Right? And so does it mean that if you already licensed it 
before under MIT that's are the previous versions, still licensed under 
that, or the new things are under GPL or how does that work? I'm not really 
familiar with it.

[00:05:52] **Alvaro:** This licensing thing is quiet complicated, to be honest. 
I'm not really an expert on the topic, but yeah, I guess what happens is so 
fullPage version 1 and version 2, they're under the MIT license, you're 
going to still find them under their releases sites in GitHub, and then after 
that I changed to GPL. I don't know how that legally works or I don't know 
exactly how it does, but. 

[00:06:16] **Michaela:** Yeah. Yeah. Probably, it will work like this, at 
least that's what I thought, but I'm also not, I'm not a lawyer 
( *both speakers laugh* ). I have no idea about it, but.

[00:06:23] **Alvaro:** So version 3 is under different license.

[00:06:25] **Michaela:** And so, so how long, because there's also another 
tweet of yours and you were saying, well, I started to play around with that 
experiment with JavaScript plugins and so on. And now three years later, I 
actually quit my full-time job. How long did that really go? And where the times 
where you thought like this could be something or, a lot of a long 
time where you just did it for fun, but never imagined that it's, going to be 
your bread winning income?

[00:06:56] **Alvaro:** Yeah. Well, at first I couldn't even imagine that I was 
like, somebody would be able to live out from, from these kinds of things.

So I guess it's kind of not right to me. I was working on it for free for three 
years under the MIT license. At some point you start getting a bit, 
you have to take decisions like, should I keep on improving this or should I 
just go for a barbecue with my friends. Right? Or, should I spend extra 
hours doing this after work or should I just chill with my housemates or my 
friends or whatever.

So, at the beginning it's very exciting. You, you get people using 
it and that excites you a lot. And then, provides you some, help to 
keep on improving it. At some point you start having to work on it when 
you don't actually feel like working on it. Right? Because people keep on 
requesting new features or they have bugs, very specific bugs that almost look 
like you are doing free consultant services for them. Right? And that's when I 
thought, well, maybe I can try to get something out of it. I got 
motivated by another developer it's called, I don't know how to pronounce it 
either.

I think it's DeSandro, he created Flickity, Masonry and another 
popular JavaScript components. He was providing licenses for them. Paid 
licenses. I went into those, I read a bit how he was doing, and then I thought 
that I could do it as well. And that's when I started charging for not for the 
product itself, but for paid extensions to the plugin.

So they were non-open source licensed extensions that I was selling on top of 
the open source project. 

[00:08:24] **Michaela:** Yeah, yeah. That's a good idea. Yeah.

[00:08:26] **Alvaro:** 
So that's how it just started. And then I saw people start 
buying them and that's what motivated me to keep on going. And then I noticed 
that I was more, I was feeling better about it all. Like if somebody reported a 
bug or wanted a new feature or whatever, then I wouldn't be so bothered about 
it because now I knew I was getting something in return.

So I think this way it works a bit better. Like when you can take the time to do 
something and you get compensated for that. And then you don't feel as bad 
because you can, you're not just wasting your free time. You're actually doing 
something in your, well, work time, I guess. And that's a win-win for both 
sides, for the developer and for the users who get better support, better 
features, better response times.

So, I started sending the licenses, sorry, extensions. And then after 
six months of doing that, I was able to quit my job. And then after a year or 
so is when I decided to also change the whole project and our license and try, 
charging for the, for the license itself for commercial use, for non open source 
projects.

[00:09:33] **Michaela:** Yeah. I think that it's really, really important that, 
projects are sustainable, especially if you have some success with 
it. Right? Because. There is more and more time that you're spending on it. 
And I think that, nobody, like if it's a hobby and you're spending one or two 
hours per week or something, this, this idea doesn't come up. Right? 

But if it gets, as you said, if you have more users, you're getting more 
requests, you're getting more ideas maybe for features. So you're 
spending more and more time. And obviously, I mean, we all have 
to live somehow ( *chuckles* ). Right? Obviously you have to think a 
little bit about how can I actually. make that maybe my, my job.

And I think, especially if you like something, that would be like a win-win. So 
yeah, I can totally understand that. Another question that I had for you when 
you were, when you were turning that around, I saw you have really big names. 
You have big names on your website for companies that are using fullPage.js. 

Yes, right? There was like a Google, eBay, Coca Cola, Sony, and so on. Right? 
Did they all purchase a commercial license? Did you reach out to 
them when you changed your licensing model and your monitization 
idea around that? Did you reach out to them and say, I'm actually 
licensed now for that?

[00:10:48] **Alvaro:**  So, some of them are using my license. That's how I 
managed to discover, website. Cause when you use the license for, when you 
buy an extension, you have to register it for a specific domain. Extensions of a 
different price, depending on how many domains you wanted, you want to use the 
extension for those. That's how I use for some of them others I think I 
just discovered them by chance and they might not be using the license.

So it depends, but no, I, I didn't reach, when somebody buys an extension or a 
license for the product, now I get their email. And I get to notify them about 
dates or changes. So yeah, when I release a new version I notify all of my 
previous customers and told them about that, but if they were not previous 
customers, they didn't get a notification.

If they were using the previous version, they can keep on using that forever 
and nothing's going to change in their sites. 

[00:11:36] **Michaela:** OK. And so what's preventing people from using the new 
version and not buying a license? 

[00:11:45] **Alvaro:** Well, I guess some people, some people might not know 
that there's a more recent version and others, I guess they they're happy with 
their website and they don't want to touch it at all.

So they don't even want to bother to update to the latest version. Others they 
might not want to pay. It's not very expensive, it's quite cheap, but there's 
all kinds of users, not only companies, but also freelancers or people 
who just make websites for fun. So that might be one reason because there's no 
other good reason to not update because it's totally compatible.

You don't have to almost change anything in your code. I think it's just one 
line, if, so. 

[00:12:19] **Michaela:** But my question was more, are there people that are 
updating and not paying if they use it commercially or is that not possible? Do 
you have some prevention mechanisms around that? What I mean is that, can I, can 
I be a little bit cheat, cheat your system? ( *both speakers laugh* )

[00:12:36] **Alvaro:** Yeah, you totally can. And there's not much that we can 
do about that. I mean, yeah. For example, I discovered there was a McDonald's 
website in Russia making use of the new version of the plugin with a 
new license and they were not paying for it. And there was a warning if you 
opened the JavaScript console.

You were able to see a red warning saying, "Hey! this software is not licensed. 
You can get the license here." There's not much that I can do about 
that. Sometimes you can try to send, I think they're called DMCA notices to 
Google or to some marketplaces to take down some of the stuff at, I 
cannot be bothered for ten dollars. ( *laughs* )

[00:13:13] **Michaela:** Yeah. So you are more focused on, directing your 
energy to creating more value for your users and, doing what you like 
and not so much bothered with, with the thefts and, trickeries and 
things like these. 

[00:13:27] **Alvaro:** I bother a little bit, but I try not to bother too 
much. It is true that with extensions, with, extensions to the main  
components, in those, you have to register each of them for different 
domains.

So you actually have more like, yeah, there's kind of like a more 
sophisticated license key that you cannot trick so easy that that's only on 
extension. I don't want to enforce that on the product because then it will be 
too much of burden for many people and I think things are ok.

[00:13:57] **Michaela:** Yeah. And I mean, I think I would probably 
draw a line a little bit between, as you said, smaller, maybe individuals that 
even though I'm mean $10, come on, ( *laughs* ) but like if then they're like 
larger organizations like Google or E-bay, using it, in addition to this small 
fee, really small fee for you, are they providing some support? Do you get some 
sponsorship like there's GitHub sponsors or something, or do you have other ways 
to, to support your work? 

[00:14:26] **Alvaro:** Well, what I do is I also, no I don't, I don't do 
sponsors and they don't usually get support unless they go for a higher, higher 
license.

They do get support with extensions. All kinds of tiers get support for those, 
but not for the main license. And also what I do to get money from different 
places is also, I sell, plugins for wordpress. I also do some affiliate things. 
And I also have another plugin that I also commercialized. So I have a few 
things that also drive money and not only the full bit licenses also like 
extensions, which are not open source.

Yeah. And, well, I just remember that another way that, many people 
don't even bother to get a license is because they don't know very well how the 
GPL license works or, they are not very up-to-date about licensing terms and 
stuff. So they don't even know that they have to purchase the license or they 
didn't even know what is considered open source or how to add a license to their 
own project.

So, this is a big issue that I see, especially on small developers, 
freelancers. 

[00:15:31] **Michaela:** Yeah, Yeah I can imagine. So you were talking about 
plugins. Is it like a package or is it like a plugin? What is the difference 
here? 

[00:15:37] **Alvaro:** So well, back in the days every time you made a 
component for jQuery, it was called a plugin, plugin for jQuery.

And nowadays I tend to call it the library, the JavaScript library, but yeah, 
also, I talk about plugins for wordpress. Because WordPress, they have these 
kind of plugin stuff and then it's the plugin that incorporates the library 
and allows you to do certain things and you have a little interface. So it's 
not just for fullPage something on top of the components that allows 
you to do things through an interface, and kind of like the word press way.

[00:16:12] **Michaela:** Yeah, so when you were right at the beginning, you 
said, well, I tried to do that for my, for my boss and try to 
implement that. And I was surprised how difficult it actually is. Right? I'm, 
I'm really in the same situation because I ported two websites ( *laughs* ) 
from WordPress to Gatsby now. Right? And I was like, oh, static site generator 
and gets me super supported and so on. And I completely underestimated 
( *Alvaro chuckles* ) how long it will take. Right? Even though there are so 
many plugins or, components that you can use. But just even researching which 
plugin to use, then writing the query really adopting it to your thing.

I mean, it really blew out of hand. And even though their websites 
are, now almost done, it's like always like, oh, this little bit, you 
know, still like that, you even have to think about. I'm like, like with 
WordPress, I was not so happy because it's slow and I didn't want to be 
bothered with, going around PHP and, changing something in the back-end to 
improve my speed.

And then the loading time of each page really was annoying. So I thought like, 
okay, I'm going to do a Gatsby website, and then I will have everything with 
markdown files and, directly gets them from the file system and it 
took me, actually no time almost. Right? To have that set up because there are 
already like start-up packages and then, but then the small 
things like that, the canonical link is direct. 

[00:17:41] **Alvaro:** That ?? principle. Right?

[00:17:42] **Michaela:** It's horrible. Yeah. I have a site map and then I have 
the keywords ( *laughs* ) and I completely underestimated that. So, yeah, I 
totally understand. So if I want to use fullPage now in my Gatsby site, 
is that. Is that a thing? Can I do that? Would that make sense?

[00:18:00] **Alvaro:** Yeah, I guess, I mean, well, I don't know what your site 
looks like. Is it more like a blog?

[00:18:05] **Michaela:** Yeah, it's mainly a blog, but it's not only a 
blog. It also has like a run pages. Right? Where landing pages and so on. I 
think for the landing page, probably something that - so if you go -

[00:18:17] **Alvaro:** yeah, I mean, you, you could, you could totally 
use it. Yeah. It's just basically a JavaScript library, so you can initialize 
it, wherever you want.

[00:18:24] **Michaela:** And then it's mainly about the look and feel. Right? 
What's the thing?

[00:18:28] **Alvaro:** So yeah, what it makes is that allows you to create this 
snap scrolling experience, full screen. So, well of course it is much 
more complex than that. It has many more options that you can configure. You 
have hash URLs, you have history back and forward. You have the lazy load, you 
have, play, pause of media elements. You have many more things.

[00:18:49] **Michaela:** Right? And I think this is it, right? So first you 
think, oh, what is it? Right. And it's really small. And now I'm like, I have 
this blog and I'm thinking like, if I'm in my blog and I mark anything, then I 
would like a pop up that says, share it on Twitter and so on. And I realized, 
( *laughs* ) yeah. 

[00:19:04] **Alvaro:** Yeah, exactly. So the very basic functionality seems very 
easy, always to implement by yourself. And then 20% of the extra features that 
you want. Those are what takes the most time. Right? 

[00:19:17] **Michaela:** Takes lot of time. Yeah, exactly. And then you 
want to have like previous article, next article, and then this is not good 
enough because you want it by category. Right? And so, yeah. 

So another thing that I was thinking a lot about and reminds me also of your 
success stories, and there are, I mean, there are similar success stories. 
I think now more and more popping up right around the internet is that 10 years 
ago, If you ask somebody to pay one Euro or dollar or what not, or 10 for 
something, they would like crazy.

I mean, everything was free and it was like software should not cost any money. 
And I think, especially in the last two years, three years, it completely 
changed. I mean, if there are like Google was sunsetting, most 
of them products that are for free. Right? And then the ecosystem completely 
changed into this SaaS businesses.

But also that you have more and more smaller, I would say, yeah, smaller, 
independent developers also really making money for their, for their software. 
Right? And suddenly I feel like, okay, we have to pay for everything. It's 
getting really expensive. Like for my website, if I don't want to use Google 
analytics. Right? Which is free. And this is like the, 10 years ago, 
mindset, like let's use Google, Google analytics, and now the mindset is, oh, 
we don't want to use Google analytics. So what else do we have here? And then I 
find like 10 different analytics platforms, but they're all atleast $20. And I'm 
like, okay, this is for my private blog.

It's already, it's already a lot. Right? Because it's not only the 
analytics that you need, you need a lot of things, but I see that people are 
starting to value software more. What's your experience here?

[00:20:58] **Alvaro:** At the beginning, it wasn't common at all to charge for 
these things. And now it's getting a bit more common. Right?

But still on the JavaScript environments, especially in the front-end side of 
it, is not yet too common to transfer these kinds of things. You see 
libraries, components of all kinds, but usually they tend to be free because I 
think one of the main reasons is it's not easy to protect in some way, like 
the code is free. Everybody can see the code when it's front-end. So it's 
very difficult to protect something like that. And when you cannot protect it, 
I guess some people think it doesn't make much sense to charge for it. But yeah, 
I know a few libraries that are starting to charge for javascript libraries, but 
yeah, it's still not very common I think.

It's more common for other kinds of products for back-end stuff for 
kind of like subscription services. But I think it still needs to improve a bit 
more in that regard, because I think it's been a ??, so like sometimes when you 
don't see this, when you don't see that the owner or the, creator of the 
component is getting some benefit out of it, then it's easier to see projects 
in GitHub that will get unmaintained or that they will eventually 
die or get obsolete or whatever, because somebody can not keep it 
maintaining forever. Some people think that you can create an open source 
project, publish it, and forget about it. But the publishing part is just the 
very beginning.

Then you have to keep on maintaining it and that's for years, like my component 
is now more than seven years old. And you have to keep on improving it and 
adding features and reporting and dealing with reports. And so many 
people don't bother doing this. And then you see the last release was four 
years ago.

So it's not really ( *chuckles* ) a component that sometimes you can trust or 
you have to look for an alternative or you open a issue, and nobody answers. 

[00:22:46] **Michaela:** So what's your experience with, there's this rumor 
I'd say, or the anecdotes around customers and especially the free 
riders, they're really like heavy maintainence customers that are asking a 
lot of things.

And then the people that are actually paying are, are much more moderate. And I 
mean, my experience is definitely like this. Whenever I provided things for free 
people come with this attitude that, "It's there, Right?" "It's there, Right?" 
( *exclaims agitatedly* ) Yeah. I mean, sometimes I get emails. Like I have a 
newsletter and you get an ebook, right that I wrote, for my subscribers. And 
sometimes they can't find their email in the spam. Right? It goes in promotion 
or spam or whatnot. Right? It's not really my fault or something I can do. And 
I'm always, if somebody is, writes me an email back and asks, I didn't get it. 
I'm always going, doing the work to write them a personal email, send them the 
book. Right? But their email's like "You said and you didnt!" 
( *exclaims agitatedly* ), ( *both speakers laugh* )

[00:23:44] **Alvaro:** Yeah totally, so aggressive sometimes right?

[00:23:49] **Michaela:** Yeah, wow, okay and for other things as well, what's 
your experience here? 

[00:23:52] **Alvaro:** Yeah. You always get some people that is a bit aggressive 
a bit, they want everything for free they want you to work for them for free, 
doing consultancy, fix their bugs that sometimes they are not even related with 
your own product. Right? 

So, well, what I used to me do is just reply to them. Very politely, explain 
them the situation. Always telling them, if you found a bug or you are not 
happy with this because you didn't pay for it. Then you can just go and check 
the code because it's open source, you can check it yourself and does it go 
same?

Like everybody can check it and fix bugs if they find them. So I think, having 
it as an open source is also a way to, move people in certain direction tell 
them, Hey, this is open source! You're taking advantage of it, but it's also 
good because you can fix your own issues. Right? If you have them. So that's 
what I do sometimes. And other times you just tell them, well, if you need my 
help, you can always upgrade to a, the business license, and then I'll provide 
one hour support or whatever. So I give them the options and that's it. Yeah. 
You get some angry people, the money so much, if they're angry and they paid 
for it and they are not happy because there's a bug that I cannot fix, for 
example, then I'm happy to refund them. If I can not find, fix their bugs, that, 
that makes sense to me. But otherwise, if they're not paying anything, then, 
I help them to, to some extent, but not, there, there are some limits. 

[00:25:13] **Michaela:** Yeah. So how much of your work day now is really, are 
you still programmer are you still a developer in your mind or are you now, like 
you are a salesperson already or, like an admin person. Yeah. How do you feel 
like in your, in your entrepreneurial journey right now?

[00:25:33] **Alvaro:** I don't know. I think I like to consider myself more like 
business person more than a developer.

It is true that I am a developer and, I have the background on this, 
and I keep on developing the product. Actually I'm about to release a new 
major version. But it is also true that I don't spend my whole time 
developing anymore. Like, I just have to do marketing. I have to do content 
marketing and I have to do, taxes.

[00:26:02] **Michaela:** I hate taxes! ( *lsughs* ) 

[00:26:03] **Alvaro:** You have to do all kinds of things like images. You have 
to think about potential new opportunities. You have to think about the license 
system. You have to think about, I don't know, so many kinds of things. So yeah, 
I guess I, I like to consider myself more as a, as a business person. I would 
like to maybe eventually in the future delegate parts of the developing side to 
somebody else that is even better than me.

Also that other people can benefit from it, you always try to look for 
the best outcome and sometimes it's also good to get rid of yourself from 
certain tasks. 

[00:26:34] **Michaela:** Yeah. Yeah. True. Yeah. So I don't know. I couldn't 
find anything about, how much you're making per month or per year. I'm also 
not sure if you're sharing something publicly.

Some people do, some people don't, I'm totally going with whatever you 
decide. Do you share it? Do you say how much you're making with it or can you 
give us an idea?

[00:26:56] **Alvaro:** In my case I prefer not to be very open about it just 
because, it's open source, so anybody can just see my code and create another 
project.

And I started doing the same, so, and that's one of the reasons if I had the 
SaaS, a back-end product or whatever, I wouldn't mind, but right now I 
prefer to be more private on these aspects. So, we can say that I 
get enough to live comfortably. And that I have different sources of income. 
That's an, all, everything comes from the main component and it also comes 
from the plugins for, for WordPress, from affliate links that I have for selling 
other WordPress themes from supporters, from consultant services from, and now 
I'm also starting a blog as well, which I'm also expecting to monetize in some 
way. So yeah. 

[00:27:41] **Michaela:** Yeah. that's good yeah. And I think it's really good to 
have multiple income streams. I also try to have more than one, at least for me, 
it gives me a little bit, ease of mind that, if something dries up or doesn't 
work out so well, maybe SEO doesn't work or, something else comes a copycat, as 
you said. Right? You have other opportunities as well. So yeah, I can totally 
understand that. Cool. So I think I probably, there are a couple of listeners 
that also like want more freedom, or at least, a side project that gives some 
side income. What's your advice for them? What would you do like now you're in 
that game for a long time or is it seven years? What do you think? Is there 
what's the right time right now to start something, you're saying a blog?

[00:28:25] **Alvaro:** Oh, the right time, the right time is always now 
( * Michaela chuckles* ) because some people are still waiting to finish that 
course to finish that book to become better. And, to master a 
certain technology, I don't think thats the way you have to take this. The way 
you have to take is do your best, with whatever and you will 
probably end up helping somebody. When I created my project, I wasn't an expert 
developer in jQuery. I created it because I wanted to keep on learning and 
creating something useful and was a good motivation for me.

And I think that's what the other people have to do. Well, yeah, it happenned 
the same when I created my first website, I created it using Microsoft 
Word. I didn't know how to code. I didn't know anything about websites, but I 
had a teacher that taught me how to make websites using Microsoft Word. And 
then I started seeing people using the website and that's what motivated me to 
keep on learning. Right?

So the right time, I think it's always now just do whatever. Keep on improving 
it, keep on iterating, get feedback from people and they will tell you sometimes
how to improve things, what features they want you to add, what bugs they 
found. So I think that's what really helped me. To improve my components 
at first.

What I would say is that don't quit your job, do something on the side, see 
how it goes, get feedback. And then when you get some traction, you can decide 
to quit. In my case, I only decided to quit. When I saw that I was going to be 
able to keep on living from this. Took me six months can take more, can take 
less.

It depends on people, but I was working in on the side for three years. That's 
what I would recommend people to do it on the side, if they can, not get too 
crazy because a great idea might not result in people buying your 
product. So, yeah, that's one of the things. And another thing that I think 
helped me a lot at the beginning was making it well, I was open source or let's 
say free - because when you have something for free, at least at the beginning, 
or you have a freemium kind of product or something, you get much more 
exposure. Like people will blog about that. People will share it on Twitter, 
on Facebook, or so you create this kind of like snowball where, the content 
keeps on spreading faster because it's free.

Unless you have a very good product and you can already charge for it or 
whatever, having it free at the beginning might be good because you not only get 
much more free marketing because people don't mind certain stuff when 
they know that it's free and nobody's going to really benefit out of it.

And you also get the feedback from the people. The more people that use it, the 
more feedback you get and the more you can improve it on different iterations. 
And then, in the future, you always can start charging for it, release 
new versions or, or even people to another area or whatever, but 
having that free feedback and that free marketing, I think it's very powerful 
at the beginning.

[00:31:12] **Michaela:** Yeah. Yeah, I totally agree. Yeah. Thank you so much 
for taking the time, talking with me about your journey and, about how we 
could, leverage open source to actually start our own little business and, 
get independent.

[00:31:25] **Alvaro:**  Yeah Thank you! Thank you for even having me here. 

[00:31:29] **Michaela:** Yeah, it was really great talking to you and, thank 
you so much.

[00:31:34] **Alvaro:** Yeah, thank you so much Michaela. 

[00:31:35] **Michaela:** Ok. Bye!

[00:31:37] **Michaela:** This was another episode of the software engineering 
unlocked podcast. If you enjoyed the episode, please help me spread the word 
about the podcast. Send the episode to a friend via email, Twitter, LinkedIn. 
Well, whatever messaging system you use or give it a positive review on your 
favorite podcasting platform, such as Spotify or iTunes.

This would mean really a lot to me. So thank you for listening. Don't forget to 
subscribe and I will talk to you in two weeks. Bye.

[00:32:08] ( *outro music begins* )

[00:32:24] ( *outro music ends* )
