---
episode: "Transcript Episode 22: Jigyasa Grover"
permalink: /machine-learning-engineer-twitter
status: publish
type: transcript
--- 

**Michaela:**[00:00:00] Hello, and welcome to the Software Engineering Unlocked 
podcast. I'm your host, Dr. Michaela. And today I have the pleasure to talk to 
Jigyasa Grover. But before we start, I just want to tell you that I'm taking a 
short summer break after this episode. This means that the next episode will be 
live by the end of August. There are many reasons for this break.
First, I really want to focus on writing the code review book right now. Also, I 
want to reflect on the past episodes of the podcast and maybe spice things up a little bit 
this coming fall. Finally, life is too short to get caught up in a hamster 
wheel, so taking a break and enjoying life is super important. And after that 
I'm back at full energy, bringing more wonderful episodes, 
and also with a bunch of new dates for my code review workshops. But let's get 
started with learning more about Jigyasa Grover, who is a Machine Learning 
engineer at Twitter. She's also involved in many communities that strive to 
close the gender gap and bring more people into open source. In 2017, she won 
the Red Hat Academic Award for her open source contributions. 
So I'm super thrilled to have her on my show. Thank you for being here, Jigyasa.

**Jigyasa:** [00:01:05] Thank you, Michaela. I'm so excited to be 
here with you today. 

**Michaela:**[00:01:10] Yeah, I'm also really excited. So you're my first Machine 
Learning engineer that I have on my show. Normally I talk to software engineers, or 
maybe product managers or CEOs. 
So, can you tell me a little bit? What does a Machine Learning engineer do, and 
how does your day to day work life look like?

**Jigyasa:** [00:01:30] Sure. First of all, I'm honored to be your first ML 
engineer guest on your show. And if I talk about a high 
level explanation of, like, expectations from what an ML engineer does.
So in a corporate setting, the task of an ML engineer would be to bring the 
element of artificial intelligence to business logic. It would be their job to 
build models, either from scratch, or use off the shelf technologies, using 
exciting, like, already existing frameworks with an added layer of their own 
variant and tooling.
They also help sculpt the format of the data that goes into the Machine Learning 
training or prediction services, and not only they build state of the art 
models, but they also help them productionize at scale, which is one of the key 
things they have to do if they work at big companies or startups that cater to 
millions of people at once.
If I talk about how a day in my life looks like, I would like to say from my 
experience so far that each day is very, very different for every Machine 
Learning engineer. Some days it would be like endless exploration of data, 
trying to find patterns and curate some useful features, which I would also term 
as feature engineering.
Some days we would try as a team to build a model from scratch for a specific 
problem or tune our old existing models to, you know, catch up to up-to-date data. 
If they are working on, like, an online mechanism. Some days it would be like 
setting up experiments, trying out different combinations of features using 
different discretizers, performing grid, search and list hyperparameters, 
experimenting with techniques to fasten the training process, 
keeping up with the latest research by, you know, reading research papers, 
analyzing results from experiments, tying them to business prep, product 
metrics, and so on. So basically the tasks are endless, and a day in my life would look 
so much different every day.

**Michaela:**[00:03:28] Yeah, that sounds very exciting. So you are now a Machine 
Learning engineer at Twitter. How long have you been at Twitter? And did you 
start as a Machine Learning engineer? Like did you interview for that position 
or did you somehow grow into that position? 

**Jigyasa:** [00:03:42] No. I specifically interviewed for the Machine Learning 
engineer role at Twitter, and it's been more than a year and a half since I've 
been working at Twitter. I work in the ads prediction team, and I'm fortunate enough 
that I was able to not only interview for the role and I also bagged it. So yeah. 

**Michaela:**[00:04:02] Okay. That sounds really exciting. So, but have you been a 
Machine Learning engineer before you were interviewed for that? Have you worked 
at another company?
And did you do that already before? 

**Jigyasa:** [00:04:13] Yeah, so the thing is, before I came to know about Machine 
Learning, I've done like a lot of software engineering and open source
contributions. I've also worked at, you know, research institutions and for 
a brief period, I also worked at Facebook, which had a very interesting 
intersection of software engineering, data science, and ads business.
It gave me a great insight into how companies leverage data and feed their 
systems, thus making billions of revenue. 

