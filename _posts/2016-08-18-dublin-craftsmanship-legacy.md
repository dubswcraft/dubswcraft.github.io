---
layout: post
title: "Hands On Session - Working with Legacy Code"
date: 2016-08-18 
summary: ""
published: true
categories: software craftsmanship
---
## Working with Legacy Code

This month was back to a hands on session for the Dublin Software Craftsmanship meetup group. This time we did a workshop on working effectively with legacy code. 

The exercise for the evening was to work with a bad piece of untested code. We started off by introducing the golden master. What is the Golden Master? 
Its a process that allows you to guard against unintended changes when working with legacy code. It protects against introducing bugs when you attempt to 'fix' behaviour.
They are another type test that allow you to characterize what the system is doing. 


Joe gave a great presentation that introduced the concepts of Functional Programming - [click here to download](https://www.dropbox.com/s/lxe54jvd5ydjjpa/Functional%20Programming.pdf?dl=0). The presentation was heavy on coding without any side effects, where a function does not rely on data outside the current function and dosen't change data that lives outside the current function.  After the presentation, It was onto the exercises. Throughout the evening we worked through 6 exercises in total. We got exposure to mapping, reducing, folding, recursing and the use of higher order functions. In short, we were trying to code without any side effects.
 
The exercises that we worked through during the evening can be found here:

[dubswcraft repo](https://github.com/dubswcraft/handson-legacy)
 
Unfortunately we totally forgot to take any photos of the evening

Some other useful links for delving into golden master and simple design:

[Legacy Code Retreat](http://blog.adrianbolboaca.ro/2014/04/legacy-coderetreat/) by Adrian Bolboaca

[Testing legacy code with Golden Master](http://craftedsw.blogspot.ie/2012/11/testing-legacy-code-with-golden-master.html) by Sandro Mancuso
 
[Using the Golden Master technique to Test Legacy Code](https://chrismelinn.wordpress.com/2013/04/12/using-the-golden-master-technique-to-test-legacy-code/) by Chris Melinn

[The Four Elements of Simple Design](http://blog.jbrains.ca/permalink/the-four-elements-of-simple-design) by J.B. Rainsberger
 
Special thanks again to Barry Alistair in Techmeetup.space for providing the excellent venue. Thanks also to Gerry from Stack & Co for sponsoring the craft beers for the evening.
 
-Paul/Joe
