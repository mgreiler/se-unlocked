# Episode 40 with Max Stoiber

**Michaela:** [00:00:00] Hello and welcome to the software engineering unlocked
podcast. I’m your host Dr. Mckayla and today I have the pleasure to talk to Max
Stoiber.

But before I start, I wanted to update you a bit on what I’ve been up to lately.
Over the last few months, I have been quite heads-down with some new exciting
productivity research. I was mainly investigating what makes developers happy,
productive and successful. I’m planning on wrapping up this research soon, so I
hope I can share more about the findings in near future.

Another thing that I have been up to is preparing a secure code review workshop. I
plan to release this worksop this fall. It will focus on secure coding
practices, and shows you what to look out for when inspecting code for security
vulnerabilities. If this sounds interesting to you, hop over to
https://awesomecoderviews.com and either book a workshop or join my waiting
list. But now, back to Max.

Max is not only a JavaScript engineer that is in love with react and node, but
also a fellow Austrian. He has a track record in the open source world and
worked for Gatsby and GitHub and he's also a successful entrepreneur.
Max built, for example, a community platform called spectrum.
It became so successful. It was a quiet, but GitHub. And now he's again
working on a new startup idea. So I'm super excited to talk
with Max about all of that. I'm super thrilled that he's here.
Welcome to the show, Max.

**Max:** [00:01:30] I am super excited to be here as well. I'm a big fan. We've
obviously spoken before. I'm really happy that I get to be here today.

**Michaela:** [00:01:38] Yeah, I'm really, really excited. Thank you so much for
joining. So I want to start with something that I wanted to ask you a couple of
times already, and that is you build this really amazing community platform spectrum.
And I recently looked on the website and I see there are forums, there
are several forums where are people in communities, where people are talking with
each other and it seems really lively. Like when I went there, they were like 50
people online in that community and 60 people in that community and so on.
Right. So it really seems like a big success, but on the other hand, there is
the announcement that. It will be read only, right. It will not survive. For me,
it looks like it's shut down. Is that, is that true? And if it's, so how do you
feel about that?

**Max:** [00:02:25] It makes me very sad to be honest. Whenever I build a product,
they're sort of like my, my babies, right?
I want them to be successful. I want them to succeed. I want people to like
them. And spectrum no longer existing or, or only existing in an archive
format is, is quite sad, honestly. But at the same time, the spirit lives on in
GitHub as GitHub discussions, GitHub originally bought spectrum with the
intention to eventually shut down the platform itself, integrated into GitHub.
And that's what, that's what they've done. And so that was part of the plan. And
I'm, I'm happy that that plan is being followed so closely, but of course I
would much rather spectrum stayed around and lived on as its own thing, but
that's not the way it's going. And we've, we've actually, I talk, I've talked
quite frequently to my other co-founders Mike, co-founders about doing the
same thing again, because with the, with the benefit of hindsight, there's so
many things we would have done differently or we would like to do differently.
We have so many ideas about how we could have built spectrum better, but of
course it's all just wishful thinking. We're very unlikely that we're going to
do that, but it is fun. A fun thing to dream about.

**Michaela:** [00:03:33] Yeah. I mean, community is such a interesting topic and I
mean, it's so powerful and it's so important and communities are, I mean, people
are here for communities, right.
We need communities to strive. So I actually also playing a little bit with the
idea of building some community, but I feel also very overwhelmed at the same
time, how to do that. but it's just a fascinating topic. Right. And just having
people around and I mean, a community can be also like five people or, you know,
two people, three people.
Right. So spectrum is on the very other end, right. There are like hundreds of
peoples or thousands of peoples. But so I think communities are really important.
So, but you were saying that when GitHub bought spectrum, you already knew that
they are going to shut it down. So you, you knew that that could be one of the
paths or this could be leading towards that shut down off the platform.

**Max:** [00:04:23] Yeah, absolutely. Spectrum itself, technically, just wasn't
architected well enough to sort of sustain GitHub's load and it was clear
from the very beginning that it would be a lot more work to make spectrum work
at GitHub scale, rather than trying to rebuild the parts of spectrum
that we liked within GitHub.
And so very quickly, we just arrived at the conclusion that we're going to have
to shut spectrum down as a platform and sort of build that integration and GitHub
completely from scratch and separately because GitHub has so much tooling
internally and that, that helps it handle the scale it's at, right.
We're talking hundreds of millions of developers, which is very different from
scale that spectrum is at, spectrum has a couple of hundreds of thousands
monthly active users, which is a lot, but it's not by far, not as much as
GitHub has and so it was clear from the beginning that we would either need to
rebuild spectrum.
I mean, it was clear that we would have to rebuild spectrum. The question was
we rebuild it as spectrum, or do we rebuild it in GitHub? And since we
were already rebuilding it, we might as well just rebuild in GitHub. And that's
where discussion came from eventually.
which again, makes me a little bit sad because I would like spectrum
to still exist, but that's the way it is.
And discussions actually turned out really well. I'm really excited about it.

**Michaela:** [00:05:32] But so for the community, there are two parts to it, right?
So there's the tech around, it enables people to meet in an online space and
talk and, you know, like, you know, write or have chat or what not. Right. So
there's the tech around, but then there are also the communities itself, which
are really, really valuable, right?
So that hundreds of people come together on that place, like type in that URL,
for example, and then meet at that forum or, you know, that, that place, that
community place. So is that my graded are people migrating or is that as easy?
Because I feel like there might be people that say, well, I'm on spectrum.
I'm going to this community on that. You're out, but I'm actually not on GitHub
in, you know, in that space, which I think, you know, on one hand it feels like,
well, what's the difference here, but I can imagine that it's not that easy.
Right? So there's like the tech around the community, but then the real heart of
the community is the people that choose to be there to go there every day and,
you know, provide benefit or value to other members.
How is that what, what, what do you think about that?

**Max:** [00:06:33] Spectrum was always mainly used by developers. A large
percentage of our users already authenticated with GitHub even before we
were bought by GitHub and most of the communities were around open source
projects, or we also had some design communities.
Those are gonna have a harder time migrating somewhere else. But most of them
were open source communities, definitely the most active ones. And so I think
those will migrate just fine. I think GitHub discussions is a great fit for that
since it is based on a repository GitHub and open source projects are just
repositories on GitHub.
Right. And so having that community right there will actually be huge for the
vibrancy for those communities and enable a lot more open source projects to
build communities around their projects. I actually think that part of our
fundamental assumptions about spectrum were, or parts of our fundamental
assumptions were incorrect.
We wanted to build a space where large communities do the order of magnitude of
tens of thousands of people could communicate and connect with each other. But
actually that doesn't work super well. When you have 10,000 people in a
community, you don't really feel connected to any person anymore, right?
Connection happens at much smaller, much, much smaller scales. And which you can
see by the sort of prevalence of group chats now, right? Like you have telegram,
you're signaling for WhatsApp and within those chat messaging platforms,
everybody's a part of 20 groups, right? And you feel connected to each and every
single one of those groups, but they're much smaller in scope.
They're much more specific which allows much more of a community feel to build
much more of a sense of community, much more of a connection to build. And so I
think actually there is probably a way where you can scale that sense of
community up to a larger scale, that you can definitely have a community of
thousands of people I think that's possible.
But there has to be much more of a mechanism of sub groups within that. Right. I
don't know exactly what that's going to look like. Somebody who's going to
figure this out eventually. But if you think about, for example, football fans,
right? If you look at Liverpool, they have a fan base of, I don't know how many
hundreds of millions probably.
Right. And they're spread all around the world, but within that massive group of
fans within that massive community, there's these tiny subgroups of the fan club
in Vienna, the fan club in Istanbul, the fan club in wherever. Right. And then
even within that, there could be even smaller subgroups. Right.
You could have your friend group of the fan, a fan group of Vienna, right. And
so then that's the 10 to 20 people you feel directly connected to, but yet
you're still part of this bigger community. And so in real life, it kind of
already works that way. The online platforms just haven't really been able to
mirror that real, real life engagement
I would say, if that makes any sense. I don't think any online community
necessarily has figured out how to represent both the large groups as well as
the small groups. I think actually the one that's the very closest is Facebook
groups. I actually think Facebook groups for what it's, I mean, it's on
Facebook, which kind of limits its usefulness, but actually Facebook groups
works really well.
And a lot of people are in very many different groups and sort of feel connected
to many different communities through Facebook, which is very fascinating. But
other than that, no, one's really figured out how to make the, how to scale
online communities beyond a couple of hundred members of most.

**Michaela:** [00:09:32] Yeah. And so when you build spectrum, was it mainly about
the tech and then you were all thinking of, you know, how many people do you
want to allow in a student group and what interactions you're facilitating and
all of that. But did you also see the community itself? So how did you get the
first people using your product?
What were some of the strategies that you had there?

**Max:** [00:09:54] Spectrum came to be because my two co-founders Brian Levin
and Bryn Jackson have a podcast called design details and they actually started
a podcast network around that podcast that at the end, I think contained eight
or nine podcasts. And it was all design and development focused podcast.
And they created a Slack community for this network and where they want it to
connect to all of the listeners together. They wanted to answer questions that
they want people to chat with each other, basically build a community around
that network. And eventually that's like group that Slack workspace grew to
eight or 9,000 members.
And then Slack came to them and said, Hey, it's really cool what you're doing
here, but either pay us or go leave somewhere else. And I think it's Slack costs
$5 per member. So they were looking at a bill of $45,000 a month for a free
community that they were running, which is obviously not something they can pay.
And so they looked around and they didn't find anything that would sort of. That
fit their niche, right? They, they wanted the community to public. They want
people to be able to read the content, even when they're not a member, but also
they wanted it to be real time chats. They wanted it to be, to feel like the
multiple people were there and talking at the same time with each other.
And so they started building spectrum just for their own podcast network, which
is where the name actually comes from because their podcast network was called
spec FM. And so spectrum was sort of the spec FM community platform. And
interestingly enough, they had a problem. They, they were using one of my open
source projects, style components, and they reached out to me from via Twitter
because they were having an issue with it.
They found the bug and I knew of Brian Levin and Bryn Jackson, but I'd never met
them in person. I talked to them before. So I, I was a big fan of their podcasts
and their work. And so I said, look, you have a problem. Don't worry. Just give
me access to the repo. And I'll, I'll take a look and fix it. And they gave me
access to the spectrum repo, and I looked at it and I told them, Hey, I need
this.
Like, this is the platform I need for my open source projects. Right. I'd been
building communities around my open-source projects for a lot, for awhile, but
none of the platforms for that were very nice, like get like basically there
was, Gitter or GitHub issues, but GitHub issues there for problems.
And for Gitter, there was just one massive chat room, which doesn't scale beyond 10
members. And so I said, look, forget about whatever I'm working on. I want to
work on this and I want to make it more general. And so that's where spectrum
was born. And that's also how we seeded it. We built the initial version and
then immediately onboard at the eight or 9,000 members at a time of spec FM
onto the platform, and immediately had that first community there, which was
huge for us because that kicked up the flywheel of people joining over time.
Because those people in those old spectrums, awesome. I'm going to create my own
community there. Right. And invite my own people there. And so that's sort of
how it started growing and that's why it really grew in the design and the tech
communities. And why there was so many open source projects using.

**Michaela:** [00:12:30] Yeah. Very, very cool. And so spectrum itself, is it open source.

**Max:** [00:12:35] Yes. Then after about a year of working on it,
but we open source the entire codebase. If he goes to github.com/withspectrum you
can look at it. It's, it's one big Monterey(??) repo basically that contains all of
our servers, all of our clients, everything we ever built.
It's all completely open source. It's terrible code, please. Don't look at it
too, too closely. I love product what we did cause we did a lot of shipping and
not a lot of cleaning up, but it works and it's open source for people to look
at. It's a, it's quite funny because I think spectrum is quite a messy codebase
personally.
Like it's not, it's not the nicest code I've ever written. I didn't have as much
experience then as I do now. And, and also we were just trying to ship as much
as possible. I'm trying to figure out, trying to find product market fit and
then eventually the business market fit And it's funny because sometimes I see
tweets of people saying, Oh, if you want to see a really well architect, the
codebase, go look at spectrum.
And every single time I see that I like please, please. Don't like, that's not,
it's not that well, I can think of, it's kind of a pain to work with. I don't
know.

