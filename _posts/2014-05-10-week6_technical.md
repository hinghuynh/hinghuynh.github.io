---
layout: post
title: Functional Programming vs Objected-Orientated Programming
date: May 10, 2014
category: code
comments: true
customid: week6technicalblog
---
Functional Programming seems to break down programs into functions that perform some operations whereas in object-oriented programming, programs are broken into classes that give behavior to some kind of data input that class represents.

So to try and break this down into the simplest terms, it's basically comes down to how you want to organize code. Do you want to organize your code by functions where things that use the function would grouped together under the function. In this case you would use functional programming.

The alternative would be where you organize your code by things and put any function that the thing can do grouped with the thing. I would like replace thing with the term object and method for function in the case of Ruby. So the way you organize objects in ruby is through creating classes and inserting methods that you want the classes to do.

So for the most part, picking between functional programming and object-orientated program is just the preference of organization, however there are specific scenarios where one might be more beneficial than the other. Objected-oriented languages are good for when you have a fixed set of functions for things, and as time passes, there become more things that you want to add. You do this by adding new classes, while existing things remain the same. Functional languages are good for when you have already know all the things need for the program, and as time passes the only thing you want to change in the function and behaviors of things over time. You would create new functions that would manipulate existing things, while old functions stay the same. 