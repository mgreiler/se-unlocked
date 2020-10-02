# Transcript of Episode 15 of the Software Engineering Unlocked Podcast with Peter Pezaris

**Michaela:** [00:00:00] Hello and welcome to the Software Engineering Unlocked Podcast. I'm your host, Doctor McKayla, and today I have the pleasure to talk to Peter Pezaris. Peter is the co-founder and CEO of CodeStream, a tool that helps developers to communicate and collaborate easier and more productively. Before starting his new adventure two years ago, Peter already started several other successful companies. 

Even though Peter is the CEO, he is still writing code and ensures that the system is involving in the right direction. The newest path is going into a code review direction, which is super, super interesting to me. Well, talking about code reviews, did you know that I'm giving remote Code review workshops?

Yeah! In those workshops, I'm helping engineers get the most out of their code review practices because code reviews can either be a teams superpower or a teams expensive bottlenecks. So if that sounds interesting to you, head over to michaelagreiler.com/workshops I'm also going to link that in the show notes and have a look at my code workshops and also all of the articles I have written about code reviews over the last few years.

Well, if you're not wondering what qualifies me to talk about code reviews, I work with all major product teams at Microsoft such as Office, Windows or Visual Studio, to help them get the most out of their code review practices. I also led several large scale studies on code reviews, and I've been part of the team that is responsible for Microsofts internal code review tool called CodeFlow. So yeah, I have quite some experience that I really love to share with the whole world, and so I hope that you consider booking a code review workshop with me, but yeah, let's go back to Peter. Peter, thank you for joining my show. I'm really, really excited that you are here.

**Peter:** [00:01:43] Thanks for having me. I'm excited to be here as well. 

**Michaela:** [00:01:45] Yeah, I'm also really excited. Peter, I want to start at the beginning by learning about your journey. I saw that, you have a Bachelor Degree in Computer science and from your work history I started, you actually didn't really start out building software systems, but you really started out building actual companies.

So what fascinates you about entrepreneurship and how did you get started on your journey? How did you build your first company? 

**Peter:** [00:02:07] I've always been fascinated about being a business owner and being a CEO. I think even when I was in high school, before I thought about what career I was going to embark on, my friends and I always used to talk about what business we're going to own some day.

I had the good fortune of attending Carnegie Mellon university at which I met my business partners who over beers one night decided that we wanted to start a company on our own. So we were all working on Wall Dtreet at the time at various financial institutions, and we were drinking beers and talking about Bill Gates and how much money he had.

And I guess there was an article that we read that said that he had to spend $3 million a day every day in order to spend his wealth by the time he died. And then we decided that rather than talking about him and his wealth, why don't we talk about us and our wealth? And so that was really the genesis behind becoming an entrepreneur.

And we started working on projects, nights and weekends, while we still had our daytime jobs. And then once our first business really started to take off, we had to choose between working full time on Wall Street or working for full time for ourselves. And eventually we made the choice to work full time on our first business.

And from then, uh, it's just been an awesome, awesome ride because I've had a fantastic time, be able to work with those same guys through four different businesses now over the last 25 years.

**Michaela:** [00:03:40] Oh, wow! And so somehow a dream of wealth and money. Right? Is that also what you achieved? Is that, did you achieve that? 

**Peter:** [00:03:48] Well, we have had good successes over the years. Uh, although at the time that was our motivating factor. You know, I think a lot of young people when they're first entering to the workforce, they, um, they want to make money, and that's a reasonable thing to do. Um, but for us it was, it turned into more than that because as we started our businesses and once we started making money and after we sold the first business, I didn't understand at the time what would be an immense sense of satisfaction just having built something of substance, something that was valuable. Uh, it gave me the most enormous sense of pride, and it's something that I identify with very closely to this day. You know, I am an entrepreneur. It's part of who I am. 

**Michaela:** [00:04:35] Yeah. I find it really interesting because I just started my entrepreneur journey very, very recently.
It's only a few months old and the motivations are completely different, right. So I'm thinking about having an impact. 
Being my own boss, deciding what I'm going to work on, flexibility and all that. I, well, also what you said at the end, right? So, it's about building something that lasts, and if you're looking back, you say, well, I did that.
I've done that right? So, yeah, I think there is some overlap, but let's talk a little bit more about the startup that you're currently working on. It's called CodeStream, and it's a collaboration software for software developers. So actually it's a really interesting tool, as I said at the beginning, because now you're P VOing a little bit, or you're adding functionality for code reviews, and if I have to describe CodeStream as it is right now, it's a software that allows users to write comments about the software, right there in the IDE. Is that, is that a good way how to describe your company, or how would you phrase it?

**Peter:** [00:05:43] Yeah. So we're develop developing something that we call a developer collaboration platform.

And there are a number of different pieces to this, but you can think about it as doing a series of features and products that enable more real time and more rich interaction between developers as they're writing code. And the way that I often explain this to people who are unfamiliar with our product is by using an analogy from Google Docs.

We're all familiar with the awesome collaborative features of Google docs. And one of the things that makes it so great, such a great product, is that if you and I are writing the same document, we're both collaborating on a document. If I have anything that I want to talk about with you, uh, I can just select one of the sentences. And then type my comment, whether it's making a suggestion for how to edit it, whether it's pointing out a typo and you as the recipient of that message will know exactly what I'm talking about because it's hyper contextual. Well, software engineers to date don't have that capability to collaborate within their source tree.

