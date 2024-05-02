---
title: "Trying Nim: So many choices!"
date: 2024-05-01
type: "post"
draft: true
---

After some time playing with **Nim**, I have decided on a project, which is to translate my project [**Human Dispersion**](/projects/human-diffusion/).

I think it has it all. Arrays, classes, complex data structures, math libraries, file readings, RNG, and plots. I hope that this will keep me at least somewhat preoccupied and walk me through the basics, as well as remind me why I love RL so much.

At the beginning everything walked smoothly. I decided I would leave classes (called `types` in Nim) for later, which means I will have the complex stuff (file reading, converting it into a bitmap, and generating a matrix from it) for much later, which gives me time to get an intuition for the language.

I also found a handy guide called [Nim for Python Programmers](https://github.com/nim-lang/Nim/wiki/Nim-for-Python-Programmers), which I guess means that I am not the first nor last to decide to go from Python to Nim in one step.

As you can see from the title the guide lists so many different ways to do a thing, most of which kind of feel illegal.

## Variable names

In Nim, a variable name is recognized and compared with other variable names with two rules. Is the first letter the same name and case? Is the rest of the name the same, ignoring case sensitivity and underscores?

This for me is mindblowing. Not only can you mix and match camelCase with snake_case to call a variable, but you can have any combination of n_a_m_e_s. Best (or worst) of all, using backticks (`) means you can have *whitespace* in a variable name. This means that

```nim
var name: string = "name"

name == nAME
name == n_a_m_e
name == `n a m e`
```
which feels insane!

The way they justify this in the [Nim manual](https://nim-lang.github.io/Nim/manual.html#lexical-analysis-identifier-equality) is by saying that this allows every programmer to use their own preferred style, without forcing other programmers to adopt the same style, with the only exception being the first letter.

```nim
proc sameIdentifier(a, b: string): bool =
  a[0] == b[0] and
    a.replace("_", "").toLowerAscii == b.replace("_", "").toLowerAscii
```

Using backticks (`), you can even assign reserved keywords as variables.

```nim
var `var` = "Hello Stropping"
```
which is wild.

