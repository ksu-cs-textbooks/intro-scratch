---
title: "Block-Based Programming"
pre: "4. "
weight: 40
---

Programming is essentially writing a set of instructions for the computer to carry out. These instructions are part of a programming language that has a well-defined syntax and grammar, and is in many ways similar to a human langauge (albeit with a much more limited vocabulary). For example, here is a program written in LOGO that moves a robot in a rectangle:

```
forward 100
right 90
forward 100
right 90
forward 100
right 90
forward 100
```

However, a computer can only interpret instructions that conform _exactly_ to the syntax and the grammar of the language. Thus, the following program would fail to work:

```
Forward 100
Right 90
Forward 100
Right 90
Forward 100
Right 90
Forward 100
```

Can you spot the problem? 
{{% expand title="answer..." %}}LOGO does not recongize the capitialized `forward` and `right` commands - it expects lowercase!{{% /expand %}}

Learning to program therefore involves several challenges - we must learn the syntax and grammar of a language, and a new way of thinking. This challenge is compounded by the need to get syntax and grammar exactly correct.  Unlike a language arts teacher, who can see past typos and mispellings to understand our intent, a computer simply cannot.

Scratch and other block-based programming languages seek to make this learning process easier by reducing the cognitive load involved. In a block-based language, instead of typing code, blocks representing the code are dragged around the screen and "snap" together. This snapping only occurs when the block is in a location that is appropriate for the language, effectively making it impossible for the programmer to make syntax errors or mistype commands.  This allows the learner to focus more on the logic of the program and how the computer actually interprets the code that we write.

That last bit, understanding how the computer processes our code, is an important part of developing our computer science skills.  We sometimes call this having a "mental model" of the computer. If we have a good mental model, we can understand what a program does even without running it. So in this course, we'll introduce not only the blocks that make up the Scratch language, but also aspects of how the Scratch Virtual Machine (its computer) makes sense of those blocks.