**Michaela:** [00:13:29] Yeah, I know you cannot respond to every tweet like that.
Like
_laugh_

**Max:** [00:13:33] exactly. Yeah. I can't really be like, ah, hello. Yeah, please.
Don't look at my work.
It's really bad. That's not a good idea. I can't really do that. But it is, it
was very interesting. I do think spectrum helped a lot of people think about how
they build apps, right. And it has a lot of people to learn and it was quite
fascinating to open source it and see how many people actually cared.
Because there is so few full products out there that are open source, right?
Usually when something's open source is either a toy product, the toy project
that somebody builds, or it's a library that's very encapsulated, very small,
but very few people open source, entire apps, right. Century being one of the
many, many exceptions and one of the most famous ones or ghost(??), for example, but
there's only like a handful of those.
And so adding to that list was quite interesting how much people responded to
that and how much they liked it.

**Michaela:** [00:14:18] Yeah, because I mean, I think so I'm a, for example, I'm
learning Python for two years now. And I'm also a little bit struggling with,
how should I actually go about learning Python. Right.
And that, that has to do that while I'm not employed as a Python developer
right now. Right. Which also limits, you know, the. The amount that I can
actually spend on it or that I spend on it. It also means that I don't have like
a network of people around me that I can learn from, right. Like code reviews
that you have.
If I would be a Python developer right now, I would have like my colleagues also
writing Python code and I can learn from them. Right. And so open source is
definitely something that I'm also sometimes doing. Right. I go and look at Ida
Python application to just understand, you know, how ID architecting something,
because these are the questions that I still have.
Right. I don't have the question on which type to use or how to do it area or
how to do a list, sorta whatnot. Right. So I know those things already from my
other programming adventures that I did, but I'm more interested in, Oh, I'm
coming from the job are object oriented C-sharp world. Right. So how do you do
that in Python and, and how would you, you know, structure applications and
open source is something that sometimes helps me, but it's very hard to find
like either like a good application again, because sometimes you find
application and I'm looking at it.
And even though I don't feel like I'm the expert for piping, I can say, Oh, I
should copy what going on here. Right. And then it's big enough that
it's interesting to look at and has, you know, good quality and you can learn
something from it. I think it's very, very valuable. I can totally see how
people are.
Yeah. Interested in, in doing that and learning more about it. So, but now you,
you build spectrum and then it was actually acquired by GitHub. Right. And so
you'd done because it was acquired, you worked at GitHub, building, you know,
GitHub or spectrum into GitHub right. And get into GitHub. How did their view
changed on software engineering practices on good code?
Did you experience something like that that suddenly you were in a team and they
are all, you know, like working together and you can learn you know, you can
improve your skillset there with, with the input of your peers or how, how
was that for you?

**Max:** [00:16:27] Because we very quickly realized that spectrum just wasn't built
well enough to run a GitHub scale. It was very fascinating to learn how GitHub
scaled itself, because obviously when they started building gets up 10 years ago
or however long that was, they also didn't build it to handle the amount of
traffic that it has now, because GitHub is massive.
It's one of the, I think, 10 biggest websites on the planet, maybe 15 biggest
websites on the planet. It's, it's massive. It, it gets absurdly much traffic.
And so it was very fascinating to be at GitHub and to see How careful they are
about the code they write and how many conventions and constraints they built
into their systems, particularly for the developers.
So that any code that that is that is written is good enough to run at that
scale because most people have never worked at that scale before, unless you've
worked at GitHub before, or one of the other 15 companies, that's this big, you
have no idea how to work with that scale. Right? And so a lot of the work that
many teams at GitHub did was building tools for other developers at GitHUb
to guide them towards success and to avoid expensive database queries, to detect
them, to warn people when they were writing them, stuff like that, where they
built a lot of internal tooling to make sure that they could run at scale and
that they could continue scaling into the future.
And I actually think a lot of what I, what I learned there was how important
constraints are with programming. You have all the options, you have all the
possibilities, you can do whatever you want, but a lot of what it means to be a
senior or an experienced developer is knowing which 90% of those options are
actually trash.
And you probably shouldn't do them because you're going to run into problems.
Right? A lot of the choices that experience developers make are based on
experience and I'm talking to other experience developers and they avoid future
problems, right. By, by making good decisions now, you avoid a lot of future
problems and sort of
avoid running into troubles down the line. And that's something I'd never done
before with spectrum. And so with spectrum, we actually had a lot of scaling
problems when there's this sort of rule of thumb that started people say where
every single time you get a new order of magnitude of users, you run into new
scaling problems.
And for us, it happened like that, like clockwork. When we ran from zero to a
thousand users at the, when we onboarded our first community, we immediately hit
scaling issues. We immediately had to move away from Firebase, build our own
backend because Firebase was couldn't sustain the load anymore. Then when we
went from 1000 to 10,000 people, we hit the next set of scaling problems.
As soon as basically as soon as the 10,000 persons joined almost to the day we
started having server issues. And so we had to resolve those, then everything
went fine. We're going, we doubled, we tripled, we quadrupled. We went from
10,000 to 90,000 people. No problem. And then as soon as we hit the a hundred
thousand monthly active users, the next set up problems, they didn't get in with
them releasing our server.
Our servers were crashing constantly. And it was very fascinating how these,
this sort of order of magnitude step change of traffic really impacted our
stability. And so GitHub really focused on making sure no one at GitHub
writes code that doesn't run their order of line of traffic, that no one,
there can even commit something to the code base, no matter how inexperienced
they are or how much they fork rails, for example, that could break their
systems.
And then when something breaks, they have a lot of infrastructure, of course,
around that, to monitor, to fix those issues, to roll back deploys so that when
problems do arise, they don't impact many users. And it was fascinating to see
that and to see how many constraints. They put on people, but they were very
productive constraints As a developer,
they made me free to build the stuff that I wanted to build without having to
worry about scaling, because I knew if I did something that was bad, there would
be an error somewhere. Right. See, I would throw an error. There would be a winter(??)
error. There will be a test error, right. Like somewhere, somebody somewhere
would catch my stupidity and tell me to do it differently.
And so that was actually really fascinating. And they learned a lot about
scaling, engineering and then organizations there.

