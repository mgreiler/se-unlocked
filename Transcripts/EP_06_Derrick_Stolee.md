---
episode: "Transcript GitHub Episode 6 Derrick Stolee"
permalink: /episode-6-derrick-stolee
status: publish
type: transcript
--- 

**Michaela:** [00:00:00] Hello, welcome to the software engineering unlocked 
podcast. I'm your host, dr. McKayla. And today I have the pleasure to talk to 
Derrik Stolee. Derrik 
is a principle software engineer at Microsoft and Azure dev ops. He also 
contributes to get prior to joining Microsoft. Derrick was a professor from a 
mathematics.
If that's not intriguing, I'm super thrilled to hear from his experience, 
switching careers and working on such a popular open source system. So thank you 
Derek for being on my show. 

**Derrick:** [00:00:29] Thank you for having me. 

**Michaela:** [00:00:30] So Derek, let's start from the beginning. How comes did 
you as a former professor are now working for Microsoft as a principal software 
engineer?

**Derrick:** [00:00:37] Yeah, I think it's an interesting story in the sense 
that I. Originally wanted to be a programmer. And that's why I went to college 
for. And so I did a lot of software engineering and programming courses in 
undergrad, but I also kind of fell in love with math and advanced math at that 
same point in which inspired me to say, you know what?
I don't want to go into programming right now. At least I can, I can maybe fall 
back to it later if this academic career doesn't work out. And so I went to grad 
school and I did postdoc and I got. If faculty position, which was the dream, 
right. You know, it's so hard to get to that point. And I, and I had a lot of 
luck getting there, but then after I was there, I was realizing that being a 
faculty isn't as fun as being a grad student, there's a lot more responsibility, 
a lot more meetings.
And, uh, just the schedule wasn't quite fitting in with what I wanted to do, 
which I wanted to do, solve cool problems. I wanted to write code to help me 
solve those problems. And that was becoming less and less a part of my daily 
life. So I was sharing with my, my spouse that, you know what, maybe this isn't 
the right career for me.
Maybe I should look into doing something else or drastically changing how I'm 
doing the career. And she decided that she could also maybe decide that you 
wanted to be in a different institution. So she, uh, went on the job market and 
found a job here in Raleigh at North Carolina state. And so I said, yeah, let's, 
let's go for it.
And I agree need to move out here without even knowing if I'd have a job. And I 
was expecting to kind of need to knock and a lot of doors. But I found out that 
there was a small group here that where Azure dev ops is built here in the 
research triangle, and they happened to need somebody to do some sort of graph 
related problems.
And I was, I had experienced with graph theory and that fit in really nicely. So 
they took a risk on me because I wasn't really experienced in building software, 
in a team, in a professional environment, but I really think that it paid off 
because I was able to build some really cool stuff here. Yeah.

**Michaela:** [00:02:44] That sounds really cool. So that was also coming to my 
mind. If you are a professor for mathematics, you're probably not at the same 
time. It's sophisticated programmer, but you said that you already built stuff 
and used code to solve some of your problems that university as well. 

**Derrick:** [00:02:59] Yeah. My research area was I called it computational 
graph theory or computational combinatorics.
So I would look at a math problem. And figure out if I could solve it using it 
computers as being my proof technique, um, or at least to help me discover 
things that will lead to deeper proof techniques. So while the entry, it was 
about super theoretical problems. I was writing a lot of code, but I was doing 
it by myself.
So when I actually started and started working on a team, You know, I was, I was 
hired for my expertise, which was mature and had a lot of deep knowledge, but 
also just how to work on a team. I was making a lot of junior mistakes, you 
know, checking in to master on at 5:00 PM and going home. Without realizing I 
hadn't run the test suite, you know, those sorts of mistakes kind of happen and 
you learn how to fix them.
Uh, but it was, so that was a, definitely a learning curve in terms of how to 
interact with a team, how to do code review, uh, how to work with the release 
cycle, managed life site stuff. But none of those things had I been prepared 
for. Um, but you know, going to grad school kind of. You know, being very 
ethical, right.
Being able to learn new things is kind of what I've been trying to do for me. 
Yeah. Years. So hopefully that translated into, I can pick the start sort of 
step up very quickly. 
**Michaela:** [00:04:21] So when you went into the interview, how did you 
approach that? Did you say I'm actually not that experienced with development or 
I can learn on the job, or how about that?
How, how did you communicate that 

