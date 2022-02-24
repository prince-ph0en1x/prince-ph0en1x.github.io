---
layout: page-fullwidth
title: "Algorithms"
mathjax: true
meta_title: ""
subheadline: ""
teaser: ""
comments: true
header:
    image:  "page_head/lil.gif"
    pattern:  "page_head/bk03.jpg"
    caption: 
    caption_url:
permalink: "/research/algorithms/"
mathjax: true
---

## Posts

<div class="row">
<div class="medium-8 medium-push-0 columns" markdown="1">
<div class="panel radius" markdown="1">
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->



<div class="medium-12 medium-pull-0 columns" markdown="1" style='text-align: justify;'>

### Pattern and Randomness

(Oct 22, 2019)

Everytime we talk about Emergence, there is a notion of a pattern, something that we consider favourable, that eventually comes into existence by the complex interactions and dynamics of the system in question. On the other hand, the word 'random' typically represents the opposite of 'pattern'. Or does it?

I argue here, randomness is an emergent property. Say I got {H,H,H} on 3 successive coin tosses, I can interpret the coin as 100% biases. But it can also happen to be one of those 8 possibilities that showed up in this Universe, while the other 7 cases were swept under the rug of the many-World's interpretation of a measurement (albeit classical). Whether it is actually unbiased cannot be understood from a few trials unless the law of large numbers comes into play, i.e. until the prefect ideal probability distribution is at least captured in some approximation in the statistics. Randomness is a statistical parameter, making no sense for a single experiment, like the temperature of an individual atom. Often, randomness is associated with the entropy of the microstate. 3 Heads has higher order and less surprise than 2 Heads and 1 Tail. But that assumes the coin is unbiased as a prior. What if we want to understand the property of the system itself? For example, if we are looking for radio signals from extra-terrestrial life, or decodings the heiroglyphs of an ancient civilization? How would we distinguish a random signal from a non-random one? The entropy of a bitstring also deals with how much information can be communicated via it, or in the Kolmogorov sense, if it can be compressed and later decompressed with a wrapper semantic overhead. Let's assume a situation where I tell a friend that I would either send a string of 1s if the answer if yes, or a string of equal 1s and 0s if the answer is no. Assuming no noise in the channel, now, the meaning of the word random loses it's entropic context, as here, a string with 75% 1s would be more near to a random message.

Is pattern also an emergent parameter? Is it a statistical low entropy configuration or a collection of semantically meaning states?
* Arguments against the 1st idea: based on how we semantically understand something, a higher entropy system can show more pattern. E.g. a program in BrainFuck printing 1s forever will have less algorithmic entropy than a program in C++ generating the Fibonacci series due to the inherent non-rationality of te golden mean; or a C++ code for 1s would have lower entropy than a BrainFuck code for golden mean; even though it should depend on the semantics of the language for the compiler, like an english sentence has lower entropy than a japanese sentence due to the higher number of japanese alphabets.
* Arguments against the 2nd idea: if something has semantic meaning, it should be reducible to a cost function for which a pattern would give a higher score than a random input. For a program/language, it would be syntactic correctness, e.g. grammarly. But still the association to the application is missing, the same problem as with shannon information metric.

