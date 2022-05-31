Transcription


**Dr. McKayla**  00:04 Hello and welcome to the Software Engineering Unlocked 
podcast. I'm your host, Dr. McKayla and today I have the pleasure to talk to 
Yehonathan Sharvit. 
But before I start, let me introduce you to an amazing start-up: tonic.ai - the 
fake data company.
So what does [tonic.ai]( https://www.tonic.ai/?ref=se-unlocked) do?
I'm sure you know how complex and cumbersome it is to create quality test! It’s 
a never-ending chore that eats into valuable engineering resources. 
Random data doesn’t do it — and production data is not safe (or legal) for 
developers to use. 
What if you could mimic your entire production database to create a realistic 
dataset with zero sensitive data? 
That sounds amazing, right
Tonic.ai does exactly that. With Tonic, you can generate fake data that looks, 
acts, and behaves like production because it’s made from production.
Yet, tonic.ai guarantees privacy so your Datasets are safe to share with 
developers, QA, data scientists—heck, even distributed teams around the world. 
Visit [Tonic.ai](https://www.tonic.ai/?ref=se-unlocked), to sign-up today or click 
the link in the shownotes to get a 
free, 2-week Sandbox.
But now back to Yehonathan. Yehonathan is a software developer, author, and 
speaker. He has tons of experience in full-stack development using various 
languages such as Java, JavaScript, Ruby, but his favorite language is Clojure. 
And he bundled and packaged all of his experience and knowledge into his new 
book Data-Oriented Programming. This is also the reason why I invited him today. 
And I'm super thrilled that I will dive with him into how to design and build 
software that deals with information. So Yehonathan, thank you so much for being 
on my show. Welcome here.


**Yehonathan Sharvit**   01:19 Hello, McKayla, I'm really glad to be here with 
you.


**Dr. McKayla**   01:22 Yeah, I'm also really thrilled. And I heard that you are 
giving away one of your books, digital copy of your book to one of my listeners. 
So what do you have to do to win this book? Well, retweet today's episode and 
like it, and then you're in the pot to get one copy of Data-Oriented Programming 
from Yehonathan. So, but, Yehonathan, what is this book actually about?


**Yehonathan Sharvit**   01:46 Okay, so this book is about a simple way to 
reduce complexity of information systems. And by information systems, I mean, a 
program that manipulates data that doesn't belong to the program., data that 
comes from the outside world. For example, a front-end application that receives 
data from a back end, or a back-end application that fetches data from the 
database or an API. It could be also a web worker that reads data from RabbitMQ 
or Kafka needs to process it and passes it forward. So all those systems have in 
common that they manipulate data. But the data does not belong to it, the data 
or the information existed before the program, and will continue to exist after 
the program dies. And those kinds of systems, which is basically what we do on 
our day-to-day basis as full-stack developers need, I think, a different and a 
simpler approach to how we represent data inside our programs.


**Dr. McKayla**   02:50 So I realized that when I looked at the first topic, or 
the first subtitle, Unlearning Objects, it was very, very clear to me that it 
somehow has something to do with object-oriented programming, and that you want 
actually a paradigm shift here. And you think now about data-oriented 
programming, more or less, right? And so, that this can somehow improve our 
applications, and probably our maintainability. So what is that shift from 
object-oriented programming to data-oriented programming? And why should we 
unlearn objects?


**Yehonathan Sharvit**   03:24 Okay, that's a great question. And let me tell 
you how I see it. I practice meditation. I've been practicing meditation for 
around 10 years now. And to me, there is quite a similarity between what 
meditation guides us to do and objects. So in meditation, the basic assumption 
of the basic principle is that the main cause of our suffering doesn't have to 
do with the reality itself, but it has to do with the way we perceive reality. 
So our mind projects, something, an object on the reality. Object causes us 
suffering. But the reality on itself does not cause any suffering. And 
meditation guides us to remove the glasses that our mind puts on reality and to 
look at the reality as it is. And if you are able for a moment to look at the 
flower as an idea, if you are lucky enough to explain that it's a joyful 
experience. And even pain, if something is painful, if you're able just to feel 
the feeling of the pain with no interpretation of the mind, with no meaning 
about what does it mean about me but just experiencing the pain as a physical 
trigger, then the pain is not as painful as it seems to be. So that's what' my 
take on meditation is. And in a sense, object-oriented programming is causing 
suffering to the developers because instead of looking at reality, at data, at 
information as it is, we took our mental model, and then we stepped into 
infinite complexity system. But that's not that the data on itself or the 
information on itself is complex, it's the tool. The object that we use to grasp 
data is causing the complexity. So in a nutshell, I would say that most of the 
complexity that we have in our program is accidental complexity. It's complexity 
that we have created because of our mental model. It's not inherent complexity 
that has to do with the business domain.


**Dr. McKayla**   05:25 Can you give a concrete example of how object and 
object-oriented programming increase the complexity of our system?


**Yehonathan Sharvit**   05:33 Yes, so let's take... In the book, I take a 
simple example of building a library management system. And let's say in the 
library, you have books, and you can do many kinds of operations with books and 
authors. And in object-oriented, what you do is that you create an object that 
represents an author, and you have methods inside the objects to manipulate the 
author object. But the fact that you bundle together code and data or behavior 
and data creates complex hierarchy diagram. Suddenly, many classes need to input 
the author definition, just in order to access a simple field from the author. 
Or if you want to create a new author or an author with different fields, you 
have to create all the method of the author. Or if you want to test how the 
function of something behaves on an author, you have to create this complex 
object just to check for little things. Sometimes we say that you want the 
banana but instead of having the banana, you get the banana and the gorilla and 
the jungle, while you only want the banana, only one, the name of the author.


**Dr. McKayla**   06:36 And so how would I design that system? Let's say with 
this library, and the books, how would I design that in data-oriented 
programming? How would that look differently?


**Yehonathan Sharvit**   06:46 So it will be very simple. First of all, you 
separate data from code. And now you ask yourself, how should I represent data. 
So you have stateless objects or modules for the behavior. And you have data 
with no methods, data objects, or data classes, or data maps for the data. And 
what is data? Most of it is just record. So its maps are HashMaps, with fields 
and values. And that's it. So you represent your whole domain as a nested 
combination of maps and arrays, and integers and strings and kind of JSON, what 
JSON has brought to the world since it has been adopted, and not only 
JavaScript, it’s simple tools to represent data. What do we have in JSON? You 
have strings, you have integers, numbers, Boolean, node, to represent 
information that belongs to the real world.


**Dr. McKayla**   07:37 Okay, and so how would I structure the code in terms of 
files, for example? Where do I put all that data information? And the functional 
information will have separate files, two files, three files, 10 files? How does 
it work? One file?


**Yehonathan Sharvit**   07:52 Yeah, yeah, the thing that I didn't mention is 
that in data-oriented programming, we separate between the data representation 
and data validation. So let me give you an example. When you create a book with 
the title, and the publication year, and the list of authors, you just create a 
map, you don't create a book object. So you don't need any class to instantiate 
a new book, it's just a HashMap. If you're in a language like JavaScript, Ruby, 
or Python, you have dataliterate for that, if you are in a language like Java, 
or C # or statically typed language, you have a HashMap constructor. So that's 
it, you don't need any type definition for the book. And you organize your 
functions, you would in a regular object-oriented program, but the functions are 
much simpler, because they are stateless, they always receive as an explicit 
argument the data that they manipulate, so there is no implicit leads or set or 
reference to the object because there is no object.


**Dr. McKayla**   08:47 Okay, and so you were already talking a little bit about 
verification. And so for me, the first question that now comes to my mind is 
that actually with the typing, right, and that I can even create custom types, 
and then, you know, enforce them in the system. This gives me somehow also 
security that a book actually is how I imagined a book to be, how do we have 
that in data-oriented programming? How do we verify that it looks like this? And 
you know, like, because JSON again, right, we have we have some simple types. 
But you know, you could present me any data. And I'm not sure if this is...


**Yehonathan Sharvit**   09:22 Yes, exactly. So you could, for example, receive 
a map that you think is a is a book and a book, you're expected to have a field 
name title. And suddenly you get a map. And the field is named D title, for 
example. So how are you going to deal with that? And that's a great question. 
And the thing is that you deal with that, like when you encounter surprises in 
the real world. So surprises happen in the real world. If you, over the wire, 
let's say you access an API and you ask for a book. And for some reason, there 
is a bug in the API, the server that serves the API, and you receive a book with 
a room field. You need to deal with that. And the types won't be helpful there. 
The types will just fail, try to pass the JSON into a book with a field title, 
and there is no field title. And you will have either an exception or a nice 
error message. So this is applicable exactly the same way. In data-oriented 
programming, you define your schema. In a schema language like JSON schema, you 
receive your data presented as a hash map. And there are libraries in all 
languages alone to validate a piece of data against a schema, you validate, if 
it's valid, to move forward, if it's invalid, you deal with that by sending an 
error message to the user, by whatever, how you deal with that. But the 
important thing is that you embrace surprises, you don't assume that everything 
is going to work as expected. Like in real life, you know, you learn at 
university, you read books, you consult professionals, if then you expect that 
life will behave exactly as you have been told, you're going to be quite upset. 
So the approach is that you embrace changes and surprises. So you have modeled, 
you have expectations, but you have little maps or glasses, but you don't 
confuse... There is a great quote that I remembered today or yesterday about the 
map is not the territory. So objects are like map, schemas are like map. Quite 
often in object-oriented programming, we tend to think that the map is the 
territory. There are no objects in the real world, the information about the 
book is not an object. It's a piece of information, you might decide to 
represent it as an object in your program. So that's your map. But that's not 
the territory. While in when you represent your program information about the 
book, string map, just a map with keys and values, this is much, much closer to 
what it looks like for real, there is less of an impedance mismatch between how 
the information exists in the world and how you present in your program. So it's 
a move of humility in the sense.


**Dr. McKayla**   09:38 And so I think I get a good understanding of how it's 
different from object-oriented programming. But what's the difference to 
functional programming now? So where do they overlap? Or where do they differ, 
those two different ways?


**Yehonathan Sharvit**   12:10 Yeah, that's a great question. So first of all, 
they overlap, functional programming and data-oriented programming, by both 
approach in that we need to separate between code and data. So that's exactly 
the same. But when it comes to how should we represent data, in most functional 
programming languages, like Haskell, OCaml, etc, you'd use custom types to 
represent data. While in data-oriented programming, you don't use custom types, 
you use generic data structures. So that's the main difference. And there is 
another area where they overlap, the data is immutable, in both in functional 
programming, and in that alternate programming, we never ever mutate, we always 
create a new version of data to manage changes.


**Dr. McKayla**   12:54 Okay, so one of the big benefits from data-oriented 
programming that you see is that we don't have the custom types. I'm a big 
custom-type person, right? I'm always happy if I can create the type. And I 
have, you know, some enforcement around that, you know, you already described it 
to me, but still, what are some of the really cool things? Or why does it help 
me not to have the custom type and not such a strong typing system around what 
I'm doing?


**Yehonathan Sharvit**   13:23 I'm going to send you back the question, what is 
it that you liked so much about type?


**Dr. McKayla**   13:27 Well, so we were thinking about complexity, and I think 
I've never, not at least intentionally wrote a data-oriented program, right? So 
I can just go from my experience that I have so far. And I would say that strong 
typing helps me to avoid a lot of complexity around ensuring that, you know, the 
thing that I'm getting is actually what I'm getting, because it's already, you 
know, somehow, even before it runs, right, so it's definitely, I can statically 
assure that this works. Now, if I remove that layer, I feel like very insecure, 
I feel like oh my god, now I have to write all this logic that you describe of 
like, I'm dealing with this uncertain world. And I have to check this and that. 
And I totally understand that this is somehow reality. But on the other hand, 
why do I have to create my reality more complex, in my mind, right? More 
challenging than it has to be? Because if I have the type system behind it, I 
can say, well, I know that this is a book and this is how it looks like, and 
otherwise I will not receive it here.


**Yehonathan Sharvit**   14:27 Perfect. Great question. Before I answer, let me 
ask you another question. Do you also enjoy the kind of help that you ID gives 
you when you have type, autocomplete... that you can never miss type a field?


**Dr. McKayla**   14:40 Yes, I actually like that. Yeah. And I like that. I have 
a tooltip that I know Oh, these are the fields that I need. You know, like, I 
love all of that very much.


**Yehonathan Sharvit**   14:49 Okay, perfect. What you said totally resonate to 
me. Now, are there anything that you dislike this type, or for you it's the best 
that could be in the world?


**Dr. McKayla**   14:59 There are probably tons of things that I disliked. But 
now that I have to think about it, but you probably can tell me...


**Yehonathan Sharvit**   15:06 Okay, let me challenge you, when you have, let's 
say a book record. That is, how easy it is to serialize it to JSON?


**Dr. McKayla** 15:13 It depends. If I need a higher library, sometimes it's 
easy. Sometimes it's hard.


**Yehonathan Sharvit**   15:18 For my experience, it's always had with static 
typing. There is no native way to take record a custom type and to serialize it 
to JSON. You need always to hack something to use reflection, or some kind of 
hack. You agree.


**Dr. McKayla**  15:35 It's not straightforward. It could be, it could be more 
straightforward. Yes, I agree.


**Yehonathan Sharvit**   15:39
if if you program let's say you write a game, for playing with the library, then 
you create the books and the books stay in the program. So you never need to 
externalize data, that's fine. I have nothing to say against types, because it's 
a closed system. But if the moment you need to externalize your information to 
other, you need to go out of your types anyway.


**Dr. McKayla**   16:04 I never saw that as a real problem. Because it's just 
another step of things that we have to do, right.


**Yehonathan Sharvit**   16:11 I'm curious, how do you serialize? Let's say you 
have a nested record that describes the whole library with books and authors. 
How do you make from it? No, I'm ot saying that... Yeah, it definitely takes 
time, right? It takes time and effort. And you have to write it, right? I 
probably write the record, but I'm not sure if this is. Or I asked the other 
person... Yeah, you write to custom logic for any piece? Okay. So one challenge, 
another challenge. Let's say you have in the book, you have a field called title 
and field, publication year and a field author. And let's say you want to rename 
one of the fields, you want to call it, author, because that's how you need to 
send it over the wire for some reason, what are you going to do? Create a new 
type, exactly like the first type. So it's going to be called Book Two, which is 
exactly a book, but just the field also is called the book author. Usually there 
is a profusion, a profusion of types. And yeah, each little module that needs to 
have a different look at the same data or very similar data will create its own 
type. That's the kind of complexity I'm referring to. There are types that are 
intertwined with different things, different glasses to look at the same 
reality. Another example, let's say you have two modules that have the same type 
with the exact same field, but one type belongs to one module, and one type 
belongs to another module. Now you have one by module, a one by module b with 
the exact same field. If you compare them, the language will tell you it's not 
the same, two different type instance. But the fields are the same. So it's two 
glasses, that look like the exact same reality. So instead of comparing reality, 
you compare your glasses.


**Dr. McKayla**   17:53 Yeah, I think I probably would need a very concrete 
example to see the different instances of how or when I encountered those 
problems. But I see where you are heading towards. So what are the programs that 
you wrote, or the products that they created, where all of those challenges that 
you describe have been so predominant, that data oriented-programming really 
made sense? And how did you switch from, you know, like, probably had like 
already a codebase? So how do we go from that codebase that we have to a 
data-oriented code base? What steps do we need here?


**Yehonathan Sharvit**   18:20 Yeah, if you take a look at the book, you will 
see that basically, data-oriented programming is made of four core principles. 
You don't have to apply all of them, you can apply principle number one of 
data-oriented programming, and change your code base according only to this 
principle. So for example, you will take a class that combines code and data and 
split it into two classes: one for the code, one for the data, and it will be 
already... It will have beneficial impact, if will lower the complexity of your 
class diagram. After that, you can say okay, this piece of data, maybe I can 
represent it as a HashMap. Instead of creating my custom type, and see if it 
makes sense, maybe something that you need to send over the wire as JSON, 
instead of creating a custom type and then a custom JSON serializer take a look 
and say, Okay, this, it will make sense to leave it as a HashMap. And then you 
get the serialization JSON for free. Then the third principle, you can play with 
schema languages like JSON schema, and see how it looks like to define the 
schema of your API, defining the rules inside your classes. And then for 
example, you have a REST endpoint that expects a payload with a specific shape. 
You define the payload of the request... JSON schema, and you validate that the 
requests that you receive correspond to the schema. And finally, the last 
principle, you can avoid mutation and instead of mutating in place you try to 
create when it makes sense a new version of data and see if it helps in terms of 
state management.


**Dr. McKayla**   20:03 But it also means that it plays nicely together we can 
have an object-oriented or functional programming environment or system and then 
add...


**Yehonathan Sharvit**   20:12 Yes.


**Dr. McKayla**   20:13 Parts that are benefiting from the data-oriented 
paradigm and transfer that into that?


**Yehonathan Sharvit**   20:20 You could have an object-oriented programming 
style or language, embracing the data-oriented programming paradigm.


**Dr. McKayla**   20:28 Okay, but it can still live together, right? So I can 
have like a large part of my codebase has objects and works in an 
object-oriented way. And as you said, Maybe I'm taking just parts of some of 
those objects and separate data from logic and so on. But the rest will still be 
very OO, right? Object-oriented.


**Yehonathan Sharvit**   20:48 Yes. And that will be the advice I would give to 
someone, not to adopt the will directly but to try when it makes sense. And if 
you... it's a place where you're really scared, let's say if you don't have your 
types, it's fine. Don't start from this place.


**Dr. McKayla**   21:01 Okay. Another question that I had for you is that I 
wanted to say data-intensive application. And in our pre-recording session, you 
said no, no, don't say data-intensive application, say, information systems. 
Why? What's the difference for you here? I think I grasp it now a little bit. 
But I think probably it has to do that it doesn't have to be data-intensive. You 
can just have normal data usage. But why do you prefer information systems and 
not data-intensive applications?


**Yehonathan Sharvit**   21:32 Yeah, that's a great question. When I hear the 
word information, it's clear to me that it's something that exists outside my 
program. information could be in a database information could be in a program, 
it could be in a file, it could be in the real world. And when you say 
data-intensive application, to me, it sounds like something at scale with lots 
of data, lots of traffic, that has nothing to say about how to manage data at 
scale, it has to say how to represent data in a simple way.


**Dr. McKayla**   22:03 Okay. Yeah. I mean, a lot of systems have databases at 
least, right? Like they are probably applications that don't have a lot of 
information. They don't need a database, but I don't know many...


**Yehonathan Sharvit**   22:15 I mean, they need a database. But what I mean, is 
that the scale doesn't have to be... the throughput doesn't have to be big.


**Dr. McKayla**   22:22 I understand. Yeah. So actually, every application that 
has or deals with data and information that stores it, somehow retrieves it 
somehow, transforms it, it would be interested to look at data-oriented 
programming, in your mind, or are there some specific kinds of applications that 
you would say benefit more?


**Yehonathan Sharvit**   22:40 Any application that is in the stack of what we 
call full-stack development, front-end, back-end worker will be... it will 
benefit. I think where it doesn't make any difference with.... it won't benefit. 
If you want to write a compiler, or to write a game engine, or something that 
lives in a closed ecosystem, where you have no surprises. If your data never 
surprises you. And you don't need to send it to other, you don't need 
data-oriented programming.


**Dr. McKayla**   23:09 Yeah, I like that. That's very clear.


**Yehonathan Sharvit**   23:11 If you communicate with data to different systems 
that use different programming languages, then it makes sense.


**Dr. McKayla**   23:18 Okay, so the last question I have for you is about the 
style of the book, actually. So your book is actually written a little bit 
differently. It's a story, right? It's a story and the whole information, the 
learning experience is actually guided through personas, characters that are 
doing something, why did you choose to write the book that way? Which is very 
different from other technical books?


**Yehonathan Sharvit**   23:43 Yeah. So there are several reasons. One of them 
is that I like story. And I need to admit, it's difficult for me to read 
technical books. It's very difficult, I get bored, or I fall asleep. And when I 
read the story, I'm entertained, I'm energized. So I wanted to invent a story. 
But it's tricky to make a story in the context of technical material, but I 
wanted to. I had this idea in the back of my mind. And then when I wrote the 
first chapter, as a regular chapter, I struggled with finding the proper tone. I 
was either too enthusiastic and too selling or too boring. I didn't know how to 
deal with the objections that I know the readers will have. So I played a little 
game between me and myself, part of me that played the data with the programming 
mentor, and other parts of myself that would play the developer. I made little 
discussions between them. So the mentor would say, types are problematic. And 
the developer say, but, why? I like types. It brings me safety. Uh huh. And then 
he challenges m,e then I need him to answer his question.


**Dr. McKayla**   24:54 Oh, that's what you did with me today.


**Yehonathan Sharvit**   24:56 Yes, yes, exactly. I was already prepared. And 
sometimes, I felt like kind of schizophrenic. Like I have two personalities. But 
for me, it was the best way I found to deal with questions. And many readers 
told me that quite often when they read the book, in their mind, they see the 
character as the question just the moment the question arises in the mind. So 
that's how I decided to make dialogues between the character and others. Okay, 
now I have the dialogue with, they're going to talk forever with no context? So 
sometimes I put them in the coffee shop, and sometimes in the university and 
sometime in the office at some time in the park, and sometimes in the 
countryside. And then I made a little story around the character and their 
journey toward enlightenment.


**Dr. McKayla**   25:45Yeah. And so Manning, right, this is a Manning book, 
right? Manning has this pre-access, early access thing. Yeah. And you have 
people that actually read already your book, and you're getting feedback. Do 
they like this kind of new style? Are they surprised? 


**Yehonathan Sharvit**   26:01 I think they're surprised and they like it, and 
they comment on it. And they provide very useful feedback on it allows me to 
improve the book, while I'm writing, I also have a reader from... As you may 
have guessed, I'm not a native American speaker. I was born in France. And I 
have a friend in Boston, I think, that liked the book and offered me to review 
the whole book, and reformulate it in proper English. 


**Dr. McKayla**   26:26 Oh, nice. That's very good. 


**Yehonathan Sharvit**   26:27 We had two weeks of fun together, we sent him the 
chapters, and it will send me reviews and comments. And it move dbeyond only 
correcting the English. He suggested little changes to the story, to the setup, 
to the characters. That was one of my best experience, my best interaction with 
readers, that they actually participated in the book, they contributed in the 
book. Is that open source, it's like an open-source book, in a sense. A 
collaborative book.


**Dr. McKayla**   26:54 Very nice, yeah. And so this actually brings me to the 
end of our episode, and I want to remind our listeners that they can win a book, 
you are giving away one copy. They have to retweet and like this episode to have 
this chance. And then in a week, 10 days later, I will, you know, raffle and 
pick one lucky person that can read the whole story and find out where the 
characters are around and how they're discussing the pros and cons of 
data-oriented programming. So Yehonathan, thank you so much for being at my 
show. It was really a pleasure to talk to you. And yeah, thank you so much.


**Yehonathan Sharvit**   27:32 Thank you, McKayla.


**Dr. McKayla**   27:33 This was another episode of the Software Engineering 
Unlocked podcast. If you enjoyed the episode, please help me spread the word 
about the podcast, send the episode to a friend via email, Twitter, LinkedIn, 
well, whatever messaging system you use. Or give it a positive review on your 
favorite podcasting platforms such as Spotify or iTunes. This would mean really 
a lot to me. So thank you for listening. Don't forget to subscribe and I will 
talk to you in two weeks. Bye.
