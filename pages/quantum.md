---
layout: page
title: "Quantum Quixote"
meta_title: ""
subheadline: ""
teaser: "quivalric qomic"
header:
   image_fullwidth: "qq.jpg"
permalink: "/research/quantum/"
---

<div class="row">
<div class="medium-8 medium-push-0 columns" markdown="1">
<div class="panel radius" markdown="1">
**Topics**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->



<div class="medium-12 medium-pull-0 columns" markdown="1" style='text-align: justify;'>

### Quantum Resources

### My favourite Quantum Programming Language

### Universal Gate Set

What is computation?
It is a set of inputs I={i1,i2,...,in} getting transformed to a set of outputs O={o1,o2,...,om}.
Now, for the processing part, let us process one output at a time, as is the convention in simple single-threaded single-core processors.
Each output variable is defined by a map from the set of input variables.
The exhaustive possibilities for each input variable and the corresponding expected output is represented in a truth table.
From a black box model, the processing logic is expected to implement this truth table's epistemological behaviour.
It can as well maintain a huge look-up table and search the entry corresponding to a specific input case and produce the output.

To derive the logic behind the truth table, we transform it to a sum-of-product form.
This transformation is very powerful, as we use only 3 logical operators to form this expression - AND, OR, NOT.
Since AND and OR are associative, if our processor supports the primitives of a 2-variable AND, 2-variable OR, and NOT, we have a universal set for any computation.
With these tools at hand, we do not need to design different logic gates for each truth table, we just need to wire up many AND, OR, NOT gates is a circuit.
These are like the protons, neutrons and electrons of the computer world.

The NAND and NOR gates are also universal by their own.
NOT(i) = NAND(i,i); AND(i1,i2) = NAND(NAND(i1,i2),NAND(i1,i2)); OR(i1,i2) = NAND(NAND(i1,i1),NAND(i2,i2)).
Isn't this great!
With just one 2-input truth table, all other truth tables can be formed.

Similarly for quantum computation, there are also universal sets.
A common one is formed from the 3 quantum gates of CNOT, H and T.
A quantum computation is represented by an unitary transform of the input state to the output state.
This arbitrary unitary is like a truth table, than can be decomposed to simpler building blocks of smaller quantum gates.
My favourite universal set is Toffoli and H.
The Toffoli gate (CCNOT) is universal for classical computation, as it can implement NAND and FanOut.
While the Hadamard gate is native to quantum, giving rise to superpositions.
I often find, most quantum algorithms I implement relies on these gates by intuition.
Also, the matrix forms of these gates has no complex elements making them easy to implement on simulators.

One important point often overlooked is that by chosing to implement a general function by a universal set, we lose some performance.
If we design special purpose hardware to support a specific data transform, it will most likely be more optimal than doing so with the blocks from a universal set, similar to how ASICs are faster than CPUs.

### Quantum Quixote

There is already a [Quantum Pontiff][1], [Quantum Sheikh][2] and [Quantum Pundit][3]. Hey, I am a Hindu by birth and pundit is already taken! Also, I am so confused - am I an atheist or an agnostic. Duh! It is not about your real faith.... do I believe in a single way of doing computation, a single enterprise taking over, a single physical platform.... no! But also, when it comes to quantum, I am not an atheist like [Gil Kalai][4]. Rather the opposite. I like to dream big - even unrealistic, quixotic. And that has set me on a course through the stormy waters on my own adventure: The Ingenious Gentleman Sir Quan' Quixote of Delft.
(Mar 24, 2019)

 [1]: http://dabacon.org/pontiff/
 [2]: https://www.quantumsheikh.com/
 [3]: http://quantumpundit.blogspot.com/
 [4]: https://gilkalai.wordpress.com/