**Michaela:** [00:20:23] Yeah. And so it seems that this is also very specific. So
some of the engineering practices, some of the tools, some of the processes are
really made for the scale there. But now if you're going back and I know you're
now building a new startup, so what do you take away from that?
What do you say? Well, you know, this is overkill not needed for me right now in
my next startup. Right. And what are some of the, the, the practices the
knowledge that you acquired your thing? Well, I'm going to build that in from
the start and get go, because I don't want to run into issues. Long-term with
maintainability, readability of the code base.

**Max:** [00:20:59] Many things. We, we made many, many mistakes, or I should say I made many of
those mistakes as the main technical person, that spectrum, I made many tech
choices mistakes. And one of the main things I really learned is that. Using
technology that's widely used is a very good idea. There's a reason people use
MySQL or now Postgres, right?
It's because those two databases, they run and they keep running no matter what
scaling crap, right? Like it's a famously uses MySQL and is the 15th biggest
website on the planet. And I think they're now starting to hit the limits of
that. And they're starting to have to really work around a lot of these
problems.
But, they managed to become the 15th biggest website on the planet with MySQL.
So why would you use anything else? And I'll be like, there's no reason to
choose anything that is less battle-tested because, you know, if, because if you
end up being the 15th biggest website on the planet, you can fix MySQL.
If you don't end up being the 15th biggest website on the planet, it doesn't
matter. Right. It it'll still work. And at spectrum we chose a database that was
a lot less populated. What's called rethink to be the company behind a shutdown
because they weren't financially successful. And the database system just wasn't
as well built as my, as going reading be.
And we ran into a lot of scaling troubles because of our database choice or
because of the database choice I made. And so I learned to rely on battle, test
that technology, even if it's under equals boring, even if it's something that a
lot of people use, that's a good thing, because that means it'll scale with you.
And if you have a problem, you can Google it right with rethink to be almost
nobody used it. And so when we ran into problems with our careers, when we ran
into problems with the database engine, we Googled them and we found nothing.
There were, there was no information, which is very different if you're using
MySQL or Postgres, if you Google any problem, I guarantee you you'll find 10
pages of Google results with people explaining different solutions to the
problem, how they approached it, how they fixed it, how it held up over time,
right.
And that that sort of Corpus of knowledge and that Corpus of experience is
incredibly valuable when evaluating technology choices. That's really one of the
main things I learned, which is obvious in hindsight and is, it's a common thing
to say. Don't use boring technology, use things that are proven to scale.
But it's really hard to keep that in mind when you're using technology, because
you will, you'll see something that's fancy and new and you're going to want to
use it. And it's, it's cool and everybody's using it. And you feel like
everybody in Twitter is talking about it, but if nobody's used it at scale
before, you've no idea if it works out right.
And you can only, I think there's often these tools have upsides, but the trade
off of the missing community, the missing usage, the missing scalability, isn't
worth, there's some tools where that isn't the case. So I would still evaluate
that sort of as a trader. Right. Does this tool make me so much more productive
that I can handle production problems?
Is it, is it production critical at all? So there's like, there's, you have to
think about that, but always err, on the side of choosing boring technology,
that's proven to scale.

**Michaela:** [00:23:42] Yeah, I think that's a, that's such a good advice. And I
also ran into that when I was I was choosing which, you know, static site
generator to use.
And like, they're, they're the ones that, you know, right. Like Gatsby or
Jacquelyn, I think like this. And then there are a lot of others, like tiny
ones. And I was like, Oh, this is one that nobody knows over there seems really
promising and interesting and you know, like shine in you. And I think it was
also curiosity.
Right? I think that a lot of engineers are very curious. I am curious. So I went
with that one. But what I forgot to calculate is how much time I'm actually
spending, building my website with that acquiring knowledge, then knowing how to
use that thing, but also at the same time, learning that there is not enough
support information around to, to get me out of errors that I run into, or maybe
it's even, you know, like the thing itself it's broken.
Right. And it also reminds me of, I actually tweeted, I think recently about
this where some tools make me cry. And it was like when we, when I was at
Microsoft and I had to use some internal tooling, that was really new and we
just build it until we were doc fooding it. And we were forced sort of like to
use that new thing, which is it's a good thing.
Right. But on the other hand, I couldn't just go and search for the problems
that I run into because it wasn't even existing outside. And so internally
people were building it, they weren't really like, you know, supporting others
or writing blog posts. So it was really a bad experience and something that made
me think a lot about so important that if you're stuck, that you can find
information that gets you out of this, that gets you unstuck, it gets you out of
this, you know, stuck situation and maturity of software projects and community
and livelihood.
Right. It's definitely something that's, that's important here.

**Max:** [00:25:35] Absolutely. I think this is. Even more critical in areas where
you don't have a lot of experience that the less, you know, about a problem, the
more you shouldn't rely on boring existing solutions.
I know nothing about databases, so I should probably use my SQL and Postgres
because I know that those are gonna work. And any problem I have, I can find a
solution for, I know a lot about react. And so I can, I know I can, for example,
use Preact instead of react, because I understand very deeply how react and
Preact work and I can debug my own problems.
Right. And so a lot of this also has to do, like you said, with familiarity,
right? If I'm familiar with, with a certain problem space, if I'm familiar with
the tools within the problem space, I have a lot more leeway to use cutting-edge
solutions. If I'm in a problem space where I have a NO experience where I
don't know how anything works, if that doesn't make sense to be on the cutting
edge, because I'm not gonna be able to resolve my own problems.
And so I think, like I said, that that really ties into it, that sort of
familiarity that understanding of the ecosystem is really critical. If you're
using something on the cutting edge.