**Michaela:**[00:04:42] Yeah, that sounds really interesting. So when I was working 
at Microsoft, I worked, I had more or less a researcher role at the beginning. 
And so I wasn't a Machine Learning engineer, but we had to do a lot with data.
So we were analyzing data, we were collecting data, different kinds of data, right. So I 
looked mostly at engineering data, right? So internal engineering data, for 
example, commit logs and, you know, communication information and things like 
that. And so one of the things that, I grew somehow into that position, right.
From, from a research background then to software engineering background. And then 
because I had to work with this data, obviously I worked or I learned how to, you 
know, analyze this data. And this was also part of my PhD as well, but. I think 
then, then Machine Learning is another, you know, it's another facet of that 
whole thing. Right? 
So I applied sometimes Machine Learning algorithm, but everything was 
out of the box. I never created my own Machine Learning algorithm or 
something, but I, I worked a little bit with that. So, how did you make this 
transition from, you know, the software engineering to Machine Learning? Did 
you do a course or was it really hands on at the company that you learned at, 
how, how did that transition work?

**Jigyasa:** [00:06:01] Sure. So I kickstarted my journey by contributing to a lot 
of open source projects while doing my Bachelor's degree in Computer Science. So 
why I took bachelor's degree, like, why did I decided to do bachelor's in Computer 
Science was something that my parents asked me, like my dad himself is a 
computer professional and he works for the Government of India as senior 
technical director.
And then he asked me to, you know, pursue something in Computer Science because 
he saw that in a spark in me maybe. And then that's where I started, but I mostly 
was, you know, contributing to a lot of open source projects and, you know, 
working with Pharo, JavaScript, you know, web technologies, Android 
technologies, and so on.
And with that, I also started participating in a summer program, Google Summer of Code, 
which basically takes thousands of students all across the world, and you know, 
makes them contribute to a lot of open source projects. And one summer, that was 
my second time in the summer program, I worked on a project called Suzy, 
which was aiming to build an open source digital voice assistant, just like 
Siri, Cortana, et cetera, but open source. 
So that's where something about, you know, natural language 
processing and Machine Learning sparked an interest in me. So I started taking up some 
ML courses in university and I wanted to do something further, and that's 
when I applied for research internships and, you know, National Research Council 
of Canada, Institute of Research and Development, France, and got sponsorship 
from a prestigious, international organization, which I'm very grateful for.
And that's where my interest in Machine Learning and Data Science 
intensified. I ended up, you know, working with postdocs and professors at these 
research institutions, talked to professors, worked on a lot of research papers, 
and that's when I decided that I should pursue an advanced degree. And 
I graduated from the University of California, San Diego with my master's degree.
You know, with specialization and focus area of Machine Learning and 
Artificial Intelligence. And that's how my journey, you know, basically 
graduated from a normal computer science and a software engineering 
background, with a lot of open source contribution still, ultimately 
being a Machine Learning engineer, and that's when I said I worked at Facebook 
for a brief period, working on intersection of data science and ads business.
And I also gained an interest in ads business and then I eventually moved to Twitter too, 
as a pure Machine Learning engineer, and it's been a wonderful experience so far. And 
I'm obviously so much grateful for all the journey that I've had. 

**Michaela:**[00:08:32] Yeah, it sounds really amazing. I mean, I heard also a lot of 
different countries, a lot of different cities.
Uh, which reminds me of my time when I traveled a lot. But, so you 
were traveling as well. You were traveling a lot. Were you traveling alone or 
did you bring your family or how was that period for you? 

**Jigyasa:** [00:08:51] So during that time, when I was contributing a lot to 
open source projects and these sorts of internships, I was also helping help 
bridge the gender gap.
So I used to work with a lot of, you know, women who code organizations, 
women technicals and so on. And because of all these, I am so honored to 
have been felicitated by Red Hat as a Women in Open Source Academic Award back in 
the year 2017. And that award, you know, the global award and recognition gave me 
actually wings.
And I started getting invitations from so many different conferences and summer 
schools and so on, like all throughout the world. And I would, like, get 
to travel. And during all these times, like even to the date, I've traveled to 
more than 15 countries all alone. And mostly I go for work. And even within the 
United States, I've traveled to like most of the states, I've covered 50% of the 
States of the United States, just for line of work, going to conferences, 
traveling, speaking at them, holding workshops, et cetera. 
And to be honest, traveling has 
opened my eyes in so many other ways, I get to experience different cultures. 
I get to meet people and I also get to see how is the working temperament in 
different countries. And yeah. So, I would say traveling definitely helps 
you, but yeah, these days, the times are such that everything's virtual. 
All of my travels are virtual.

**Michaela:**[00:10:15] Yeah, that's true. 
Yeah, I'm actually really, I'm really happy that I did my last travel in February, 
just before the lock-down, yeah, I came back and I was like, I'm 
really happy I did that! Because now we are all stuck, right? I canceled all my travel 
plans. I should have gone to so many nice countries. Yeah. I'm really missing 
the travel, but I also, so you're, you're traveling and then for your 
internships, you actually stay a longer time in different areas, right? 
So, because internships normally are like three months, or what is the 
time period that you did your internships? 

