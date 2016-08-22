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

For the golden master section we used an [approvals test suite](http://approvaltests.sourceforge.net/). This library will tell you that something has changed, it won't tell you whether it's correct that it changed. Maybe you fixed a typo for good reason. 

Next we started unit testing. The rules for the exercise was when a class/feature was 100% unit tested, then we could refactor it. 
We used code coverage for this. Not necessairly to hit a percentage. More to ensure that the section of code we had intended on testing was tested by the unit test. 
We learned when testing, it is important to test from the shortest branch to the deepest branch. Otherwise there is too much setup in your tests.
We introduced seams for helping us break the singleton/static dependencies in our sample program.

We learned that when testing legacy code, it is important to test from the shortest branch.
Remainder/Unit testing
 We are going to take the piece of existing code without tests and write tests for it
   ☐ Only automated refactorings are allowed till your code is covered by a test
   ☐ When it is 100% covered, then we can refactor it
   ☐ Look at trip service, started testing from the shortest branch - this is when a user is not logged in exception
 ☐ Introduce Seams
   ☐ The problem that we have is that this is a singleton, we can't inject it, we can't mock it.
   ☐ What can we do? We can only use automated refactorings
   ☐ We can create a seam - a seam is where the two classes meet, the UserSession and the TripService, what we do is isolate the bit that goes to the other class and that is our seam.
   ☐ We can create a private class that extends teh trip service
 ☐ Run your code coverage, make sure that the test that you have just written tests the short branch.
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
