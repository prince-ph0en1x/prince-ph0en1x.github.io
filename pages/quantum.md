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

### Quantum Computing Resources

(Jun 21, 2020)

There are some great resources available over the internet.
The first stop in my opinion should be the [Awesome Quantum Computing][5] GitHub page.
Other good meta-resources are [Quantum Computing Report][6], [Quantum Computing Stack Exchange][7] and [Quantiki][8].

Some of my recommendations for recorded talks:
* [Quantum Machine Learning and PennyLane by Maria Schuld | QWorld](https://www.youtube.com/watch?v=pe1d0RyCNxY)
* [The Potential Impact of Quantum Computers on Society by Ronald de Wolf | QWorld]9https://www.youtube.com/watch?v=ych-yB9QP_A)
* [Quantum Computing: From Qubits to Quantum Accelerators - Koen Bertels](https://www.youtube.com/watch?v=Gz5XZJ5QnlU)
* [Q2B 2018 - Quantum Algorithms Landscape](https://www.youtube.com/watch?v=PJRatgm8sL0)
* [WQCG Episode IX, Variational Quantum Machine Learning, 07.10.2019](https://www.youtube.com/watch?v=P52iqU50NHg)
* [Scott Aaronson on Computational Complexity Theory and Quantum Computers](https://www.youtube.com/watch?v=0jrybODBUpA)
* [Keynote address by Seth Lloyd](slideslive.com/38918779)

 [5]:[https://github.com/desireevl/awesome-quantum-computing]
 [6]:[https://quantumcomputingreport.com/]
 [7]:[https://quantumcomputing.stackexchange.com/]
 [8]:[https://quantiki.org/]

### Quantum Programming Languages

(Jun 21, 2020)

The first question a quantum software/application developer faces is, which programming platform to use.
Especially with the large number of choices already available, this becomes difficult to choose.

If you plan to develop few-qubit programs and eventually test the implementation on an available physical chip, then choose the toolset from the corresponding provides, e.g. Qiskit for IBM, Forest for Rigetti.
Beware, developing 'realistic' application is difficult due to the limitation in quantum volume.

If you are interested in the computation logic and remain hardware agnostic, choose a platform that offers more simulation capabilities.
The larger unitary matrix (i.e. number of qubits) you are allowed, the better you can test the logic.
Often access to the internal state vector and execution capabilities on HPC systems are useful.
Available algorithmic primities, ease of expressing a logic in high-level and analytic tools like metrics and visualizations are also desirable.
Do not worry too much about not choosing the mainstream most popular one as cross-compilers between the dominant tools will soon be a norm.
Beware, developing 'realistic' application is difficult due to limitation in quantum computer simulation using classical logic.

### Universal Gate Set

(Jun 21, 2020)

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

(Mar 24, 2019)

There is already a [Quantum Pontiff][1], [Quantum Sheikh][2] and [Quantum Pundit][3]. Hey, I am a Hindu by birth and pundit is already taken! Also, I am so confused - am I an atheist or an agnostic. Duh! It is not about your real faith.... do I believe in a single way of doing computation, a single enterprise taking over, a single physical platform.... no! But also, when it comes to quantum, I am not an atheist like [Gil Kalai][4]. Rather the opposite. I like to dream big - even unrealistic, quixotic. And that has set me on a course through the stormy waters on my own adventure: The Ingenious Gentleman Sir Quan' Quixote of Delft.

 [1]: http://dabacon.org/pontiff/
 [2]: https://www.quantumsheikh.com/
 [3]: http://quantumpundit.blogspot.com/
 [4]: https://gilkalai.wordpress.com/
