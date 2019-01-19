---
layout: post
title: "Code Bite 🍽: Capitalize Class Declarations"
date: 2019-01-18 21:37:00
image: '/assets/img/'
description: 'For beginners: styling your class'
tags:
- Code Bite
- styling
- beginner
categories:
- Code Bite
---

# Code Bite 🍽: Capitalize Class Declarations

Code should be written cleanly and with consistent style.  By following conventions of the language, it is easier to convey the code's intent and make it more readable for a reviewer.  A common mistake amongst new developers is missing on style nuances.  One in particular is the capitalization of classes. Capitalizing a class is universally accepted by coding languages to mean a class declaration.

```swift
class MyClass {
  var myVariable = nil
}
```

It is still possible to have a class declaration be lower case, but going against code conventions (especially code conventions across multiple languages) is not recommended.

```swift
class myClass {
  var myVariable = nil
}
```

I remember making this mistake even when I was just starting as a Junior Developer, unfortunately it lead to significant debugging session with a senior developer!  If you are currently maintaining a project, take a quick glance at your code and see if you are following the style recommended for your language.  More experienced developers can run linters that check your code style for you!  

## Call to Action

- Check out the style guide for your language.  Here is the raywenderlich [swift style guide](https://github.com/raywenderlich/swift-style-guide)
- Skim through your code base, are all your class declarations capitalized?

I hope you learned a little more about styling your code!