**Michaela:** [00:26:31] Yeah. Yeah, definitely. And so maybe, I mean, what me too
is very often startup founders, especially ones that are new and maybe they
don't even have a tech background.
Right. They're like what tech stack should I use? Grade one? What what languages
and so on, should I build up? And most of the time the answer is, well, the ones
that you're mostly familiar with, right? So if you are a Python developer,
probably just stick with Python. If you're a Perl developer, maybe it makes
sense, you know, to update your texts.
Most of the time you're like, Python is just fine or Ruby is just fine. Right?
You don't have to have, like, you don't have to learn JavaScript and react if
that's not where you're coming from. But so now for your new startup, I want to
talk a little bit about that. So you're going to do something new.
How are you going to, you know, how are you going to come up with the idea? And
maybe with ties in a little bit here, it's like bedrock. So recently you
released a new product called bedrock and that's like everything you need to
know or everything you need to have to build SaaS apps. Right. So it would be
authentication.
It would be emailing a little bit community subscription payments and all of
that. Right? So sort of the boilerplate code of SaaS applications that people can
use. And when I saw it, I mean, it, it got really viral on Twitter. So people
were really like, very happy to get that. And and I think it's one of those
problems that you see people running into.
And so how was that for you? I mean, it looked like super popular. Was it also
from the sales perspective, was it as successful as you hoped and, and will the
next product that you're working on being that space or will you go somewhere
completely else? How are you going to, to tackle the next problem?
How did you come up with this idea?

**Max:** [00:28:19] Sure. So I'll start from the beginning. I I've spent the past,
basically all of my career building JavaScript tooling. I'm sort of, I would say
mainly well known for making a bunch of open-source projects, like react
boilerplate and style components that are cutting edge, new ways of doing things
right.
And I have a very deep understanding of react and JavaScript tooling and to have
a good overview of the ecosystem. And I know how things work at a very deep
level. And particularly at Gatsby now over the past year, I really dove deep
into that because Gatsby basically is just a bunch of open source 20 combined in
a very nice way.
And what I realized was that I kept building SaaS products on the sides, but I
kept doing the same setup every single time. And every single time, it kind of
sucked. Like I have enough experience to know, like I said, to avoid 90% of the
bad choices, but in the JavaScript ecosystem, it can sometimes feel like 99% of
the choices are bad.
And you have to just make that 1% of choices to make all of the tools that you
use work really well together. And making all those choices right, is really,
really, really difficult and takes a very long time. When I set up my last, my
last sort of SaaS product feedback Fisher, I probably spent at least a week just
setting up the boilerplate code, right.
Just setting up TypeScript, prettier easily in payments, authentication
database, a GraphQL API, graphical client, all of those stuff, all of that
stuff. So that it works well together and sort of is easily usable. And doesn't
just break down after a while. It's actually really difficult. And even after a
week, I wasn't happy with where I was at, but we just kind of have to build our
product at that point.
Right. Like you can only spend so much time setting up. And so after that, I
actually took what I had after a week. And I said, okay, I'm going to sit down
and I'm going to make this as nice as possible. And I spent at least three weeks
of evenings and weekends just building Building a boilerplate really like I just
plugged together glucose(??), right?
Like it's basically a bunch of configuration and glucose(??) so that everything just
works really well together. And now it's at a point where, for example, if you
change, if you add a required field in the database, your seat data for your
end-to-end test is going to throw an error that, that the required field doesn't
exist.
And the entire thing from tobacco(??) just works really well together from testing
over client, over backend, over everything you need just works really, really
well together. And I had that, I had that boiler plate and I was like, well,
this is kind of nice. Like, this actually feels really fantastic to work with
just yesterday.
I set up a new version of change feed one of my SaaS apps. Cause we were we, we
kind of need to rebuild it because the tech stack isn't very nice that we chose
there and slowing us down a lot. And so I basically rebuild all of the core
functionality in an hour. Right. I took bedrock. I added a bunch of stuff to the
API.
I added some fields to the client and it's ugly as hell. Like the client,
doesn't it it's completely front-end list. So the client looks likely to sell,
but everything works. And that only took me an hour. And of course there's a lot
of stuff to make it production ready into, add to make the build the client of
course, make everything nice at onboarding, whatever, but it works right.
And it has everything I sort of need. And so long story short, that's why I
thought about selling it. Right. And I was like, well, if I think this is nice
and it's, if it took me, somebody who really understands this problem very
deeply into really understands that ecosystem deeply. If it takes me four weeks
to set up something that's good, that that's really good.
And that, that that sort of saves people time and is better than what they could
do themselves. Then maybe it's we are selling that, that sort of knowledge and
that experience to people as a boilerplate and people were kind of excited about
it. Then I think by now I have about a hundred pre-orders somewhere in that
order of magnitude, 105, I think, which is really exciting to see.
It's kind of funny. I, I honestly didn't expect to get a hundred pre-orders
because there, there isn't even a demo on the landing page. It's just a landing
page to explain what I want to do. It doesn't even show anything yet. And yet
people, a hundred people pre-order, which tells me two things. One, the
community really trusts me, which is fricking scary.
Like that is very scary to, for me because now I have to deliver and I have to
deliver something that's actually as good as I promised, which I think I can
do, but it's a lot of pressure. And then secondly, there's a, there's a need for
this, right. People struggle with setting up JavaScript project very well.
And they're willing to pay for a solution to that problem. And so that's
exciting to see, I don't think I'm going to make this, my next startup per se,
but it's a really nice product to work on. And it's just something that I
personally really care about and I really enjoy doing. And so it was just like a
fun, fun project, if that makes sense.

