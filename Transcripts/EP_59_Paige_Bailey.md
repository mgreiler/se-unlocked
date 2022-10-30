
**Dr.McKayla**  (00:03):
Hello and welcome to the Software Engineering Unlocked podcast! I'm your host, 
Dr.McKayla and today I have the pleasure to talk to Paige Bailey about 
improving developer productivity through machine learning, a.k.a. Github’s 
Copilot. But before I start, let me tell you a little bit about my latest 
project: [Awesomecodereviews.com](https://awesomecodereviews.com). 
Yeah, all my work on code reviews has now its 
own dedicated home at [Awesomecodereviews.com](https://awesomecodereviews.com). 
You can find articles about code 
reviews, best practices, code review checklist, news about the latest research 
on code reviews and of course, workshops and courses I offer around this 
topic. So please hop over to awesome code reviews.com and check out my 
latest work. Now back to Paige. Paige is the director of machine learning 
and machine learning operations aka MLOps at GitHub. Before that, she was the 
principal product manager at Microsoft and also worked in DeepMind and
Google. Paige has had over a decade of experience with machine learning and data 
science as a practitioner. Paige also told me about the great opportunity for 
all my listeners today, which is getting into the beta program, which is super 
hard and has a very long waiting list for Code Spaces for data science. So for 
everybody that is listening and would like to get a chance to try out not 
only Code Spaces but also other awesome extensions like GitHub Copilot, you can 
think that today, what do you have to do for this? Well just like and retweet 
today's episode, and for an additional chance to win, you can also leave a 
comment about what kind of data science work you're currently doing or what you 
like to do. So isn't that really cool? But now back to Paige. I'm so so happy 
that she's here with me today. So welcome, Paige. Welcome to the show.

**Paige Bailey**  (01:51):
Excellent. I am very excited to be here and to talk to you about how machine 
learning can be used to improve developer productivity and also the great work 
that we're doing at GitHub to try to make it into a better home for data 
scientists and machine learning engineers.

**Dr. McKayla** (02:07):
Yeah, both topics are super close to my heart. I would really love to learn more 
about that. But I would also like to know a little bit more about what  'Director 
of machine learning or machine learning operations' is. What are your responsibilities? 
What do you do? And how do you get there?

**Paige Bailey**  (02:24):
That's a, you know, that's a great question. And the role is very new at GitHub. 
So it's only been around a couple of months and that means that I kind of have 
the pleasure of being able to help grow it and to define what that role 
actually looks like. But the primary focus is really around this goal of making 
GitHub a better place for machine learning engineers and for data scientists to 
do their work, to collaborate with their teams and then to also deploy and 
maintain models in production. So to that point many, many millions 
of repos today have things like Jupyter Notebooks in them. We haven't done a lot 
of work historically to make Jupyter Notebooks, you know, kind of a first class 
data type on GitHub, but that is changing. And so So as part of this work, I 
get to collaborate with a lot of teams across GitHub, but also across Microsoft, 
so particularly the VS code team, they've been building out wonderful extensions 
and tools and features for their IDE, as well as Azure ML. And so many of the 
many of the features that we're adding to Github’s machine learning products are 
using Azure ML products behind the hood. So you're able to get all of that 
sort of goodness within your application, within kind of the 
projects you're working on, without necessarily having to go through the 
mechanics of setting up all of the infrastructure yourself. But that's 
kind of the idea. So it's, you know, it's like professional machine learning 
cat herder is kind of the idea.

**Dr. McKayla** (04:07):
Yeah, I think this is so so important. And I'm just thinking back when I was 
working at Microsoft, we did a study on code review comments and the value of 
culture, your comments. And we looked at when are, you know, when is it 
easier for people to give good code review comments that are helpful, 
valuable for the code author? And we saw that the way how we present code, 
obviously, right? And if it's now maybe production code, or is it like C# 
code, or is it you know, Yama files or up to notebooks right made a big 
difference if there wasn't a good diffing, if it wasn't nicely presented, it was 
really, really hard for people to give good code review feedback. So yeah, I'm 
super excited that you will work on that and really tackle that problem to make 
it easier for people to review. Also code that I think is quite complicated 
today. I would say it's sometimes more complicated than normal code, if you have 
like a machine learning model somewhere, and you have to understand that, what's 
your take on that?


**Paige Bailey**  (05:08):
Exactly like the process for reviewing Jupyter notebooks on Github.com today is 
quite painful. So to your point, you know, when you view a notebook PR, it's 
still in its raw JSON format, you know, if there are output images, it's really, 
you know, pretty much impossible to kind of see them. That is something that 
we're hoping to change, within this year and in the meantime if 
you're looking at a PR on a notebook, within GitHub, and you hit the period on 
your keyboard, you're immediately launched into GitHub dot Dev, which gives you 
a nicer VS code facing interface to do the review for the notebook, you can see 
it nicely rendered, and you can also leave that you're just mentioning, so 
it's a lot more pleasant. And tear, to your point about data science code being 
trickier than, you know, like normal source to review, I think you're 100% 
correct especially since so often data science code is both describing a 
scenario as well as having a code snippet and some sort of output. And much of 
the time, those outputs are kind of random, right? Like they're not deterministic.
If you're sampling from some sort of distribution, and you sample 10 points,
you're probably not going to get the same 10 points and if you if you sample twice,
so making sure that those considerations are, you know, sort of front of mind as 
we're building out these systems. And also, you know, working closely with data 
scientists, machine learning engineers, code review experts like yourself, to 
make sure that these things are landing in a way, that's delightful. 
And that works for your use cases.

**Dr. McKayla**  (07:09):
Yeah. And so there's the tooling on one hand, but there's also the process on 
the other hand, in my experience, and I think it changed over time, right? As 
data scientists are more and more, I think, more collaborative than like five 
years or 10 years ago, but I still see a lot of lonely ranchers or people you 
know especially at companies that are a little bit smaller, there's only one 
data scientist or one person that really understands this machine 
learning model. And so sometimes it's really hard to get others on board and get 
feedback from them. How do you see that from a process perspective? For code 
reviews? What can we what can we learn there? And how can we shape the processes 
around code reviews so that it fits scientists, researchers also, right, and data 
scientists?


**Paige Bailey** (07:59):
I'm so excited that you mentioned that because there have been so many instances 
where data science work happens just as you described, it's all local 
development, you know, you might have a Linux workstation and a GPU under your 
desk and you're just rapidly iterating in this notebook context. 
You might have intermediate steps where you dump out a CSV. And then 
there's not really this concept of version control. Because if you're 
working in isolation, then it doesn't quite seem like it's worth the time 
to take for version control. Whereas what we're hoping to have happen is if 
folks aren't familiar, Code Spaces is a way to immediately launch a 
a development environment that's attached to a GitHub repo. So you could imagine 
a scenario where you have a project, you're spinning up Compute directly from 
GitHub. So if you see an interesting repo that sawn papers with code, you can 
click a button. And immediately you have Compute attached storage attached, and 
you can play with it with all of the dependencies included. And as you make 
changes, as a data scientist, this is all in your browser. So it feels a lot 
like Google Colab. They folks have familiarity with that, or Databricks 
notebooks. And these changes are automatically version controlled so you don't 
have to worry about it. And when it comes time to perhaps take that notebook or 
machine learning model to production, it's easy to say hey, software
engineering team, all of the artifacts, all of the version history, all of this 
kind of past knowledge. It's just right there, like go take a look at the repo. 
If you have questions, you know, definitely ask me or ping me on live share, but 
it's at least a little bit. It's a little bit easier in the sense that all 
of the work is kind of centralized in a single place. And it's a place where 
data scientists feel comfortable, but also software engineers feel comfortable.

**Dr. McKayla**  (10:11):
Yeah, this sounds so exciting. I think even for normal code reviews, right? If 
we are going not now into this data science, you know, area or field, but for 
normal code reviews, I always say it's so cool if you can have like a PR 
preview, right, where you can click on it and look at it. And obviously
code reviews. It's not testing, but it's always nice. If you can run the 
code, if you can give it a spin, if you can, you know, if you want to try it 
out, you can try it out. And I think for data scientists is even more important, 
right? And you play around with the codes. Super exciting about that. Yeah, 
very, very cool. And what about Copilot, I want to talk a little bit about this, 
because I think a lot of people are extremely excited. And I saw actually a 
tweet from you on on on your Twitter, and it was you use Copilot to explain you 
a little bit what's going on in the code, right? And so, now that we are talking 
about, you know, this kind of code or in general code is difficult to 
understand. But I think, you know, machine learning models, etc, are even harder 
to understand. So how can I? How can you know, Github’s Copilot really help us 
to understand code? Is that really something that's doable? Or was it 
just a toy example where we say, okay, here it works, but in general, it's not 
that helpful?


**Paige Bailey**  (11:29):
It is. I am over the moon excited to have Copilot is kind of a, you 
know, a partner collaborator as I write code. And it's precisely for the 
reasons that you mentioned it, so for folks who perhaps aren't familiar
copilot is an extension for VS code, as well as other other IDs. So if you're 
more of a fan of pi charm, if you're more of a fan of other sorts of 
environments, copilot is also available for you. But it generates source code, 
so as you so for example if you type out a comment explaining, I would like to 
merge these two columns in a panda's data frame. Or I would like to get or I 
would like to normalize, you know, the values in this column, or I would like to 
take this data frame and build a scatterplot, or whatever it happens to be even, 
you know, outside of the realm of data science and machine learning, you just 
describe what you would like to do. And then co-pilot suggests source code that 
accomplishes that task and that was kind of its first iteration. And now we're 
starting to investigate more and more opportunities to apply similar concepts to 
the end to end development lifecycle. So as you were mentioning, the latest, the 
latest feature that was added is the ability to highlight a code snippet. And 
then just say,'hey, co-pilot, please explain this to me, like, what on earth is 
this code doing?' And it works surprisingly well. Just like, you know, when I 
first heard about copilot, I was very skeptical that like, oh, okay, like, all 
right, yeah, so I will describe the thing, and then it will give me a code 
snippet, like, I guarantee you, it probably will not work well enough for me to 
want to use it. And then it's gotten so much better as the months increase. 
So shockingly good that, you know, I am happy to stay at GitHub for as 
long as GitHub will have me just so I know that I constantly have access to 
code. But it's great. And the source code, the source code 
descriptions, you know, it's both the code that you've highlighted, as well as 
any of the functions that perhaps are defined elsewhere. But that are
are highlighted in that code snippets. So if you're calling a 
function that's defined in either a library that you've imported, or a python 
file within your project, it still looks and inspects those locations where the 
function is defined in order to give you better descriptions of what the code is 
actually doing.

**Dr. McKayla** (14:21):
So it goes in both directions. So I either write natural language and it 
magically gives me snippets. And I know that I can, you know, hop through 
different snippets and find the ones that I'm more happy with or that 
I trust more. And then I can do the reverse saying, Well, this is the code that 
I would like to understand and it produces some natural language around that. 

**Paige Bailey**  (14:44):
Yep. 

**Dr. McKayla** (14:45):
Yeah. Another thing that I saw is that it's also helping you write tests, which 
I think are also extremely important, not only for tests but also for 
understanding reasons, right, because if you have tests, it gives you a use case 
for this code. You can, and also I think you can learn a lot from test cases 
there was also a paper by Alberto Celli and others around code reviews. And when 
you start the code reviews, actually from the tests, which are somehow use cases 
of the code right, you could see that code reviewers actually perform a better 
job. And so I wonder if you can also reuse co-pilot a little bit to generate 
test cases around something that you don't understand. And you see input 
outputs. And, you know, it creates a little bit of model for how it's actually 
used.

**Paige Bailey**  (15:29):
Exactly, yeah. And the way that you can do that is just as simple as saying, 
like, you know, perhaps a function is defined somewhere above, like, if you're 
operating in a Python file and a function is defined towards the top, all you 
would have to do is kind of add a comment to the effect of like, test out, you 
know, this function with these values, or even just say "test function name", and 
then hit enter. And then Copilot goes through the work of giving you a testable 
code snippet below. Like I said, it's shockingly straightforward to do these 
things. And I feel like it's honestly made me better at code reviews 
better at collaborating in general, because to get the best recommendations from 
Copilot, you have to be very precise with language, and very specific about the 
task that you're trying to accomplish. So you have to know exactly what you want 
to do. And then and that's the only way that you can get these really nice, very 
accurate code snippets.

**Dr. McKayla**  (16:37):
Yeah, so it's a little bit like test-driven development on one hand, right, 
where you have to understand your requirements quite well. Yes, specify the 
test. And I think here the same, if you have to write down this common 
very precisely in, you know, in a good way, then you have to know your 
requirements. And I think this is so important. And very often a lot of 
developers just jump in and they start massaging and you know, and then you have 
this code, and then you realize, oh, actually, I forgot to think about this 
part, right? So yeah, I can imagine, what about people that are not native 
speakers like myself? Right? So have you probably have tried out with, you know, 
people that are not native English speakers, when you write down? Is it still 
working? Or does it have problems?

**Paige Bailey**  (17:24):
I think, you know, just like every large language model, this is an area of 
active research of, you know, trying to make sure that there are consistent 
performance across every single kind of language. So I've tested code comments, 
and at least a couple of other languages. And I know that colleagues have tested 
with so for example, you know, Mandarin characters or other types of 
language comments, it works. But, you know, being a native English speaker, 
myself, I speak German, but  that's the only other one really fluently. 
The, it's, it's tricky to save for, you know, definitive, like, Yes, this is 
performing better, or, you know, no, it's it's not performing as well as it 
would be with English. This is something that we're investigating.

**Dr. McKayla**  (18:21):
But is it sourcing from you know, because I can imagine, like the 
English body of work that you have for your models in the center is, it's much 
larger the data set is much larger, is it sourcing from a global data set, or 
would it then source from Mandarin, for example?

**Paige Bailey**  (18:39):
Right. So that's a that's a great question. And to your point, the the source 
that it's trained on is really all of the code snippets that we can find on the 
internet, but primarily, GitHub's public source code. So not any private repos, 
just public repos. But the majority of those are implemented in English 
language. And so you know, just like any other machine learning or deep learning 
experiment, you know, you're kind of beholden to the data that you have 
available to train the model. And so we've explored some techniques around 
kind of fine tuning, but mostly fine tuning based on programming language. So 
for example, Copilot performs much better on you know, Python, JavaScript, you 
know, things where there's a lot of code publicly available in terms of computer 
programming languages. And then for things like you know, say Fortran it 
performs a little bit a little bit you know, less accurately 

**Dr. McKayla**  19:44
Than Corinthia?

**Paige Bailey**  18:46
Yeah, but it's it's ah, it's the same for you know, it's the same for spoken 
languages. So so if the majority of the source code is implemented in English 
and the comments are implemented in English, then that's, that's the best 
performance we're going to see and we can fine tune for other languages to 
try to get better performance. But it's always going to be a bit tricky to have 
parity across each kind.

**Dr. McKayla**  (20:10):
Yeah. So I think a lot of people are waiting to get into the attendee preview, 
I'm on the waiting list. But when will it be available for the public? Do you 
have like a date already in mind? Is it like this year or so?

**Paige Bailey**  (20:26):
So I do believe that we're hoping to GA Copilot this year. And though the 
specifics around that are still being discussed, you know, should it be teams? 
Should it be, you know, like, different usage tiers across GitHub? 
Should it be you know, individual access, still very much up for 
debate. But I agree with you like, it is very exciting. And we're hoping to get 
it out to to GA as soon as we can.

**Dr. McKayla**  (20:55):
Yeah, cool. So another topic that I wanted to talk with you about is security 
vulnerabilities, and especially how to find them automatically. Which brings me 
also a little bit to automatic code reviews. And you know, people always say 
it's automated code reviews. And then when I look a little bit closer, I think 
it's steady and dynamic analysis of the code. And then we just have like the 
comments instead of having this output in our, you know, comment 
line or somewhere we have it SPR comments, what's your experience with that are 
there like, Was there really a lot of invention over the last five years, in 
terms of its really automated code reviews. And what I also sometimes wonder is, 
if these PR comments are not too late, I'm more of a fan of a pre commit 
hook, right, where you have your code in your IDE, and this is wrong, right now,
and you can fix it, then pushing it up to GitHub, and then having a PR common,
they are going back to your IDE, changing it. So how do you see this whole process 
with automated code reviews? How does it work? And what are some of the tools 
that you know, that are really helping us here?

**Paige Bailey**  (22:08):
Those are wonderful questions. And I think that you're right that often, the 
automated code reviews are just kind of, you know, checking code for, 
you know, formatting, or those sorts of things, as opposed to actually, you 
know, a little bit more intelligent suggestions about how the code is 
structured, or, you know, like, perhaps this should be extracted into a class 
method or something like that. So I do think we're getting a little bit 
better. And they're, you know, we're just beginning to start applying deep 
learning techniques to things like detecting security vulnerabilities doing code 
review. But this idea, and this concept of sort of having a, an 
automated check to the developer, before the PR even occurs, is my preferred 
route as well. And so I'm not sure if you're familiar with the Python extension 
in VS code, but it currently only working for Python files that we're adding 
Jupiter support to, but it does things like recommend refactorings. So the 
Python extension for VS Code. 

**Dr. McKayla**  (23:26):
Yeah?

**Paige Bailey**  (23:27):
Yeah. And so it's just kind of the, you know, and I don't 
know how well the refactorings are advertised, because I didn't know about them 
up until just recently, when I started to work with the team. But they've 
started like, you'll see these little light bulbs, kind of similar to 
the little light bulbs that exist for Visual Studio. And if you click one of 
these guys, then a gives you suggestions for you know, like renames, and some 
other things. But also one of the one of the examples that I've been most 
excited about are, recommendations for when to extract functions from 
these like big, bulkier, these big, bulkier blocks of code, because it cuz I am 
not sure if you've had similar experience, but the the data science code that I 
normally see or the research code, it's not super modular, often. You know, it's 
like you have data ingestion, and you have like pre processing steps and 
visualization steps in the model piece, and they all might be part of the same 
big, big thing and any sort of nudges to refactor that is great. And the, but I 
do think that there are opportunities to apply, you know, things like natural 
language models to suggest perhaps, better names for functions, right? Like if 
if if copilot is capable of explaining code, then maybe it can also do things 
like say, hey, you know like this function is named in a way that's not 
quite understandable. Like, perhaps you should, you should call it something 
different, or this function doesn't have a comment, you know, 
like, here's an example doc string that you could use to explain this function, 
that sort of thing.

**Dr. McKayla**  (25:19):
I also wonder about consistency, because very often, I think consistency goes 
way beyond any other practice, right? So for example, for naming, having 
consistent names like, let's say, instead of saying, maximum sum, and then 
you say, some min, right, you're switching it, it's somehow confusing. So having 
the consistent naming, for example, or having consistent style within your 
project, and I think this is a really good opportunities for machine learning, 
because you can find the patterns how you know, code is written of the majority 
of time, or if you specify this, this is how it should look like, and then find 
ways where maybe it's not written in, you know, in the same consistent way. And 
style, is that something that you're exploring as well?

**Paige Bailey**  (26:06):
I'm not sure if we're exploring it within Git, GitHub itself, but we might, 
within dev div, like, and I know that in web dev, for example, the intellicode 
team is investigating things like merge conflict resolution, or suggestions for 
merge conflicts. And so I wonder if they might also be investigating some of 
these opportunities to, you know, like, encourage consistency 
in terms of naming, or similar sorts of things. But it's a great idea. 
And I also like, this is also a convenient time for me to say Microsoft is 
hiring. So if anybody if anybody is interested in such things yourself included, 
Microsoft is certainly hiring. And we would love to have a, you know, machine 
learning folks who are concerned about developer productivity and who care about 
these experiences.

**Dr. McKayla**  (27:07):
Yeah, I will. I will link that in the in the show notes so that people don't 
wear the suit, send their CV, or maybe page you or something. So maybe to bring 
something a little bit different into into the mix, because we are coming a 
little bit to the end of the of the show, when I looked at your GitHub profile, 
I found something that's called "Paige Views". Right, like your view on things. And 
and there were two that I wanted to talk with you about. And one was it was 
bring data to opinion fights, right. And I'm just reading what you what you 
wrote there. And it says, like, "folks who are adept at spotting opportunities to 
apply machine learning and automation to existing business processes will 
inherit the earth. That's the one or only way to win by bringing data to opinion 
fights and making every decision data driven", right. And I'm a huge fan of 
decision, data driven decisions. But I'm also always a little bit skeptical. 
When I say we have to balance the qualitative with the quantitative, right? So  
I'm always saying you have to be so cautious with this quantitative 
data, because it tells you a lot of what's going on, but not really why. And so 
it can easily lead to wrong decisions or opinions. And so what's your take on 
that? And how do you balance? Like if we say data driven right, how do we 
balance this really this deep understanding of data with the quantitative, you 
know, way of what, when we have an understanding, we can quantify it?

**Paige Bailey**  (28:45):
Yep. And to your point, all data is biased, right? Because all data is 
collected-all data is collected by humans, and by instrumentation, which, you 
know, has flaws. But the data that we use for machine learning experiments for 
deep learning experiments, and just for analysis, like to understand 
productivity metrics, or telemetry, all of that had kind of a human behind the 
decision of like, Oh yes, we should measure this and not measure this other 
thing. And so to your point, the data that we collect, we need to be very 
cautious about, you know, what we do choose to measure. And then also humble 
enough to recognize that, the data can tell us about users who are 
already using our tools, but it can't tell us anything about people who haven't 
tried them yet. Right? Like the the telemetry that you have for a given product 
for, you know, like button clicks, or like, usages of functions 
are those sorts of things. It can tell you kind of present state activity, but 
it can't tell you like, oh, the reason why people aren't using this function is 
because they don't know about it, or, you know, like discoverability, and the 
documentation is low, or, you know, we don't really have kind of helpful hints 
in the IDE that would nudge them towards these behaviors. So I think the best 
recommendation is always to be curious to constantly ask "why?" and to constantly 
question your data, to make sure that it's the correct thing to be including, as 
part of your analysis, like whether it makes sense to to kind of hang your hat 
on a particular metric, as the thing that you want to increase, as opposed to, 
really just constantly trying to better understand users 
and to recognize that, you know, no matter how much data you have, there is no 
way that any of these quantifiable metrics can can sort of give you a single 
understanding of any user, right? Like, just like a person can't be reduced to 
like an LSAT score, or a GPA or whatever that is. You can't, you can't solely 
rely on metrics to understand folks.

**Dr. McKayla**  (31:10):
Yeah. And I think it's a really good example. And I'm going now completely out 
of our area here, I think, is COVID. Where we have all this data, which is 
presented without any context of how did it was collected? Why was this 
included? Why was it not included? And I'm always like, this whole pandemic, I 
think the thing that stressed me out the most was like people presenting data 
and like just even, you know, already conclusions based on some data where they 
have no idea about how did we even collect it, right? What does this even mean? 
Who was included? Who was excluded? Why did we do it this way? So this is also 
my papers, like, if we think about scientific papers, the results section is 
tiny, right? And there's a large Methodology section where actually we can 
really, or we have to really look deeply to understand if our conclusions or you 
know, the results actually make sense or, you know, make sense for how we 
interpret them. Right? Yeah, exactly. And then maybe the last thing, and 
it's also page view, is give without expecting a return, I really liked that so 
much. It was so resonating with me. And so you said someone very vise once told 
me that throughout the career, you will meet people, and you will help support 
and encourage them, not even thinking about it. But those influences will change 
lives. And if you're lucky, you will find out later. I think this is so 
beautiful. And did that happen to you? Is it happening constantly? How do you 
apply that in your day to day work?

**Paige Bailey**  (32:48):
Yeah, so I have been so fortunate that and it has happened many, many times 
throughout my life. So an example that I was just thinking about this morning 
was when I was when I was an undergrad, I had emailed a professor at MIT just 
kind of, cuz I think everybody has heroes growing up, and I had seen some of his 
research and I was like, you know, hoping to grow up to be like the sky. 
Whenever, you know, whenever I was a geophysics undergrad. And he recommended,  
I interest I mentioned that I was interested in programming that my first computer
was an apple too, I had made text adventure games, I had, you know, gotten into
MATLAB or started getting into MATLAB for some of my coursework. And he recommended 
that I check out Python, because it was becoming increasingly important in kind of
the Space Sciences and the natural sciences, etc. And I was prepping to apply for
planetary science research internships. And so I did, and like, based on his
recommendation, my entire career trajectory changed. That was over a decade ago,
and I'll never forget it. And first computer, I, my family, grew up in a very 
small town, we didn't have much money, and there was no one really around to as a 
computer scientist, but the library was about to throw out an apple two computer 
that had been donated, because nobody could figure out how to get it to work. 
And a family friend who was an electrician, like, I told my mom, like my mom took 
it, took it back home, they got it up and running. And that also, you know, 
ended up being kind of a life changing thing. That was just a 30 minute act of 
kindness. So, yeah, so I think that, you know, that is constantly happening 
through through all of our careers. And, you know, we're all so 
fortunate, like to to, you know, be able to be part of this field and to have, 
you know, kind of the background and the the Uh, teaching and the the 
experiences to work in the tech industry and to help build these systems 
that really power the world and to help empower them to, to, you know, build 
other things or to do their jobs more efficiently. So that's a, you 
know, a if there's anything that I can do to help others that's that's forefront 
of my mind all the time.

**Dr. McKayla**  (35:26):
Yeah, and it's really nice. Okay, Paige, this actually brings us to the end of 
this episode, I want to remind our listener about you know, that they can get a 
technical preview like a better seat for Code Spaces and Copilot for data 
science if you retweet and like the episode or let us know what you're doing 
data science wise right now. And I also will link the Microsoft career thing. So 
if you want to apply, apply and yeah, is there something else that you would 
like my listeners to know or you know, some some thing that you want to give 
them on their way while they are navigating this space?

**Paige Bailey**  (36:07):
Absolutely. Try out GitHub for your machine learning projects. Try out 
[GitHub.dev](https://github.dev/github/dev) 
VS code and its extension ecosystem. And we are always, always open to 
hearing your feedback and to your sort of your ideas for how to make the 
platform better for data science and machine learning work. So that is that is 
my one ask download VS code, download the Python extension and the Jupiter 
extension. Use it for your work and tell us how we can improve.

**Dr. McKayla**  (36:38):
Cool, yeah, and how do we tell it? Do we write you on Twitter? You have open DMS 
or do you write it via email?

**Paige Bailey**  (36:48):
Yep, I'm dynamic web page pretty much everywhere on the internet. So DM’s work 
and then also dynamicwebpage@github.com. 

**Dr. McKayla**  (36:56):
Cool. Yep. Thank you so much Paige, thank you for your time was really a 
pleasure to talk to you and have a good day. This was another episode of the 
Software Engineering Unlocked podcast. If you enjoyed the episode, please help 
me spread the word about the podcast, send episode to a friend via email, 
Twitter, LinkedIn Bell, whatever messaging system you use, or give it a positive 
review on your favorite podcasting platforms such as Spotify or iTunes. This 
would mean really a lot to me. So thank you for listening. Don't forget to 
subscribe and I will talk to you in two weeks. Bye!


