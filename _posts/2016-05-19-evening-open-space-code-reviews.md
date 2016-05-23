---
layout: post
title: "Evening Open Space - Lightening Talks, Code Reviews"
date: 2016-05-19 
summary: ""
published: true
categories: software craftsmanship
---
## Evening Open Space 19th May 2016

This month seen a return to the evening open space format where some excellent lightening talks kick off the night.

The lightening talks kicked off with Brian Matthews giving an overview of a maven plugin that he started some years back that can be used for integration tests that rely on an LDAP server. He gave some insights into how he handled dependency resolution dynamically.

![brian-matt.jpg](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/evening-open-space-19-may-2016/brian-matt.jpg)

Details here: [ldap-plugin](https://github.com/bmatthews68/ldap-maven-plugin)
 
Next up was Colin Graham giving a talk about his testing framework 'Contract'. Very extensible testing framework for tesing http clients and servers. If you have used wiremock, it is similar but more extensible.

![colin-graham.jpg](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/evening-open-space-19-may-2016/colin-graham.jpg)

Heres a link to the docs: [Contact Testing Framework](http://harmingcola.github.io/contract/)

Presentation slides: [Contract Slides](http://slides.com/harmingcola/contract#/)

Finally Joe Bentley finished off the evenings lightening talk with a brief intro to property based testing. If you have never heard of property based testing, it's typically one property-based test runs hundreds of times with different inputs. The testing framework will try to get the test to fail by passing empty lists, negative values, all the possible edges cases. It'll pass in long lists and high numbers and strings with special characters.

![joe-bentley.jpg](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/evening-open-space-19-may-2016/joe-bentley.jpg)

Presentation slides: [Property Based Testing](https://docs.google.com/presentation/d/1kArFu4WnUAGmLCzUHtWDw9pVMPJXR2-dEKjdiTGe6UY/pub?start=false&loop=false&delayms=3000)
 
The rest of the evening followed the ‘unconference’ format where we all voted on the following topics:
 
![vote-board.jpg](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/evening-open-space-19-may-2016/vote-board.jpg)

 ### Pairing/Code Reviews was the clean winner.                     

Really interesting discussion here. Opinions divided whether pairing should be done instead of code reviews.
Most agreed that pairing on it's own was quite silod and should have at least another opinion.
 
Code review key points:

Pros:

 - Tooling is great (gerrit, stash)
 - Everyone on the team keeps up to date with different areas of the source.

Cons:
 
 - too slow feedback, you have completed the block of work and send it for review.
 - Reviewer has no real context of work especially if he is looking at a large git diff. Would need to pull down the source.
 - BLocked while waiting for review

Other comments:

 - Sonar (findbugs, checkstyle etc) all very useful for linting but can't be used solely to ensure code quality.
 - Commits should follow the single responsibility principle and do one thing and act as documentation
 - Should fail a code review if a single commit contains too many changes.
 
Best case

 - Consensus that reviews should definitely be small and frequent.
 - A 'tech huddle/story kick off' or similar name should be started with a dev on the team who is most familiar with the area affected prior to starting on the story. Technical direction will be decided then. That way there should be no big surprises at the end of the story, changes should be cosmetic in review then.
 
Great discussion as always.
 
Other photos from the evening
![conversation.jpg](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/evening-open-space-19-may-2016/conversation.jpg)
![intro.jpeg](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/evening-open-space-19-may-2016/intro.jpeg)

Special thanks again to Barry Alistair in Techmeetup.space for providing the excellent venue. Also, thanks to Gerry from Stack and Co for sponsoring the craft beers for the evening.
![intro.jpeg](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/common/techmeetup-space.png)
![stackandco.png](https://raw.githubusercontent.com/dubswcraft/dubswcraft.github.io/master/_posts/images/common/stackandco.png)