[*^ back to top ^*](http://aritrasarkar.com/research/emergence/#posts)

### Fascination with Fractals

(Oct 22, 2019)

Why are fractals so ubiquitous in Nature than Euclidian geometry? What property of fractals make them so favourable for these blueprints? I like to approach this from 2 different angles.

God is a lazy programmer. Imagine you have to render the graphics of fire or clouds with triangles or ovals! Hell of a task, right? Indeed, a few iterations of a simple yet elegant fractal equation can generate these on your game world. It is not so difficult to drive home the point that fractals are the generator equations of the world we see around us, so fractal equations can easily generate models of them - low algorithmic complexity - lazy programmer. But, that's a bit of ouruboros logic. The real equation is, why do we see fractal generator equations in the blueprints of the Universe? Why can't clouds just be oval or fires as triangles like in the computer games of the early 1980s?

This has to do with compressing. Fractals are the edge of chaos, where the system transitions from a periodic attractor to a chaotic randomness. This also goes hand in hand with class 4 Wolfram automata which are universal computers which has enough expressive power to program everything in an unified structure, yet, the rules are simple enough and don't get lost in chaos. Fractals are also great data compressors that can be prioritized with respect to the iteration level, working exactly like a Discrete Wavelet Transform, where the larger amplitudes and low frequency terms are captured in the lower iterations whereas the finer details can be compressed in the higher iterations allowing viewing the final product at different levels of approximation without losing the big picture, to interpret the general law behind them. Thus, there is a very subtle difference between a fractal of 100 iteration (say a Koch curve) and a fractal of 100 iteration with a small variation allowed at each level (say the coastline of Britain). In the later, an enormous amount of information can be encoded at different level of approximations. A little child can build an encoded message with pebbles on a particular beach without changing the overall fractal dimension much.

So fractals in a way allows us to start with a vague design and then periodically tweek it with small modifications to reach the design of interest. The question remains: is that how the Universal laws emerged? Chunks of smaller and smaller sized phenomena adding higher order refinements to the evolution of the universe.

[*^ back to top ^*](http://aritrasarkar.com/research/emergence/#posts)

### GUT from It

(Mar 27, 2019)

Recently I was reading this article on [constructing space-time from computation](https://arxiv.org/abs/1602.06987) which opened the flood gates of correlating theories in my head.

Before I describe my proposition, let's list down the ingredients:
* [Plancherel's theorem](https://en.wikipedia.org/wiki/Plancherel_theorem) which states the integral of a function's squared modulus is equal to the integral of the squared modulus of its frequency spectrum.
* Kolmogorov/Algorithmic complexity
* String length
* Launderer's principle
* Fourier transform
* It from Bit
* Thermodynamics
* Measurement in Quantum Mechanics

The equation:

 {% raw %}
  $$ \biggl\Vert \int_0^{t_u} |f(x)|^2dx - \int_{-\infty}^\infty|f(\xi)|^2d\xi \biggl\Vert \equiv \bigl(len(S) - K_\mathcal{U}(S|X)\bigl)kTln2 $$
 {% endraw %}

The interpretation:

Let $f(x)$ be the state of the Universe encoded as a bit string. The absolute difference between the integral of the function's squared modulus and the integral of the squared modulus of its frequency spectrum gives us the amount of new information generated by the Universe in the time duration of the integral of the function, i.e. $[0,t_u]$. This is equivalent to the work value of the bit string given by the fuel value of the string scaled by the Boltzmann constant and the temperature, following reversed Launderer's principle. The fuel value is the difference between the length of the string and the conditional Kolmogorov complexity of the bit string, given the Fourier transform of it. This transform represents the derivable physical laws given the bit pattern of the Universe.

[*^ back to top ^*](http://aritrasarkar.com/research/emergence/#posts)

### (A)daitva

(Jul 23, 2019)

When you are into the topic of emergence, you can't help but wonder about the phase transitions where different laws take over at different scales. Quoting Douglas R. Hofstadter (from the book I am a strange loop), "thinkodynamics is explained by statistical mentalics", sometimes knowing everything about individual components of a system (e.g. neuron) tell us very little of how the components behave as a whole (e.g. consciousness). It is not sorcery that the usual scientific method of reductionism does not work here. It is simply that many laws of the overall system is embedded in the interaction behaviour of the components, rather than the components themselves. In physics, we call this coupling. In quantum computing, perhaps, a similar notion is of entanglement. Following the ideas of Juan M. Maldacena (in his ER = EPR paper with Leonard Susskind), in classical mechanics, they are wormholes.

A question that perhaps keeps popping up is, are gravity (general relativity) and quantum mechanics one and the same - two different ways (even mutually conflicting at times) of interpreting the same thing? They work extremely well in their own niche scale - GR for galactic scales, QM for atomic scales. The obviously problems arise when there is both, mass concentrated in small space, as in the early Universe or blackholes. One way of approaching this problem is called the Holographic Principle, where two very different interpretations, a bulk theory in n-dimensions and a boundary theory in (n-1)-dimensions, describe a single reality.

However, grand unified theory (GUT) and consciousness are not the only places where scientists have trouble going from two views of reality to one. It is very much a problem within the [basic postulates][1] of quantum mechanics itself; where normally a closed system evolves unitarily (which is invertible, deterministic and continuous), while any interaction with an observer (nothing to do with consciousness), results in a measurement (which in irreversible, probabilistic and instantaneous).

What is more interesting as a computer scientist is to wonder, is this duality true for computability and complexity as well? For complexity, Shannon and Kolmogorov metrics converge asymptotically for true randomness. For computability, what is the difference between the state machine and the tape in the Turing Machine. For languages, what is the difference between syntax and semantics? Why does the explaination capability of a neural network inversely proportional to it computation expressibility - is that the Godel's incompleteness theorem in action?

Are there more such dualities?
* the idea and the meta 
* the syntax and semantics 
* the body and the soul 
* the particle and the wave 
* the observer and the object 
* the theorems and the axioms 
* the first and the zeroth 
* the natural and the supernatural 
* the known and the unknown 
* the knowable and the unknowable 
* the statistics and the probability 
* the output and the program 
* the program and the compiler 
* the tape and the state machine 
* the system and the environment 
* the continuum and the quanta 
* the memory and the processor 
* the cardinals and the ordinals 
* the nodes and the network 
* the position and the momentum
* the energy and the duration
* the entanglement and the coherence
* value of a field and its change at a certain position
* spin on 2 different axis

Does generalization take you only as far as indentifying 2 fundamental ideas working in a symphony? We can either call it a single coin, or we can call them two opposite faces, or acknowledge only the face facing us, or the entire set of possibilities while they/it are/is spinning.

[*^ back to top ^*](http://aritrasarkar.com/research/unification/#posts)

 [1]:[https://www.scottaaronson.com/blog/?p=3943]

### The Grand (Un-)unified Theory

(Jul 23, 2019)

While theoretical physicists are lamenting over the differences and compatibility of two of the most fundamental physical laws, a more birds eye view of the landscape of the universal design reveals some very important structures, that are so deeply embedded around us, we need to ask, why?
Here I ponder over some of those structures that I find particularly interesting.
* Godel's Incompleteness Theorems
* Kolmogorov Complexity
* Quines
* Fractals
* Chaos
* Shannon Entropy
* Holographic Universe
* Quantum Entanglement
* Golden Mean
* Neural Network
* DNA
* Thermodynamics
* Standard Model
* Brainwaves
* Plank Units
* Cellular Automata
* Church-Turing Thesis

[*^ back to top ^*](http://aritrasarkar.com/research/unification/#posts)