And instead, because most developers live in their IDE where they write code all day and today's IDE's don't have that capability. So that's how we started with CodeStream. Just a very simple user interaction where you can just select any code directly in your editor and type of comment on that. And that comment gets shared with your teammates.

So that was the first feature that we built. And since then we've built all kinds of different user experiences that are developers specific, but they all center around connecting you with your teammates and allows for realtime collaboration around source code. 

**Michaela:** [00:07:31] Yeah. Yeah. So what I really liked when I worked with your system, what I really liked was that you have some ground truth, right?

So you can select a piece of code and then this snippet is actually sent over to the other party, to the person that you are talking about it, and they really know what you're talking about. So this is something that I liked very, very much. Um, but what I was also thinking about, especially when we are talking about communications is Slack. 
Slack for example, was several years ago, it was... It conquered the business communications, right? So it was like boom, and suddenly everything, and everybody was on Slack and they were so happy that they find an alternative to the never ending emails, right? But now, over the last few years ago, I saw a shift.
People are starting to get overwhelmed by the amount of messages that are now happening in tools like Slack or Microsoft teams, or you know, all these real time communications. And so my question is, how does CodeStream fit into this evolution of online communication? What's your role? How do you see your role as CodeStream in that space?

**Peter:** [00:08:40] Yeah, that's a fascinating question. So we have a customer, in fact, we just spoke to him yesterday and he has the following challenge with, I think this pain is felt by a lot of development teams today. He says that the conversation around the source code is fragmented. That when a developer asks a question about, for example, how a chunk of code works, what they often do is they copy and paste that chunk of code into Slack because Slack is the realtime communication tool that they use for back and forth, you know, quick answers to questions. But if they're doing work on a particular bug or a particular feature, well that conversation often happens in Jira. And then when there's time for code review, well, that conversation about the code happens in Github and then if there's customer feedback, the conversation happens in yet another tool.

So all of these different systems are somehow housing different chunks of conversation, but they're all related in some way to your source code and the state transitions that your source code goes through as you make commits and changes. So CodeStream's role in all of this is rather than providing yet one more place to go check for conversations, our role is to connect all of those existing conversations that are happening across all those different systems and provide users the ability to connect those existing conversations to the relevant parts of the code base.

And I'll give you a quick example. Instead of copying and pasting code from your editor into Slack to ask a question about it. Well, with CodeStream, you can type that question directly or in your IDE, and it will post that question to Slack so your teammates can still reply on Slack the way that they're normally used to doing, but now because CodeStream knows what code you're talking about, that conversation thread will be visible inside of your IDE, not only for you, but for anybody that looks at that code, whether it's today, tomorrow, or three years from now, after that code has changed and merged. So CodeStreams unique capability is to be able to tie artifacts, whether it's another conversation, another system. It's a Jira ticket, it's a commit ID. It's a PR to tie all this activity that's related to your code, back to the relevant portions of your code base that those things reference, and that provides the correct context for when you look at that code down the road.

**Michaela:** [00:11:19] Yeah, that sounds really interesting. In my introduction I said, you are still hands on writing code, but as the CEO, how closely are you really involved with the engineering activities? 

**Peter:** [00:11:30] Um, that's a great question. So, and I'm, I'm, the reason I'm hesitating is because I, I think different people on my team would answer this differently.

Um, it's a very delicate role to play. If you're a CEO who's writing code, I like to tell the team, or I like to present myself as essentially having two jobs. During the day, most days I'm performing the functions that a CEO would typically do. I'm talking to investors, I'm dealing with team issues, the financing, the customer communications, uh, interfacing with the marketing team and all different aspects of the business.

And that's pretty much a full time job. Uh, but because I love what I'm doing so much, I like to say that I have a second full time job. And so most nights, uh, when all of that activity has died down a little bit, I have some time. Some quiet time to write some code. And lately that's actually been quite a lot of time, uh, because we're super excited about some new features that we're building out and so I've just been, you know, coding into the wee hours of the morning because I, I just really love doing it. 

**Michaela:** [00:12:32] Yeah. Cool. So how big is your company? How many people are working on CodeStream in general, and how big is the engineering team? 

**Peter:** [00:12:40] We have 13 employees in total, and eight of them are on the engineering team.

**Michaela:** [00:12:45] Okay. So eight of them are in the engineering team. And does that include you, Peter? 

**Peter:** [00:12:49] It does. And so, uh, I guess I could be included on both sides, but it's, you know, 13 people in total. And one of the things I try really hard to do is when I put on my developer's hat, I take off my CEO hat. Because I think it's important for me not to dictate to the rest of the team that like I'm right, because I'm the CEO.

I think for a lot of founders who are still contributing code, that's a very, I've mentioned a delicate balance, and so I try very hard to just. Be a regular developer, equal to everybody else on the team, uh, and, and to not ever rely on my title in order to make a decision go my way. 

**Michaela:** [00:13:31] You overrule everybody, right?

By saying, I'm the CEO and these are actually a CTO. Do you have like a CTO role as 

**Peter:** [00:13:40] well? We do not, but we're actively recruiting. So if this company sounds interesting to anybody where, uh, please send your application. We've got it listed on our website. 

**Michaela:** [00:13:50] Okay. So what roles do you have among those eight engineers?

What, what roles are there?

**Peter:** [00:13:57] Uh, I believe very strongly in a flat development organization and me being equal to everybody else as part of that, um, we do have developers who have particular strengths in certain aptitudes in terms of what they're good at doing. So we like to assign work based on those strengths.

