---
layout: default
title: Mechanical Verification and Hidden Dependencies: The Case of UA and FE
---
I finally embarked on the (exhausting) task of tagging all the results that depend on the function extensionality (FE) axiom. What ultimately convinced me that I had to do it was an exercise in Chapter 4 that defines a seemingly equivalent variant of the univalence axiom (UA), which actually implies it, but is bogus. That is, if it were added as an axiom, it would lead to a contradiction.

I did this with the help of the imakeidx LaTeX package, which allowed me to implement my idea of tagging the results that depend on FE. For that, I simply need to add the \fe command to each result that requires it (\begin{thm}\fe, \begin{lem}\fe, etc.). With that package, I was able to compile an index of all those dependencies. My macro also makes the tag visible. Although it was a crazy amount of work, I am happy to have done it because making that explicit seems like a great help to understand things a bit more deeply.

![FE tag](/assets/Fe-tag.png)

And from this, something interesting emerged. When I decided that, to be sure the proof of UA ⇒ FE was correct, I built the reference tree of the proof and "verified" that those references did not use FE. How did I do it? I visited the leaves of the tree and made sure they didn't use FE. With that, I considered myself satisfied.

Now that I have all the results using FE tagged, I started a second verification: I had to check that no leaf was on the list. And shortly after starting, I found out it was wrong! I mean, I was using results (in the plural) that depend on FE! This, which slipped past me with the first method, became evident with the second.

It is not that I distrust the result. It is famous. The point is that I do not want the proofs in my notes to be wrong. The first error was easy to fix, but it requires an explanation that I had not discovered. The second one I found (right away), I have to think about, but it seems it is also easy to fix. I suppose by tomorrow I will have everything properly reviewed.

The moral is that mechanical checks (to call them somehow) discover things that are invisible to the human mind. I cannot help but link this to Lean and the other proof assistants, which are much more sophisticated and can handle the entire tree of a reasoning, or at least a very wide family of mathematical reasoning. This is something (relatively) new to me, and I find it fascinating.

As I said above, I do not distrust the veracity of UA ⇒ FE. What I see is that the proof requires much more work than it seems.
