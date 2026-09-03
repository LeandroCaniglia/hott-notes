---
layout: default
title: Beyond Simple Induction. W-Types and the Sum-Product Analogy
---

Sections 5.5, 5.6, and 5.7 of the HoTT book seemed to me the weakest part of what I have studied so far. They are complicated, excessively wordy, and not very well defined in their objectives. It is a pity, because up to that point, the chapter was progressing very well. What I did then was work with Gemini (and Notebook) to try to understand and clarify some things that, apparently, are good to know before tackling Chapter 6.

That decision was much more arduous than I would have supposed. The good thing is that it led me to study generalizations of the notion of inductive type, such as: inductive families, mutual induction, and inductive-inductive definitions. At the same time, it became clear to me why W-types, which promised to be the supersimplification of inductive types, are not suitable for proof checkers. The latter are forced to take a sort of shortcut by which they momentarily set aside the theory and impose definitional computation rules where only propositional equalities can be reached.

Apparently, this is not enough to invalidate W-types (which proof assistants discard), since their theoretical value compensates for their practical deficiencies. Somehow, this gap is widened in Chapter 6, where it seems the full justification for all this is finally seen.

The result of having tackled these induction variants with greater precision is ambiguous. On the one hand, it lengthens the chapter considerably. On the other, it shows the foundations of the theory in more detail. For example, inductive-inductive definitions are what allow us to define contexts (the ones usually symbolized as $\Gamma \vdash \cdots$). Mutual induction is needed to inductively define some basic types like the sequence $\mathsf{Even} \to \mathsf{Odd}$, where it is necessary to define two (or more) types simultaneously. Inductive families are behind definitions like $\mathsf{Vec}(n)$, where vectors of dimension $\mathsf{succ}(n)$ are obtained by adding an element of the base type to those of dimension $n$.

I did take care to provide plenty of examples. This is fundamental because, as one might easily guess, the subject is exceedingly abstract.

I still have the last section left to study. I hope it is approached in the way the book had been presenting things. We will see what the PDF holds.

***

### A Note on $\Sigma$ and $\Pi$ Types

I almost forgot. Yesterday, during a YouTube talk, someone made an interesting observation about an elementary concept that I had not noticed. One of the first things the theory introduces are the $\Sigma$- and $\Pi$-types. At first, these notations, especially the former, are a bit bewildering. The binder $\Sigma$ generates dependent pairs, while $\Pi$ generates dependent functions. For example, $\Sigma_{x: A}B(x)$ has as constructors the pairs $\langle a, b \rangle$ where $a : A$ and $b : B(a)$. On the other hand, $\Pi(x: A).\, B(x)$ is constructed by functions $\lambda x.\, f(x)$, where $f(a) : B(a)$ for all $a : A$.

The fascinating part is that when $B$ is constant, meaning $B(a) \equiv B$ for all $a : A$, the sum type is identical to the Cartesian product $A \times B$. That is, if we "sum" $B$ exactly $A$ times, we obtain $A \times B$. In the case of the product, the analogy should lead us to conclude that if we multiply $B$ exactly $A$ times, we obtain $B^A$. And this is exactly what happens, because as we have seen several times, $B^A$ is precisely $A \to B$, which is the type of functions $f$ such that $f(a) : B$.