For example, uh, some of the engineers are particularly good at UI. Uh, and others are particularly good at backend or database systems. So we definitely have a, a natural tendency to assign work based on those strengths. But we work very hard to, uh, encourage people to go a little bit outside their comfort zone to support and encourage full stack development.

And so what we like to say is that whatever, would ever portion of the stack that you're most comfortable, we want you to be regularly going at least one stack higher and at least one stack lower. So at the very least, you learn how your code impacts and interfaces with other areas of the code base, but constantly encouraging developers to move up and down the stack so they can get exposure to more technologies, more experiences, and just a greater understanding of the entire code base.

**Michaela:** [00:15:09] Yeah, that sounds really, that sounds really good. I think it shapes the way you develop your code. If you see. As you said, if you're seeing how your code is interfacing with something else, how it's used, and actually also the problems that your code might create on a higher level or on a lower level or something like that.

So another question that I have for you is, do you have like testers in your organizations? Do you have like do, do automated tests and we have like manual tests? How does testing work at CodeStream? 

**Peter:** [00:15:40] As we talked about earlier on the podcast, I, I've run a engineering team for the last 25 years and over the years we've tried a number of different approaches when it comes to testing and there are plus and minuses to all those different approaches.

The one that I'm most fond of, although my teammates will disagree with me, the one that I'm most fond of is one in which there is not a separate QA team, but rather engineers are responsible for testing each other's work. I find that that often produces the best results and the highest quality code, uh, rather than relying on a separate QA team.

**Michaela:** [00:16:20] So the internees are supposed to write automated tests and also do a manual testing? Is that what's happening? 

**Peter:** [00:16:27] That's right. 

**Michaela:** [00:16:28] And what about operations? Are the engineers also responsible for the operations of your system? 

**Peter:** [00:16:32] Uh, one of the, one of our engineers, uh, handles 95% of our operations, uh, and has over the years because he's been one of my partners that I've worked with for 25 years. Although his role has definitely changed. Um, I remember, I'll tell a fun story about our first business when we were scaling it up. We had, we ended up with thousands of nodes, you know, computers that we were managing ourselves in data centers across the country. And he came to me one day and asked me, He said, "We need to buy some new power strips for the data center". I said, "Sure, buy some power strips". And he said, "Well, they're kind of expensive". And I said, "Okay, how much are they?" They said, "Well, these ones are $650 and these ones are $700 and I need to know which one to buy". And I said, "I don't care. It's 150" and he says, "No, they are $650 each".

And I said, "Well, wait a second. First of all, how many do we need? And second of all, what is a $650 power strip?" Like, I don't understand how robust could it possibly be. And at the time, data centers were doing IP addressable power scripts. So you could literally tell net into the power strip and a little micro computer on it that could tell you what wattage was being drawn by each outlet, you could turn each one on and off by sending a command over an IP request. 

**Michaela:** [00:17:54]: The start of IOT, right?

**Peter:** [00:17:56] Yeah, it was. It was! But what was crazy is that at the time we were building a fantasy sports business, right? This is a sports industry, and I said. The last thing in the world I feel I need to be an expert on is the IOT of power strips and finding the best value.

So thank goodness that Amazon and Google and Microsoft have taken a lot of that headache away from us entrepreneurs, and now, you know, they worry about the data centers and we just rent space from them. It makes our lives a lot easier. 

**Michaela:** [00:18:31] Yeah. And it's so true and it's so different right now. I also remember when I was still in university and had our server, I mean it wasn't production server or something, right?

But so we had our little website on it and our projects and things like that running on it. And you had it right under your desk and you were always totally terrified that something, or somebody will hack into the system or you know that something will happen to it right in here. Yeah. So that sounds cool.

Um, so I want to understand a little bit more about your software development practices, because in your 25 years, you probably have seen a lot of different things and you have tons of experience. I don't want to put waterfall into your mouth or something like that, but 25 years ago, waterfall, most of the things, so even when I was at university studying, people were still talking about waterfall and waterfall processes. And I can imagine that this was also something that happened in some of your first startups, so that you really had, like you first had your requirement phase, and then you had the implementation, and then you weren't testing it only after you finished writing every code.

So this was a very traditional waterfall model. So is that something that, um, was a thing in one of your companies and how did that progress over the years? How did that software development change? Um, well, I think this are probably too many questions in one, but I'm looking forward to your answer.

**Peter:** [00:19:59] Um, well, I'll, I'll talk a little bit to the history and then where we are today. Um. So we definitely had more of a waterfall process, and it was before, you know, the word agile was ever really used. Uh, so we didn't know that we weren't agile because it was just sort of the way that, um, we wrote software.

But actually our first business didn't allow for a traditional waterfall because we had such hard deadlines because it was a. Um, uh, sports-related product. You know, the NFL is going to start on September 6th, whether your software is ready or not. You know, they're very, very hard deadlines when you work in the sports industry and there are probably 20 deadlines a year that you have to keep to.

And so that keeps your dev cycle short. You don't have a long time for a long planning cycle. And then a big implementation phase and then a giant rollout. You're just constantly releasing software. So it's sort of agile that we didn't call it that back then. It forced us into that type of mode. But our second business was more of a waterfall approach. And this is sort of in the, in the early 2000's and one of the biggest mistakes I ever made as an entrepreneur is that we did this massive redesign of the website without doing sufficient testing and without doing a gradual rollout. And so we did this months long rework of everything. And we were so happy with that, what had come out, we were certain that it was gonna be loved by our customers. And what we found out was that, although they didn't object to it and they kind of like the new design, it had some fundamental flaws in terms of how it impacted our growth metrics. And it did real damage to our overall business.