**Michaela:** [00:32:36] Yeah. When I started tweet was like, wow, that's such a great idea
because I was exactly imagining something like this that you run into the
problem over and over again, you have this expertise, you have the wig Dan sort
of, right. So you're there, there's obviously more work that you probably could
in now to make this even better than what we would do for yourself.
But in general, there's like this foundation. And I mean, especially if people
want to start a SARS app or, you know, do their own startup, I hope that they're
smart enough to realize that, you know, I think right now you're selling it for
150 or 149 bucks. And later it's like 200. I mean that this is like a bargain,
right?
Because I mean, if I'm spending a month, I could do. And as you said, they
probably spend two months. They could really think about their, their solution.
They could talk to customers, they could, you know, find out which problems to
solve instead of doing that work for you. So I think it's really a fantastic
idea to, to go that route and do that.
And it's also great to see that people are backing you up. I think, I mean,
obviously it's frightening, right? If you have like, you have a platform, you
have like a community around, but it also see you also, I think it's also really
beautiful to see that. They are people who care about what you're doing and who
trust, you know, you and I experienced you as a very authentic, very honest
person.
Right. So it's not like, Oh, I'm doing everything that I do is really cool, but
like, Oh, I'm making mistakes, but I'm learning from it and I'm sharing it here.
Right. And so I think this is definitely something that people can, they
realize, and, and this is why they are there right beside you. Right. And so but
now we're coming, you said, this is probably not what you're going to do for
your, for your new startup.
So how, how is that? No, this tricky, first part, like we have this idea, you
want to do something and now you have to start in one direction. Right. And so
how are you going to tackle that problem? And, and yeah. How do you think that
you can set yourself up for success in the right direction?

**Max:** [00:34:38] I think, Multiple, multiple things. One is being very clear about what I
want to accomplish. I want to build a billion dollar startup in my life. That is
sort of the thing I want to try next. I'm not right now. I don't want to build
a, a indie hacker business. Right. I don't want to build something on my own and
I I'm perfectly happy to do that.
Right. But right now at the life stage, I'm at, I don't have kids. I'm
relatively young, still. I don't have a lot of commitments. I have the
opportunity to try and really build something that changes the world. And so I
want to try doing that. And that immediately already tells you a lot about the
problems I can tackle, right?
There's problems I can tackle with that, that are big enough. Like the,
basically the promise has to be big enough to eventually be worth a billion
dollars. Right. They have to be really big problems. If you're solving something
that's a small problem. It's never going to be a billion dollar startup. It
might be a nice indie hacker product business, but it's never going to be a
billion dollar startup.
And so I know that that already deletes 80% of the ideas I have probably if not
even 90%. And then the other, the other fundamental assumption, or, or axial I
have is that I want to build something that I use, that I need myself. And that
doesn't necessarily mean a problem that I have myself right now, but something
that we're, if it exists, I'm an, I'm a user.
Right. And I can think about what I needed and talk to my customers and figure
out what they need and sort of reconcile that with my own needs, for the
product. I don't, I'm not very good at building stuff for other people. I would
say, like, I, I'm fine at doing that, but I'm much better and much more
motivated if it's something that I want to use myself and that I want to make
better for myself, where I see, ah, This part of the app kind of sucks, right?
Like I want to fix this NAF part because it's really confusing. Right. And no
one needs to tell me that. I just feel it because I use the thing every single
day. And so again, that restricts the problems based on a lot, right? There's
only so many things I know so many problems I care about. And so immediately
that restricts the problems I can tackle a lot.
And where exactly that Venn diagram of big problems that I have sort of
overlaps. And then ideally that the other part of this is that I want to solve
something that businesses are willing to pay for it because we spectrum, we had,
we built a product that many people found valuable in that many communities
found valuable, but we never managed to get anyone to pay for it.
We never made any money. And so that's why eventually we just had to sell
because we ran out of money and our server costs were exploding, but we didn't,
we that doesn't correlate to an increase in income. And so now I want to build
something that businesses are actually willing to pay for it that solves a
problem for them that they're willing to pay for.
And so again, that restricts the progress based on even more. Right. And so the
more of these sort of axioms, I add the more of these properties I want to have
in my idea, or in the problem that I want to solve really that the smaller, the
space of possible problems kits. And I have no idea what I'm going to build.
I have a couple ideas that that I want to maybe explore. We'll see. But right
now I think. The main thing I'm doing is talking to people. Right. And I'm doing
a lot of customer research. I'm talking to people I'm talking mainly to developers
because I kind of want to build something for developers, not for again, I want
to solve my problem.
Right. And so talking to a lot of developers about what they struggled with day
to day, what their work life looks like and thinking about how one could make
that easier. And we'll see where that leads. I have no idea. It's very scary.
It's sort of a pretty scary time in my life right now because I have no idea
what I'm going to do.
But it's fun. I'm looking forward to it. I'm looking forward to the challenge
and I'm really excited to be back in sort of back in the trenches of trying to
figure out how to leave my stamp on the world, if that makes any sense.

**Michaela:** [00:38:10] Yeah.Yeah. It definitely makes sense. And I mean, I think we are in
very different situations, as you said, right?
You're looking at your own situation, do you think? Well, right now I'm really
free and I want to tackle this 1 billion dollar thing. And for me it was more like,
well, I'm completely not free. Sorry, I'm completely not free. I have my two kids and I
want to spend a lot of time with them. But on the other hand, I want to go.
And for me the thing, he was more, how can I use the time that I have right now
to set myself up for success in two, three years, right? When my kids are a
little bit more grown up. And I think that I'm getting closer and closer to that
clip where I feel like, well, maybe, you know, my time to build something really
cool will start soon.
And And so, yeah, I think this, this all, I, it really resonates with me, like
thinking about, you know, what can I actually tackle? What do I want to do?
Right. What is really my, my ambition to, to do here and then trying to figure
out. But I still think that even if you take this Venn diagram, it's a huge
problem space still, right?
So there are so many things that you could tackle. And so if you do something
like, do you try to get now this idea by talking to people, or are you going to
build a little bit and testing the waters? So, so what will be the next steps to
really understand if there is there's a market for it? Or, or do you say, well,
I'm completely committed.
This is the idea I'm completely committed. I'm going to build it. I give it a
year. Or is it like tiny bats that you do? Like, Oh this week I'm trying out,
you know, I'm sending a tweet and see if people respond or I'm building like
this little email list about something. How do you, how do you see that?

