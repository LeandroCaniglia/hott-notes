---
layout: default
title: The Architecture of Types - Judgments, Opacity, and Paths
---
When transitioning from classical mathematics to Type Theory, one of the most significant hurdles is abandoning the intuitive comfort of Set Theory. We are used to thinking of a set as a collection of items. Type Theory demands a more syntactic approach: a type is a primitive notion defined entirely by the rules that govern it—how to construct its elements and how to compute with them. 

This shift from semantics to syntax fundamentally alters how we perceive mathematical truth, abstraction, and even equality.

## Judgments vs. Propositions

In classical logic, a statement is either true or false, and if proven, it becomes a theorem. Type Theory introduces a crucial distinction between *judgments* and *propositions*. 

A judgment is a formal certainty guaranteed by the rules of the deductive system itself. It is true by construction and is applied automatically by the mechanical type-checker. For instance, the equivalence $f(3) \equiv 3^2$ (assuming $f$ squares its input) is a judgment. It requires no proof; the system simply rewrites it.

A proposition, on the other hand, requires an intelligent agent to construct a witness (a proof). The statement $3^2 = 9$ is a theorem. The machine will not automatically rewrite $3^2$ to $9$ without a predefined logical path provided by the user. By separating what is mechanically trivial (judgments) from what requires intellectual construction (propositions), the theory elegantly isolates the creative act of doing mathematics from the bureaucratic act of verifying it.

## The Power of Opacity

It is tempting to think of computable theories as strictly algorithmic, where every element must be broken down into observable data. However, Homotopy Type Theory thrives on *opacity*. 

In this framework, we often postulate the existence of terms or equivalences without ever looking inside them. For example, the unit type $\mathbf{1}$ has a canonical element $\star$, but if we prove another element equals it, we simply possess a witness to that equality. We cannot inspect the internal "gears" of that witness. 

This opacity is a feature, not a bug. In science, naming an abstraction—like energy or mass—allows us to establish relationships between concepts without constantly calculating their underlying values. By keeping elements encapsulated and interacting with them solely through their defined behaviors (constructors and eliminators), the theory prevents us from relying on the accidental details of a specific implementation. It forces our proofs to be universally applicable.

## Equality as a Journey

The most radical departure from classical mathematics lies in the treatment of equality. In ZFC, equality is extensional: two things are equal if they contain the same elements. In traditional Type Theory, equality is intensional: two things are equal only if they share the same construction.

Homotopy Type Theory mediates between these extremes by interpreting equality as a space of paths. An equality between two elements $x$ and $y$ of a type $A$ is not a static fact but a type itself:

\\[
x =_A y
\\]

The inhabitants of this type are *paths* from $x$ to $y$. This means there can be multiple, distinct ways for two elements to be equal. Furthermore, because equality is a type, we can formulate equalities between equalities (paths between paths), creating an infinite tower of homotopies.

This topological analogy breathes visual life into pure syntax. A proof of symmetry becomes a function that reverses a path. Transitivity becomes the concatenation of paths. By transforming equality from a rigid logical identity into a geometric journey, the theory provides a profound new language for capturing the deep, structural equivalences that classical mathematics often takes for granted.