And it took us months to recover from it. I'm not sure ever we ever did fully recover. And that made me realize that I never want to do that again. Um, and so now, now we, we have much, much shorter dev cycles for our business. Uh, but what's really interesting is that as part of my job, I talk to customers all the time. And since we're a dev tools company, I talked to them about their dev process. And so we ask these types of questions, uh, to at least 10 customers every week. And we amass all the results in a, in a big database. And it's incredible. Even today, hearing the diversity of different types of processes. There's one customer at one extreme, who has two engineers and they pushed to production 20 times a day.

**Michaela:** [00:22:34] Oh, wow!

**Peter:** [00:22:36] Basically every little micro change goes through this, you know, continuous integration, continuous deployment cycle, and they're just constantly releasing new stuff to production, like in tiny little chunks 

**Michaela:** [00:22:38] and how many people are using that system?

**Peter:** [00:22:40] Uh, thousands, thousands, and they charge a lot of money for their system per user.

So they're generating an amount of revenue, a good amount of revenue from just having a, a small engineering team. Uh, the other end of the spectrum, some larger and older companies are still doing sort of quarterly giant releases, which, you know, we would referred to as a waterfall dev cycle. And there, they all know that they're trying to change the corporate culture, but it's really difficult to do that.

**Michaela:** [00:23:11] Yeah. There have been several studies on how frequent releases just increased the quality of your software system, and I think it has a lot to do with the immediate feedback that you have and with the ability that you gain from the frequent releases that if something goes wrong, you can actually react. So you know where something happened and it happened, you know, within the last code changes that you did, and if you are not merging very often, right? Let's say you're merging only once a month or something, then there are weeks that are passing by and then you cannot reliably say any more when the problem originated from. So, by frequently merging, you can find the root cause much critical.

Well at CodeStream now you say you're more agile, but what does it mean? How often are you releasing? How often are you pushing the button and saying, "well, let's go push it into production"? 

**Peter:** [00:24:04] Um, well, that's changed for us. Uh, actually very recently. Um, as you mentioned earlier, we're working on a new product, which is a code review product.

And our code review review product is unique in that it's a much lighter weight solution than existing solutions that require you to sort of jump between your IDE over to a website, go check your email for a notification back to the IDE interface with Git on the command line. Sometimes. Um, so our code reviews are all-in editor. They're super lightweight. And in that it takes one button to request a code review. And you can do that regardless of the state of your repo. Even if you have code that's not committed, uh, or if you've got code that that is but isn't pushed, and you can get feedback from your teammates at any time. And they do the review also within their editor without having to use a bunch of different tools.

So it aims to streamline the process. And of course. We are the first users of this product. You know, we're building the product, but we're also using it. And it has dramatically changed the frequency with which we are branching and merging, because it's just so easy now to get feedback from each other.

Uh, it's in real time. And I, I don't have the stats yet cause we haven't pulled them, but I, myself am probably landing code three or four or five times a day, and that's, uh, at least an order of magnitude faster than it used to happen. 

**Michaela:** [00:25:34] And what did you use before to do the code reviews?

**Peter:** [00:25:37] Gthub, yeah. And that, and what we found was that because it was a more formal process, we would wait until the end of the PR and, and the, and the problem with that is that it really encourages you to think in the mindset of, I have to wait until I'm done in order to get a review. So, and as engineers, we're often never really satisfied with something being done. There's always like one more change and one more thing and one more thing. And so it promotes this sort of activity, at least it did for our team, that we would have these branches that we thought were only gonna live for a couple of days, and then they ended up living for a couple of weeks because we're not quite ready to have other people look at it yet.

And we will be like, "Eh, I can add that one more thing", or "Maybe this feature is related enough that I'm going to put that on this branch too". Um, and because of that, it really extended our release cycles. 

**Michaela:** [00:26:29] Yeah. So especially if you are a company that develops software for developers, so developer tooling, I think it's a really easy to dog food, your own software, your own product.

And well, as you said, if you are a sports company, it's a little bit harder. Right? But, um, have you seen also some drawbacks of dogfooding because also means that you're only one company, right? So you're having one development style, you're having one culture. So do you think that it can also make you a little bit, um, blind sighted or blind for what's, um, how people outside would be using your software?

**Peter:** [00:27:06] That's always something that you have to keep in mind because whenever you build a tool, unless you build a very opinionated tool that tells everybody exactly what the, which way to do it, then ultimately, your customers are gonna use the tool in ways you had never envisioned. And I think there's also a myopia that people develop that they assume everybody else is like them, which you just pointed out.

And that's something that you have to really, really work hard to, to remember and remind yourself that you're not the only user. There is one other technical challenge that we face. It's a minor one, but it's something that we have to deal with, which is that when we're dogfooding our own software, we're often doing it in a development environment.

And yet we're doing it with like real... We're really using the tool, right? So we don't want to have to switch between development and production because then we lose the history of what we're working on. And yet we want to use production because you know, it's a production usage. So that's something that we, we haven't really come up with a great solution yet, sort of how to switch back and forth between the two, because every time we switch, it's like we lose half of our content.

**Michaela:** [00:28:14] So how do you do it?

**Peter:** [00:28:15] Um, we lose half our content, which is, which is not, um. Uh, every like, it's when, when we are working on a pretty big project, like this code review thing is a pretty big project for us. And so we'll switch to the development environment to dog food it because we want to use that there.

