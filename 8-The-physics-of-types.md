---
layout: default
title: The Physics of Types - Magnitudes, Semantics, and Structure
---

# The Physics of Types: Magnitudes, Semantics, and Structure

It can be somewhat jarring when we first begin studying Homotopy Type Theory (HoTT) to realize that the book does not provide a definition of a type. While there are ways to define types formally, starting there is not considered pedagogically convenient. 

But then, how can we think about these entities that are subjected to a syntax the book introduces as it builds new types by combining more basic ones? Even though something tells us this is not the right path, the cultural baggage of thinking in terms of sets tempts us to interpret types as collections.

A perspective more faithful to the idea of a type arises from recalling something we once discussed in this channel: pure mathematics has no concept of time. 

Thought out carefully, this sort of epiphany leads us to recognize that it also lacks other physical notions like length or mass. 

This total absence of contextual connection with nature means that speaking of units makes no sense in mathematics. In physics, on the contrary, every concept comes equipped with a system of units that allows it to be quantified and strictly determines which operations it makes sense to subject it to. Furthermore, dimensional analysis plays the role of a type checker: the equation $E=c^2m$ could not even be formulated if the units of energy were not those of velocity squared multiplied by mass; it would simply not be a well-formed expression.

The method of endowing mathematical objects with a certain structure via Set Theory ties an object's character exclusively to its membership relations. Ultimately, everything ends up being a set, meaning that expressions lacking any interesting interpretation, like $2 \in 3$, are nevertheless syntactically well-formed.

Understanding this, we can think of types as filling this semantic vacancy. To express that $x$ is an object with a certain intrinsic structure, we introduce the concept $A$, and we declare $x: A$ to denote that $x$ is an element with the characteristics defined by that abstract and opaque shape we call $A$.

In this way, the role that magnitudes (frequency, power, temperature, etc.) play in physics is played by types in HoTT. By saying that $A$, $B$, and $C$ are types, we are assigning a structural semantics to the variables $x: A$, $y: B$, and $z: C$. Variables are no longer independent entities that belong to one or several sets; instead, they are born with a meaning that governs their behavior.

Just as physics defines new concepts from more primitive ones (like velocity from position and time, or momentum from mass and velocity), Type Theory introduces a bounded set of basic operations between types, such as the Cartesian product $A \times B$ or the functions $A \to B$. The only qualitative difference is that in physics, primitive magnitudes are predetermined by length, mass, and time, whereas in HoTT, although fundamental types exist, the system allows us to declare an open list of abstract types $A$, $B$, $C\dots$ without any explicitly preassigned meaning.

The introduction of types is disruptive. For instance, just as physics does not require introducing subconcepts, foundational Type Theory sees no need to define subtypes as direct inclusions. This contrasts sharply with the idea of a subset, through which natural numbers are integers, integers are rationals, and so on. Therefore, the notion of a type is inherent to each variable; the strongest property characterizing a variable is the type with which it is born in its declaration, which remains invariant throughout the entirety of its syntactic scope.
