---
layout: page-fullwidth
title: "Quantum Quixote"
meta_title: ""
subheadline: ""
teaser: "quivalric qomic"
comments: true
header: no
image:
    title: "page_head/qq.jpg"
    caption: 
    caption_url:
permalink: "/musings/quantum/"
---

## Posts


<div class="row">
<div class="medium-8 medium-push-0 columns" markdown="1">
<div class="panel radius" markdown="1">
**Topics**
{: #toc }
*  TOC
{:toc}
<!-- {:toc_levels:"1"} -->
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-12 medium-pull-0 columns" markdown="1" style='text-align: justify;'>

(abbreviations: Q for Quantum; QC for Quantum Computer/Computing/Computation)

### QC Resources

(Created Jun 21, 2020) (Updated Sep 26, 2021)

There are some great resources available over the internet.
The first stop in my opinion should be the [Awesome Quantum Computing][5] GitHub page.
Other good meta-resources are [Quantum Computing Report][6], [Quantum Computing Stack Exchange][7] and [Quantiki][8].

Some of my recommendations for beginners:
* [Quantum Computers Explained – Limits of Human Technology](https://www.youtube.com/watch?v=JhHMJCUmq28)
* [Five Quantum Computing Misconceptions](https://www.youtube.com/watch?v=kEry1TaN4-k)
* [The high-stakes race to make quantum computers work - Chiara Decaroli](https://www.youtube.com/watch?v=r_t96FqWE4M)
* [Quantum Computing Expert Explains One Concept in 5 Levels of Difficulty - WIRED](https://www.youtube.com/watch?v=OWJCfOvochA)
* [Computing a Universe Simulation](https://www.youtube.com/watch?v=0GLgZvTCbaA&)

Some of my recommendations for recorded talks:
* [Quantum Machine Learning and PennyLane by Maria Schuld](https://www.youtube.com/watch?v=pe1d0RyCNxY)
* [The Potential Impact of Quantum Computers on Society by Ronald de Wolf](https://www.youtube.com/watch?v=ych-yB9QP_A)
* [Quantum Computing: From Qubits to Quantum Accelerators by Koen Bertels](https://www.youtube.com/watch?v=Gz5XZJ5QnlU)
* [Quantum Algorithms Landscape by Adam Bouland](https://www.youtube.com/watch?v=PJRatgm8sL0)
* [Variational Quantum Machine Learning by Jacob Biamonte](https://www.youtube.com/watch?v=P52iqU50NHg)
* [Computational Complexity Theory and Quantum Computers by Scott Aaronson](https://www.youtube.com/watch?v=0jrybODBUpA)
* [Quantum Quandam Quantum Futurum by Seth Lloyd](slideslive.com/38918779)

Quantum events:
* [Quantumapalooza](https://quantumapalooza.com/)

Quantum computing platforms:
* [Quantum Inspire](https://www.quantum-inspire.com/)
* [Quirk](https://algassert.com/quirk#circuit)
* [Quantum Programming Studio](https://quantum-circuit.com/)
* [Quantum IDE](http://www.quide.eu/)
* [Quantum-Kit](https://sites.google.com/view/quantum-kit/)
* [Phase Space Computing](https://phasespacecomputing.com/)
* [QC Ware Forge](https://forge.qcware.com/)
* [Quantum JavaScript](https://quantumjavascript.app/)


[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)

 [5]:[https://github.com/desireevl/awesome-quantum-computing]
 [6]:[https://quantumcomputingreport.com/]
 [7]:[https://quantumcomputing.stackexchange.com/]
 [8]:[https://quantiki.org/]

### Q Mythbusters

#### DeHyping Quantum

List of resources presenting a realist view of the current challenges of quantum computing:
* [2008 - The Limits of Quantum Computers](https://www.scientificamerican.com/article/the-limits-of-quantum-computers/)
* [2015 - Read the Fine Print](https://www.nature.com/articles/nphys3272)
* [2020 - The bitter truth about gate-based quantum algorithms in the NISQ era](https://iopscience.iop.org/article/10.1088/2058-9565/abae7d)
* [2021 - Quantum Computing: From NISQ to PISQ](https://www.computer.org/csdl/magazine/mi/2021/05/09537173/1wTizdRwupa)
* [2021 - Focus beyond Quadratic Speedups for Error-Corrected Quantum Advantage](https://journals.aps.org/prxquantum/abstract/10.1103/PRXQuantum.2.010103)
* [2023 - Where are we heading with NISQ?](https://arxiv.org/abs/2305.09518)
* [2023 - What will a quantum computer be good for, exactly?](https://idnm.github.io/blog/posts/what_to_do_with_a_quantum_computer/what_to_do_with_a_quantum_computer.html)
* [2023 - Disentangling Hype from Practicality: On Realistically Achieving Quantum Advantage](https://dl.acm.org/doi/10.1145/3571725)

#### 200 qubits can map to all the atoms in the Universe

(Jul 9, 2020)

Well, no.

So, where does this claim come from?

The basis of this is the [Eddington number](https://en.wikipedia.org/wiki/Eddington_number), estimating the number of protons in the observable universe. Of course with assumptions like all matter can be taken to be hydrogen and estimates of the number and sizes of galaxies and stars in the universe.

The number of elementary particles of matter is roughly 2<sup>200</sup>. The total [information](https://www.youtube.com/watch?v=XxVlGAFX7vA) (including other informational carriers like photons, neutrinos, blackholes) still it below the 10<sup>120</sup> Bekenstein bound of our Universe's volume (more on that in a seperate post later).

By the way, 2<sup>200</sup> equals ~10<sup>80</sup>. Not that it helps in wrapping our head around the trail of zeros in the decimal version.

The exponent in base-2 (binary) helps when we compare computing powers.

Now coming to quantum computing using qubits (yes, you can use qutrits, or qudits too), each qubit can be in a superposition of 0 or 1.
That means, 200 qubits has 2<sup>200</sup> basis states that can be in a superpositions.
You can encode a complex amplitude for each of those states.

But what can you do with 200 qubits?
You can encode 2<sup>200</sup> classical states and run some algorithm.
This is indeed the power of quantum computation when you are processing classical data like in optimization or machine learning.
Again, assuming, the algorithm design does the heavy-lifting of interfering the superpositions such that on measuring, you get the 200 bits dictated by the [Holevo's bound](https://en.wikipedia.org/wiki/Holevo%27s_theorem), corresponding to the answer (e.g. the optimal assignment).

Now to physical simulation of quantum states, a.k.a. Feynman's use-cases of quantum computing.
You can simulate 2 quantum particle's quantum degree of freedom, with, well, 2 qubits.
Not with 2 bits.
You would need 2<sup>2</sup> complex numbers for that.
This is where quantum shines in molecular simulations.
However, the 2<sup>200</sup> from the Eddington number were the number of quantum particle in the universe.
To quantumly simulate that, we need a quantum computer memory of, well, 2<sup>200</sup> qubits.
To classically simulate that, we would need (2<sup>200</sup>)<sup>200</sup> bits.

Coming to the Mythbuster, this correlation in cardinality of number of basis states in 2<sup>200</sup> qubits and number of atoms in the Universe should be taken in the same spirit as [1 person's total DNA in all cells could stretch to the sun and back 61 times](https://www.kqed.org/quest/1219/a-long-and-winding-dna).
That doesn't say much about the power of quantum computation except just dilate your retina on the incomprehensibility of the powers of 2.
This has nothing to do with the Quantum Supremacy limit that I will discuss soon.

[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)

#### Quantum supremacy

(coming soon)

[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)

### IN Quantum

(Created Mar 1, 2022)

A list of links regarding quantum (especially, computing) activities in India.
Will eventually help in contributing to efforts of QIndia.

Organizations:
* QTpi - [link](https://sites.google.com/view/qtpi/home?authuser=0)
* QIndia
* QETCI = [link](https://qetci.org/)

Academic programs:
* tbd

Academic research groups:
* [IISc Bengaluru](https://ceqt.iisc.ac.in/)
* [IIIT Hyderabad](https://cqst.iiit.ac.in/)
* [TIFR Mumbai](https://www.tifr.res.in/~quantro/)
* [HRI Prayagraj](https://www.hri.res.in/~qic/)
* [IISER Mohali]()
* [QuEST](http://210.212.36.85/quest/institutes.html)

Industrial groups:
* IBM
* TCS Research and Innovation
    
[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)
    
### Career in QC - a guide for highschoolers

(Jul 8, 2020)

The answer to the ultimate question of life, the universe, and everything might not be as simple as [42](https://en.wikipedia.org/wiki/The_Hitchhiker%27s_Guide_to_the_Galaxy#42,_or_The_Answer_to_the_Ultimate_Question_of_Life,_The_Universe,_and_Everything). Rather, a more intriguing inquiry that fascinates scientists is, can a sentient computer like the ones we find in Sci-Fi stories and movies be built? What questions can it answer once it is built? What are the [fundamental limits](https://en.wikipedia.org/wiki/Limits_of_computation) we come across while building increasingly powerful computers? 

What is this cool gadget? What can you do with it? Where can you find one? How to use it? Read on.

#### “…the coolest gadget…”

The computer revolution has been immensely successful. From the internet explosion to [DotA playing bots](https://openai.com/projects/five/); from mobile phones to Martian rovers - it has transformed almost every aspect of human life.

Unfortunately, this steam-rolling advancement of the digital age will soon face a major roadblock – the boss-fight with the fundamental laws of physics. 

To explain this in brief, this huge advancement in digital applications were sanctioned by the growth of processing power, which in turn was possible due to miniaturization of the electronic circuit elements (called [Moore’s law](https://en.wikipedia.org/wiki/Moore's_law) of transistor scaling). The limit where these circuits are a single-atom-wide is within sight. You can’t manufacture it any smaller, ramifying its effect as a standstill in processing power and thereby of the thriving global economy based on upgrading computing devices.

Major computing corporations (like IBM, Google, Microsoft, Intel) place their bets on a fundamentally different way of computing – quantum computing. In this paradigm, instead of being restricted by the [strange properties](https://en.wikipedia.org/wiki/Quantum_computing) that arise in the single-atom-width domain that deter making faster computers, these properties are used to perform the calculations itself. 

Surprisingly, these quantum methods are theoretically much more powerful than normal (classical) computers based on binary switching logic of 0s and 1s.

There’s a catch. Nature seems to hide this powerful device very well with its laws. This form of computation is only possible if these small particles (called qubits) are secluded from any outside disturbances and influences, like energy from heat and magnetic field or the programmer trying to glimpse how much of the computation has it completed.

Thus, these computers are shelved in 2 floors tall refrigerators which are cooled to almost 0 kelvin (that’s colder than outer space). These literally are the ‘coolest’ computers out there!

This fragility makes them very costly to build and maintain. Well, at least for now.

What would you use such an immensely powerful computer for? Of course, it should be able to do everything your laptop PC can. You can play games on it if you want. But that will be like using your PC to calculate 7*13. You can as well do it on your handheld calculator at the same speed if not faster, as they are simpler, specialized to do such calculations. 
Similarly, most of what you use your laptops for is too easy a task for a quantum computer; not worth the trouble of building such a costly gadget. Instead, a powerful gadget like that better fits the pursuit to tackle the more notorious problems that we deal with – in [mathematics, physics, chemistry, biology, economics, etc.](https://www.gartner.com/smarterwithgartner/the-cios-guide-to-quantum-computing/) So hold on to your laptop for playing your favorite game just yet (or possibly for a very long time).

You might always be on the lookout for the latest graphics card in the market to allow you to play the latest game. Graphics cards or GPUs (graphics processing units) are different from the generic CPUs running the OS in that they are specialized electronics (called accelerators) designed with the purpose of speeding up graphical calculations. The CPU takes the help of the GPU every time it is tasked with some heavy graphics processing.

In the foreseeable future, quantum computers (QC) will be another accelerator like the GPU, to which the CPU will offload specific tasks that are beyond the league of classical computation.

De-hype alert: while quantum computers are the most powerful gadget we can imagine with our current theories of computation and physics, there are many questions which remain tough (at times impossible) even for a QC – and perhaps for any computation process (e.g. predicting the next coin flip result).

#### “…there is?”

Why don’t scientists already use a QC to solve all the difficult problems of the world and liberate mankind?

Well, the short answer is, we don’t have a good quantum computer yet. 

It is a field that is [still maturing](https://dilbert.com/strip/2012-04-17) and started the engineering efforts only about a decade back. In comparison, our present computers have enjoyed a development time of over half a century.

To make a perfect QC, it must be absolutely isolated from any environment, which is incredibly difficult. As a bargain, we now have Noisy-Intermediate-Scale Quantum (NISQ) devices. These are gadgets that can perform limited calculations using the secret recipe but may not be powerful enough to dethrone their classical competitors.

Nevertheless, there is a group of experimentalists who are exploring the usefulness of NISQ devices. They use the quantum computing stack (check out this [infographic](https://www.tudelft.nl/en/eemcs/current/nodes/how/the-wonderful-world-of-quantum-computing/) from the [Delft University of Technology](https://www.tudelft.nl/eemcs/the-faculty/departments/quantum-computer-engineering/quantum-computer-architecture-lab/)) where a high-level algorithmic logic for the application gets transformed to precise electrical control pulses that are sent to the quantum computer housed in the refrigerator. Building each layer requires different expertise.

#### “…can you tinker with…”

The good news is, these NISQ devices are already available as cloud computing services. And you can run your calculation on them for free! IBM, Intel and D-Wave offer some of their devices for experimentation while others require paid subscriptions. 

They are programmed differently though. To [tinker](https://www.scientificamerican.com/article/the-quantum-app-store-is-coming/) with them, be sure to spend some time first on the tutorials of these webpages.

#### “How soon…”

How long before these gadgets become computing behemoths? Scientists are optimistic. In the 10-15 year timeline, the power of QC for certain specialized tasks will reign supreme. The most promising advantage would be in optimization tasks, molecular simulations and cryptography. There are lots of work to be done to progress in this field.

The timeline fits perfectly if you are a high-schooler or in your undergrad. It takes training to develop the background and intuition. It’s one thing to study counter-intuitive quantum phenomena for passing your physics examinations, it’s another thing to master wielding these incredible powerful weapons against real-world problems. 

Hardware developers need to unravel how to scale up quantum computers and make them less erroneous. Training in experimental physics, micro-electronics are computer engineering is helpful. QC is costly to build in a garage. Most work in academic labs or MNCs with lots of funding, closely guarding their secret techniques of making such a device.

On the other hand, many individuals and startup companies are thinking about real-world applications. The theoretical field of quantum computation is much matured, but in those days, there was no drive to test the algorithms on a real device. 

The new generation of quantum programmers is more aware of the developments of quantum hardware balancing implementation feasibility with usefulness. Quantum programming demands a mix of domain knowledge (say, of the stock market for financial modeling), theoretical computer science, linear algebra and some basic quantum mechanics.

The cherry on the cake is that a host of programming platforms and tutorials are freely available. So, grab your laptop and start learning the basics. [It is never too early to start!](https://thehill.com/opinion/cybersecurity/503779-do-we-need-a-quantum-generation)

Back to the question: 

*How soon can you tinker with the coolest gadget there is?*

*You already can. Buckle-up to train in the ways of its magic. The world awaits the quantum wizard in you.*

[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)

### Q Programming Languages

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

[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)

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

[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)

### Quantum Quixote

(Mar 24, 2019)

There is already a [Quantum Pontiff][1], [Quantum Sheikh][2] and [Quantum Pundit][3]. Hey, I am a Hindu by birth and pundit is already taken! Also, I am so confused - am I an atheist or an agnostic. Duh! It is not about your real faith.... do I believe in a single way of doing computation, a single enterprise taking over, a single physical platform.... no! But also, when it comes to quantum, I am not an atheist like [Gil Kalai][4]. Rather the opposite. I like to dream big - even unrealistic, quixotic. And that has set me on a course through the stormy waters on my own adventure: The Ingenious Gentleman Sir Quan' Quixote of Delft.

[*^ back to top ^*](http://aritrasarkar.com/research/quantum/#posts)

 [1]: http://dabacon.org/pontiff/
 [2]: https://www.quantumsheikh.com/
 [3]: http://quantumpundit.blogspot.com/
 [4]: https://gilkalai.wordpress.com/

