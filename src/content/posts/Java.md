---
title: Java.md
published: 2024-04-19
description: ''
image: ''
tags: []
category: ''
draft: false 
---
# What is an Object?

> [!Note]
>
> A object is a software bundle of related states and behavior.

Objects share two characteristics: they all have state and behavior. Dogs have state (name, color, breed, hungry) and behavior (barking, fetching, wagging tail).  Identifying the state and behavior for real-world objects is a great way to begin thinking in terms of object-oriented programming.

![image-20240404092438434](https://raw.githubusercontent.com/satorussgojo/images/main/img/image-20240404092438434.png)

Software objects consist of state and related behavior. An object stores its state in *fields* (variables in some programming languages) and exposes its behavior through *methods* (functions in some programming languages).

Methods operate on an object's internal states and serve as the primary mechanism for object-to-object communication. 

> [!NOTE]
>
> Hiding internal state and requiring all interaction to be performed through an object's methods is known as *data encapsulation* —— a fundamental principle of object-oriented programming.



![image-20240404094427520](https://raw.githubusercontent.com/satorussgojo/images/main/img/image-20240404094427520.png)

> [!IMPORTANT]
>
> By attributing state (current speed, current pedal cadence, and current gear) and providing methods for changing that state, the object remain in control of how the outside world is allowed to use it.

For example, if the bicycle only has 6 gears, a method to change gears could reject any value that is less than 1 or greater that 6.



Bundling code into individual software objects provides a number of benefits, including:

1. Modularity: The source code for an object can be written and maintained independently of the source code for other objects. Once created, an object can be easily passed around inside the system.
2. Information-hiding: By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.
3. Code re-use: If an object already exist (perhaps written by another dev), you can use that object in your program. This allow specialists to implement/test/debug complex, task-specific objects, which you can then trust to run in your own code.
4. Pluggability and debugging ease: If a particular turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement.