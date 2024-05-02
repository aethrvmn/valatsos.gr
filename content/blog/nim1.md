---
title: 'Trying Nim: A low level journey'
date: 2024-05-01
draft: false
type: "post"
---

## The context

After 5 years of venturing into **Python**, I have decided that I want to delve into a lower level language.

**Python**'s strength is that it's easy to learn. There is no compile time vs runtime, no syntax sugar, no strongly typed vars, no static types.

It essentially allows anyone to learn data analytics, machine learning, computer vision and artificial intelligence, without needing to know either programming, or how any of this works under the hood.

In the spirit of learning something new every so often, I decided that it's time to leave my interpreted, dynamic, extremely slow comfort zone for something faster. Something compiled, that *can* be unsafe, but only when I want to learn how to shoot myself in the foot.

## The options

Looking at all the available options we have the good old **C**, and **C++**, and more modern options like **Rust**, **Go**, **Nim** and **Zig**.

First things first: I *do not* want to learn **C** or **C++** at this time in my life. I am just figuring out low level languages, and **C** and **C++** seem like they are out to get me. 

The main things that scare me are:

- No memory safety
- Weird syntax
- Unfriendly compiler and error messages

I do eventually hope to become a **C** wizard, maybe contributing to the Linux kernel, maybe doing my own thing, but for now **C** seems too daunting, and everyone with whom I've spoken to about **C++** suggests to never touch it, for I will never be able to understand the code of others, or of myself a few years down the line.

This leaves the rest of the options.

**Rust** is probably the most popular of the options, with cargo being probably the best packaging system, which completely evades whatever the hell Python is doing with its own system of pip, or conda, or poetry, or rye, or etc etc, and the versioning system. As a mostly solo dev, I havent had many experiences with dependency hell, but I have gone through moving to a different system which somehow broke the packages (looking at you MacOS). **Rust** however has an extremely bizarre syntax (remember, I am an only-Python dev), and wrapping my head around borrowing is extremely difficult. It sounds like an extremely simple topic, but most of the people act as it is more difficult, so I always have a feeling that I am missing critical information.

**Zig** is memory unsafe, since it does not have a GC, which means I will mess things up and starting with failure is not something that I find productive. Failure with some success, yes, but you need to gradually go deeper, not dive straight into the abyss when you can barely swim.

So in the end it came down between **Go** and **Nim**, and the deciding factor was syntax.

**Nim**'s syntax is almost identical to **Python** down to the error messages. This means that, *in-general*, I can transition easier to a system's language, since it will be a far more familiar setting. You also care about whitespace, which I highly prefer over `{;}`, and means that, at least in my opinion, the resulting code is highly readable. I also enjoy the fact that **Nim** is very unopinionated when it comes to writing code.

As an example, here is how to make a print statement in **Nim**

```nim
echo "Hello World!"
echo("Hello World!")
"Hello World!".echo # This feels wrong coming from Python but it also feels very fun, like when you eat sweets when you're not supposed to.
"Hello World!".echo()
```

This fact makes the language feel a lot more playful, whereas I've heard **Go** being described as boring.

So moving forward, I need a project to choose, in order to have something to work on to grind myself and make the language and the low level stuff more familiar. Probably something related to my field of expertise of reinforcement learning.