Uh, but for most features we can sort of wait until it hits production to start using it and we turn it on with a feature flag for us first and that type of thing. Uh, but for code reviews, it was a big enough project that nobody else has tried it yet, except for us. Uh, although we are excited that next week we'll have our first beta customers, uh, giving it a try. Um, and then we'll switch back to using production. 

**Michaela:** [00:28:57] So CodeStream actually works with many different IDEs. So for example, it works with Visual Studio Anthem and the JetBrains IDEs, and you also have different messaging systems that you're integrating with different issue trackers. So there are so many integration points and so many different environments that you have to work with.

So I was wondering how much of the code base is actually, you know, universal across all of those different environments and how much of the codebase do you have to customize to work and be perfect for those environments? 

**Peter:** [00:29:29] Yeah. Um, so we, we worked hard to... because we knew that in order to be successful that, you know, the development culture right now is sort of a bring your own tools type of culture. It's rare that we talk to a customer where they've dictated the tool set to their employees, and because of that, there are some 16 or 18 different editors that are in pretty good use today. Uh, there are, as you mentioned, a number of issue trackers, and so we set out to write our software in such a way that we didn't have to build a custom solution for each one of those things.

And that meant spending a lot of extra work upfront to build a generic service that can then have sort of plugin components to talk to the individual different issue trackers or messaging systems, for example. Uh, and so that required quite a bit more work than we. Would have had to undergo to support one of them.

Uh, but now that we're there, it's pretty straightforward for us to support additional types of integrations. 

**Michaela:** [00:30:31] Okay. So I worked for the team that was responsible for Microsoft internal code review tool called CodeFlow. And from that experience, I know that, for example, just making sure that the comments are in the right place, even though you know, there are changes to the, to the code, and the new versions of the code is a pretty extensive work, and I can imagine that you have different IDEs and different issue trackers, it's becoming even more complicated. So I'm wondering how do you test that the things are appearing at the right place? For example, how do you test that things are working smoothly, especially if you have so many integration points and for example, IDEs and developer toolings have a lot of frequent releases. So how do you make sure that everything is perfect? Everything is working fine? How do you test that? 

**Peter:** [00:31:20] Sure. Um, the one commonality we have among all of our customers is that everybody's using Git and thank goodness. Um, we, we don't support a subversion or per force. Um, and I guess there, there are some customers out there using those tools, uh, but Git as something like 94% of the market by now. And so that makes it easier for us, uh, to make that decision to only support Git at this time. Maybe someday there'll be another version control system that we will support cause it'll have enough of a customer base or an important enough customer, but that's simplifies things pretty dramatically for us because the most complicated things that we do are exactly what you just mentioned. You know, tracking different versions and where this chunk of code ended up post-merge and, and those types of things.

So supporting an additional issue tracker, for example, like Jira versus Trello. Uh, versus Github issues. That's relatively straightforward. Each one of those services has a set of published API's. And they're all pretty similar. Um, so it's really just building the glue software. Uh, the one challenge that we do run into is in the IDEs, because IDEs are under pretty rapid development today, especially with their extension API's.

And we rely heavily on those extension APIs. And so we've built essentially a layer that sits on top of the different editor, extension APIs, that gives us a common set of primitives that we can build against. And so we just have to ensure that with every release of a new API or a new IDE API, uh, that it continues to work.

And that's where we spend a pretty significant amount of our QA resources. 

**Michaela:** [00:33:04] Okay. Yeah, I can imagine. And so what does the tech stack look like at CodeStream? What are the languages that you, are you saying, what are the technologies that you're using? 

**Peter:** [00:33:13] We built the software using TypeScript whenever possible.

So the front end is built with React. And essentially our architecture on the client side is a little bit more complicated than it needs to be, but it allows us to support different IDEs, and it's a three tier architecture on the client side that has the front end, the presentation layer in React and TypeScript.

Then we have a middle glue layer, which is essentially our API layer that interfaces with the editors APIs, things like what's the currently selected file, what range of selecting in their editor. It allows us to open up new files in the editor and those types of things. Also, importantly, it allows us to, uh, invoke a web view within the editor, and that's how we present our React front end. So that's the middle layer, which is the IDE extension. And then there's a little demon or an agent that runs on your computer, which is an LSP server. And that's also written in TypeScript. So on the client, the top and the highest, the React component, and the LSP agent are both written in TypeScript and they're both identical across every IDE.

We support. And then in order to support an additional IDE, we just have to write that little middle glue layer that talks to the editor itself. And so that that's how our clients work. And then they talk via HTTPS to our backend, which is an API server written in TypeScript using Node. And then it talks to a Mongo backend and we run that in the cloud in AWS, or we also have an on-prem installation option for customers that they can run in a Docker container.

So we provide them the image and you can manage it yourself behind your firewall.

**Michaela:** [00:34:54] Yeah. Very cool. So now that you described a tech stack, what I want to know is, did the tech stack change over time, or did you have the same tech stack for the different companies? I mean, probably not because you're going back 25 years, but let's say for the last two companies that you build, did you have the same tech stack or did you change frequently and if there was a change, why did you change it?

**Peter:** [00:35:19] Well, it's changed even for this company. We started out writing just one solution for one editor. Uh, and then we sort of quickly realized that we have to, you know, change it in order to support a number of different editors. So we started out just writing plain vanilla JavaScript and only targeting the Atom editor because a couple of years ago that was more popular than it is today.

Um, so we moved from JavaScript to TypeScript, which I initially provided, uh, a little bit of resistance to, um, but I'm a convert. I like TypeScript now. That's, I think it's, uh, it was a good move for us to make. Um, but the tech stack has been very different for every company that we've started. The first company, uh, the product was written in Perl.

