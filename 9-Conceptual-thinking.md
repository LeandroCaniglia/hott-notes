---
layout: default
title: The Role of Conceptual Thinking
---

# The Role of Conceptual Thinking

Now that I am thinking about the exercises in Chapter 4, I realize that something that had been hinted at until now becomes evident in this chapter.

From the very beginning, the Book makes it clear that proofs in HoTT are functions. At first, what we do is construct those functions by following some route of more or less simple transformations of generic terms from the domain into terms in the codomain: $a \to a_1 \to \dots \to b$.

Things get complicated as we start transforming types, not terms. There, the goal is to prove that one type is equivalent to another $A \simeq B$. Equivalence is a sort of isomorphism (adapted to equality in HoTT). That means a single arrow $f$ is no longer enough; we also need to define its inverse $g$ and prove that the two compositions $f \circ g$ and $g \circ f$ are homotopic to their respective identities.

Well, in Chapter 4, those equivalences begin to combine, and we no longer have a single letter on each side, but increasingly complex expressions instead of $A$ and $B$. And there, the strategy of trying to define $f$ and $g$ does not scale, and we have to argue differently.

This does not usually happen in classical mathematics. If we have an isomorphism from one space to another, we can normally describe it explicitly. It is true that this approach (which I call computational) can often be replaced by another (conceptual) that does not track elements, but rather reasons categorically. But one does not preclude the other. Therefore, I do not see a direct analogy there. What I do see is something slightly different. In classical mathematics, functions in a certain category are usually preserved not only by composition but by a rich collection of operations. For instance, continuous, integrable, and differentiable functions, etc., can be added, multiplied, composed, and adapted to other categorical constructions such as limits and colimits; they can have extensions, and so on. What does not scale there is the proof by definition: there is no way to show that a function obtained through these operations meets the definition; we need higher-level abstraction theorems to conclude that they are continuous, integrable, differentiable, or whatever it may be.

That is what begins to be seen in Chapter 4. That the most basic theorems of type equivalence play an increasingly leading role as the theory evolves. This, ultimately, is a skill we must develop in the exercises: that of conceptual thinking. The ability to interpret equivalences by their meaning, not by a succession of element transformations. That is why the most basic theorems are so important. And that is why it is not easy to use them, because the complexity of the expressions often means that the constituent parts of long formulas are not obvious, and one must learn to see them.
