---
layout: default
title: More Than an Allegory: The Working Logic of HoTT
---


When we think about the logical interpretation of HoTT, types take on the role of properties, and the inhabitants of those types take on the role of proofs of their validity. When considering this for the first time, we think of the type $P$ as an abstract (opaque) property, and of an element $p : P$ as an equally abstract proof. That is to say, it seems like nothing more than an allegory that helps us think using our intuition. Of course, there are other equally useful interpretations, such as the topological one, where a type is viewed as a space and its terms as points in that space, etc.

If we focus on the logical interpretation, the analogy can be naturally extended to dependent types $P : X \to \mathcal{U}$. Here, $P$ is a predicate; that is, a property that can be predicated of the elements $x : X$.

What this kind of description prevented me from seeing is that this interpretation, seemingly abstract and purely mental, materializes within HoTT itself. In other words, the underlying logic of the theory is expressed precisely in this way: by constructing types that represent properties predicable of other types. In turn, the proofs end up being functions between predicable properties embodied in composite types whose meaning is quite concrete. This means that the logical interpretation is not trapped in the Platonic world of ideas; it is heavily used within the theory itself.

For example, consider implication as the type $P \to Q$ of non-dependent functions from the "property" $P$ to the property $Q$. In a concrete scenario, proving this implication means working with expressions where $P$ and $Q$ are built from simpler types. The formulation produces a precise semantics within the theory: the meaning of the implication adopts the semantics dictated by those expressions. The proof of the implication must be an expression $\lambda x.\,\Phi$ mapping each element $x : P$ to an element $y : Q$. The expression $\Phi$ must be explicit, ensuring that the construction of $y$ from $x$ does not belong to the realm of the hypothetical but, as I am saying, is constructive.

In short, what is initially presented to us as an innocent "you can think of it this way" soon becomes the natural way to understand each of the theorems in the theory. The logical interpretation ceases to be merely a way of looking at things and becomes the mechanism by which definitions are established and results are proven. Moreover, this is the very way the theory is built upon itself.