And, uh, you know, that's not a language that's in common use today. And it was a... You know, as a mod Perl website running on a patchy, um, with a, mySQL database and, uh, you know, the front end was like hard coded HTML and, uh, CSS templates. Yeah. 

**Michaela:** [00:36:24] And one was the text tag off to company before. 

**Peter:** [00:36:27] So Glip was our previous company, and that was written using vanilla JavaScript using the backbone framework.

Backbone isn't super popular today, but it was sort of a competitor to what people would choose, React or Angular over backbone today. Um, but backbone service pretty well. Um, and that's actually still in use in production today. There are millions of paying customers using Glip today using that same client software that we wrote back then.

It was a, very, very similar to Slack in terms of its capabilities as a team. Communications tool, uh, built as a single page app that's delivered over the web. Either you could use it in a web browser or a, an Electron app on your desktop. 

**Michaela:** [00:37:11] So now that you worked with different engineers and different companies, and we're always in a leading role somehow.

Um, so what have you learned about collaboration? How do you make sure that people are working well with each other? That they are, you know, there is a good engineering culture, a good team culture in the engineering team. 

**Peter:** [00:37:32] Well, the first thing I would say is openness and transparency, um, is if you have good communication, not just about the work that you're doing, but also about other things, uh, about job satisfaction, about your personal life. Um, that means a lot. As I mentioned earlier, I've had the good fortune of working with the same senior management team for 25 years. So by now, these people are not only my business partners, but they're my best friends. You know, we, we were at each other's weddings and each other's best men. And you know, we, we baptize each other's children.

And that, I think, gives our whole company this culture of being part of something, but being part of a family that's more than just writing code and finishing specs. So what I have always done, and I think it served us well, is to promote the social aspect of working with somebody. And that means going out to dinner with each other, having each other over for barbecues and having a relationship outside of the office, and that, I find opens up conversations so that you can see who's happy, who's unhappy, and how you can improve that, uh, and make sure it's consistent over time. 

**Michaela:** [00:38:46] Yeah. So this makes me a little bit, think about remote companies, I don't even know is a CodeStream alittle bit remote?

Do you have like remote positions or you're completely colocated? Um, but yeah. What, what does this mean, um, for companies that are remote? Because what you're telling me is face to face connection, right? It's really a moment where you can touch it under, right. Very in the same space, in the same country, in the same city, in the same office.

Um, so have you thought about how those things can be transferred to remote settings? 

**Peter:** [00:39:20] Yeah, that's a challenge and it's been a challenge for us because we have managed primarily remote teams over those years. Um, you know, Dave, one of my business partners, he's our head of product. He and I haven't lived in... we've been business partners for over 20 years, but we haven't lived in the same city for any appreciable time.

Like for I think the only two years out of those 20 plus, and I work very closely with Dave and now we rely heavily on Zoom, on video conferencing on tools like Slack that allow for remote collaboration. And for development work. You know, we're eating our own dog food by using CodeStream. So I think that's incredibly important that we can use the tools that allow us to build tools that will help other remote teams, but also we are helped by them, not only our own tools, but by other tools like that, that doesn't really address the social aspect.

And so we generally speaking, have to travel in order to have that. Um, I have not, I've tried, but I have not yet found a good remote socializing work solution. right? We've tried to do like happy hours where like, I'll open a beer and you open a beer at the same time over a video chat, that doesn't tend to work for us.

I'm not sure if it works for any companies, but it doesn't work for us. 

**Michaela:** [00:40:39] So one of your cornerstones is really having onsite events where the whole company meets and does something nice together, or how does it work?

**Peter:** [00:40:47] I think that the money that we save by not having offices, you know, we spend very little money on actual office space.

There are a couple of guys that don't have enough space to work from home. So, uh, they end up in an office. But other than that, we, we save money on, uh, on that expense. And we invested it in travel. So we do see each other pretty frequently as a big group. We do that around once every six months or so, but we also frequently are just flying to locations, either for a trade show or a conference or a customer meeting, and we tend to congregate in groups of three or four or five.

And whenever we do that, it's like assumed that we'll have the meetings during the day and then we'll socialize at night. You know, we don't even have to ask each other. We just sort of know that that's going to happen and that's a good way for us to stay connected as well. 

**Michaela:** [00:41:36] Yeah, I can imagine. So I want to talk about something a little bit different here.

It came to my mind when you were talking about your system and the architecture and I was like, Oh, I would really like to see it. I would like to, you know, dig into code and see how it's done. And um, what I heard is that you're actually open sourcing part of your system. Is that true? And if it's true, why are you doing that?

**Peter:** [00:41:59] That is true. And not just parts of our system. We're open sourcing the whole thing. Basically everything not related to billing and payments. So you'll be able to see this source code on the front end, the backend, any middle layers, and in the on prem installation that you'll, you'll get. You can build it from source if you'd like to.

So we're doing that for a couple of reasons. Uh, one is that we think it's the trend that even commercial enterprises are increasingly making their source code available for other people to either learn from, to contribute to or to raise issues on. And we think that's important, especially being a code collaboration platform.

We're really looking forward to and excited by the concept of people being able to ask questions about the CodeStream and source code using CodeStream itself. Uh, cause that'll be a great way for us to be able to answer questions about how our own code works to potential contributors. And the second reason that we're doing it is one of transparency.

