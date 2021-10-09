---
title: Programming Paradigms 
date: 2021-07-27T12:00:06+09:00
description: Paradigms are essentially the method in which we instruct our machines to perform instructions and solve problems
draft: false
hideToc: false
enableToc: true
enableTocContent: false
author : "Calil Drissi"
authorImage: /images/whoami/author-3.jpg
categories:
- Software Engineering
image: images/feature1/paradigm.svg
---

![paradigm](/images/feature2/Programming-Paradigms.png "paradigm")

Paradigm can also be termed as method to solve some problem or do some task. Programming paradigm is an approach to solve problem using some programming language or also we can say it is a method to solve a problem using tools and techniques that are available to us following some approach. There are lots for programming language that are known but all of them need to follow some strategy when they are implemented and this methodology/strategy is paradigms. Apart from varieties of programming language there are lots of paradigms to fulfil each and every demand. 

Paradigm is a school of thought or model that has distinct features, frameworks, patterns, and style which help you solve a particular problem. Paradigms are used in all fields such as psychology, sociology, etymology, computer science and so on. In the field of computer science, new programming languages emerge from existing languages and add, remove and combine features in a new way. The languages may follow a particular paradigm or can be a combination of many paradigms. Did you know that there are 256 programming languages? It is evident that each of them has evolved from the other with an amalgamation of various programming paradigms.

Programming languages are tools and not all tools are good for all jobs. Some tasks are easier to solve functionally. Some are clearly suited for Objected Oriented programming. Others get simpler when you use constraint solving or pattern matching.


## Imperative Programming

**Imperative Programming** expresses commands for the computer to perform - it is focused on the explicit process of how a program operates. For example, if you wanted to get the even numbers of an array, here’s what imperative code might look like:

### Procedural Programming
This language deals with procedure calls, which are also known as routines or functions. These contain a series of computational commands to be carried out to achieve a certain outcome. It is essentially like a recipe, with a list of step-by-step instructions for the computer program to follow. The code can easily be reused in different parts of the program. One benefit of this is that the code can be easy to learn and read in simple programs, though when dealing with something more complex you run the risk of ending up with a huge volume of code.

Examples: C, Pascal, BASIC.

### Object Oriented Programming
This paradigm is based on the idea that code can be broken down into ‘objects’ that have different properties and perform different actions. Objects can interact with each other to achieve desired outcomes. A core principle of OOP is ‘encapsulation’, which involves wrapping all the object components (i.e. data and methods) into a single, self-sustaining unit (sometimes known as a ‘class’). OOP is a popular paradigm as it mimics our ‘real world’ view of objects, making it relatively simple to grasp. Due to encapsulation, objects/classes can be reused easily, while it is also scalable and secure.

Examples: C++, Java, Python.


### Parallel Processing

The basic idea behind this paradigm is to break up different parts of a task among multiple processors, which simultaneously work on a problem. It’s like having someone make a sauce while you prepare the pizza base - you reduce the time it takes to complete the whole task. With a computer, this implies connecting multiple processors to memory, which is either pooled across all processors or distributed over a network. As such, this typically requires software and hardware resources. A number of programming languages can support parallel processing.

Examples: C, C++, MPI, NESL

## Declarative Programming

 **Declarative Programming** is higher-level, focused on logic and concepts rather than procedural flow. In other words, it is concerned with what needs to be done rather than exactly how it should be done. Using the same example as before, this is how declarative programming would solve the problem:


### Logic 
This programming is based on the notion of formal logic. Programs are written as a series of facts and rules that follow a logical structure (e.g. ‘X is true if Y and Z are true’). This logic serves as a knowledge framework through which computers can produce certain results - rather than being told explicitly what to do, a computer is given the boundaries for what it should be considering. Logic programming is primarily declarative as machines can use reason to solve a problem, though in some cases imperative commands can also be included in the code. Logic programming can be used for research and testing complex theorems - it is also closely connected to development of machine learning and artificial intelligence. Key benefits include flexibility and minimalist syntax. However, it can be confusing if the logical rules are not expressed well. 

Examples: Prolog, Datalog, Mercury.
### Functional 
As the name suggests, this paradigm is based on the execution of a series of mathematical functions, which form the building blocks of the program and perform all manner of tasks. These languages avoid flow controls like loops and instead favor recursive functions. This paradigm reduces code complexity and can be used to solve complex problems. However, it can be difficult to learn and tricky to scale for larger projects. As with the logic paradigm, some functional programming languages can also support imperative style programming if required. 

Examples: JavaScript, Haskell, Scala.

### Database Processing

This programming methodology is based on data and its movement. Program statements are defined by data rather than hard-coding a series of steps.

A database is an organized collection of structured information, or data, typically stored electronically in a computer system. A database is usually controlled by a database management system (DBMS) ("What is a Database", Oracle, 2019).

To process the data and querying them, databases use tables. Data can then be easily accessed, managed, modified, updated, controlled and organized.

A good database processing approach is crucial to any company or organization. This is because the database stores all the pertinent details about the company such as employee records, transaction records and salary details.

Most databases use Structured Query Language (SQL) for writing and querying data.


## Conclusion

As with many things in software development, there is no objectively ‘right’ or ‘best’ programming paradigm. It all depends on what you need to do, what resources you have available, and who else is working on the project. Often, you’ll find that blending some declarative and imperative programming, which as we’ve seen is supported by some languages, is the optimal solution. 
