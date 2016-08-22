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
They are another type test that allow you to characterize what the system is doing. Also they shouldn't be seen as a replacement for unit tests. Rather it gives you your initial safety net. 

For the golden master section we used an [approvals test suite](http://approvaltests.sourceforge.net/). This library will tell you that something has changed, it won't tell you whether it's correct that it changed. But it will inform you.

Next we started unit testing. The rules for the exercise was when a class/feature was 100% unit tested, then we could refactor it. Until we reached that point we could only use automatic refactorings from the IDE. We used code coverage a lot during unit testing. It's very useful to use code coverage when refactoring legacy code.
Not necessairly so that you can hit a percentage. More to ensure that the section of code you had intended on testing was indeed tested by the unit test. 
We learned when testing, it is important to test from the shortest branch to the deepest branch. Otherwise there is too much setup in your tests.
We introduced seams for helping us break the singleton/static dependencies in our sample program. 

During refactoring steps for the evening we tackled issues like feature envy, violations of single responsibility princple and many more.

We tried to leverage baby steps throughout. This is a technique that works really well with legacy code. You are working on a system that you are not familiar with. Mistakes can come out from any small change. You would not like to be in the situation where some tests stop passing and you do not know what you did.

As with a lot of the hands on sessions the evening was up a little too soon. Maybe a full day legacy retreat is in store for running a session like this again. 

The exercises that we worked through during the evening can be found here:

[Legacy code github repository](https://github.com/dubswcraft/handson-legacy)
 
Unfortunately we totally forgot to take any photos of the evening

Some other useful links for delving into golden master and simple design:

[Legacy Code Retreat](http://blog.adrianbolboaca.ro/2014/04/legacy-coderetreat/) by Adrian Bolboaca

[Testing legacy code with Golden Master](http://craftedsw.blogspot.ie/2012/11/testing-legacy-code-with-golden-master.html) by Sandro Mancuso
 
[Using the Golden Master technique to Test Legacy Code](https://chrismelinn.wordpress.com/2013/04/12/using-the-golden-master-technique-to-test-legacy-code/) by Chris Melinn

[The Four Elements of Simple Design](http://blog.jbrains.ca/permalink/the-four-elements-of-simple-design) by J.B. Rainsberger
 
Special thanks again to Barry Alistair in Techmeetup.space for providing the excellent venue. Thanks also to Gerry from Stack & Co for sponsoring the craft beers for the evening.
 
-Paul/Joe
