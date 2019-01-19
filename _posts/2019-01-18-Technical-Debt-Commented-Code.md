---
layout: post
title: "Code Bite 🍽: Technical Debt - Commented out code"
date: 2019-01-18 22:47:00
image: '/assets/img/'
description: 'For beginners: delete unnecessary comments'
tags:
- Code Bite
- styling
- beginner
categories:
- Code Bite
---

# Code Bite 🍽: Technical Debt - Commented out code

Code should be maintainable and readable.  Writing elegant code is like writing an essay.  Anyone fluent in the language should be able to read it with ease.  In the same way we don't want run on sentences or too many commas in a sentence, we also should avoid writing code that could be distracting to the code's intent.  Code that functions correctly, but is not clean is called `Technical Debt`.  Even if you are writing code solo and you are the only intended audience to read it, readable code is a long term investment when you revisit your code base a month or a year from now.

New developer can fall into the trap of commenting out code too frequently.  Yes, commenting out code quickly gets rid of code that should not be run, but leaving commented code can pollute your work space.  Each and every line of code should serve a purpose in functionality and understanding.  It is not uncommon to find a snippet like this in your code base if you are not careful:

```swift
class MyClass {

  // var myInt = 0
  var myInt = 3

}
```

The commented out code serves no purpose - nothing depends on it.  Would we lose anything if this was taken out?  If not, trash it.  The biggest problem with technical debt is when collaborating with multiple team members.  Assuming master has been thoroughly reviewed and finalized for production, each line is necessary for the success of this program.  The last thing I want is to break someone else's code. I would have to understand why this code was commented out before deleting it.  Unfortunately this results in more headaches for everyone 😥.  Please be extra cautious when merging into master!

Straight to the point, the class should look like this:

```swift
class MyClass {

  var myInt = 3

}
```

When I started to code in college, I used comments in a heartbeat using the hotkeys.  For the most part I was inpatient and I just wanted the tests to pass so I could sleep!  Don't worry the longterm investment is worth the immediate struggle.

## Call to Action

- Read your code aloud, does it make sense?  Could someone new to the code base understand what is going on?
- Skim through your code base.  If there is commented code, ask yourself, "Is this code absolutely necessary for it to function".

I hope you learned a bit more to write more readable code!
