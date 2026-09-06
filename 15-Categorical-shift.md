---
layout: default
title: A Categorical Shift. Why Path Induction Makes Sense
---

What characterizes HoTT is the analogy between the identity type $x =_A y$ and the paths connecting $x$ to $y$, if these were viewed as points of $A$ considered as a topological space. However, this intuition clashes with a fundamental principle (path induction) satisfied by identities: to prove that a property holds for all $x$, all $y$, and all $p : x =_A y$, it is sufficient to prove it in the case where $y \equiv x$ and $p \equiv \text{refl}_x$, where the latter is the constant path that never moves from $x$. This shocks us: we do not see what the reason would be to impose such a deductive leap.

While trying to understand the last part of Chapter 5, which examines these topics in considerable detail, I encountered three facts that made me view the problem through different eyes.

First, it seems that before the formulation of HoTT, the Type Theory (TT) community was trying to prove that the constant path $\text{refl}_x$ is the only possible one. If this were so, the path induction principle I stated above would be trivially true, and there would be nothing to suspect. What happened is that in 1993 (well before the introduction of HoTT), two mathematicians constructed a model that satisfied the TT axioms and had non-trivial paths.

Second, the most basic example where there are "clearly" two paths between $x$ and $x$ (the trivial and another) is the one that occurs in the case where $A :\equiv \mathcal{U}$ (the universe) and $x :\equiv 2$ (the boolean type). Here there are two equivalences: the identity $\text{id} : 2 \to 2$ and the negation $\text{not} : 2 \to 2$. By the univalence axiom, these equivalences construct two distinct paths in $2 =_{\mathcal{U}} 2$. The first is trivial, the second is not. It seems the necessity of using univalence to find this kind of examples is unavoidable. In other words, there is a strong link between univalence and the existence of non-trivial paths.

Third. If, instead of thinking of $A$ as a topological space, we think of it as a category whose objects are the terms $x : A$ and whose morphisms $\text{Hom}(x,y)$ are the paths from $x$ to $y$, a perfect analogy arises between the (counter-intuitive) principle of path induction and the Yoneda Lemma. This happens quite clearly by replacing the category $\mathsf{Set}$ with the universe $\mathcal{U}$, the functors $A \to \mathsf{Set}$ with the families $A \to \mathcal{U}$, the representable functor $\text{Hom}(x,-)$ with the family $x =_A -$, and the natural transformations with homotopies.

The third point is illuminating. What seems doubtful when considering the topological analogy acquires plausibility when thinking about Yoneda. To top it off, the Yoneda Lemma is possibly the most famous theorem in category theory, even though its proof is so simple that it could be reduced to an observation. Nevertheless, that two remarkable phenomena, each in its respective theory, are so clearly connected is beautiful and clears our suspicions: what was wrong was our intuition.

![Table](/assets/Categorical-shift.png)