Um, oftentimes when you trust, especially something as valuable as your source code to a third party SAAS provider, there is a very large issue of trust there. Um, and CodeStream is not yell yet a well known brand in the same way that Slack or GitHub is. And so a customer might feel a lot more comfortable cutting and pasting or copying and pasting a code snippet into Slack.

Um, but we have to earn their trust in order for them to comment on it using CodeStream. And one of the ways that we're doing that is by open sourcing our software so they can audit it at any time and knowing that we're not doing anything malicious with their data. 

**Michaela:** [00:43:43] That's super smart. That's I think, a very, very good strategy because, well, what came to my mind was that your users are developers, right?

And so developers are curious and they will definitely ask the question like, what is actually sending over? How much does CodeStream see about myself? Their system. And what's actually going on here. What happens beneath the surface? And by open-sourcing it people, you know, you're circumventing that people can just look at the code, can go there and see what's actually really going on.

And I think that's a very smart move to build trust. So yeah. So you mentioned a little bit earlier that you're looking for a CTO right now. So my question is how do you hire at a startup and what do you expect from a CTO? For example. 

**Peter:** [00:44:31] Yeah. Um, it's, it's, it's a challenge. Um, I've had, I've had a number of very capable technical leaders that I've had the good pleasure of working with over the years, and the most successful of them have been ones who can, uh, deeply embrace the startup culture. Um, what we won't be doing for this next role is hiring somebody from a big organization that knows how to schedule a meeting and put together budgets and interface with the vendors. That's the wrong set of qualities. We have to find somebody who is hungry, um, wants to get their hands dirty and can lead by example.

And I find that it's those engineers that can rise up into the more management, uh, responsibilities of being a tech leader at a startup and can be more successful doing it. So that's our primary objective, is finding an employee who we have confidence in, can lead us from an engineering perspective and earn the trust of the rest of the engineering team, uh, and lead us where we need to go.

Um. And so that's really provides the framework in terms of the mechanics of how we're going to do it. Uh, we have, uh, our company was part of Y Combinator a couple of years ago and Y Combinator is involved with so many different companies, that hiring is often the most critical need of all of their portfolio companies.

So they've got a set of great resources that can help companies like us, uh, hire for different positions, including one custom solution that they built for themselves, which anybody who's interested in working at a Y Combinator funded startup can go apply. It's called Work at a Startup. That's the name of the product.

And it's a hiring platform that anybody can apply to. And you can see a list of all the YC companies that are hiring and you can apply to work at them. 

**Michaela:** [00:46:26] Okay. And so do YC Combinator gives you access to the recruit list and access to the talent pool or only access to the talent pool. So how does the help that you just described really look like?

**Peter:** [00:46:38] Yeah, all of the above. So sometimes they'll help you. So each YC company like us has one or more partners that we work with that are YC employees. Um, so the partner might help you by recommending somebody specific because they have a very strong network of relationships of engineering leaders. Um, they may have a, another YC company that's not doing so well that you could acquire the company and bring over the engineering team, and that might be one or two or three or five engineers.

So that happens pretty frequently as well. And they give you access to those tools, um, and inside access to those tools, including, you know, when they introduce you to a particular recruiter, for example, being a YC company, that recruiter is motivated to help you perhaps a little bit more than they would a regular company because they want to develop a stronger YC relationship because YC has become such a powerful force within the startup community that a lot of people just want to work at YC companies.

**Michaela:** [00:47:43] So one of the things that I wanted to talk with you, especially because you brought it up, is I want to talk with you about the funding itself. So how did that work? How did you get out to get some of the fundings. I mean, you have already a track record of companies that you successfully started. So somehow I think you had already your foot in the door, but still, when you had the idea of CodeStream, how did you, you know, how did you go about getting the funding for that idea?

**Peter:** [00:48:09] So I'll start by saying that until recently I would have answered you by saying that fundraising is a soul destroying experience. That's the way it was described to me once, and I think that's accurate. Like it's really, really hard and it, it messes with your own psyche because I think us founders often take it too personally, when you hear the word "no".

And the reality is when you're raising money, at least 90% of the time, the answer is going to be no. And when I was first starting out, I used to take that personally because I thought that a no meant that they didn't like you enough and didn't like your company enough. But what I learned is that, most of the time, the no comes for a very specific reason.

And that investors often have contractual agreements with their limited partners who provide the funding that they're going to invest in your company. So they have a contractual agreement to only invest in companies that meet certain criteria. And that could be geographical criteria, it could be revenue criteria, it could be that what sector you're in, what type of business you're building.

And it could be a variety of other things. And so a lot of times when you talk to an investor, it's really just a match banking process. Sort of like pattern matching, like do the qualities of your company even fit the criteria that I could possibly invest in? And if it doesn't meet that criteria the answer is going to be no.

And I used to think that they were just sort of letting us down nicely. You know, it's finding an excuse not to invest, but oftentimes if the answer is no, just the answer is no, and they couldn't possibly invest even if they wanted to. Now, having said that, I, I struggled with fundraising for the vast, vast, vast majority of my career because it was a very difficult thing to do.

And it is difficult for most founders. Um, Y Combinator changed all that, at least for us. And I have heard through the grapevine, it changes it for most YC companies. Just having that badge, that logo, that stamp of approval. Changes the whole dynamic of the conversation. And there's a whole class of investors that are out there that are very interested in investing in whichever YC company they can invest in.

And that makes the conversations a lot easier. And so we've had a relatively successful fundraising efforts, didn't require a whole lot of work on our part. We've announced that we've raised five and a half million dollars in a seed round. And that came almost entirely from YC connections.

