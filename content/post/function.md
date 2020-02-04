+++
date = 2017-05-17T01:57:06-05:00
highlight = true
math = true
tags = ["math", "functions"]
title = "What is a function?"

 # [header]
 #   caption = ""
 #   image = ""

+++

One of the most commonly seen terms in computer science is *the function*. I've seen many of my classmates, co-workers and students missing the key aspects of what function are and why we use them. This post is a *simple* (I hope) explanation of both interrogants. <!--more-->

We are used to see functions everywhere while in class. Something that looks like:

$$f(x) = 2x + 3$$

This is, in fact, a function.

However, we may have listened to our programmer friend saying something about a `print` function. Is `print` a function too? What's the difference? Well, they both refer to the same thing. Let's start with a simple explanation.

A function, in this sense, is a magical box. This magical box has magic powers, of course! The box uses its powers to convert apples to apple juice. Isn't it nice? Whenever we want some apple juice, we simply put an apple **inside** the box and we get apple juice as a **result**.

This magical box idea is exactly what a function is. If we look at this box from a more abstract view, it may look like this:

![Abstract representation of a function](/img/function-box.png)

We give something (e.g. an apple) to the box and the box gives us something back (e.g. apple juice). So for a function we have three basic elements: **input**, **function** and **output**. Considering this basic notion as a function will answer both previous questions: Is $f(x) = 2x + 3$ a function? Is `print` a function? Yes, they are functions:

The first case refers to a linear function, in which the input is $x$ and the output is $f(x)$. So when $x = 5, f(x) = 13$. The whole $2x+3$ is the box, while $f(x)$ is the output.
The `print` function receives a parameter: what is it what you want to print? And then it generates an output, as it appears in your screen. Therefore, that is a function too.

The *real* definition of a function goes back to the very foundations of mathematics: set theory. A function is a *relation* between two sets such that one input never has more than one output. In a more algebraic manner:

A function from a set $A$ into a set $B$ is any binary relation $R$ satisfying the condition $\forall a \in A \exists ! b \in B$ with $(a,b) \in R$.

Each element in the set of inputs $A$ should have exactly one element in the set of outputs in the relation $R$.
Since a relation is actually a set of inputs and outputs paired, then it is only natural to think of a function as:

$$ function = (input,output) $$

which is quite clear. We can always think about our juicer as the function $juicer = (apple,\,juice)$.

Of course, a function may have a *set of inputs* as an input, and have a *set of outputs* as the output. The three elements remain the same, and the notation is pretty much the same. Since there are already some sets defined, we can think of a function like this:

$$f \colon \mathbb{N} \to \mathbb{N}$$

This notation is telling us that $f$ is a function which **maps** a natural number to another natural number. What could this function be? Well, whichever function that complies with these requirements. Maybe take a natural number and multiply by three. This is a function: any number we pick will *produce* only one result after being multiplied by three, and both the input and the output parameters will always be natural numbers.

To round things up, a function could be any *magical box* transforming any *input* to an *output* if and only if for each input there's only one output.
This basic notion of functions really helped me in my junior years to understand how agents and algorithms work: what should I give the box in order to obtain a certain output?
The rigorous notation is useful to develop a formal sense of what type of input we should provide the box with, and what type of output to expect.

I recommend checking Makinson's Sets, Logic and Maths for Computing [^1] for further reading, as it explains stuff like this in a simple yet formal way. Plus there are lots of Alice boxes!

[^1]: D. Makinson, *Sets, Logic an Maths for Computing*. London: Springer-Verlag, 2012.