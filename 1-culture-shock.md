---
layout: default
title: Culture Shock - First Impressions of the HoTT Book
---
## **Culture Shock: First Impressions of the HoTT Book**

Approaching Homotopy Type Theory (HoTT) requires a certain level of mathematical maturity; to give meaning to the formalization of the theory, one must first pass through a naive approach to gain intuition about its underlying ideas. However, navigating this intuitive introduction is a demanding and tedious process, primarily because the exposition is riddled with gaps, ambiguities, and analogies.

For a reader with a formal mathematical background, the book holds immediate appeal because it does not stop to explain basic mathematical concepts, assuming the reader is already equipped to handle them. Yet, this is exactly where a profound stylistic clash occurs.

### **The Inverted Logical Sequence**

The greatest difficulty in reading the HoTT book lies in how it inverts the traditional logical sequence. In classical mathematical texts, the sequence of definition, lemma, theorem, and corollary makes it explicitly clear where the argument begins and what is derived from what.

The HoTT book abandons this structure. In an attempt to motivate the subject, the text presents a long enunciation of half-explained concepts in a style forcibly divorced from standard mathematical literature, heavily masked by symbolic notation. This creates a disorienting experience where it is unclear when a provable result is being informally anticipated to create a more fluid narrative. This confusion is exacerbated by the use of words like "principle," which blur the boundaries between the theory's axioms and the consequences that can actually be derived from them.

### **The Danger of "Intuitive" Introductions**

When a text relies on informal tone rather than strict mathematical definitions, the reading naturally relaxes, making it far more likely for errors to slip by unnoticed.

Because the text does not clearly separate what is a statement, what is a proof, and what is an amicable explanation, the chances for confusion multiply. A prime example is the book's loose syntax in early definitions. For instance, writing an expression as $\mathsf{rec}(C,g,(a,b))$ instead of the formally correct $\mathsf{rec}(C,g)((a,b))$—given that $\mathsf{rec}(C,g)$ is a function with a domain in $A\times B$—forces the reader to stop and question whether they are misunderstanding the theory or merely looking at a typographical error. The burden of parsing these ambiguities falls entirely on the reader, who must remain hypersensitive to details that the informal tone attempts to gloss over.

### **A Poorly Signposted Trail**

Ultimately, reading the HoTT book feels like embarking on a trekking route with terrible signposting. The landscape it reveals is undeniably beautiful, but the path is incredibly easy to lose. It leaves the reader in a constant state of duality: half enjoying the breathtaking views of a new logical foundation, and half cursing the trail.
