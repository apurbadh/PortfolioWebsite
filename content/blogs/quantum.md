---
title: "Quantum Computing: Part 1"
date: 2021-04-03T23:29:21+05:30
draft: false
github_link: "https://github.com/gurusabarish/hugo-profile"
author: "Apurba Adhikari"
tags:
  - research
  - quantum
image: /images/quantum.jpg
description: ""
toc: 
---

## Abstract  

Quantum computing is a field that combines concepts from classical information theory, computer science, and quantum physics. Following Richard Feynman's finding that certain quantum mechanical effects cannot be efficiently replicated on a computer, it was hypothesized that computation, in general, could be more efficient if these quantum effects were exploited. When Peter Shor described a polynomial-time quantum technique for factoring integers, this speculation was confirmed. Since then time, the field of Quantum Computing has been in the mainstream and has been widely discussed. Due to that, there are also a lot of misconceptions about it, for example, Quantum Computers are not another generation of Supercomputers like many people think them to be, it also is not suitable for a normal person who just wants to use computers, for normal tasks, classical computers are way better than their Quantum counterparts. Quantum computers are meant for deeply specialized fields like machine learning, cryptography, and calculations related to Quantum Physics. I am trying to give a short introduction to Quantum Computing to people who are unfamiliar with this concept in a short and sweet way.

 Keywords : _Quantum Computers, Information Theory, Quantum Physics_

##  1.1 Background 

Richard Feynman ignited the quantum computing revolution. He addressed the following problem at MIT in 1981: traditional computers cannot efficiently model the evolution of quantum systems. As a result, he suggested a fundamental model for a quantum computer capable of doing such simulations. He outlined the possibility of massively outpacing traditional computers with this. However, it took more than a decade for the Shor algorithm, a unique method, to shift people's minds about quantum computing. Peter Shor created a method in 1994 that allows quantum computers to factor huge integers tenfold faster than the best classical algorithm on regular machines. Factoring 300-digit figures take millions of years in the latter. The Shor algorithm has the potential to break many of today's cryptosystems in theory. Quantum computers' ability to break cryptosystems in hours rather than millions of years sparked interest in quantum computing and its applications. Twenty-two years later, in 2017, IBM announced the first cost-effective quantum computer, bringing the competition to a new level.


##  1.2 Objective 

The term Quantum Computing is unfamiliar to a lot of people even in Physics, Mathematics, and Computing fields. I think that is because of less availability of resources and a very mathematical approach to the available resources. The main objective of this paper is to provide a general resource for people to read and understand what is Quantum Computing with less mathematical background. I am writing this paper in a very easy and understandable way so that even normal people can understand it. That being said, I will not include many deep concepts in Quantum Computing. The objective of this paper is not to make a person professional in Quantum Computing but to give general information about Quantum Computing and how it works.

##  1.3 THEORY 

A bit is a concept used in traditional computing to describe how computers represent information. Quantum computing uses quantum bits, also known as qubits, as a memory unit. A two-state quantum-mechanical system makes up of qubits. The power of quantum computers grows exponentially with more qubits. A quantum-mechanical system is one that can exist in any two quantum states that can be distinguished. This is because of the phenomenon called Quantum Entanglement and Quantum Superpositioning. It's normal to be confused by phrases like superposition and entanglement; we don't see these phenomena in our daily lives, so I will be introducing them in later sections. Like normal computers have gates like NOR gate, OR gate, AND gate, etc, Quantum computers have Quantum Gates to decide what to do based on the input. Similarly, Quantum Computers have Quantum Circuits instead of normal circuits found on normal computers. 

## CHAPTER 2 : SOME NOTATIONS 

### 2.1 Hilbert Space 

A Hilbert space is a complete inner product space with respect to the norm defined by the inner product in mathematics. Hilbert spaces are useful for clarifying and generalizing the concept of Fourier expansion and certain linear transformations such as the Fourier transform. Although many basic features of quantum mechanics can be understood without going into detail about Hilbert spaces, Hilbert spaces are critical in the mathematical formulation of quantum mechanics. In functional analysis, Hilbert spaces are investigated. 

The components of an abstract Hilbert space are sometimes referred to as "vectors." They are typically sequences of complex numbers or functions in applications. In quantum mechanics, for example, a physical system is described by a complex Hilbert space that contains "wave functions" that represent the system's possible states. For more information, see the mathematical formulation of quantum mechanics. The Hilbert space of plane waves and bound states, which is commonly used in quantum mechanics, is formally known as the rigged Hilbert space.


### 2.2 Bra-Ket Notation 

In paper related Quantum Computing or Quantum Physics, the appearance of symbols like shown below is quite common. So, what are they and why are they used ?

|0|1⟩ *or* |ψ⟩

As it turns out, they are nothing but vectors, but not the normal vectors, unlike normal vectors they are not in a space but a vector in an abstract mathematical thing called Hilbert-space which we discussed previously. And another difference between them and vectors would be that the coefficients in Quantum Mechanics are not real numbers, but are complex numbers. [2]



### 2.2 Operators 

An operator acts on a function to produce another function, it is denoted by “^” symbol
It is like how a function acts on a variable like We often (but not always) indicate that an object is an operator by placing a 'hat' over it