**Jigyasa:** [00:10:49] Yeah, same. So in Canada I did for three months and same 
goes for France in Paris. 
**Michaela:**[00:10:54] Okay. Okay. And then you also moved, right? So, because I, 
for example, I traveled a lot, but I also moved to different countries.
So I lived, which means, I would say living is more than six months, so that you 
really have to open a bank account, you know, find a proper, a proper place to 
stay, where you cannot live out of the hotel because it gets too expensive. So I 
lived in the UK, in Canada, in the US, in Germany, in Austria, and in the 
Netherlands.

**Jigyasa:** [00:11:21] Oh, wow. 

**Michaela:**[00:11:21] How about you? I heard also that there were like, uh, a 
few countries, right, and cities?

**Jigyasa:** [00:11:28] Yeah so, I mostly grew up in India and I've lived with 
my parents. And then as I said, I moved to San Diego to pursue my master's 
degree, and I've lived there for around, I would say two years. And then. 
Or maybe less like in a year and a half.
Yeah. And then I eventually moved to San Francisco. So, living alone is of 
course a different experience altogether, but I also enjoy the freedom that 
I get and yeah. Embracing different cultures is what I like. 

**Michaela:**[00:11:57] Yeah. Yeah. I can imagine it. I mean, coming from India and 
then being in the United States must be quite eye opening.
I mean, I moved from, I moved the first big move that I made was from 
Austria to London, and then to the Netherlands. But somehow, because it was all 
European countries, I thought, you know, it's all the same, which wasn't true. 
Right? Like, so I got a big shock when I realized that people, you know, it 
seems like we are, we're very similar in culture, right? Western
culture and things like that. But then we are very different. Like the values, 
especially the values were something that were really difficult for me. Like 
when it comes to things like, going to the doctors and what experiences or 
expectations you can have there. Right. Or how they would, you know, what they
would treat as a serious illness and not so serious illness, those things, right. I 
didn't expect that this will make a difference, but it did. But I can imagine 
that coming from India and then going to, you know, the United States, is even a 
bigger, a bigger difference. How was that for you? 

**Jigyasa:** [00:12:56] Trust me, I'm still scared of the United States healthcare 
system that I haven't stepped out of my apartment since four months ago, because I'm 
so scared of getting sick.
So yeah, the cultural side, of course, like really different, but I value both 
of them because you know, one is very close to my heart and the other is very 
close to how I work and all, but I'm trying to, you know, pick the best of both 
worlds, and yeah, as you said, things might look same on, you know, from a bird's 
point of view, but when you go deep inside, but in the case of Indian and
United States, they are completely different and yeah, but the thing is when I go 
back home, I enjoy that because I've always grown up there, so. 

**Michaela:**[00:13:36] Yeah. Yeah. And so, in India, where did 
you grow up? Was that like in a big city or in the countryside?

**Jigyasa:** [00:13:44] So in India, I grew up in a place called Chandigarh, which 
is the capital of the states Punjab and Haryana, like both the states share the 
capital city. And then it's looking through in the foothills of the Himalayas. 
So it's a very pretty town, I would say, it's not super big, but yeah it's growing. 
And then I went to like a proper convent school, like a Christian convent 
school and it was like, so great, like all girls convent school, 
so life was so different. So yeah, so not 
something that I experienced, like the outside world was like completely 
different from what I experienced in that all girls convent school. 

**Michaela:**[00:14:18] Yeah, I can imagine. So, one of the things I want to talk 
with you a little bit about is your experiences at Twitter, but also maybe 
at Facebook for software engineering practices and Machine Learning engineering, 
or I call it now data engineering, right. Or Data scientists. So when I was 
working at Microsoft, maybe I was in a very specific situation, right. So I was 
one of those research has slash software engineers, right? In this large 
software engineering team. 
And so all the data engineering and, you know, the research obligations were on 
my shoulders, but there weren't a lot of others, right. So we were always the 
driving forces, right, for those things. And then we informed like the, the other 
people that were doing the implementations or, you know, like we were, for 
example, making the prototypes and they were doing the real implementation down 
and things like that.
Right. But what I realized that, is comparing with software engineering 
practices, the practices that we had as data engineers, they were less 
sophisticated. There was less rigor, right. There were still a lot of 
questions on how do we test our data efficiently, right? How do we review our 
code or, not only the code because the code is probably not that important, right? 
It's the data, and how do we version our data? And somehow those questions seem 
quite unanswered, a little bit, in this dark data science world versus what 
we have in engineering, software engineering world, right. You know, it's like a 
push of a button and you know, like you have your, your DevOps chains that are 
automatically doing everything for you.
How is that for you? Do you have like this software engineering rigor as well, 
in this data engineering world. And do you feel also, like, I felt sometimes 
like, so lonely ranger more or less, right. Because I was surrounded by a lot of 
software engineers, but then the data science tasks, right, were only on my shoulder, 
maybe there was one or two other people that we occasionally talked about what's 
happening.
But I guess at Twitter, in your team, it seems like you're a bigger team where 
there are a lot of people that you can exchange your ideas and things like that.

