---
title: Setting Up Your Development Environment
description: 'Before learning Python, you need to set up some tools.'
---

## The Python Programming Language

### The Course
Welcome! This course was written with the intent of helping cadets of the
[Civil Air Patrol (CAP)](https://gocivilairpatrol.com) with no programming
experience gain the knowledge necessary to contribute to the Col John W.
Barainca Spaceflight Simulation Project. There isn't anything CAP-specific
about this course, though, so it should be useful and accessible to non-CAP
cadets.

There are many Python tutorials and "learn to code" courses out there. I'm not
so conceited as to claim that this tutorial is better than others. In fact, I
would encourage you to check some of them out (Someday, I'll put together a
list). One of the major gripes that have with these courses is that&mdash;in my
opinion (you'll learn all about "opinions" in this course)&mdash;they do a
fantastic job of teaching you a programming language, but they don't really
teach you how to *program.*

My goal is to not only get you familiar with how Python works, but also to help
you become literate in the techniques and strategies that developers in the
industry employ to solve problems. The focus will be on the problems we face on
the Barainca Project since it's hard to talk about problem solving when you
don't have an example problem to work. The principles, however, are the
important thing.

### Who Am I?
If you're not one of the cadets that I personally duped into working on the
project, you're probably wondering who I am. My name is Robert Hawk, I'm a
Captain in the Civil Air Patrol which is pretty much where I spend most of my
free time. My paid job, however, is as a Software Engineer (CAP is a volunteer
organization, in case you're not familiar with it). For close to a decade, I
have used Python professionally for applications ranging from controlling
telescopes and reducing astronomical data to managing payment systems. So,
while I won't pretend to be a genius, I do feel somewhat qualified to opine on
the subject.

### What is Python?
At its most basic level, a computer is a machine. The earliest computers were
machines of gears and levers that&mdash;when the levers were pushed/pulled in
certain ways&mdash;the machine would act in ways that simulate mathematical
operations. Modern computers do pretty much the same thing, only we use
electrical voltages instead of gears and levers.

Exactly how we are able to build these machines is a fascinating topic which,
if you're interested, you can learn about
[here](https://the-hawk.us/courses/how_computers_work) (dead link right now,
still getting content moved over). However, having to figure out which buttons
need to be pushed and when gets very tedious very fast. This is why, in the
early 1950s, Rear Admiral Grace Hopper (she was a Lieutenant Commander at the
time) envisioned a way to "&hellip; to be able to write programs in English,
and the computers would translate them into machine code." She went on to
invent FLOW-MATIC, the first "high-level"[^1] programming language.

Python came about four decades later, when it was developed by Dutch computer
scientist Guido van Rossum. Van Rossum wanted a language that was easy for
developers to read and straightforward to write (not the easiest thing to
accomplish, as you will discover over the course of this journey). Unlike
FLOW-MATIC (and it's immediate successor COBOL), instead of having to translate
the program to "machine language" (the instructions the computer actually
understands), Python ships with an interpreter that can compile and run the
program on the fly. This makes it easier to write code once and have it run on
multiple platforms (such as Windows, Mac, Linux, etc.) The language was named
for *Monty Python's Flying Circus*. (Don't be surprised if you see Monty Python
references littered through the official language documentation.)

### Why Python?
Despite being a professional Python developer (at the moment), Python isn't the
only language I know. It isn't even my favorite language. So, why did I chose
Python as the language for the Basic and Intermediate courses? There are a few
reasons for this. As programming languages go, Python is very simple while
being very powerful and it enforces certain good habits in the syntax itself.
That, alone, is enough for me to recommend it as a first language for
beginners, but it also tops the Institute for Electrical and Electronic
Engineers (IEEE) list of most popular programming languages and is more or less
the only choice in some programming domains (especially data science and
scientific computing).[^2] In the 21st Century, Python is a good thing to know
even if you don't plan on becoming a professional software developer.

## The Python Interpreter
Before you begin developing in Python, there are some tools that you will need
on your computer. The first of these is the Python Interpreter itself.