**Max:** [00:39:47] I do all of those things. It sort of depends on how serious I am about an
idea and how much I believe in it, myself. Right. There's thanks to my audience.
There's a lot of things I can validate just by tweeting. Like you said,
particularly if I'm building something for developers, I can tweet, does anyone
else else have this problem?
And then I will feel the resonance or not. Right. Maybe nobody will respond or
maybe a thousand people respond. Right. And sort of in that spectrum, I can tell
how much that problem resonates with people. And then I can think about how
would I approach solving that? There's a, there's a little validation that
happens that way.
And then the other thing is that I Just ping friends and colleagues that I've
worked with before or people that I know are using certain technologies. And I
talk to them about how they're using them and what they're struggling with. And
usually I go into those calls with some sort of hypothesis, right.
I think maybe there's this problem that maybe I could solve this way. Let's see
if they have the problem. And if you ask people straight up, do you have this
problem? Would you pay for a solution if they're friends of yours? They're
probably just going to say yes. Right. Because they're friends of yours.
They're like, they're probably not going to pay for it, but they're still going
to say yes. And so I actually go into those conversations and don't even talk
about my idea of what I want to do. I asked them what their problems are and
then I look and listen and see if they even think about that problem at all.
Right. And if they sort of stumble upon it themselves, and if they, if they're
annoyed by it, if it's grinds their, their gears, right. Like the sand in
the gears that grinds and it's been really fascinating. It's helped me
invalidate a lot of ideas and, and tell me that people probably wouldn't really
care about them.
Which has been really fascinating to do. I learned that from a great book called
The Mom Test. I highly recommend it.

**Michaela:** [00:41:12] Yeah, I know that one. Yeah. When you said that, I was thinking I should have
mentioned it, but then
_laugh_

**Max:** [00:41:18] it's really well, it it's helped me invalidate a lot of ideas. I
have very, very quickly by just talking to someone for five minutes and being
like, Hey, you know, what are your problems? What are you struggling with right
now? What do you care about? And that very simple approach would be to the
tests.
We do daycare about your. Problem. And then could your solution solve that
problem or not? And it also helps us cover other problems, right? Like I've
discovered other problems that people have. And now I've talked to, I don't
know, 10 to 20 people and I'm starting to see patterns. Right. I'm starting to
see, Oh yeah.
A lot of people care about this one problem. I wonder if we could maybe solve
something there, maybe there's a solution for that. Right. And so that, that
process is very, it's very fun right now.

**Michaela:** [00:41:53] Yeah. That's so smart. It's so smart because it's not like
just, Oh, I'm going to build this and then you build it.
Right. And you're spending so much time doing it. Then I think it felt, feels
maybe a little bit slow. And because you're not really building something, which
I think everybody wants to fill it, rightly we want to do, and we want to make
progress. And if you just, just talk to people, it doesn't feel like progress.
It feels like, Oh, I'm still, you know, even before my idea phase, but this can
pay off so, I mean, tremendously, if you're studying and you're going the wrong
direction, I actually tweeted recently about that the tiny steps actually bring
you the big success and, and, and do you have to be in the right direction?
And this is also what I, I try to be very patient with myself thinking, well,
you know, my steps are tiny right now, but as long as they are going in the
right direction that I want to go and, you know, have a go completely straight.
Right. So you, you learn and you bounce back and you think well, but if you're
open enough to see, well, this is the wrong direction.
Now I have to go the other way around. And you know, even six sucking your way
to success. I think this is so important and I see that. Yeah. I think you will
be very successful. I can can see that. And so I'm definitely going to invite
you again. Yeah. In, in a couple of years, right? I know we talk about like how
it went

**Max:** [00:43:12] That would be fun.
Yeah. We should do that

**Michaela:** [00:43:13] Yeah we should do that. Like we do that like in a year, maybe we do it,
like go on a journey. Right. So in a year we talk again and then in a year we
talk again and look how it goes.

**Max:** [00:43:23] Exactly. Yeah. I do think one of the things you, you said is
really important is, is realizing when you're doing something that's wrong when
you're building a company or when you're building a product, you're so enamored
with that product that you forget to think about
Am I even building the right thing in general? Right? You're so in the deep, in
the specifics you're showing, Oh, which button do we put? Where, what feature do
we build next? What features should we not build? What is more important? What
do our users care about? Then you stop to think about the higher level.
Does it, is this even a problem we're solving, right. Is this even something
that people care about at all? Or should I do something else entirely? Right.
And I see a lot of startup founders particularly end up with problems or
solutions to problems that no one cares about. And they never stopped to sort of
reflect on, am I even working on the right.
Thing right now, like, am I even doing something that anyone's going to care
about? And there's, there's sort of different there's different problems to
solve, right? Some are more immediate, some are problems that are problems right
now. And people try to solve them right now. And then you very quickly learn
whether it's something that people very much care about or don't care about
whether you have product market fit or you don't, if you sort of want to talk in
the startup lingo.
But then there's sometimes there's founders that are working on stuff that is
way in the future, right. They have an idea of how the world should look like in
10 years and they want to help people get there. And that is really, really hard
because at that point right now, no, one's going to care, but maybe in 10 years,
people care and you have to have a lot of conviction to sort of stay on your
path, stick true to your values and goal the 10 years to see if that's actually
the future.
That's something I'm way too scared to do, right? Like I, I don't have time to
wait 10 years. I only have very limited time on this earth. And I know a lot of
funders that are doing that and I respect the hell out of it. Right. But I'm,
I'm way too scared of that. I would much rather solve an immediate problem right
now where I know that people care about it rather than trying to do something so
big.
And so future that it would take decades to realize. Does that make sense?

