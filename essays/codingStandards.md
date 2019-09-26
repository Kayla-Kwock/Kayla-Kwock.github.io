---
layout: essay
type: essay
title: Coding Conformity
# All dates must be YYYY-MM-DD format!
date: 2019-09-25
labels:
  - Coding Standards
  - Learning Code
---

# An (Unfortunately) Normal Situation
When you start off a coding project, your main concern is most likely trying to make sure that your the compiler doesn't complain. Once you finish the project, the next goal is most likely to clean up and add some comments in to the absolute mess of spaghetti code you just wrote. But where to even start? How do you begin to unify your code so that not only is it easy, but enjoyable to read? You could try yourself to come up with a consistent style, but it's difficult to remember every little detail, whitespace and variable naming convention. On top of that, what might seem logical convention to you might be completely confusing to someone else. Enter Coding Standards: your new best friend or worst enemy. 

## Laying the Law
Coding standards (AKA Coding Guidelines, Style Guide, etc.) are a set of standardized conventions that one follows while coding in the appropriate language, with the goal of increasing code readability which helps in maintenance and debugging. These standards define a wide variety of things from how to name functions and variables to how much whitespace to put. For example, in Python's PEP8 style guide, they suggest naming variables in a `camelCase` format and functions `using_underscores()` and also suggests using multiple lines of whitespace depending on the situation. Overall these rules are created such that the code written in the same standard are virtually indistinguishable from one another.

## Order from Chaos
As for my personal take on it, standards are a necessary evil to keep the world sane. Imagine you've just picked up a project halfway through the development cycle and you're trying to figure out what's going on, but you're hopelessly sifting through lines of code trying to decipher the mess. This could all be avoided if they had used a Coding Standard such as ESLint. However, it can be quite a hassle trying to follow each and every niche and seemingly small rule, even with IDEA helping you by providing familiar squiggles for warnings. As mentioned before, annoying but necessary.

## A Little Formatting: A Lifetime of Understanding
It may seem like the conventions and rules defined by a Coding Standard to be arbitrary; and you'd be right. These rules aren't required; your code will still compile regardless of how much whitespace you put in. But the most important thing to keep in mind is that this ruleset is agreed upon to be the way that code should be written. Like in English, if someone said 'fighted' for the past-tense of 'fight' you would most likely understand what they are talking about, but it just doesn't sound right. Trying to learn a new coding language is like learning English; there seem to be set rules, but with so many exceptions to them it's hard to know what applies when. If we were able to reduce the number of exceptions in the English language, it would be much easier for someone to learn, much like if we were to remove the variation in coding by following a Coding Standard, it would be much easier to learn, read and understand. 