**Jigyasa:** [00:16:29] Yeah, Michaela. So in that I would 
totally want to echo, like software engineering practices are more like, 
sort of rigid, like if you know, you follow the agile method or the 
waterfall software development method, you always have like a strict set of rules, 
like after this, you will do testing, and if it doesn't work, you go back to the steps. 
So the rule book is like, one, two, three, and you follow the bullet points, 
like straight up to the fleet (??), but 
in Machine Learning engineering or data engineering, as you said, things are not 
at all rigid because they, they are mostly trying to solve open ended questions.
There's no like strict solution to a question, right. You always have to do a 
lot of, it's more of like, I like to think of it as science, where you know, like a 
chemistry experiment. So you have to do a lot of experiments, until the thing 
works. So that's why you cannot put like a time, you cannot timebox any 
experiment, because you never know the model training would take two extra 
hours than what you thought of.
Or it could take two extra days. And then sometimes after running the entire 
module, you would realize it doesn't work as I expected. So you have to like 
rerun all over again, whereas in software engineering, I think that the idea 
of open-ended-ness or the idea of ambiguity is less as compared to data engineering or 
Machine Learning engineering, hence it's easier to timebox those things.
It can easily be said, oh, after one week from now, I want, you know, this UI to 
be present. So it's much more feasible than what you set expectations or milestones in 
Machine Learning engineering. Hence, even our team at Purdue 
does not follow these strict, because I guess everyone in there is from a Machine 
Learning background.
Like most of the people have PhDs, or masters degree. So the very well known 
would be how experimentation goes. So we are mostly allowed to, you know, free 
form it and deliver as and when we think the model is performing as per our 
expectations. 

**Michaela:**[00:18:23] Yeah, that's really good. I mean, my experience was when 
I started and we had like this team, then we had a very, very great leader, like 
a wonderful manager.
That was also a reason why I actually joined the team at Microsoft. And he 
absolutely understood the exploratory nature of our work, right and the research side 
that we had. And that, you know, as you said, you cannot timebox it, like you 
cannot say, oh, we are going to solve that problem, and in six weeks, we are done, 
right. Because sometimes you don't, you don't even know if you are able to solve 
the problem, you know, in a good way, in a good enough way, like really makes 
sense. Right? Otherwise it wouldn't be research. And then at the very end of my, 
my time at Microsoft, we had like a reorg, and I got a completely different 
manager and he tried to, um, put us into scrum.
You know, time-frames and things like that.

**Jigyasa:** [00:19:16] Yeah. Does not work, yeah.

**Michaela:**[00:19:16] Always had to predict, you know? And, 
he always had, but there must be a positive answer at the end, right, and it 
must work. And then I said, well, if I can only try out what will work in 
the end, right. Then this is not research, right. It's not a bold enough 
question if you know that it will work from, from the get go, right? 
Or if you know how long it will take. Yeah. So there was a big clash 
between different, you know, ways of working. So, yeah. Interesting. So you are 
a group of Machine Learning engineers that really understand that the nature of 
the thing that you're doing, was it the same as at Facebook? Or was that a 
different experience there?

**Jigyasa:** [00:20:00] So at Facebook, as I said, my role was not pure Machine 
Learning. It was like a mix of software engineering, data science and ads 
business logic and so on. So yeah, the working side was completely different. 
There they followed like strict set, oh, by this, this should be done. And, you 
know, doing like a strict bag.
And of course that company is more advanced, like, more mature in terms of 
engineering. So, yeah, things were completely different, but I enjoyed working there. 
I enjoyed like both the sides of the coin, so. 
But it depends on the role, I guess. Yeah. 

**Michaela:**[00:20:31] Yeah. And so how do you review, for example, 
your code, do you review it, or do you work together with other people that are 
looking at what you're producing, or maybe at the data that you're working on, and 
how do you test your systems? Or do you have like a methodology in place there for 
doing that? 

