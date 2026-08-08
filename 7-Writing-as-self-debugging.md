---
layout: default
title: Writing as Self-Debugging - The Syntax of Thought
---

There is a profound connection between the physical act of writing and the cognitive process of understanding. Writing is like squirting dish soap on a tire: it makes the hidden leaks and holes in our reasoning blindingly obvious. Writing is not merely documentation; it is a vital mechanism for self-debugging.

This reality becomes painfully clear when attempting to formalize mathematics in Type Theory. Human parsing limits are severely tested by the need to construct mental Abstract Syntax Trees (ASTs) from linear, one-dimensional text. In traditional mathematical notation, natural language connectors—like "then" or "it follows that"—separate hypotheses from conclusions, providing structural rest stops for the mind. In HoTT, these logical implications must be expressed strictly as functions, collapsing the vertical structure of a deductive argument into a dense, horizontal string of symbols.

The contrast is stark when compared to Gentzen's 2D logical notation, which separates premises and conclusions with horizontal bars. This verticality makes the underlying deductive rules explicit and clearly distinguishes the object language from the meta-language. However, because programming environments and text editors are inherently one-dimensional, we are forced to compress these structures, adding to the cognitive load.

The discipline required to write out every detail—such as manually subscripting equalities with their underlying types, or fully expanding a double induction—exposes the fragile nature of our intuition. The difficulty often lies not in grasping the macro-concepts, but in the micro-reasoning: mechanically articulating simple branching logic without relying on informal assumptions. Emulating the rigors of a type checker on paper forces us to slow down, confronting the errors we naturally gloss over and ultimately forging a deeper, more robust mathematical understanding.