**Michaela:** [00:45:30] Yeah, I think it's, it's painful. I mean, it's painful to
look at what you have invested in what you have spent your time on and to say.
Honestly, I have to do something else here. Right. It's it's like I was
standing, so I was, I was studying in London and then there was this really cool
discotheque(??) where you can go in the night.
Right. I think it was called February(??) or something like that. I forgot. And so
we got a ticket there and we went there probably at, I don't know, maybe it was
like one in the morning or something or 12. And there was a line around like one
of these huge buildings and we really wanted to go in, first of all, the ticket
was expensive.
Right. And say, if we wanted to see it and experience it. And so we stand in
line and we stand in line for an hour and I say, you know, we didn't even come,
you know, like sit around. So what are we going to do? But then, because you're
already standing in our, like, it feels like, Oh, any minute, anyway, we stood
actually three and a half hours and it wasn't a morning when we could enter it.
Right. And so it, and it was really this problem off, you know, like you're
standing already in line, so are you going away now? Or, and you leave all this
waiting time for nothing. I was really horrible. And I think that this happens
also to, to founders. I mean, it, it also happens to me that you feel like, and,
and it's, it's a blurry line.
Like it's, Oh, is there not traction because I'm doing it wrong? You know, is
there not traction because I don't have an audience yet? Or, you know, nobody
goes to, I mean, there's also build it and they will come if it's not true.
Right. So. It's a little bit different, I think for especially people that don't
have like a platform and an audience yet to say, well, I'm tweeting about this
amazing thing.
And it could be that I am getting zero likes. So one like, and it doesn't green
really mean that, that what you're building is not interesting. And so, you
know, it's not always easy to really understand is that the wrong direction or
is it not? And then to be as honest to you and take this pain to say, well, I
think it's the wrong direction.
Let's do something else. Let's start over. Yeah. So, so what I try to do is I
try to have my, my activities always have one purpose that I know it will
definitely work out. Right? So I'm doing this stuff and maybe the whole idea of
turns out, but at least I know that whatever happens, there are three steps that
are going into the right direction, right.
Is it building an audience or, you know, building a community or learning
something about the tech that I know I will use. Right. So I have, I have a
couple of different goals around something where I say, well, maybe it doesn't
completely work out, but I can for sure say that those three checkpoints that
are on my way to success, those three are going to work out.
Right. I don't know if that's something, how you think about things, but this
is, this is really my salt pattern pattern for everything I do. And very often
it's just learning right? Learning about. You know how to blog or how to do a
podcast or, you know, something like this, which brings me to the right, you
know, brings me closer to where I actually want to want to go.
And then I know I have it. I have control over that.

**Max:** [00:48:40] Absolutely. That's one of the big reasons I joined spectrum was
because I said, there's no downside, right? I get to work with two fantastic
designers that I know online that are very famous for their great work. I get to
watch them close and learn about design myself.
I get to be a technical co-founder, even though I had no idea how to do that, I
could learn how to do that through spectrum. And then the worst case scenario,
if it doesn't work out at all in one and a half, two years, I've made two new
friends, at least if not many more and learned a ton about how to build a
startup and what that even means.
Right. And so really even if the product itself had gone in a completely mood, I
knew there was no, like, I wouldn't have any regrets about it, but I knew it
could only work out and any success at the proton(??) on top of that was just a
bonus. Right. There's the fact that we got acquired, but gets up is just a
bonus, right?
Like that's sort of like that happened and it's fantastic. And it was a great
experience, but it's not something that was required for it to be a success in
my mind. Right. It was always already a success just by the fact of me doing it.
And I, I think very much in the same way that you do where I sort of consider
the, the whole, the, the implication of everything that I do on a sort of
broader scale, right.
It's not just, I'm building a startup, is it going to be a success or not? And
that sort of binary, the outcome is good or bad, but it's. How much do I learn?
Who do I get to know? What do I, what do I do? Do I enjoy my life? Do I have
fun? Right? Like all these things can tie into it and can make something a
success.
Even if maybe directly it isn't the success. If that makes any sense.

**Michaela:** [00:50:04] Yeah. That's exactly how I approach things in life. So I
think I'm fairly new. I'm happy that I got some confirmation bias here.

**Max:** [00:50:16] yeah, maybe it's an Austrian thing. Yeah. I have no idea.

**Michaela:** [00:50:21] Yeah. We can see, maybe people can reply to this episode on
Twitter and tell us if they are the same pattern.

**Max:** [00:50:30] I really curious if anybody else thinks that thinks that way.
Yeah, absolutely. Please let us know. I'm I'm I'm super curious.

**Michaela:** [00:50:34] I only start
things where I know it can,
can only be a success and it
can be a bigger success.
Right. But it's sort of the things that I'm doing are already success, right?
Independent of how it turns out. I mean, yeah. So, well, I took already much
more time than we actually that I actually set out to talk with you. So I
already stolen a little bit of your day-to-day, so I I'm going to end it here,
but we did promise that in a year I'm going to schedule again and then in a year
we are going to talk again because I really enjoy it.
I could talk on and on. And so I'm really curious where your journey goes and
how, you know, how you think about the things that we talked about today in a
year from now and 10 years from now. So thank you so much, Max, for being on my
show today, talking with me about all. All these really interesting topics and
getting, picking your brain and getting a little bit an idea of how you approach
things.
I think this was so valuable, at least for me, I hope for my listeners as well.

**Max:** [00:51:31] Thank you for having me. I hope it was interesting or valuable
or at least entertaining, I hope it was at least entertaining. And I can't
wait to be back in a year and see, I, I honestly can't wait to listen to myself.
Talk about what I've just done for the past year. Cause I'm really curious to
see where I live.

**Michaela:** [00:51:47] Cool. Yeah. Okay. So I will link everything in the show
notes like bedrock and your Twitter profile. Is there something else that you
think my listeners should know or, you know, they should check out that that's
important to you?

**Max:** [00:51:59] No, I think that's it. If by then I'll have a, start-up maybe
link that to but I don't know what that is yet. So can't link it here yet.

**Michaela:** [00:52:08] Thank you so much for taking the time and enjoy your Sunday
and talk to you in a year on this podcast again, hopefully. Yeah.