**Jigyasa:** [00:20:50] Yeah, sure. So for testing, of course we have like 
different, you know, services that we use and different expectations that 
we want, the, you know, the product or whatever model that we build to satisfy. 
And as I said, we have a team of like all Machine Learning engineers and people 
who come from like very advanced backgrounds. 
Many of them are very experienced. So they obviously help me as I'm growing in 
my role. So review process, they help. And then for, as I said, for 
expectations, we have them set already, and then we rigorously keep testing the 
model on different sets of data to see how it's performing and is it, you 
know, as per our expectations and so on.

**Michaela:**[00:21:31] And so now you're in San Francisco and while there's COVID
happening right now, the pandemic, do you, do you go to the office or are you 
all working from home now? 

**Jigyasa:** [00:21:42] No, it's been more than four months that I've been working 
at home and Twitter has been completely supportive. They have provided, you know, 
all the budgets for setting up a work from home office, like a home office 
and so on.
And til date  they haven't asked us to come back to the office and I don't think 
that's going to happen anytime soon, but the good part is Jack, our CEO, 
he also announced, like. flexible working style. That is, you're free to be 
remote forever if you want to. So that's something that I'm really excited 
to look into, yeah.

**Michaela:**[00:22:17] Yeah, I can imagine this is opening up a lot of 
opportunities, I think. And so, do you see any drawbacks? Do you experience 
drawbacks working with your colleagues, some collaboration issues that you're 
having because of the remote set up?

**Jigyasa:** [00:22:33] I would like to say so far it's good, but of course I miss, 
you know, a little bit of the personal interactions we used to have, you know, 
it's like going for a coffee break and then you meet someone and then you're just 
chatting in the elevator, you meet someone or in the lunch line or something. 
Of course I miss those little personal interactions, but yeah, work-wise it 
hasn't been like a drastic change because we've been able to collaborate 
successfully virtually so far. 

**Michaela:**[00:23:00] Yeah. So everybody is remote right now or are some people 
back in the office?

**Jigyasa:** [00:23:05] No, everyone's remote. 

**Michaela:**[00:23:07] Yeah, I think that that helps, right? So if a 
few would be onsite and a few would be remote and it's probably harder, but now 
everybody is on the same, on the same, you know, has the same challenges. And so 
everybody has to work towards making it work, right?

**Jigyasa:** [00:23:23] Yeah, the conversations actually happened on the team 
channel now, it's not like, oh, someone, some of them are, you know, talking in 
person and the 
people who are remote, they feel like, oh, fear of missing out. Did I miss on 
some conversations? Like interesting ones. So yeah, everyone and everyone's 
remote. That definitely helps. 

**Michaela:**[00:23:42] So I imagine, I mean, I feel like this, when I'm talking to 
you, you did so many things and it seems like you're super ambitious and 
you were very, very successful with your way.
So can you tell us a little bit about how did you get into open source software 
and you know, how, what would you say, like for somebody at the beginning or, you 
know, that wants to advance their career? What are some really good steps that 
you thought well, these are some of those steps that really brought me forward 
because they are maybe a few steps that looking back, you think, well, this was 
really, like, leveraging or boosting my career.
You already sound like this open source academic award really opened a lot of 
doors. Is there something else like that you said, well, if I would do it 
all over, this is exactly where I would focus my energy. 

