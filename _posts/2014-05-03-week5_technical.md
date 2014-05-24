---
layout: post
title: Classes and Objects
date: May 3, 2014
category: code
customid: week5technicalblog
---
Ruby is an object orientated programming language, what this means is that whenever you are creating an instance of a class, you are creating an object. Objects are often used to model the real-world objects that you find in everyday life. How we used these objects is through the manipulations with the use of messages.

Classes are used to give a name to reference its behaviors or functionalities. So that when we want to created an object of that class, and be able to make use of all of functions and behaviors associated with that class.

For the most part classes is just a collection of methods. The purpose of creating classes is so that you can create objects that are instances of the class. Classes respond to messages, which are generally whatever left of the dot. You can define a using the class keyword.

You can write your own classes, modify existing classes and add in new behaviors or functionalities. So once you create a new object, which is an instance of the class, the object adopts characteristics of that class. Classes can inherit properties from one other class. To illustrate this example, the class humans can gain inheritance from a class like mammals. So humans in this case, would not only have the properties of humans but of mammals as well. In Ruby, however one class can only inherit from one class other class, so you have to choose wisely what class you want your class to inherit from.

All Ruby objects have a set of instance variables. These instance variables are assigned when you create the object or whenever you assign them. The object's class does not define them. Once these instance variables are created, you can call upon them at anytime.
