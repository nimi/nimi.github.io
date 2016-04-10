---
layout: post
title:  "Thoughts on Codemash 2016"
date:   2016-01-14 09:20:42 -0500
categories: conferences
---
I've never been much of a "blogger", but I figured I'd give it a shot in 2016 as a way to reflect on my own learnings as well as share my experiences/thoughts/ideas (both good and bad) for anyone who might care and perhaps inspire some similar learning or inspire further reading or discovery. And as an inaugural post, I thought I'd share my thoughts and experiences attending the Codemash tech conference (and for those unfamiliar with Codemash, check it out [here](https://twitter.com/codemash).

 This was my first year attending the Codemash, and the presentation lineup was something that I've been really excited about since I read through the list. The range of topics was both large and diverse, just a sampling included talks on C#, Sprint Retrospectives, Deep Learning, Angular 2, and Application Security. This conference seemed to have mass appeal in each corner of the technology field. It would be easy to find a 'track' to follow that aligns with your area of expertise. And in the past, I've made the mistake of attending talks that are too similar and/or too closely aligned to technologies that I use on a day-to-day basis. I wanted to approach things differently with Codemash especially given the wide-range of topics.  I made it my goal to attend talks on topics that were outside my domain, and I found this to be extremely valuable. Below you can find some notes and reflection on some of my favorite talks.

### OO Programming w/ Smalltalk

For those of you that aren't familiar with Smalltalk, Smalltalk is a highly influential OO Language developed by Alan Kay and others in the 1970s.  Many of the ideas in Smalltalk can be seen applied in Ruby, Python, Java, etc. The presenter, Larry Stanton Jr., offered great historical perspective on how Kay's biology degree influenced some of the language concepts and design as well as insight into Smalltalk's impact on OO design patterns. Smalltalk was designed around the idea of messaging. Objects in Smalltalk hold all of their state privately and communicate with other objects via its messaging system. This robust messaging allowed later implementations to structure objects in an MVC way ([This is great article](http://peter.michaux.ca/articles/smalltalk-mvc-translated-to-javascript) discusses using Smalltalk MVC designs to help write better MVC JavaScript).

Another really cool thing about Smalltalk that's been carried over to other other languages, like Ruby, is that everything is an Object including primitives AND you can change or extend any implementation of these primitives as well as any other class implementation. This can be dangerous, but also powerful due to the fact that Smalltalk programs each exist in a unique image.

Despite it's age, Smalltalk is still a really powerful language that we can learn from even if we don't program with Smalltalk. The Smalltalk-80 book is excellent weekend reading. You can read it for free [here](http://stephane.ducasse.free.fr/FreeBooks/BlueBook/Bluebook.pdf).


### Machine Learning w/ Music

This was a great talk by data scientist, Ali Kheyrollahi on how Machine Learning was used to find out some really interesting things about music and music history. Kheyrollahi scraped a significant amount of data on musicians throughout the last century from Wikipedia to find out and visualize the relationships that exist among the many different artists. The results were fascinating, for example, there was an observed decline in rock music starting around 2000 (Of course, there is plenty of speculation as to why that may be) My takeaway, though, and the main point of the talk was on how we can use models to learn more from our data. Kheyrollahi explains his definition of a simple visionary model to understanding which artists had the most influence on other artists. As we attempt to provide useful data visualizations, we should look to already-defined or defining new data-models to gain more insight into the story behind raw data.


### The Future is Immutable

John Daily made a great case for looking to immutable data to solve and/or aide in the challenges with storing and modifying data. The lesson here is that you should never mutate or modify existing data. If you need to update it, you should copy part of your graph or tree and add that as a new piece of data. There are drawbacks to using immutable data, such as the fact that multiple clients reading a data store may not be synced.

There are tradeoffs to be had, definitely, but I believe immutable data is the way to go in most cases to keep data sane and safe. Daily spoke about immutable data in the context of data storage in databases, especially in distributed systems. However, understanding is very important to understand for application development. Many languages provide immutable data by default such as Clojure and Rust to ensure better data safety. It's not limited to backend languages as we can use libraries to assist in data safety and app performance when we handle important client data. In JavaScript, [immutablejs](https://github.com/facebook/immutable-js) and [seamless-js](https://github.com/rtfeldman/seamless-immutable) can assist us in safely storing application data and state while reducing bugs and in some cases improving app performance.


### Well Behaved Elixir

This was my favorite talk Codemash. Despite, the talk being aimed at the functional Elixir language, Chris Keathley spoke more generally about Type safety. He made a strong argument on how and why we should use statically typed languages and tools. He provided examples on how type safe languages aide in detecting bugs and ensuring app data is consistent. Overall, though he argues that types help us write better software. Types are obviously a major part of many languages already.  But this is an issue that I've thought about quite a lot lately in the context of JavaScript. I've been split on the issue of static typing add complexity to initial setup. Compiled languages like TypeScript and Elm offer static typing by default. While libraries like Facebook's Flow are allowing JavaScript developers the option to add static typing to their applications without any additional compilation. After Keathley's talk, I feel much more inclined to begin a project with types in mind as it seems to substantially improve code quality and prevents common and hard to detect bugs in the language.


### Art and Code: Make useless things

This was a really fun and silly talk on how you should build things that are useless. I wanted to mention because I totally agree with the presenter. We should all spend some time building things that may not seem all that useful and are fun. Many times building useless things help us to break up monotony, it helps us learn new technologies and may in fact be useful for someone else, even as a form of entertainment. As per the title of the talk, make useless things!


### Conclusion

Overall, it was a great conference. It seems functional programming, machine learning and immutable data are areas that are having a pretty large impact in software development right now. I'd recommend looking into those areas as we move into 2016. I would also definitely recommend you attend next year if they have the opportunity. For more info, check out Codemash on [twitter](https://twitter.com/codemash) or their [site](http://www.codemash.org/) for the latest updates.