**Jigyasa:** [00:24:33] So I would like to share how I actually got started 
open source. It's actually a very interesting story.
So I was pursuing my bachelor's degree, you know, as a normal college
student would do, like back in those days would visit the library just to use 
like, you know, the high speed internet and I was calling on the phone mindlessly 
through all researches (??). So I was doing exactly the same and that's where I 
came across a tech conference that was happening, you know, on social media. And they 
mentioned something about Pharo. And then I heard the word Pharo, like, then I 
heard back in the day, like I only thought about, you know, monarchs of the 
ancient Egypt and I could not relate it to tech. So, you know, that day I just 
went back home and I did a quick Google search and that when I realized like 
Pharo with a P, H, A, R, O. 
It's an actually immersive programming experience and a 
powerful environment focus. Basically it's like an IDE and an OS rolled into one 
based on an object-oriented programming language known as Smalltalk. So I thought, 
hmm, really interesting to have like a very interesting name. And then I  
started reading more about it. 
They had like internet, really a chat, like a chat link to join. I thought, you 
know, why not give it a try? Like. But I joined the chat, but I didn't know what 
to post. I saw lots of developers. Now back in those days, IRC was still really what 
open source developers used to talk to each other. So, you know, gathering all 
my courage.
I talked to a few people in my university who were actually contributing to 
open source and said, 
oh, you know, they said, you can just go and say hi and I read their messages 
and on the blogs. So I gathered all my courage to enter that 
IRC link and just posted "Hey, my name is Jigyasa. I recently came to know about 
the word Pharo and this programming environment.
I would love to know more about it." That's it, like that was my message. And it 
was my luck or something. There was a mentor from China named Martin who was 
online. And then he sent me like a couple of links to the documentations said, 
oh, you should read through these. I was like, okay, yeah, I'll try the examples, 
and the tutorials out, because the tutorial had, you know, links to basically, 
steps to install it, you know, make some very small UI games, tic-tac-toe and all 
that stuff. So I said, okay, sure. Why not? Summer break came. I was like 
enjoying at home. So I thought I'd get started, I opened the link and that days 
Pharo 3.0 was in the works and Pharo 4.0 was getting like, you know, traction. 
And they were like helping in productionizing 
it. So I tried an example basically, I had Pharo 4.0, and then I thought, oh, 
that's not work. And I changed that example, like changed some code and it started 
to work. So I went back to Martin and said, hey, I was trying this example.
And then I see this works in Pharo 3, but not Pharo 4. And for Pharo 
4, I had to do this change to make it working. And he said, oh, good find in 
the documentation. Why don't you go and open a pull request? I was like, what. 
And then he talked to me about, oh, I should open an issue first and then submit 
a pull request. I was like, okay.
And unknowingly the small bug fix, turned out to be my first open source 
contribution. And that's when I got the hang of it. You know, I used to, not 
only trying examples, I ended up making my own games like, you know, Contact 
Manager and so on in Smalltalk. And then I got the opportunity to work on 
Google Summer of Code.
For both times I've worked with the organization known as Fossasia and 
then I said, the second time is when my spark in Machine Learning and all 
interest intensified. So that's how, like I connect my journey from, you 
know, being a normal student at the college, you know, trying to get through all 
the Computer Science classes in the end, turning out to be now interested in 
Machine Learning and Data Sciences. So that's how my interest in open source started and it was, I 
owe it all to my curiosity, I would say. And the fun fact is, Jigyasa in Sanskrit 
actually means curiosity. So, yeah. So I guess I would always want 
to say like, however difficult things missing, but if you try, you know, these 
days you have so many, like just a quick Google search helps, so at least try to, 
you know, make sense of what you see, and yeah.
Curiosity helps. 

**Michaela:**[00:28:54] Yeah. And, and what you were saying is what I hear very often. 
People advise that if you want to get started in open source, the easiest foot 
into the door would be to start with the documentation, right. Make some changes and 
improvements to the documentation because it's, it's a little bit easier, but 
you also get to know the software and to get to know the people, because you 
also said, well, there was this mentor, right?
So you have to get somebody that gives you, lends you a hand, right. On your, on 
your way into, into open source as well. 

**Jigyasa:** [00:29:25] Yeah. So on that note, I would also want to say in my spirit 
to give back to the community, I want to be a mentor now. Like I've mentored 
people in so many global community programs like, Outreachy, Rails Girls Summer of 
Code, Google Coding, Google Summer of Code, and even like
locally in all these communities, because I feel like there were so many mentors 
that helped me during my journey, nd it's my turn to give back. 
And regarding the views getting into open source, so people usually think like, 
coding is the only way to get into open source. Whereas I think that open source 
is a way of factuality, it's a way of collaboration and project ideas 
and thinking. So I also do like different talks and workshops at conferences 
where I talk about different ways to dive into open source, like diving deep 
into open source.
It's not all about coding. So there are so many other ways you can, you know, 
get involved with open source, and the documentation is the one and the foremost. 

**Michaela:**[00:30:22] Yeah. I think that, especially for me, for example, there 
is this probably social aspect that's also holding me back from contributing a 
little bit because, you know, you're, I would get intimidated quite quickly.
Right. And then I feel like you, you need a little bit help to 
understand where you start or you, you know, very quickly people could say, oh, 
this is a dumb question. Or, you should have known, or, you know, be, be maybe a 
little bit rude to you. So I think that knowing how to approach different 
communities and having, you know, a mentor that helps you can be very, 
can be very helpful. Did you make any negative experiences in the open source 
community?

