---
layout: default
title: A Final Reflection on Tags and Dependency Trees
---

As I have explained, to prove that UA $\Rightarrow$ FE, we first show that UA $\Rightarrow$ WE and then that WE $\Rightarrow$ FE. The problem is that these two theorems rely on others, which in turn rely on others, and so on. Furthermore, those preliminary results were proven without paying special attention to which axioms they used.

The dependency tree of each of the two main theorems acts much like a frozen execution stack. Seeing exactly where the axioms are used is akin to inspecting the classes of the objects instantiated in the stack. In our case, we have two stacks: one for UA $\Rightarrow$ WE and another for WE $\Rightarrow$ FE. For the purposes of the theorem, having these two stacks visible is enough: we review each of their frames and verify that neither used FE. In the case of the second theorem, FE was actually used, but those proofs can be modified to use WE instead, making everything perfectly sound.

The situation becomes more obscure because the sixth exercise introduces a new variant of UA, let us call it UA', and asks us to prove that UA' $\Rightarrow$ FE. This forces us to revisit the stacks and reprove the results that relied on UA so that they use UA' instead. It is an excessively tedious job because it requires reviewing several proofs and modifying the necessary ones. Moreover, all that verification would remain purely in our heads; it is very difficult to write down. This convinced me that I had to tag each of the previous results with UA, FE, and WE, so that a simple inspection of the dependency tree (the stack) would make it evident where each axiom is used and where it is not. I did exactly that, and I proved that the effort of tagging was absolutely worth it.

The finishing touch came with the chapter's final exercise, which introduces the "naive" variant of FE, which I called NE. The exercise asks us to prove that NE $\Rightarrow$ FE. The obvious strategy is to prove NE $\Rightarrow$ WE and WE $\Rightarrow$ FE. To do this, we must review the first stack again. Only this time, it is easy because the results are already tagged, and it is obvious which proofs need to be modified.

Without all this machinery, the proof of the main theorem UA $\Rightarrow$ FE and the solutions to the two exercises would have been obscure, and their writing insufficient and inelegant.
