---
layout: post
section-type: post
title: "Object Orientated Programming"
category: concepts
tags: [ 'analogies', 'programming' ]
---


Many concepts are inter-related and so it makes sense to look at the big picture.

### [Abstraction](http://en.wikipedia.org/wiki/Abstraction_(computer_science))

##### a concept or an idea 

There are layers of abstraction; each simplifying the idea by hiding details about underlying concepts. 

e.g. Vehicle is an abstraction for any object used to transport things. Beneath that layer of abstraction, you could use a palanquin (human driven) or carriage (horse driven) or motor car (fuel driven). 

In programming, a queue is an abstraction which can be implemented using arrays or linked lists. 

### [Interface](http://en.wikipedia.org/wiki/Interface_(computer_science))

##### describes a layer of abstraction

It is very closely related to abstraction and that causes the confusion. An interface specifies and defines some properties for a layer of abstraction.

e.g. An interface of a vehicle could be an object on which people can climb, sit and get transported to another location. Thus camels and elephants fit the interface for vehicles but a Jet pack doesn't.

The interface for a queue is an object which accepts a list of things and emits them in the same order. 
 
### [Polymorphism](http://en.wikipedia.org/wiki/Polymorphism_in_object-oriented_programming)

##### similar behavior of objects

Given a layer of abstraction and an interface, any object satisfying the interface can be used to complete the task. It is one of the building blocks of object oriented programming. 

e.g. Since a Magic carpet satisfies our interface for a vehicle, it can be used for transportation if it existed. 

A queue built using a Heap (data structure) would be the same as one built on arrays if the interface is followed. 

### [Inheritance](http://en.wikipedia.org/wiki/Inheritance_(object-oriented_programming))

##### passing on to children

Concepts built upon other ideas can be thought of as children of the original ideas. They include all the characteristics of the original idea and add some more functionality. 

e.g. 4-wheeler is a class of vehicles having exactly 4 wheels. It retains the concept of transporting things but adds a restriction of 4 wheels.

Priority queue is a type of queue but considers object priorities in addition to insertion order. 

### [Encapsulation](http://en.wikipedia.org/wiki/Encapsulation_(object-oriented_programming))

##### packaging and locking things

Packaging smaller components into a single entity so that their inner structure is hidden and safe from manipulation. 

e.g. Once a car is bundled together in a chassis, you don't know about the inner working i.e. it can be petrol or diesel or even CNG powered. And you get the security that it can only be started with a specific key. 

The ability to combine data and functions into a single entity, i.e. an object. The queue object should be able to add, retrieve and store things instead of having to access the underlying implementation of array or linked list. 

### [Is-a](http://en.wikipedia.org/wiki/Is-a) relationship

Signifies that an object satisfies a given interface. A child class satisfies all its parents interfaces in addition to its own. 

e.g. A car is a vehicle, so is a motorcycle. 

### [Has-a](http://en.wikipedia.org/wiki/Has-a) relationship

Signifies that an object contains another object. 

e.g. A car has a fuel tank and also an engine.


### Abstract type v/s Interface (Java)

A interface in Java is just a collection of properties and function signatures. It doesn't provide any implementation for its methods. For a class to satisfy the interface, it must implement (define) all the methods. 

An abstract class on the other hand is similar to an interface, but it can define some methods leaving out the rest. A sub-class must implement all the remaining methods for it to be instantiated.

e.g. An interface is like the specification for a car. It mentions what all properties and functions a car would have. 

An abstract class would be like a car without an engine. You can buy it but cannot use it until you fit an engine. The advantage is that it gives you the freedom to select any type of engine - petrol or diesel.

Note: Encryption isn't a part of OOP but an entirely different branch.