**Jigyasa:** [00:31:05] I would like to say, like so far, my experience has been 
mostly positive. Of course there have been like, like teeny tiny instances where 
I felt, oh, this is not the right way. For example, when I was a student and 
applying for Google Summer of Code.
I would actually receive messages like from people, like received from like a couple 
of them asking me to not apply for a different project since they were also 
interested in applying for the same project and it would create a clash because 
then the mentor would have to choose like, which one of them like he should 
select.
So, but I was very adamant because I was like, I was contributing to this. So maybe the 
mentors should just see like, who contributes the most or maybe who has the 
talent and it should be mostly based on, just because you eliminate competition 
does not mean there won't be any competition, and you'll go further, right. So you 
should have like confidence in yourself.
And I think it comes with, it does not come overnight. I totally agree with the 
social aspect of, you know, being hesitant, I've been in your shoes. Initially when 
I used to contribute, like no one, no one other than maybe my father 
knew that I was contributing because I was so scared to, you know, share with 
people and like, oh, that I'm contributing to open source.
So even my new GitHub handle was my first and like my initials initially, and 
then I changed it after a year because I realized that, the initials won't 
work, my initials, it was just like JG or something, because, and then I didn't even have 
a profile picture because I was very hesitant because I didn't want, you know, 
people, you know, as I said, judging, and I didn't even want people in my new class 
to know that I was doing something like that, but later on it changed. So it 
just took me a couple of months to get used to, and after that it was fine. I 
had my like full name up there, I had my profile picture. But it just took 
me like a couple of months, I would say.

**Michaela:**[00:32:48] Yeah it's probably, how I get into Twitch right now because I 
started streaming and it's also weird, right? Like you're streaming and you get 
to know what you actually have to do, or, you know, if you even like it or not, 
so I'm not announcing it a lot because I don't want, you 
know, a lot of people to actually watch.
So I'm actually happy if there are only a few people on my stream because I want 
to get, you know, used to and grow into that new experience, I think. And I 
think when I, when I'm a little bit more confident, I will probably announce it 
a little bit more. Maybe I'm not even continuing who knows, right? But I think 
maybe I can relate to that for open source as well, right, so you make your tiny 
contributions and they are like a little bit hiding 
behind a pseudonym or you know, just your initials. And then if you're 
feeling confident, you actually can have that much more. So you were 
also talking about the bridging the gender gap. And so I know that you have been 
active in the Women Techmaker community, and also a Women Who Code community. 
How did you get into that? And are you still doing that? And now you told me 
that you're mentoring. Was that the same thing or was where there differing 
activities? 

**Jigyasa:** [00:34:06] So I started off by, volunteering at local Women 
Who Code and Google Women TechMakers communities back home.
And it initially started with, you know, sharing how I did my first open source 
contributions or, you know, helping people set up their GitHub profiles and, you know, 
fork projects and so on. And then later on I started, you know, holding workshops 
that I would talk about, you know, oh, let's build a game in Python, and so on.
So I did that, you know, there, and then virtually, also in programs like, you 
know, Learn IT Girl, or Real School, Summer of Code, or Google Coding, I would just 
be a mentor. You know, if they had any 
questions or just questions and like not even technical, but how to approach 
the, you know, open source contributor or open source developer and so on. And 
I did that back home, and even here in San Francisco, I'm doing it. 
The physical aspect might have 
reduced because I have a full time job now, but I try to keep it virtually. For 
example, I would join, like, a workshop at a conference or just go to like, 
weekly coffee chats they have around here, the city (??) and so on. So that's how 
I've tried to, you know, give back to the community, because I've been helped a 
lot by mentors.
I thought, like I should also help the other way round. 

**Michaela:**[00:35:25] You know, what also would help, I think? If you would be 
open to share your interviewing experience, especially for me Machine Learning. 
How can I imagine that? How did you, you know, you applied for that, how does an 
interview look like for a Machine Learning engineer?
What were your questions and how did you prepare? And yeah. 

**Jigyasa:** [00:35:48] So yeah, for Machine Learning interview, I would say this is 
a little more trickier than a usual software engineering jobs because, you know, 
software engineering job interviewers would mostly focus on data structures and 
algorithms, whereas Machine Learning you are required, especially if you work in a 
big company, as I said, you not only build models on paper, you also have to 
help them productionize at scale.
And for that, it requires engineering skills. So they test you on engineering 
skills. First, they would ask you to now implement data structures, algorithms, 
and all the usual shenanigans. And then later on, they would move on to, 
you know, specific Machine Learning questions. They would ask you what 
different kinds of models are they would give you a use case.
And for that use case, you would have to think from top to bottom, like 
what kind of features, now you have to go creative, what kind of features you 
would want in a model? What kind of model would work the best? Supervised, 
unsupervised, SVM, PC analysis. All those. Feature importance, feature 
correlation, all these, what kind of metrics or 
what kind of loss functions would you base judge your model on? What is the 
objective function you would optimize on? And all of these things, you have to be 
like very thorough with the fundamentals. They will ask you the ins and outs of it. 
That's what my experience has been. I would suggest if you would have like, you 
know, fundamentals of Machine Learning clear, it would be like a very smooth 
interview, but make sure that you also have your engineering skills brushed up, 
like you would 
have know your data structures and algorithms as well. 

