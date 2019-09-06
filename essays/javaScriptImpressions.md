---
layout: essay
type: essay
title: JavaScript, Both Blessing and Curse
# All dates must be YYYY-MM-DD format!
date: 2019-09-05
labels:
  - JavaScript
  - First Impressions
---

# A First Look Into JavaScript

Throughout all of my college career, the thing I believe I've become most adept at is coding. Whether it be for a class, job, or own personal enrichment, it's a skill that's a very important part of what makes me who I am today. It first started with C, a nice, simple and fairly straight forward language to learn. Next came C++, my first venture into the world of Object-Oriented programming. Since then, I've picked up RobotC, SystemVerilog, and Python. Now comes JavaScript, a language that seemed daunting at first but is much easier than I expected!

## How Does JavaScript Stack Up?

### Versus Python
JavaScript has a similar learning curve to Python, if not a bit harder. They're both scripting languages and both are fairly high level, with a bunch of included data types and methods to manipulate them. The only reason I say JavaScript is harder is due to the fact that Python can essentially be completely written in English while JavaScript requires syntax markers to work like curly braces and semicolons. For example, a Python `for()` loop would look something like this...

---
```
for(i in range(100))
    #do stuff
```
---
Contrast this to JavaScript...

---
```
for(let i = 0; i < 100; i++){
  //do stuff
}
```
---

Both of these loops accomplish the same task of iterating 100 times. However, I would argue that the Python representation is much more user friendly. It's all written in what is essentially plain English aside from the `range(100)`. In contrast to the JavaScript, where everything is covered in syntax markers. Python here is the odd one out however, as many other languages use the exact same syntax as JavaScript, like C and C++.

### Versus C

I would say that of all my languages, JavaScript is most like C. Essentially *all* of the same syntax carries over, from `for()` loops, to `if - else` statements, to even `switch()` statements! Syntactically they're the same. The main differences to me are that C uses strict typing and JavaScript doesn't, C has access to pointers and references and JavaScript doesn't, and that JavaScript offers multiple data types by default like `strings` and data structures like `queues` and `stacks` while C doesn't even come with `Boolean`! Also, I really like the inclusion of _strictly equal to_ (`===`) in JavaScript as opposed to C, makes doing comparisons a whole lot easier.

### Versus C++

C++ is a very interesting case. It's like C syntactically, but is more like JavaScript when it comes to features. The main differentiator to me is the simplicity of declaring classes in C++ versus JavaScript. When I was learning JavaScript by using the online course offered by [FreeCodeCamp.com](https://learn.freecodecamp.org/), I was absolutely baffled when it came to declaring classes. It seemed so convoluted and difficult to understand. However, I'm assuming that with time this will get better.

### Versus RobotC/SystemVerilog
RobotC is essentially C, but specifically for programming VEX robots, so the use cases are completely different so I will not compare the two.

The same argument can be made for SystemVerilog: it's specifically made for coding firmware so I will not be comparing the two.

## The Mumble and Grumble

When it comes to programming, I expect a certain behavior from the language. If you're going to use a common keyword, it should behave the same. For example `for()` loops, `switch()` statements, and `print()` should all behave the same or at least similarly. However, JavaScript says that a variable declared with `const` is not constant, rather simply unassignable. Similarly, there is no `global` declaration, but there are global variables. I personally believe that using globals is something to avoided at all costs unless you know exactly what you're doing. These can create super difficult bugs to diagnose and with such a simple way of creating one in JavaScript, I wouldn't blame unaware coders to be frustrated. 

However, these two are simply annoyances that can be solved simply by either `freeze()` the variable or avoid using `var`. My most critical gripe with JavaScript is the lackluster error messages on interpretation. Every other language I've written in has had an error handler that would explain each and every problem that arose with the code. It doesn't solve the problem, but at least gives a simple way to look at every potential error. JavaScript on the other hand will simply stop interpreting upon finding a bug, and not going any further. Along with that, the error handler often times doesn't pinpoint the problem to what is actually wrong. For example, when this JavaScript snippet is compiled

---
```
for(let i = 0, i < 200; i++){
  function(i);
 }
 ```
 ---
 
The compiler incorrectly diagnoses the problem as redeclaring i as opposed to using a comma instead of a semi-colon. The compiler also fails to bring up the fact that `function()` is not defined. Maybe it's my development environment and using Chrome's inbuilt console as opposed to a dedicated IDE such as IntelliJ's IDEA. 

## JavaScript in the Workspace

Although I just bashed JavaScript, I do think JavaScript is a perfectly acceptable language to use. What it does, it does very well: web applications. I won't be switching to this as my main programming language, I still prefer C or Python to do any sort of program coding. But if I were to ever need to code a webpage, JavaScript would be my go to. You can make your code so compact and elegant that the amount of actual data you have to send over is miniscule 

## Athletic Coding: The Speedrun of Coding

In the gaming community, a _Speedrun_ is when a game is played with the sole purpose of completing it as fast as possible. For example, think of the original _Super Mario Bros._. With all the worlds and stages, running through them all normally would probably take an hour or two. However, people have managed to complete the entire game in under 5 minutes with the current record being 4:55.746! My personal favorite is _Super Mario 64_, where runners have managed to complete a typically 13-18 hour game in just 6:39.099! The reason people can perform these amazing feats is that they __know__ the game. They know exactly how each frame of the game is rendered and how the player interacts with each individual object, or teleport to a completely different location because you're going so fast that you cause a buffer overflow and are erroneously placed somewhere else on the map.

So how does this relate to coding? Well, with the introduction of WODs into the workflow, learning how to code efficiently is a must. For background, a WOD is a timed exercise in which you are given a problem and are timed on how long it takes you to develop and code the solution. In order to complete these WODs in a timely manner, one must know their tools inside and out. Like how a speedrunner needs to know every little detail to make the fastest run, a programmer should know what's at their disposal in order to quickly and effectively solve the problem. 

For me personally, it's a mixed bag on their actual use. I understand conceptually how and why this works, and I totally agree with the theory. However, I feel this situation is not representative of real world scenarios. Sure we're given a deadline for when our code is to be completed, however normally it's at least a week if not more. This gives me time to think about the problem carefully and make sure that my solution is both efficient and effective. But with only a few minutes, I don't have that luxury time to think and come back if I can't find a solution, I just need to plow on through which sometimes causes me to panic as I've not completely thought my solution through. This style of learning pretty much goes against every skill I've picked up as a developer, which is not necessarily a bad thing. But I don't think I would voluntarily choose to use this method of learning; it feels like a nice to have rather than a need to have.

## So What?
I have mixed feelings about JavaScript. It's really easy and simple to learn, but it's quirks and gimmicks are annoying and sometimes confusing. It's not and won't be my go-to programming language, but I can see how and where it has its uses. I feel that with time and practice, JavaScript will grow on me as I learn what I can and can't do with the language. But for now, I'd like to focus on making sure I know the basics before trying to cram everything into one line!
