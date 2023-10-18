---
episode: "Transcript Episode 73 Alexander-Serebrenik"
permalink: /emotions-software-engineering
status: publish
type: transcript
---

[00:00:00] **Michaela:** Hello, and welcome to the Software Engineering Unlocked 
Podcast. I'm your host, Dr. Mikayla, and today I have the pleasure to talk to 
Alexander Serebrenik about social aspects of software engineering. 

But before I start, let me tell you about an amazing opportunity that allows you, yes, you, 
to earn additional income! 

Do I have your attention? Yes? Great. So, User Interviews is a company that connects researchers 
with study participants. And, they especially are looking for developers that share 
their feedback on products. 

Share your opinion with top brands such as Spotify, Adobe, Amazon and many more, and get paid. 
Most studies take less than one hour to participate and pay over $60. 

So, sign-up today - It’s free - apply to give feedback for products that interest you, 
and make a nice side income. Additionally, you help to shape the future of the tools we also use. 
What’s not to like, right? So, hop over to [userinterviews.com](https://www.userinterviews.com/hello)

And now back to Alexander. Alexander is a full professor of software, social software 
engineering, and I University in the Netherlands. Alexander's research goal is 
to.

Facilitate evolution of software by taking into account social aspects of 
software development. So I'm super thrilled to have him on my podcast
today. Uh, So welcome Alexander. Welcome to the show. 

[00:00:57] **Alexander:** Good morning, Mihaela. Thank you very much for 
inviting me. It's a great pleasure for me to talk to you about.

Well, my favorite subject, . 

[00:01:04] **Michaela:** Yeah. That, that's so cool. So you sent me a couple of papers. You have plenty of papers, so people should really check them out. But 
one really stroke my attention, right? It was called Emotions and Perceived 
Productivity of Software Developers at Workplace.

And maybe I'm very inclined to talk about this paper because I was working on 
productivity, perceived productivity and well developer experience. How do 
developer experience their work environment and how does this influence their 
productivity for the last couple of years? So I'm super interested to what this paper is about and what you found out. So can you maybe give us a 
little summary of the paper and also how and why do you look at perceived 
productivity of software developers? Why is that interesting? 

[00:01:50] **Alexander:** Well, let's start looking at the entire story of 
emotions, right? So of course we know that people experience emotions and we also know that emotions influence cognitive processes such as problem solving, and also influences how people collaborate with each other.

And this is exactly what software engineering is about. It is a collaborative 
problem solving. So if you want to think about increasing productivity, if you 
want to think about improving collaboration, we need to understand what emotions 
people feel when they are working together or when they are performing 
programming tasks

So for several years and I sometimes independently and sometimes together have been trying to understand emotion as expressed. For instance, code review 
comments or in second flow question. But of course, emotion is expressed. It's 
not necessarily emotion is experienced. Mm-hmm. . So to get further insights and 
emotions as experienced, we wanted to go for more direct measurement for 
biometrics.

[00:02:54] **Michaela:** Can you, can you outline a little bit more what's the 
difference between expressed emotions and experienced emotions? How do you draw 
the line here? How can we understand it as we are not that 
familiar with emotions and the research behind emotions? 

[00:03:09] **Alexander:** Well, there are all kinds of series that explain how 
emotions exactly are being expressed.

But roughly speaking we need to understand that not everything we feel we 
express. in general and in particular in the professional setting, norms of 
professional behavior restrict the way emotion is expressed or sometimes force it to amplify. Mm-hmm. you are thinking about things like cause of conduct.

Cause of conduct will typically say don't be a jerk and welcome newcomers, and 
so on and so on. If I'm an experienced software developer and I don't 
care about those newcomers, I'm not going to be as excited, as welcoming as 
maybe this kind of norms of behavior expect me to be. So I will be amplifying 
something, which I do not necessarily feel as strongly as expected.

And on the other hand, of course, I might feel frustrated, but I might be 
required to tune down those emotions such as that I do not offend my colleagues. 
Mm-hmm. . Okay. So this is an intuitive difference between what you feel and how 
do you express it. . So of course we can ask people how do you feel?

And we hope that during the experiment people will be more open about what they 
feel as opposed to the real workplace environment. But of course going even 
deeper to the hardware level would be even cooler. So this, this work actually 
has started with the work of Nicole Naviele and her team Philip Daniela Gerardi.

So they have conducted a controlled experiment with several students. So the 
students have been asked to perform a certain programming tasks and they've been 
interrupted on a regular occasions to measure their biometrics. Biometrics. 
Think about heartbeat. Think about Skin response. So if you are stressed, then you are 
starting to sweat a little bit.

It doesn't mean that you know the entire environment is suffering because of it, 
but electrical conductivity of your skin changes and sensors can actually 
measure it and see it as a reflection of stress. And then of course, you can 
compare it to emotion as reported by the students. So this was an interesting work.

They have successfully built a machine learning classifiers. It succeeded to classify emotion according to those biomed signals. But of course, those were 
students. And it was only one hour. Mm-hmm. . So it was a controlled experiment. 
And as any controlled experiment it is not necessarily representative for the real world.

And so in the paper you have mentioned we have actually went to this real world 
and tried to see how this kind of uh, questions can be answered on the 
workplace. So we have contacted uh, five dash companies, small companies, large 
companies and we've been extremely lucky. For them to agree to participate, 
agreeing to participate meant that several of their employees had to wear the 
wristband.

For two or three weeks. So all those companies have been using some kind of 
agile methodology, and this was the sprint. So as you can imagine wearing this 
wristband for two or three weeks required quite a significant commitment. I 
mean, it was not harmful in a sense of just a wristband. It's. It makes you, you 
know, it hurts you in some way but of course you need to remember to turn it on, 
to turn it off, to download the biometric signals on certain moments and so on 
and so on.

So we have been very, very lucky to get those uh, this information. And in 
addition to this biometrics, we have been also asking people to report how they feel 
and what makes them feel in terms of what triggers their positive or negative 
emotion therapy. Mm-hmm. . And of course you also ask about perceived 
productivity.

Again, we are stressing the word perceived because productivity as as a 
productivity expert definitely knows, can be operationalized in many different 
ways, and perception is only one of. So ultimately, what have we figured out? 

When it comes to what makes people happy or unhappy. So we have seen things 
which are related to the individuals themselves. For instance, feeling in the 
flow makes, trigger positive emotions as opposed to being stuck, which triggers 
negative emotions. But you have also seen that uh, positive emotions are 
typically associated with collaboration.

At least then collaboration goes well. And also breaks just taking regular 
breaks and understanding, you know, this is a work time and this is a not work 
time health developers when it comes to negative emotions, we have seen that 
typical challenges are related to problems of mapping behavior to cause, right.

Frustrating situations when you see that the system does not work and you have 
no idea why. So essentially figuring out the root cause of the problem is one of 
the most frustrating experiences and developers report negative emotions 
associated with it. And of course we have things we probably expect, like time 
pressure like unconstructive meetings and so on.

And so. By the way, constructive meetings actually trigger positive emotions. So 
it's not true that all the meetings are horrible and that software developers 
just hate them because they're meetings. Meetings can be constructive and then 
trigger positive emotions. Meetings can be not constructive, not productive, 
and then they can trigger negative.

[00:08:59] **Michaela:** Can I ask you about the positive emotions? Yeah. So I 
understand that, for example, negative emotions we would detect with this 
sensors by sweating, for example, right? Or the heart rate goes up. But how do 
you detect positive emotions? Is it just not negative emotions or is it really, 
is there neutral and is there a positive reaction of your body?

How would you, how would you measure that? In, you know, my biometric. 

[00:09:24] **Alexander:** Well it's not that we measure, we directly link stress 
to positive to negative emotion or , it's essentially you're measuring the same 
things, right? You're measuring certain biometric signals and then you are 
mapping them to balance arousal and so on and so on.

Mm-hmm. . So it's, it's pretty much the same. Whatever you are measuring, you're 
measuring indeed different you are, you are indeed predicting different 
categories. You're predicting high balance, low balance, and so on. , and that's 
how, that's how it works, right? Mm-hmm. When you are trying to connect it to 
productivity then it seems that indeed balance, so positive versus negative is 
the most important predictor, which explains up to 12%, which is kind of a lot.

Mm-hmm. . And what's also interesting is that there is an interaction of balance and time.
and. . Uh, Essentially it means that at the end of the day, in the second half 
of the day your emotion is more likely to affect your productivity. Okay. And 
this is essentially related to fatigue. Mm-hmm. , right? So, fatigue reduces 
control, and this is, this means that your emotion is more directly connected to 
product.

[00:10:36] **Michaela:** Mm-hmm. . Can I ask a little bit more about this link 
and how you looked at it between productivity and demotion? So it's perceived 
productivity. So how productive do I feel, right? It's not really how yes. 
Actual productive I am or it's not How many tasks, you know, it's really how, 
how productive do I feel?

Do I feel like I get a lot done, or do I feel like, oh, I'm a little bit stuck? 
So, Probably you know, tell you that on some likelihood scale, right, some 
I feel very productive or very unproductive. And then you are also asking me 
about my emotions. So I would say, oh, I'm very stressed. And then you look at 
the link whether or not, probably negative.

So the hypothesis will probably be that um, negative emotions reduce your 
perceived productivity. So if I'm, if I have anxiety or if I'm stressed, I feel 
less productive. And if. Let's say relaxed or happy, I feel more productive. Is 
that, is that how, how uh, 

[00:11:33] **Alexander:** roughly? Yes. Right. So, so productivity is indeed on 
a liker scale from very low to very high.

And we operationalize emotions through the so-called uh, VAD model, which is
essentially a valence, arousal and dominance. And balance is indeed this 
positive negative from annoyed to pleased. Arousal is from calm to um, excited And dominance 
from control to controlling. Mm-hmm. . Those are the three dimensions of 
emotions.

There are different ionizations of emotions. This is the one we use here. And 
when I said that balance is the most important predictor, essentially it says 
that when people are more positive than they are feeling more productive. 
Mm-hmm. Of course, you know, it's a simplified thing because there is more to it 
than only balance, but it still explains 12% of your variance.k

So it's quite important as opposed to it. For instance, arousal will explain 
only roughly 3% of your variants, right? So arousal ranging from calm to 
excited, more excited you are. You might be inclined to think that you are more 
productive, but. Essentially it explains only a small part of this productivity.

[00:12:40] **Michaela:** Okay. And so you were talking about that we are 
fatigued. And then you also mentioned a little bit earlier that breaks, you 
could see that taking breaks actually increases your perceived productivity, 
which I think is similar. Right? So being fatigued and then what can you do for, 
you know, reversing that you're going on a break.

So how, how? , how did you measure that? Or what were some instances that you 
saw? Did people go for a lunch break or did they go for stretching? You know do 
you have some insights into that? What kind of breaks do we have to take to to 
increase our productivity, our, our wellbeing? 

[00:13:16] **Alexander:** Probably. . Yeah. So essentially we did not connect 
breaks.

So directly to productivity, we connected breaks to emotions, to what, to 
triggers of emotions. And then they are indirectly, of course, related to 
productivity, as you just discussed. Mm-hmm. So. When it comes to breaks we 
talked about individual breaks and we talked about social breaks. For instance 
lunch or taking a rest.

So we have also separated our day into morning and afternoon. So when we are 
talking about this fatigue, right? Uh, Based on the lunch break. So essentially 
before the lunch break, after the lunch in one of the companies which we have 
observed they have this tradition of going for a walk uh, during the lunch 
break.

So they seem to be very excited about their lunch breaks. 

[00:14:04] **Michaela:** Okay. Yeah, I mean, I think that a lunch break is an 
interesting pro, probably, and here we are probably going a little bit into 
speculation, , but I can imagine that if you have a lunch break that's very 
heavy, that you're actually more fatigued afterwards because of, you know, your 
digestive system and so on, like, I definitely recall some of my lunch breaks, 
and then I changed them when I felt like, oh my God, I'm really, I can't work 
now.

Right. So I don't feel very productive, even though I have been on a break right 
now. And then, as you said, as I changed a little bit, the lunches that I took, 
like smaller meals or. Adding some, some exercises. So when I was working in 
the, the Netherlands in the university, we walked up to the eighth floor right 
after lunch, it helped a little bit, right?

Getting your, your system back on track and so on. So have, have you seen that 
maybe directly in the study or did you get some, some insights into that? 

[00:14:59] **Alexander:** Not directly into the study but there is of course , 
separate line of research by Thomas Fritz , mm-hmm. , and back then Manuel 
Siegler on interruptions, right?

Mm-hmm. . So what kinda interruptions? When can you interrupt people? When you 
cannot interrupt people? Most of the time interruptions are being seen as 
something negative, right? You are working, you don't want to be interrupted. 
But Discussion makes me think that maybe we need to be more careful in this 
discussion of interruptions and see them as something which can be positive as 
well.

Going for coffee can help you not only to catch up on the local rumors, but 
maybe also to switch off your brain from solving a very technical problem. Or 
maybe you can actually talk about the problem. to some other colleagues who are 
also waiting for the coffee and find a solution together.

Yeah, I 

[00:15:52] **Michaela:** think anecdotally, right, anecdotally there were many 
stories that I hear where people say, oh, I was stuck and I couldn't figure out, 
and I was there doing it, I don't know, debugging for two hours and then I took 
a small break, came back and you know, right there in front of me, lost a 
problem.

Crisply clear. I think I've heard at least stories like that. Quite, quite frequently. 

[00:16:13] **Alexander:** Absolutely. Absolutely. And I also think now about the 
work of Pedro de Guerro, I dunno whether she has already been on your podcast. 
If not, please consider inviting. Mm-hmm Her, she's doing very cool things. . So 
one of the things she was doing, she was looking for how people ask for help.

Mm-hmm. And essentially asking for help is a major challenge for software 
developers. She was observing mostly because people feel uncomfortable 
interrupting more senior colleagues with their, you know, questions that they 
themselves might find not meriting interruption. . Uh, So from this perspective, 
I do wonder whether this kind of coffee breaks can help to reduce the social 
anxiety, which is involved in asking for help.

Mm-hmm. Because you know, right. So maybe you can, it's kind of easier to talk 
to people. And also reminds me, of course, the scientific conferences, which you 
are of course familiar with, right? When you have more junior people who do not 
really dare to talk to more senior people, unless there is someone who would be 
ready to introduce them.

So there is a. Discomfort here, which might also play a role even in software 
companies. Yeah. When people are supposed to know each other. Yeah. 

[00:17:28] **Michaela:** So Alexander, you were studying emotions not only in 
that paper or in this study, but in many, many different studies. And you 
already talked a little bit about it.

Also emotions and uh, Code reviews, for example, right there. We can look at the 
cultural comments and we can, you know, try to figure out whether or not it's a 
positive comment or a negative comment, you know, if it's, if you are a little 
bit angry, frustrated, or happy and so on. So what's your experience with 
emotions?

in code reviews, do we see? Can we detect them? Do we see them? Do people try 
not to share them

[00:18:06] **Alexander:** them? We do see them. They are different in a sense 
that more of course the laws of professional behavior prevent people from 
expressing some emotions, but not always. . One of the more commonly seen thing 
phenomena we have observed is a phenomenon of confusion.

We can wonder whether confusion is strictly speaking in emotion or not, because 
it's more cognitive states and effective state. But we do see people getting 
frustrated because they're confused. Mm-hmm. And confusion is of cause a painful 
issue because if I. As a reviewer, I'm confused what the source code is doing.

I might be tempted to approve it. Essentially relying on the developer having 
done their job, and obviously in a sematic way. If I'm a developer and if I'm 
confused about something that some other code is doing, I will just assume that 
it's doing something reasonable and hopes that the reviewer will catch my mistake.

So this confusion is essentially related to mistakes passing through this kind 
of quality gains. Mm-hmm. . So we've been looking at confusion quite 
extensively. Uh, We have been serving people, we have been mining data from 
repositories on GitHub. And indeed you see a whole bunch of issues and the most 
common problem, which is triggering confusion

in relation to artifacts is essentially missing rationale. People are not, 
developers are not understanding why certain things are being done. Mm-hmm. And 
this brings a cause opens an entire direction of can we find some kind of 
knowledge in previous discussions. or in some other kind of documents or some 
other kind of artifacts which might be present.

Uh, Because if we cannot rely upon developers to actually comment to, to 
explicitly status rationale, then we need to find a way to mine it in Salway. 
Mm-hmm. . 

[00:20:12] **Michaela:** And so how did. What, what are some of the patterns 
that you detect to detect confusion? Is it that they're asking a lot of 
questions or is it that there's a long discussion going on?

Or what are, you know, how do you detect confusion in, in co code 

[00:20:28] **Alexander:** reviews? So we have been lucky in a sense that we have 
reused theoretical model of confusion, which has not been designed for software 
engineering, but has been designed for human communication in general. And it 
has several textual cues which can be used to identify confusion.

Indeed some of them are related to asking questions. So in any case, , there is 
a theoretical model of Michelle Jordan, which defines it as situations when 
individuals have a sense of wandering doubt or unease. Mm-hmm. about how will 
unfold, what the present means, or how to interpret the past. So this was 
essentially the theoretical model we have used and.

based on this model, we have mixed automatic detection of certain keywords with 
manual labeling of the confusion of the confusing or non-con confusing card 
review comments. Mm-hmm. . And on top of it, you have also conducted a survey 
asking people how, when does they feel confused?

What usually makes them confused? Can this, can they describe a change for code 
changes, for instance, has confused them and so on. And so based on this kind of 
questions, we have obtained more examples of confusing situations than whatever 
we would've been able to detect directly by observing.

Culture view comments. 

[00:21:48] **Michaela:** Yeah. So what I was wondering as well is culture view 
comments. Especially the ones that we are talking about, they are written, 
right? It's in a written format. It's also what you are analyzing, right? We. 
Right. It's hard to analyze if we are doing a, a synchronous code review and we 
are just speaking, right?

So what you probably focus on, and I think what the majority of people are doing 
when they're doing code reviews is they're writing each other comments and it's 
text-based. And in my experience, and also research shows that written 
communication is quite different from, you know, verbal communication.

A lot of things are missing. Like social clues are missing, facial expressions 
are missing body language, right? So, Code reviews tend to, or code review 
comments tend to create more misunderstandings, I think, than if we are talking 
to each other face to face. I, I expect, or I, I think that it has also to do 
that we are confronted with this.

Computer right. With, with this interface we are actually working with the 
program and not really talking to a person. Right. So it's hard to, there's 
another level of, oh, actually I'm talking to another person with this. Right. 
By writing down my comments. Have you looked at that as well? And do you see 
that, you know, comments maybe they.

They seem to be offensive, but they are not meant in an offensive way or that 
they seem, you know, that there is mis miscommunication or misinterpretation 
happening. Have you studied that a little bit or have you had that, has that 
impacted your work in some way? 

[00:23:19] **Alexander:** Well, thank you very much for this question.

So of course computer mediated communication is different from direct 
communication, even if you are talking about talking face to face, right? So 
this conversation we are having now Uh, might have looked differently if it 
would have been in the same physical space. Mm-hmm. On top of this, as you are 
correctly pointing out we have this relatively poor communication channel, 
right?

So the just text in the most fancy way, it can include a emojis, but this is 
more or less it, right? I would not dare to say that it causes more confusion. , 
it's tricky. Usually when we are in the same space, we are also in the same time 
in a sense that, you know, you need to uh, decide now whether this is good or 
bad.

Well, of course, if you are separate, then you can take your time ideally and 
try to figure out whether this change is actually okay or not. So I would not 
necessarily be advocating for joint code review, essentially behi sitting 
together because then it's kind of becomes a pair programming, right?

It becomes a different kind of working. It's not that it's better or worse, it's 
just a different kind of working. So when it comes specifically to 
misunderstanding and to intention. Yes, this is of course a very important 
thing. Part of the confusion is understanding of the communication intention.

Uh, This is not always easy. And part, and we have actually seen on several 
occasions that communication intention was the reason for confusion in our 
study. Mm-hmm. Just to give you an example Different communication intention as 
opposed to the face value of it. Let's forget for a second about our software 
developers, but when the police officer tells you, can I see your id, please?

It's not the question that you can answer with the answer yes or no. , right? I 
mean, it's Victoria, so grammatically right? It is, it's a re it's a request for 
action. Mm-hmm. , it's not an information. It's not a confirmation request, 
right? It's a request for action, which is being expressed as a question as for 
the sake of politeness.

And this is also what we see in communication between developers. Questions are 
often used to. soften the uh, negative message or to request an action, could 
you please do something, something? Most of the time it actually means you 
should do something, something rather than asking for an opinion whether you 
actually could do it.

Yeah. So this is a matter of communication intention. Another topic you are 
touching upon is Hurting someone's feelings, right? This is related to the 
matter of toxicity, which is an important topic both societally and in software 
engineering research. You might know that Bot Vaco has published on this topic 
recently.

You might know some work of Bra Adams in this space. So there are quite some 
people who are working on toxicity. and indeed toxicity is a problematic ma 
matter partially because of its intersection with cultural expectations. Lion of 
Starz, very well known example has argued very often that he use of expletives 
is essentially a Finn management.

at least part of the finished management culture. So this is tricky because to, 
to some extent the rock cultural differences, which might explain interpretation 
of a certain text or isation of a certain uh, behavior as toxic or not toxic, 
but at the same time you cannot. Claims that everything can be attributed to 
cultural differences because this would kind of means that everything goes, 
which clearly is not a thing.

So this is, this is a difficult matter, right? Why, where do you draw the line? 
And it is difficult for human beings and it's a cause even more difficult. for 
any kind of automated tools which might be used to detect negative uh, uh, 
behavior, such toxic behavior. There are several bots if you are looking around, 
and we hope you'll find several toxicity detectors.

The problem is that many of them are based on dictionaries and the moment. 
people figure out that those tools are based on dictionaries. It'll start 
replacing characters and playing all kinds of tricks just to pacify as a tool. 
Yeah. Which is essentially not really solving the problem.

Another issue is that of cause toxicity and emotion are related, but not the 
same. You can have a very negative and very toxic comments, and we have seen. 
However you can have a much more subtle behavior, which would be still toxic, 
but would not necessarily express negative emotion. So those things are related, 
but they're not the same.

Yeah. 

[00:28:32] **Michaela:** Yeah. So I wonder also about the thing that you said at 
the beginning, right? Intention, because this is something that comes up in my 
workshop quite a bit, right? When I'm working with, on people on how to give 
feedback, how to, you know, how to respond to feedback. And you said, well, a 
lot of people ask questions even though it's not a question, right?

So could you maybe change that? Right? So we really make it very subtle with the 
could and then maybe, maybe. But in, in reality, it's a, I want you to change 
that. Right. I want you to make, actually take an action as you said. Right. 
What do you think, how, how should people work with that? What, what's your 
opinion on it?

Should they just say, or please go ahead and change that? Or are questions 
actually valid way to express that because it's more polite? What's your 
perspective on that? 

[00:29:22] **Alexander:** here. I'm mostly looking at all the way I tend to 
communicate with my coauthors when I'm reviewing papers, typically written by 
students uh, or rather than actually, you know, with my scientific perspective 
on how software developers are doing it.

Mm-hmm. , it really, really depends on whom you are talking to. In some cases 
asking questions is a perfectly valid strategy. , in some cases you should be 
more direct. It really depends on your relation with the person to whom you are 
giving this feedback. It's hard to say like it also depends on the situation, 
right?

Of course when you are asking a question, you are kind of living space for the 
other party to say no.

If this talk, if this feedback is so important for you, then you might consider 
reiterating this point in a no explicit way. Yeah. Even after the person has 
said no. Yeah, but I still think that you should, if this is something you kind 
of suggest but don't necessarily want to fight for, then you'll. , leave it 

[00:30:36] **Michaela:** first.

Yeah. Yeah. Pick your pedals. 

So when you did all this work on emotions also how people interact, the social 
aspects of software engineers, what's your advice for my listeners? Were. You 
know, a large portion of it are software engineers. What's your advice for them 
to, you know, make collaboration better, improve their productivity, improve 
their emotions, make their work life better?

What are some of the key aspects that they should, you know consider or keep in 
mind? 

[00:31:06] **Alexander:** Well, I think that I will stick to um, a quite generic 
statement. Keep in mind that you are a human being. This means that keep in mind 
that you have emotions and keep in mind that other people have emotions, and 
that when you are raising things in particular in such a poor channel as code 
review, text comments.

Be aware that your comments should or might be misinterpreted. So try not to 
hurt feelings. Try to be explicit about what you want, but try not to be a hard. 
And beyond that, take break. 

[00:31:48] **Michaela:** I like to take the breaks thing. , I think they're so 
important. Breaks are really important. I think it's so important to have, you 
know, this flow state.

Which means really less interruptions. You know, turn off your notifications for 
your emails. Just, you know, look at your emails every two hours or maybe just 
at lunch and, you know, before you go home, something like this. But then on the 
other hand, take breaks. I think this is such an important.

Message. And I really like that research is also, you know, pointing into that 
direction saying We should really take our breaks. Yeah. 

[00:32:20] **Alexander:** If we need to be very careful, there's not to create a 
rat. Uh, Unfortunately we know we are getting more and more studies which um, 
reveal highly problematic behavior.

You might have known there is a recent paper about uh, drug use of software 
develop. We know from our own studies that older software developers being 
pushed out of the field and as a way to con to contract it. Some of them are 
adopting useful patterns of behavior which might range from working extra hours 
to.

adjusting slash line on your cv, for instance, by hiding previous employment to 
undergoing plastic surgery. Mm-hmm. . So this kind of things or to taking 
performance and enhancing drugs, things, right? So, so we need to be careful 
with this because not allowing yourself to be human. Makes us machines and 
machines are supposed to be productive for the sake of productivity and not for 
the, I mean, there is no real thing like wellbeing of a machine, and this is 
essentially a very, very dangerous plan.

Yeah. 

[00:33:39] **Michaela:** And there are also papers around the pandemic and how 
the pandemic also increased overworking, you know increased productivity well 
for the sake of, you know, decreased wellbeing and decreased work-life balance. 
So, yeah, I, I definitely see. that this is a hot topic. And I think with the 
working from home movement, which I, I'm, I really like working from home, but I 
think it's even harder to set your boundaries, right?

And say, well, I'm out of office right now. I don't watch my emails . I'm not on 
call right now. Right. And, and yeah, and really making sure that even though 
maybe I can take a break in the afternoon. I don't have to completely compensate 
overcompensate for that. Right. Like having over hours and working much more.

Yeah. 

[00:34:28] **Alexander:** Yeah. It's, it's tricky, right? So the pandemics thing 
seem to suggest that there is a separation between people who can uh, handle it 
and people who cannot handle. Uh, And there are many, many reasons why some 
people can, and why some people cannot. But for instance, the Brazilian study 
has studied, has shown that one of the variables is gender.

Mm-hmm. . Their study has clearly indicated that women had much harder time 
dealing with the pandemic where of working than men. And this was partially 
related to the fact that the needs were different. Some men were typically 
complaining about environmental. Like noise. Women have been mostly complaining 
about the fact that they need to combine their working from home with 
homeschooling of their kids because the schools have been closed and so on and 
so forth.

And then it also turned out that it's not only that the needs were different, 
but that also the abilities of companies to meet their needs were very 
different. Of course, as a company, it's much easier for you to give your 
employee. Noise canceling headset on ergonomic chair rather than to throw away 
the entire schedule of meetings and reviews to accommodate for homeschooling of 
the kids.

So essentially this study has shown yet again that um, in case of stress and the 
pandemic is obviously a situation of. People who are disadvantaged under normal 
conditions are becoming even more disadvantaged under stressful conditions.

And in this case, it was clear this case for women in Brazil. 

[00:36:05] **Michaela:** Yeah, I think it wasn't probably not only in Brazil, it 
was in so many countries. 

[00:36:10] **Alexander:** Right. Yeah. That the study was, so that's why I'm 
trying to be careful with 

[00:36:14] **Michaela:** generalizations. I, I know, I know. Yeah. Well 
Alexander, thank you so much for being on my show today, talking with me about 
all, you know, all those social aspects of software engineering and and yeah, 
thank you so much.

I will definitely link your papers in the show notes and and your website. Is 
there something else that comes to your mind that you want to share with? , 

[00:36:37] **Alexander:** I can just say that the topics of human aspects of 
collaborative aspects of software engineering are very close to my heart.

So if some of your listeners want to talk to me or want to participate in some 
of our studies or want to ask any kind of questions, they can always contact me 
via Twitter, via email, or in any other. And it'll be my pleasure to answer any 
questions that your listeners might have.

Yeah. 

[00:37:02] **Michaela:** Thank you so much. Cool. I will link everything in the 
show notes, so thank you Alexander, and have a good day. Thank you very much. 
Goodbye. Bye-bye. This was another episode of the Software Engineering Unlocked 
Podcast. If you enjoyed the episode, please help me spread the word about the 
podcast.

Send the episode to a friend via email, Twitter, LinkedIn. Well, whatever 
messaging system you use, or give it a positive review on your favorite 
podcasting platform such as Spotify or iTunes, this would mean really a lot to 
me. So thank you for listening. Don't forget to subscribe and I will talk to you 
in two weeks.

Bye.