**Michaela:**[00:37:25] And so did you have, like, did you have to code, did you 
whiteboard or how, how was that at Twitter? How long was the process also, like at
Microsoft I think it was a whole day, probably eight to nine hours of interviewing.

**Jigyasa:** [00:37:38] Oh, that's long.
That's long. Yeah. 

**Michaela:**[00:37:39] Yeah. And it was really long. Yeah. 

**Jigyasa:** [00:37:41] Yeah. I remember having three interviews of one hour each. 
And with like 20 minutes break between each or something. So it was around four to 
five hours, not longer than that. Yeah. And between that, they also had a round with 
my to be manager or to be tech lead where they would just ask like, you know, usual life 
questions or behavior questions, they would ask me like, you know what I expect 
from the job, just to know, like, if I'm the correct fit or not.

**Michaela:**[00:38:14] Okay. And so was it all on one day or did you have like a 
screening interview first and then you had this onsite interview? 

**Jigyasa:** [00:38:22] Oh, for me, it was all in one day, I was actually approached 
by the manager of my current team via an email asking me to interview. So. 

**Michaela:**[00:38:32] Okay. So you went straight to the onsite interview? 

**Jigyasa:** [00:38:36] Yes.
Yeah, fortunately. Yeah. 

**Michaela:**[00:38:39] Okay. Yeah, that's really good. And so now that you're a 
Machine Learning engineer, what does the, is there some career path for 
Machine Learning engineers? Would you become a Machine Learning engineering 
manager, for example? Is that something that exists at Twitter or?

**Jigyasa:** [00:38:55] Yeah, definitely.

**Michaela:**[00:38:57] How does that work? 

**Jigyasa:** [00:39:09] So we have like, as a Machine Learning engineer, of course we 
can grow on to be like a staff Machine Learning engineer, Principal Machine 
learning engineer and so on. But if you also want to get a little more inclined 
towards other managerial positions, you can, after you reach a certain level, 
you can also be like a Machine Learning engineer manager and Machine Learning, 
and so on.
So what a Machine Learning engineer manager, like  Machine Learning engineering
manager would do, would be to manage a team of Machine Learning engineers. So 
that is something like, if that's the part you're looking for, like managing the 
team, you could do that. Or if you want to be like pure engineer, you can also 
pursue that path. 

**Michaela:**[00:39:40] Okay.
So what, what, what do you think that you will do? Do you know already ?

**Jigyasa:** [00:39:44] So far I'm, I don't plan like my life, like 10 years in 
advance or something like that. I try to take it, you know, step a day, but for 
now, if I see myself, I would, you know, continue the tech part as long as I can. 

**Michaela:**[00:40:01] Yeah. That's, that's also what I really liked at 
Microsoft that you didn't have, you have to choose, like there was not like 
you're an engineer and then you're a manager as the next, you know, as a next 
step.
But you had like this parallel, really technical track, and it wasn't called 
staff engineers, but it's like Principal. And then you would be like one of 
those technical leaders, right. So you could even become like, if you, if you're 
very ambitious, right, you would be this distinguished engineer, for example. 

**Jigyasa:** [00:40:25] Yeah, same, yeah like a, yes.

**Michaela:**[00:40:27] you don't have to take over the management part, which I liked, right. 
Because very often in smaller companies, especially, there is like, if you want to 
advance your career, you have to switch from the technical side to the managing 
side, right? 

**Jigyasa:** [00:40:40] Yeah. This is something that I like too, yes. 

**Michaela:**[00:40:43] Yeah, that's really good to know. 
Okay, so, very cool. Thank you so much for being on my show 
today, for sharing everything that you learned on your way with us.
I think it was very, very insightful for me and I hope also for my listeners. Is 
there something else that you would like to share with us and that we haven't 
talked about? 

**Jigyasa:** [00:41:01] No, I guess I've touched most of the aspects. Thank you so 
much Michaela, it was like wonderful talking to you today. 

**Michaela:**[00:41:07] Wonderful.
Yeah. So I will link to your profile, to your GitHub profile, to your Twitter in 
the show notes. If you want to see for yourself, what Jigyasa is all about, 
just look at my show notes. And so, just have to say thank you, so much.

**Jigyasa:** [00:41:21] Thank you so much. 

**Michaela:**[00:41:22] And have a good day. Okay. Bye bye. 

**Jigyasa:** [00:41:25] You too, you too. Bye bye. 

**Michaela:**[00:41:27] I hope you enjoyed another episode of the Software Engineering Unlocked 
podcast. Don't forget to subscribe, and I will talk to you after the summer break in a few 
weeks. Bye.