**Derrick:** [00:04:32] started out being very humble, you know, trying to just 
lead with, you know, I'm really excited about writing code. I definitely, you 
know, I'm switching careers. I understand that I'm not gonna be doing the same 
things and I have a lot to learn, but I'm really excited about it.
Some of the technologies, you know, C sharp and.net. I was familiar with from 
really early days. Um, but I wouldn't, I knew I was gonna have to learn a lot on 
the job. And so I was very open about that during the interview cycle, talk to 
everyone's like, yeah, I'm not expecting to just be able to do a research, like 
things anymore I'm expecting to contribute.
In fact, one person very early in the loop says, you know, Before, every major 
release everybody gets together and we spend a day during a thing called bug 
bashing. Or do we just try to break the product and we report a bunch of bugs? 
Is that something you're willing to do? And I said, yes, absolutely. I want to 
be a good citizen and contribute to the team.
And I get the feeling that that's not the answer they always get from people 
with PhDs and research background. 
**Michaela:** [00:05:34] Yeah. Yeah. Yeah. So I think also my experience and see 
that there is some, Hm. How to put it, maybe. But some reluctance of researchers 
to actually do the daily work of developing software. And so I think it's just 
fair to ask whether or not that's actually something you're committed to and 
whether that's something that you would want to do.
Right. But now that you program on a daily basis, do you think that the work 
that you did prior to that? So the work you did as theoretical mathematicians 
shaped your mindset as an engineer, and does it influence how you approach 
problems? 
**Derrick:** [00:06:08] I think it, I think it does, especially when I'm trying 
to, sometimes sometimes I'm able to say here's a really deep algorithm insight 
and here's a connection to something that's actually math, but it's not super 
important that you understand the math it's.
Do you understand that it's working correctly? And how do I prove that to my 
peers? Or how do I break down a problem into pieces? Uh, that's also one of the 
biggest things to be able to do research mathematics is, you know, I want to 
prove this big theorem, which is like the big result, but in order to get there, 
you have to prove a lot of smaller pieces called lemmas that then combined 
together an interesting way to create the full argument like that breakdown into 
kind of components is, is very important to be able to isolate how much logic 
you have to keep in your mind at one time.
But then also there's the idea was that after you prove a big theorem, you try 
to look for things that can be easily proven after that you get your corollaries 
and in software, I think that's really important. You know, you want to, as 
you're building to this big finish, have these smaller components that are 
reusable are testable and can be developed, delivered in a small commit, but 
then they build that a large piece.
But then once you build this large piece, Is that the end game or is there 
something else you can do? Is, is there now that I have this can something else 
fall out of that? 
**Michaela:** [00:07:35] And so can you tell me a little bit about the interview 
experience? What do people ask a former professor during an interview? Did you 
experience a typical interview process with white boarding coding exercises or, 
yeah.
What are people expecting from you? 
**Derrick:** [00:07:50] Yeah, the interview process has updated a little bit 
since the four years ago where I, uh, interviewed, but there's some similarity. 
And I remember the first part being, uh, uh, over the phone. Well, you know, via 
computer chat where I was given a programming problem and I was supposed to 
share my screen and do a text editor to.
Actually do the program. And I remember that the problem I was given was 
actually a homework. I had assigned my C programming students a semester ago, 
even like, you know, are you sure you want me to solve this problem because it's 
probably not going to be hard for me. Uh, but they, you know, went through it 
and they, it was more about.
Can I explain the solution and, you know, if there's a, there was a twist at the 
end, like, okay, now that you've built it this way, for the simple case, let's 
make it a little bit more complicated. And can you adapt to that change of 
requirements? I thought that was a very interesting way to take this. What could 
have been a simple problem, but turning on his head a little bit.
And then I got to the onsite interview. There were several of those that I met. 
I think I met with four people. Um, and I remember at the time I was. 
Interviewing. I, I talked to four, uh, three principle engineers and one senior 
engineer, and I was thinking, wow, there's a lot of principal engineers here 
just turns out.
It seems like they were trying to figure out what seniority I should be coming 
in at because of my lack of experience. So they put their best people on to make 
sure what I knew. And again, it was a lot of the white boarding, siders 
problems, sorts of sorts of situation. You know, here's a problem. Explain to me 
your solution and actually try to write some pseudo code on the whiteboard.
And even the whole time I was feeling it, I was like, I think I'm actually well 
qualified for this specific type of interview because I solve problems all the 
time. I did programming competitions and undergrad. So I feel like they weren't 
really necessarily getting to how good of a sound engineer could I be.
Uh, and I felt like I was. Unfairly succeeding in those things. But then I got 
to my optional interview, the one that the very end where it's like, this is the 
person that's going to do the side. If I did badly at the other ones, they 
wouldn't even talk to me. Uh, that's usually a common thing. And when I got to 
that person, they do mostly was.
They were asking me the higher order questions, you know, what has your biggest 
success, Ben? How would you design a system to do something as opposed to show 
me how you can write code? And so that one, I actually then got very nervous in 
retrospect. I think I did. Okay. I know they hired me anyway, but I went for 
awhile thinking, why did they say yes after that interview?
But. It worked 
**Michaela:** [00:10:31] out. So when you started working at Microsoft, what did 
you actually start working on? So what is your project that you are contributing 
to? 
**Derrick:** [00:10:39] When I first started, I joined the team that, uh, builds 
what is now Azure Rebos and working on the get server. And we have our own 
C-sharp implementation of a good server that is very focused to work in our.
Uh, architecture of Azure dev ops, and there were some scale problems we were 
running into because at that point we had not built it strong enough to 
withstand the windows repository, which now the windows iOS repository is 
running and get on Azure repose. And so that was kind of our North star of, we 
need to make this scale to that size.
And at that point we were using just the Azure DevOps code. And some other ones, 
uh, internal customers, but we were definitely the largest repo at that point. 
And we were running into scale issues there. And the thing I was hired to do was 
to fix our commit history story. Uh, there was a really interesting design 
decision, mostly because this is all built based on top of TFCC.
Our team foundation version control was the same team who built that started 
building the get server and team foundation version control is primarily run 
through sequel. SQL has all the data and it's very centralized. So it's really 
easy to use SQL as the centralized source of truth. But then a lot of those 
architectural decisions transferred over to the good server, including using, 
trying to use sequel for commit history.
And it was a very impressive attempt, but it wasn't, they can never get it to 
match what get log would output and customers were complaining. And the biggest 
issue is that commit history in get is an, a graph. It's a directive, basically 
graph. It is not a linear history and you need to be able to navigate that.
And so I was, when I, after I did my first couple of months of getting used to 
the system and fixing a few small bugs and making sure I knew how to interact 
with my team, I moved into the, working on that problem and deciding like, what 
is the solution there? And the solution we came about was to create a 
compressed.
Commit graph that was focused on the structure between the commits. And once you 
start at one, you can walk the rest very quickly and a lot of algorithms to make 
those walks be fast, but also just having a new file format. And it wasn't 
something you could do in SQL. You just have to make a new binary file and have 
a job that keeps up to date.
And that allowed us to do things like when you look at commit history in the web 
on Azure reposts, you see it in topological order. Uh, that was kind of the 
thing that we knew was a differentiator. The, the command line has to explore 
every commit possible. And so even on our small repo, it took seven seconds, but 
we could do it in 200 milliseconds.
And that was kind of the, the, the ground, the start of being able to build 
these bigger and bigger features to get us to the window scale. 
**Michaela:** [00:13:40] Okay. So maybe to give a little bit of context, this 
was actually the time when windows tried to move over to get and use, get as a 
source code repository and versioning system.
Right. And the problem they ran into was that windows was, or yeah, is too large 
to smoothly work with guests. So then your team was responsible to help out at 
that point. And those tweaks that you described plugging into that larger effort 
of making good work. With windows or windows with get, is that correct?
**Derrick:** [00:14:09] Yeah, so that, I'm just talking about one small piece of 
a large system that you know is about that. And it was focused very much on in 
the cloud. How does, how do the cloud servers stay running with so much data 
that they're processing not, and. Because was also that it grows right. As 
people are interacting with it, there's the scale of 4,000 engineers are pushing 
and pulling and all that.
But it's also just after a year, they've got millions of commits. And what do we 
do with that? In parallel, uh, other colleagues on my team, we're building, uh, 
what is now called VFS forget, which is a tool kind of built around good for the 
client site experience and making that 
**Michaela:** [00:14:52] yeah. The individual pilot system, right?
Yeah. 
**Derrick:** [00:14:54] A virtual file system. Forget it allows it instead of 
needing to have every single file. In your source directory, actually be 
present, have get managed. All of that. It uses a file system driver to act like 
it has it, all that. So it's kind of projecting what get expects to be there. 
And so if you look at it and explore, it looks like all the folders are there, 
but as you start drilling down, we're dynamically populating that data as you go 
down.
And that's how you can take this 3 million file repository at a single checkout. 
And really you only need maybe 200,000 files out of there. You don't need to 
have all of them. 
**Michaela:** [00:15:31] So are there other projects that you are aware of that 
are also benefiting from that? So is it something other larger repositories out 
there could use or is this really, really specific to windows and the repository 
of 
**Derrick:** [00:15:43] windows?
I think that there's a lot of things that are specific to windows. Uh, but also, 
you know, we're working currently with the office team to get them moved over, 
to get, and they have very similar scale targets. But in terms of those are the 
only two repos we've seen out in the wild that are big enough to really require 
that.
It's complicated system. And part of that is because, uh, in the process of 
making this client experience better, a lot of it's just, you need to make, get 
better in, you know, get as a very core part of this. Yes. We've added a lot of 
bells and whistles around it or integrated pieces into it. But those have 
actually gotten into the core products that get is actually so much faster and 
can handle what other repos are out there.
**Michaela:** [00:16:29] Okay. Can you explain a little bit more to me how the 
work that you do at get, or get for windows or get from Microsoft fits into the 
work of the open source project get, how did those two projects connect and 
well, where do they differ? 
**Derrick:** [00:16:44] Yeah. So a couple of years ago I switched teams from the 
server side into the client side.
And part of the goal was, you know, I've got all these ideas and thoughts. We 
did integrate into the server side and it's like, I wanted to contribute those 
into the client and make the client faster. And I could see that we were going 
to have issues on the client side for the, even on the window scale, because we, 
while the investor get, had all these things to make the amount of data 
transfer, be less and all these work directory things.
I knew that as we grew, we were going to have some problems. So 
**Michaela:** [00:17:17] this is not a good client. 
**Derrick:** [00:17:19] Yes. So moving over from the service side, into the get 
client and the get client has, I would say there's a few forks a bit. So if you 
go to github.com/get/get. In a good organization that get repo is they get code 
that is maintained by the get community.
And it's, it's reviewed all code is being submitted through a mailing list and 
it's being maintained by the one maintainer of get who has been maintaining it 
for many years. Then there, get for windows slash get and they get for windows 
thing, which is a fork of get that has a lot of extra things just to make sure 
it works on windows properly, because it was built for Unix machines.
There's a lot of assumptions about that and making that all work through a 
compatibility for windows. Uh, it goes through that repo and that's maintained 
by my colleague, Johannes gentlemen. He does a great job. And that's where if 
you were to download, get for windows. You would want to go there a while that 
gets slash get is mostly cross-platform, you know, it's got the core version.
You can install it on the Linux immediately. You can stall on the Mac, even 
installing the windows. We just might have a few, uh, rough edges. And then we 
have our Microsoft slash get fork. So in the Microsoft organization on get hub, 
and that's where our team is running things on top of the get for windows.
Uh, patches, things that are specific only tied to VFS forget. Uh, so there's 
some things that we'll never make upstream because they're really just when we 
are in this particular environment, we need these patches, but sometimes we just 
take performance fixes a little bit faster there, but the intention is we want 
that fork to be as small as possible.
So we are trying to, uh, send all of our performance enhancements to the main 
line, to the core, get project. So that way, everyone who uses get anywhere can 
benefit from these improvements. 
**Michaela:** [00:19:15] Yeah, that actually means you're in a very interesting 
position. So you work for Microsoft, but not solely for project Chris owns or, 
um, built, but in contrast, you're working on an independent open source project 
and the kit and you help well enhance kit and change and develop this open 
source project.
But it should go into a direction that is also beneficial for both Microsoft and 
the open source community. This means that you have to constantly think about 
win, win situations and how every stakeholder benefits. How is that reflected in 
your daily 
**Derrick:** [00:19:46] work? Yeah, it's really interesting too. When we could 
internal our team saying what's our priority list, that's definitely motivated 
by what what's our next scale target.
What issues are internal customers having a, what sort of things do we think, do 
we need to get ahead of before? They're a problem. But then we need to take 
those ideas and bring them in, connect them to what, how is the L the community 
going to respond to these ideas? How can we make them as beneficial as possible 
for everyone?
And so a great example is I took the idea of this commit craft that I built for 
the server in the C sharp layer and said, we should have this and get as well, 
uh, without it. These windows developers are going to have a lot of difficulty 
working with the millions of commits they have, but also let's take a look at, 
you know, let's take a look at a regular sized repo, like the Linux kernel 
repository, or just the get code itself.
You know, the gate code has 38,000 commits something around that line. That's 
very small compared to the windows repository, but I was able to demonstrate, 
Hey, if you use this commit graph file. Even the getrepository will speed up. 
And you know, it goes from maybe three quarters of a second to a quarter second, 
but that's enough to notice that a user ran a command and it either responds 
immediately, or you had to have a pause and then it responds, or in the Linux 
repo, it's something that took 10 seconds.
Now it takes one second. And having that. Be mean that this is going to be a 
realistic improvement for a lot of engineers. A lot of people working in get 
that. That's what makes it worth the community's attention. 
**Michaela:** [00:21:31] Yeah. One of the things I was thinking about about, 
because on your Twitter profile, you say you are making get faster, was how you 
make such a mature and widely used project faster.
And it seems that you are really talking about algorithmic changes to the 
underlying system. Is there something else you do to improve the performance of 
such an implant? 
**Derrick:** [00:21:51] Yeah, the, the, sometimes it's, you know, let's make the 
code do less, right? Here's a, you know, we have this black box of the get 
command should do X.
And can we make it do X without actually doing as many operations? So is there 
a, just a, you know, the algorithmic view is can we just modify the order of 
which we're computing things? The other way is to say, can we do some sort of 
caching where the commit graph is this thing that if you just run this one 
command.
It'll build it and now it's on desk and now we don't have to do all these 
parsing, these expensive parsing later. We've kind of pre-computed and save that 
time and later things. So we're not actually changing how many oppor or how many 
commits we're inspecting. We're just making that inspection faster.
But then there's other things where it's like, well maybe if we just change how 
it works. Like, maybe it's doing something that it doesn't need to do. Uh, one 
example is in the status command, if you have a local branch and it's tracking 
an upstream branch in your remote it'll status will say, Hey, your local branch 
doesn't agree with the remote.
You are a hundred commits behind an eight commits ahead. So you can say, Oh, I 
know that there's a difference here, but there's also that count. That count. 
Isn't always super helpful in the sense that especially say the windows 
repository, where you wait a day and your 10,000 commits behind doesn't matter 
that you're a hundred commits behind or 10,000.
But if you are 10,000 computing, that exact count is really expensive. So, you 
know, we modified that command to say, well, if you put in this config setting, 
it'll just say you will differ. I don't know how by how much, but you're just, 
you don't have the same ref. So maybe you want to rectify that at some point, 
but it doesn't cost you every single time you run status, do this expensive 
computation for values you don't really need, but it is changing behavior.
The, the, the output is different. 
**Michaela:** [00:23:50] Well, so now you're working for several years on the 
problem of improving the performance of kids. So I wonder, is there still room 
for improvement? Is there still opportunity for that or are you now looking into 
other areas? 
**Derrick:** [00:24:04] There's absolutely ways to improve it. And you know, one 
of the big things we're trying to do that.
You know, it's been a, kind of a, the whole community has been trying to figure 
out how to do it. Is that VFS forget one of its the ways it works. We made a 
custom protocol that you know, is currently only implemented on Azure repose and 
it doesn't use get to do it. It's just, how can I transfer some amount of 
objects?
But not the whole repository. Like if you do a get clone, you get every single 
object that those commits can reach and how, how can we make that? So it's not 
so expensive. Maybe we don't need to do that. And the community had with some 
Microsoft people and some Google people and other community people have built 
this idea of called a partial clone where you say, maybe I want to have, I want 
to do a clone, but I don't want to have any of the blobs.
I will ask the blobs as I need them. That would be a dramatic improvement to 
clone because you don't have to have every version of every file in your 
repository. When you do a checkout, it'll say, Oh, I don't have this blob. Let 
me go download it. And that is still being. Uh, maturing on the, in the 
community.
I would say it's one of those things where it, it's definitely the, the next big 
way to allow vanilla get just regular, get out of the box to scale, but it 
requires not just the client improving, but the server experience, improving, 
making sure that the way we're doing these problems can actually scale for that.
The services do not fall over when people are asking for all these blobs. And it 
just changes the way you work with, uh, uh, with gets so much that it needs to 
go slowly. 
**Michaela:** [00:25:45] So, okay. When you say it needs to go slowly, what do 
you mean by that? 
**Derrick:** [00:25:49] Uh, it goes, it goes slowly in the sense that, you know, 
we had to agree first on what does it mean to be a partial clone?
Where, where do we draw the line? And then it's actually been implemented in the 
client that you could have, you could, could request a partial cologne, and 
we're at the point where the services are still trying to figure out, you know, 
how do we. Be able to serve partial clones at scale, and actually be able to 
turn it on for, uh, for clients.
But if you actually just use, get itself to run into patchy web server, you 
could set up one that has partial clone. It's just might be a little slow. It 
might have some performance issues on the server side, and we're still trying to 
track down all these different places where get isn't really good about handling 
that.
That expectation of, I want all my objects because it sucks. I couldn't all be 
there. And so there's all these usage patterns where it'd be better to ask for 
this set of objects in a big batch, as opposed to asking for them one by one and 
get still trying to figure out how to do that. 
**Michaela:** [00:26:51] So if I imagined that people are listening in now and 
they are as excited about algorithms as I am, that they think, how can I 
contribute to such an interesting project?
You also mentioned that Google and Microsoft are working on that project. So who 
are the other players that contribute to that open source project? And how can 
others outsiders have their say or be part of that open source project as well? 
**Derrick:** [00:27:14] Yeah. So, you know, in addition to people at Microsoft 
and Google, there's also our colleagues at get lab, get lab, get hub, and all 
the other places that kind of run get as a server.
And there's also just a lot of community members who they're just really 
passionate about get, and they are very. Uh, present on the mailing list, which 
is how we do all of our code review and all of our communication about where she 
gets you go. Uh, you could find out most of that, if you want to just look at 
what the history and the archive is, you go to public dash in box.org/get, it 
has a list of all of our discussions.
So it's out in the complete open. You can also join the mailing list and there's 
some instructions on that inside of the read me forget. Okay. The thing that's 
interesting is that get doesn't have a backlog. There's nothing where the 
maintainer says, this is the vision I have forget, or this is what these are the 
things we've accepted as being the place we want to go with.
Get it's more reactionary to people, come with ideas about here's something I 
think get could improve in. And here's something I, I, I am passionate about. 
Uh, and that's usually how things get done. Somebody comes in and says, you 
know, this feature doesn't work the way I want it to, or doesn't work as well.
Let me go and try to do something to help. And then the community decides, is 
that something that is valuable? And 
**Michaela:** [00:28:39] do you know, what is the percentage of individual 
contributors versus contributors of larger organizations? Do you have an idea of 
the proportion? 
**Derrick:** [00:28:48] I would say it's probably, I would, I would guess half 
and half.
I would say there's about half that are, you know, that it's clearly their day 
job to work on this. And then half where it's just, they are passionate. They 
work on evenings and weekends and are very vocal about, you know, the things 
that they care about. 
**Michaela:** [00:29:08] Yeah. That is quite an essential number. Actually.
Quite a few people are involved in that project. It seems. 
**Derrick:** [00:29:15] And I'm sort of thinking about this in, in a weighted 
sense. Cause not everyone is contributing at the same rate, so there's 
definitely many more individual contributors in terms of just literal number. 
But again, because they can't, they can't spend all day every day thinking about 
it and contributing that they're.
Their rate of interaction on the list is, is smaller. Sometimes there's also 
some individual contributor contributors who contribute way more than even me, 
because even though it's my job to do that. So, uh, but I would say in terms of 
the volume on the mailing list, I would say it's half and half. 
**Michaela:** [00:29:52] Okay, well, you mentioned already code reviews.
So I want to know a little bit more about your engineering practices that you 
have. So you do apparently do code reviews. How do the work and, well, I know 
that good actually is driven via a mailing list, like many open source projects. 
Can you explain a little bit about how to do code reviews via. Well, how does 
that work?
**Derrick:** [00:30:15] Yeah, it's very interesting that, you know, we use email 
even though, you know, we, we are building get, but get, has ways of creating 
patches, uh, email patches based on the commits. So it'll include your commit 
message, uh, information about who wrote the commit and when, and then it 
essentially supplies the diff for that commit.
And that's what you send up. Now, you can group those patches into a thread of, 
you know, a patch series include a cover letter, and that's usually how you 
would do it. And the cover letter can kind of justify here's the full series of 
commits and what the whole series is trying to do. And that way each individual 
patch can be self contained, can be small enough for a human to digest it and 
review it on its own.
And. What happens is, is that the email threads sort of starts to expand. You 
know, people will reply to each individual patch saying this part of the patch 
could be better or here's, here's a style issue you had, maybe you could write 
it this way. Hey, I don't understand how this is going. Could you explain it 
better in your commit message sometimes it's maybe you don't need both of these 
patches.
Maybe you should combine them or this one's too big. You split it up. There's a 
lot of attention to detail that's for sure. Way more than I've ever experienced 
on any other project. Uh, because, you know, get is used by so many people that 
it's really important that it doesn't break and it's built in C you know, which 
is, uh, uh, it doesn't have any memory management, a, you know, it's, it's very 
fast, but it can, it isn't very forgiving to programmer mistakes.
So having all of these things. Be meticulously looked over is really important. 
So that way we know that this change that we're making one is, is valuable, but 
also has low risk. It's low risk as possible. Every change has some amount of 
risk. But can we find ways to minimize that? Or at least if we have risk 
localize it to a place, like maybe we hide it behind a config setting for now, 
and we'll, we'll move that can fixed setting to be default later.
Or maybe it's just a, it's just when you have this particular feature and then 
we'll expand it to use later. Um, how can we kind of limit that? And then also. 
Do you test it enough? Do you know how deep do you want to go on your testing to 
make sure that this is going to be covered? And not only it works right now in 
the building, but a year from now when people have built upon it or change some 
of the underlying API APIs.
So. Maybe the things you're relying on don't work the same way is your, is your 
feature going to be working correctly? Yeah. 
**Michaela:** [00:33:00] Testing is one of the things I wanted to ask you about. 
So is there some policy around testing, do you have to submit a test with every 
batch that you submit or how does that work?
**Derrick:** [00:33:09] It really depends. Uh, get, has the overall opinion, is 
that test should whenever possible be. Uh, user-facing tests in the sense that 
we're building a real repository and we're running a real get command and 
expecting certain output. So it's not the typical unit testing you would expect. 
**Michaela:** [00:33:28] That's an end to end test.
**Derrick:** [00:33:29] Yeah, I would call it end to end test as much as 
possible. Uh, there's some limits in terms of, you know, we don't always do big 
fetches across an HDP connection. Sometimes we'll just do a fetch across your 
file system. To kind of mimic that, but also demonstrate some other behavior. 
But the, I means the test suite is really a bunch of shit, all scripts that 
execute a bunch of good commands.
And so we're, there's some limits in terms of how specific those tests can be, 
you know, can we actually get it to trigger this air conditioner, this assert 
statement? It's not always possible. Uh, one thing that I did, uh, I think it 
was last year because I realized that I had accidentally not tested something or 
the test I had written wasn't actually hitting the code.
I thought it was heading, uh, there was some code in the make file to run it 
with, uh, GCC with the right things, to do coverage analysis. And you could run 
the test suite and see what had been covered or not. Now, if you run that on the 
gate code base, you're going to find a lot of lines are not covered.
Partly because this philosophy that, you know, we try to cover the main 
scenarios and some of the error scenarios, but what's valuable is to say like, 
what, what has been attributed recently that hasn't been covered? You know, have 
people been writing new code without creating test cases? And so I started 
creating the test coverage report, which means that every.
A few weeks, I run this build and I run test coverage. And then I do the diff 
between what was master on, you know, two weeks ago. And what is master on now 
and all of those lines in that diff which aligns are uncovered. So did you 
change something that wasn't covered before, or do you add a new line and you 
didn't produce a test case for it?
And that's been really interesting to see. Especially as that report's been 
coming out, how it's been getting smaller. People don't want to be in that 
report anymore. So people are being very careful to include better test cases 
and cover all these scenarios and definitely send in the year or so since we 
started doing this, people have, uh, I think people have been seeing the test 
cases improve.
I definitely have seen the reports get smaller. Uh, there are many fewer 
uncovered lines being introduced. 
**Michaela:** [00:35:50] Yeah. So one of the questions I like to ask you is, are 
there some differences between how you develop software at Microsoft? So for the 
projects that are Microsoft internal or completely owned by Microsoft and the 
good mailing list.
So do they, engineering practices differ and if so, in which ways, all 
**Derrick:** [00:36:08] right. Yeah. I would say that, you know, when you're 
working internally on a team, there's, you know, essentially anything you're 
working on is sort of assume that. This is something that's on the backlog, your 
team lead, and your program manager have decided this is something important to 
do.
And so, as soon as you create a PR, everyone says, okay, you are working on 
this. You want feedback? I don't need to say why is this important? Because 
there's some reason why it's important. Uh, and we just need to work on making 
that the best version. It can be well, and to get mailing lists every single 
time you submit code, you have to say, this is some justification for why I did 
this and why we should take it.
No one else in the community has like created a backlog that says, Oh, look, 
just look here. We've had this on our list for, to do for awhile and no one's 
gotten around to it. I'm getting around to it. It's I had this idea. I think 
it's helpful. Here are the benefits for users. Here are the benefits for people 
in the community.
And the other thing about it is that usually the poll request is the unit of a 
review. I'm reviewing this, this pull request. Make sense. Should I merge it or 
not? While in the mailing list it's is each individual commit each patch worthy 
is each patch perfect or as perfect as it can be. And being able to justify 
small changes with a paragraph of text is a skill that needs that I have been 
working on and still working on, because it can be very difficult to actually 
take some change that.
Needs to be big in order to make the change you're going for, but then breaking 
it down into smaller pieces so that people can understand it can digest it all 
at once. They don't have to just review thousand lines of code. They can, you 
know, take, you can take that thousand lines of change, split it across 10 
commits and suddenly.
It's a little bit more digestible. 
**Michaela:** [00:37:56] So this means that there is no actual roadmap for the 
good project so that you can say, well, that's our roadmap. That's where we want 
to be in two years. 
**Derrick:** [00:38:05] Right. Right. That's you know, a junior or the 
maintainer is very busy just taking in all the input. Like there's plenty of 
ideas coming in from the community that he's not reaching out for.
Hey, let's do this as well. Um, it seems that he's much more about where did the 
community want to go? He doesn't want to dictate. This is where we're going. He 
just wants to respond to people's feelings. And you know, what sort of 
situations are there that we need to resolve now? Uh, very much believing. 
**Michaela:** [00:38:34] And so can I imagine that it's decided in the moment, 
so I'm sending an email and saying, well, I want to improve the performance of 
that piece, for example.
And then it depends on the feedback that I got to this email. So let's say how 
many years and nays do I get from the community decides whether or not this. 
Change actually happens or not. Right? 
**Derrick:** [00:38:56] Yeah. I guess there's, you know, we can say things like, 
here's an idea I have, I haven't even started building it.
You know, just I'm looking for comments. Is this a good direction to go? And 
people can respond saying, yeah, I think that's a great idea. You should watch 
out for this. Here's. Here's why I didn't do that already, because it seems 
challenging in this way. Or you can say, you know, what I frequently do is I.
Quickly build something. I haven't perfected all the patches. And I say, I'm 
spending an RFC and request for comment saying here's a rough outline of how we 
could build this. Do people think this is worth building? Uh, do people see 
problems with my approach? Because I, you know, before I go and start building 
all these test cases and really polishing and doing a bunch of deep perf work.
Is this even an idea that we want to think about. And sometimes people come back 
and say, no, this isn't actually what we want to do. You know, going this 
direction would be better. Or, you know, that's just not the way it get works. 
But sometimes I say, well, yeah, you know, we've had this idea before here's the 
previous discussion.
Even people have found that in the archives, you know, things from 10 years ago 
that I wouldn't have no reason to unders to know that existed. And they can say, 
this is why we didn't do it. Then. Can you solve those problems now? 
**Michaela:** [00:40:10] So this means that there is only one place and that's 
the meeting distance.
Everything is discussed via this mailing list. And while there is no other place 
like a board where you, for example, have issues or milestones that the 
community members can vote or comment or discuss on, it's really just the 
meeting list. 
**Derrick:** [00:40:29] The philosophy I've heard is that if it didn't happen on 
the mailing list, it didn't happen.
But there are other ways of communicating. Um, we have a, an IRC channel, for 
instance, occasionally people put up, uh, uh, different places where you could 
submit issues or things. Uh, again, my colleague  has made the submission 
process a lot easier. He built a tool called get get gadget, and it's actually 
how I submit my patches to the main list.
You go to get hub.com/kitkat gadget slash get. And open a pull request there, 
you know, they get community, doesn't take pull requests, but you can create a 
pull request and then type slash submit in your comment. And a bot will pick it 
up, convert those commits into emails, and then send them off to the mailing 
list for you and even handles versioning.
Like if I, if you update it and you say, okay, now I've changed my commits to 
respond to feedback. I push it again. It'll say, Oh, here's patch series V2. And 
it's all nicely threaded. It shows a diff from your last one. It's really, 
really nice. And there he's got a, he's been storing issues as well. Like here's 
an issue that is maybe somethings for a new contributor or could be helpful, but 
it's, it's mostly because it's been discussed in the list.
He's like, well, let me create an issue for it and links to it on the mailing 
list saying, you know, if no one's gonna pick this up right now, I've archived 
it here as well for other people to look at and, and point to. But that's also, 
that's part of the decentralization of get is that while there's the mailing 
list is the central point for all of get there's.
All these little bifurcations of this sub community talks about it over here, 
and this subcommittee talks over better over here, but when they want to bring 
it into court, get they talk it on the mailing list. 
**Michaela:** [00:42:16] So the main decision, power lies also in the mailing 
list and while the community there. Right?
Well, one of the things I wanted to know is you're talking about the good 
maintainer and in general, maintainers of open source project seem to have quite 
some authority over the decision making process. So how much do you think, for 
example, the good maintainer has the final say in whether something is going to 
be implemented in good or not.
**Derrick:** [00:42:43] Yeah. Um, junior Romano is the maintainer and he 
definitely does have the final say in terms of which commits get into the 
releases. He, you know, I found that he's been very reasonable to, uh, take 
ideas that are out there and kind of defer to, to the community. And that's kind 
of his stance. He is, uh, he has shown and also said explicitly that that's his.
His mode is what does the community want? I'm here to facilitate that, not to 
dictate from above, but to just be the central source of, you know, maybe the 
final guard in terms of quality, but not necessarily, you know, I don't want 
that and because I don't want it it's, it's not in its, you know, he'll 
sometimes voice an opinion.
And if enough people say, you know what, this is really important. He will. 
Probably change his mind as opposed to just given. Uh, but also, I don't think 
that that happens very often. Like, you know, he doesn't, he tries to let 
people, one thing I find is that he tries to let other people to review patch 
series before he gets to them.
Partly because there's just such a volume of, of code for him to be able to read 
it all as it comes in the first time, it'd be better. If somebody comes in and 
says, Oh, I can find your silly style issues, or I found this performance 
problem, or here's why you need to rethink it. And then he comes in with his, 
you know, very deep knowledge and very, you know, very particular to the, get a 
community knowledge and can find things that no other reviewer would find.
But he tries to do that after everything else has polished and he's getting 
ready to merge it in. And then he has his own method of giving enough cooking 
time for something to make sure like, Hey, you know, it seems like review is 
calmed on this. I've got it in this branch. We can do some testing. We can build 
upon it.
Make sure there's nothing weird. And then it finally gets in the master. 
**Michaela:** [00:44:34] So that means that every patch via the mailing list is 
reviewed by the good maintainer and that the patch will never be merged into the 
code base without his approval. 
**Derrick:** [00:44:44] Uh, yeah, I would say that, you know, every single 
commit outside of the times when he's on vacation and is appointed as some 
maintainer, if you look at the good code base, he is the committer.
Uh, and that's the idea that the committer and author are different is very much 
a get centric thing because of the way it was designed for this mailing list, 
sort of a contribution model where the author is the person who submitted the 
patch. And then the committer is the person who took that patch and created a 
commit.
And so every single thing that gets from the mailing list into the get repo has 
gone through his computer. And so at least at that sense, he has stamped it as 
something he's willing to take. Now, sometimes it's, here's a subsystem that I 
don't know very well that we're really just taking updates from stuff that's 
been going on elsewhere.
Like get gooey is particularly one of those things where it lives in the gut 
code base, but it's kind of the second tool that isn't critical to the rest of 
networking. So they get gooey has its own container and just pushes updates. And 
then a junior takes those. But a lot out of it is, you know, even this change 
over here, uh, to this one, builtin could have rippling effects to the rest get, 
uh, he is, I've been amazed at the amount of attention he's been yeah.
Able to pay to all of these different changes in all these different areas. 
**Michaela:** [00:46:06] And so do you know what is the process of becoming 
invitation? So if I want to become an open source maintainer, what are the steps 
I have to take is an open source, maintainer selected or elected. Is there a 
democratic vote now and then about who should be the open source maintainer of a 
given project?
How does that work? 
**Derrick:** [00:46:27] I know for the forget in particular, it was like it was 
started by Linus Torvalds. And Linus wanted to be able to do more curdle 
development and not have to maintain get. And junior was there doing lots and 
lots of that early development of get and knew most of the system and Linus just 
trusted him to be the maintainer.
And that's just how it's been. Uh, he occasionally appoints people who are 
trusted members of the community to be maintainers when he wants to be on leave. 
Uh, and those have been people who have been in on the mailing list for years. I 
have been at trusted opinions in terms of, if that person reviewed it, junior, 
doesn't need to review it sort of like that quality of person.
But I, and then there's also a board of, of people who are kind of, you know, 
there's some, somewhat of a governing body, which is more about a vote process 
and that's less about what commits specifically, but where's the good community 
want to go? Things like protecting the, get trademark. And who, who is, who is 
paying for the get-scm.com, which has all our documentation on it.
That that board is, is democratically alive. It did. If you wanted to become an 
open source maintainer. The thing you need to do is build an open source 
project. And, you know, I'm technically a maintainer of several repos I put on 
GitHub, but you know, they're more of a toy toys that I've put and yes, people 
could go contribute to them and I'd probably pay attention, but I'm not actively 
pursuing a community.
Like I'm trying to build a community around it. If you really want to be a 
maintainer of a community. It's how do you actually attract new people to your 
project? How do you get people to use it enough to care? And that's really 
tricky. 
**Michaela:** [00:48:11] Okay. But yeah. So coming back to the maintainer and 
the role of a maintainer, can I imagine a maintainer similar to a founder of a 
company?
So there is sort of a belonging of that open source project to the maintainer, 
because he said, if you want to be a maintainer, then you have to start your own 
open source project. So somehow the maintainer owns the open source project. Is 
that something that you could take away from the maintainer. 
**Derrick:** [00:48:37] Uh, you know, if you wanted to make a forklift, get, you 
could, you know, it's all open source.
It has GPL license. So you can always create a fork of get. And in some sense, 
that's what we've done with good for windows. Right. Good for windows is a fork 
of get your harness is the maintainer. Uh, but he's also similarly just, he's 
just trying to make sure that get works as best as he can for windows.
If there's a fix, that's actually a good fix. It goes back into core kit and 
he's also been working really hard to reduce the distance between those two 
forks. And so you can always create a fork. The question is, will anyone care? 
So in a sense that we do have free and open software and get, but if you want to 
be on the version that is getting all the fixes, that's getting all of the 
improvements.
You should move along with the community as much as possible. 
**Michaela:** [00:49:27] Well, yeah, I definitely agree. The community, the 
healthy community is super important. So I'm not suggesting to take over an open 
source project, like a pirate ship. Right. So, well, I think we've covered 
really a lot. Um, is there something that you want to say to round up that 
interview in a good way?
**Derrick:** [00:49:44] Uh, I guess I just want to mention that, you know, the 
gay community is working really hard to, uh, be more open to new contributors. 
We find that it can be really difficult for especially young contributors who 
maybe don't have as much experience in see, or have never worked with code 
review on a mailing list before.
And they're used to, they've always been growing up doing pull requests as their 
model, uh, that can be really daunting to people. But in the community, you've 
had a lot of discussions about how can we improve that environment for the new 
contributor gate gate gadget is one of those tools that help help us along, but 
we're also working on just how can we be more welcoming to new contributors?
How can we pair off people with mentors? And so if you're interested in 
contributing to get, please get in contact with me or, you know, just chime in 
and then get mailing lists saying, Hey, I'm new. I'd like to get started. Oh, 
the one thing to keep in mind is that we don't have a backlog to then say here's 
yeah.
Quick issue outside of these, this replaces. But if you have something where you 
have not only the desire to contribute to get, but you have a specific direction 
you'd like to get to go in or a specific feature you'd like to make better. 
We're definitely welcome to new people and we would love to see your ideas.
Okay. Yeah, 
**Michaela:** [00:51:01] that sounds good. Great. So thank you Derek, for being 
on my show, it was really lovely to talk to you and learn so much about good and 
open source. Thank you so much. 
**Derrick:** [00:51:11] Oh, thank you for having me. It's been great. 
**Michaela:** [00:51:13] Yeah. Bye. Bye. 
**Derrick:** [00:51:15] Bye. 
**Michaela:** [00:51:16] I hope you enjoyed another episode after sup 
engineering unlocked podcast.
Don't forget to subscribe. And I talk to you again two weeks. 
**Derrick:** [00:51:27] Bye. 
**Michaela:** [00:51:30] Hey, if you like this show kind of help me spread the 
word. You can also rate it on iTunes. Thanks so much.


