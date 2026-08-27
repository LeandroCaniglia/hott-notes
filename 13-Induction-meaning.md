---
layout: default
title: What Does Induction Mean?
---

In classical mathematics, when we define a function by induction, what we do is state two things: its value at $1$, and how to define its value at $n+1$ based on its value at $n$. What we omit to say explicitly is that the function defined in this way respects these two originating conditions. It is something we consider so obvious that we do not even mention it.

This unspoken assumption, in reality, transforms into implicit knowledge that we do not manage to articulate. It is something we do not see. Not something we see and do not say. A sort of hidden property.

In HoTT, on the other hand, this coherence fulfilled by inductively defined functions acquires a more relevant character. The reason is that the two identities that define it (the one for zero[^1] and the successor) must be syntactic equalities (judgmental). This condition is strong because, as we know, regular equalities are homotopical: they are not subject to automatic rewriting but to proofs.

The case of the natural numbers is not unique. The book presents, starting from Chapter 1, a series of types that have inductive rules similar to the induction of $\mathbb{N}$. In all cases, the coherence conditions (a.k.a. computation rules) are syntactic equalities.

Reaching Chapter 5, the idea is to capture this notion, embodied in various types, into a formal definition that generalizes it. This gives rise to W-types, which are something like universal inductive types. This is very good, because it takes a concept floating in the air and turns it into a formal and precise definition.

Using W-types, one can reconstruct, under the same framework, the inductive types that had been defined individually. This is quite remarkable, because the family resemblance among all those types is not clearly recognizable as derived from a more general type that engenders them.

Halfway through the chapter, however, the book draws attention to a drawback: if we redefine a concrete inductive type (say, $\mathbb{N}$) as a particular case of a W-type, what we obtain fulfills all the standard properties of the type, except that the coherence conditions are no longer syntactic identities but propositional (homotopical) ones.

Several problems arise here. First, what seemed to be a happy generalization ceases to be one. If those conditions can no longer be used for automatic rewriting, anything we derive from induction will suffer a significant increase in complexity. Identities that the compiler could previously resolve will now have to be proven as theorems.

Second (and on another level of the discussion), the observation that W-types have this drawback is stated very hastily. Verifying that this observation was true in the case of $\mathbb{N}$ took me quite a bit of effort, and what takes up one line in the book took me two pages of derivations to write down properly. This, on the other hand, is not the only example in the chapter where the details of something simply stated are much more arduous to complete than it would seem at first glance.

Third, the solution to this problem is justified by several theorems that, as I mentioned in my previous post, the book does not prove. And it does not do so because they must be a computational mess entirely opposed to any notion of elegance.

Past these theorems, we learn that there are several definitions of inductive types whose goal is to solve the problem of W-types. It seems Chapter 6 leans towards one of them and develops it (I have no opinion on this matter yet because I have not leafed through that chapter).

The impression I get from all this is that the person who wrote Chapter 5 is someone who worked on that complicated approach which, apparently, Chapter 6 does not utilize, and who put the results specific to that line of attack there. Consequently, I will most likely not include them in my "curated" version of the book, because what I am writing is not popular science and, on the other hand, I am afraid of embarking on a long and tedious development of pages and pages of formulas that do not seem to present much interest within the vision of HoTT that the book intends to offer.

This does not mean Chapter 5 is dispensable. I am only referring to the section on opaque theorems. Even the first part of that section is interesting, especially because in my version of the book, the problem posed by W-types is exposed very clearly.

---
[^1]: In HoTT, the natural numbers start at $0$.