**Michaela:** [00:50:48] Okay.

That's really good to know. I mean, I'm a little bit involved in the indie hacker community. It's a community of entrepreneurs, but it's more bootstrapped companies. So there are obviously people also looking for funding, especially if it's the right time. So Y Combinator is definitely something people are looking into.

Well. So we are sort of at the end of our interview, we're running a little bit out of time, so I wanted to ask you, is this something that you want to talk about that we haven't discussed or something that you want to say that you think would be very valuable for my listeners? 

**Peter:** [00:51:23] Well, I imagine that listeners to this podcast are either interested in dev tools or entrepreneurship or something related to that.

And what I'd like to close with is a word of advice to anybody who's out there that's interested in entrepreneurship but hasn't taken the plunge yet. And it's not so much a word of advice, but a word of encouragement. Is that being an entrepreneur has been the best decision I've ever made in my life.

It provides me unending levels of job satisfaction. It, I can't even describe how awesome it is to think back and look back at all the lives we've changed, all the jobs we've created, all the customers that we've impacted in a positive way and built, to be able to build something from nothing and to do it again and again and again.

It's the most rewarding thing I've ever done, other than being a dad, um, with the first book I ever got when I thought about starting my company, yhe first page described being an entrepreneur and it said, um, "once you start your company, you're going to become obsessed with it. And every moment you'll think about your business".

And I actually disagreed with that cause I had never built a business before. And I said to myself, well, that's exactly the wrong reason, because I want to build a company so that I only have to work like 20 hours a week, right? And I can sit back and enjoy life and have a company that feeds me money.

And I'll say that the author of the book was right. That it becomes obsessive, but in a fantastic way. That you want your company to succeed so much because you're so connected to it that you'll give it everything you have. So my advice is, if you're thinking about starting a company, do it. The hardest thing that any entrepreneur does is start and you can do it.

**Michaela:** [00:53:10] Yeah, that sounds really, um, motivational. It sounds really good, but because I have you here and you have such a long history of starting companies, I'm definitely have the, you also had some times that maybe didn't go so well. What would you say, what advice would you give for people that you know, starting out and don't get traction and, you know, did they build the tools?

And I mean, I have many friends in the startup scene and it's not always, you know, shiny and happy faces. It's often. You know, maybe a little bit soul crushing as we talked before. Because when you're trying something and you believe in something and you're building it, especially engineers, you know, they put in the hours, they put in the work and they are building really cool tools.

And then maybe, you know, Micah didn't get some rides and nobody comes. What would you tell them? Because I think it's not always a sign that if nobody uses your tool that the tool isn't valuable or that the idea isn't good, maybe something else is lacking. So how can you overcome those difficult times where you, maybe you're still waiting for your success and it's not coming and it's not inside.

And when do you think is the right time to say, well, I'm pulling back. I'm saying "That's it. It's not working, and I'm going back to find a job again". 

**Peter:** [00:54:30] Well, one of the things that we learned with our YC experience is that one of the things that they do there is they bring in a speakers to talk to you about their successful companies.

So we heard from the founder of Dropbox, we heard from the CTO at Facebook, we heard from, uh, the founders at Airbnb, and inevitably, and a number of others, inevitably, they all have a different version of the same story, which is that they failed and failed and failed and failed and failed until they succeeded.

But when you hear how many times, for example, Airbnb were thinking about shutting down because they couldn't find any product market fit, until they finally sort of cracked the code and found out what it was for them to be successful. It's inspiring in that like, it makes you realize that you're not the only one.

That's going through it. And YC even has, uh, a name for it now they call it, you know, you've got the excitement of coming out of YC, you get funded, and then you got the trough of despair. And so there's this very frequently, this period of time where you, you're not taking off like a rocket ship.

And you're focusing on a whole bunch of things to try to make your business work and YC, his advice for that period of time, which I think is really great advice and advice that we're taking to heart right now, is that when you're in that grind and trying to find that product market fit, you said do two things and focus on only two things.

Number one is you should talk to customers, and number two is you should build a product. And don't do anything else. Um, and that's, that's it. Uh, it means don't hire people before you're ready. Don't build a board of advisors. Don't go spend a bunch of money on marketing and things. That's how you're going to solve your problems.

Just talk to customers and build product. And when you find product market fit, you will know it because the seams will start falling apart. Your database will be smoking in production. You know, you'll have too many customers coming in. You can't handle their billing. You know, you'll know when you have success, but until you get there, only do those two things. 

**Michaela:** [00:56:40] Yeah. Yeah. I think that's really, really good advice. And I also heard very often that if you're trying something out, you will know when you reached success, you will know how that looks like, especially if things failed beforehand. So maybe we close with that one. Um, Peter I would like to thank you so much for being on the show.

It was really, really good to have you here and that we covered so many different topics, so thank you. Thank you. 

**Peter:** [00:57:07] Thanks very much for having me. It was a pleasure. 

**Michaela:** [00:57:09] Yeah, it was really great. Thank you so much. Bye. 

**Peter:** [00:57:10] Bye bye!

**Michaela:** [00:57:14] Hey, if you enjoy my show, it would mean the world to me if you could help me by spreading the word.

There are few things you can do. Send this episode to a friend or spread the word by a Facebook, Twitter, LinkedIn. You can also leave a rating on iTunes. I heard those go a long way. In any case. Thank you for listening to the Software Engineering Unlocked podcast. Don't forget to subscribe and I will talk to you in two weeks.

 