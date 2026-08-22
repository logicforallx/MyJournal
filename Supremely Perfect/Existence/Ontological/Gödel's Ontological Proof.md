# Gödel's Ontological Proof


## Intro 

Gödel's ontological proof is a formal argument by the mathematician Kurt Gödel (1906–1978) for the existence of God. The argument is in a line of development that goes back to Anselm of Canterbury (1033–1109). A more elaborate version was given by Gottfried Leibniz (1646–1716); this is the version that Gödel studied and attempted to clarify with his ontological argument. --- From Wikipedia

## Original Formal Argument

$$
\begin{array}{rl}
\text{Ax. 1.} & \left(P(\varphi) \;\wedge\; \Box \; \forall x (\varphi(x) \Rightarrow \psi(x))\right) \;\Rightarrow\; P(\psi) \\

\text{Ax. 2.} & P(\neg \varphi) \;\Leftrightarrow\; \neg P(\varphi) \\

\text{Th. 1.} & P(\varphi) \;\Rightarrow\; \Diamond \; \exists x \; \varphi(x) \\

\text{Df. 1.} & G(x) \;\Leftrightarrow\; \forall \varphi (P(\varphi) \Rightarrow \varphi(x)) \\

\text{Ax. 3.} & P(G) \\

\text{Th. 2.} & \Diamond \; \exists x \; G(x) \\

\text{Df. 2.} & \varphi \text{ ess } x \;\Leftrightarrow\; \varphi(x) \wedge \forall \psi \left(\psi(x) \Rightarrow \Box \; \forall y (\varphi(y) \Rightarrow \psi(y))\right) \\

\text{Ax. 4.} & P(\varphi) \;\Rightarrow\; \Box \; P(\varphi) \\

\text{Th. 3.} & G(x) \;\Rightarrow\; G \text{ ess } x \\

\text{Df. 3.} & E(x) \;\Leftrightarrow\; \forall \varphi (\varphi \text{ ess } x \Rightarrow \Box \; \exists y \; \varphi(y)) \\

\text{Ax. 5.} & P(E) \\

\text{Th. 4.} & \Box \; \exists x \; G(x)
\end{array}
$$

## Translation of Individual Symbols From Wikipedia (25-1-16)

### Common Notation in Symbolic Logic:

- \( \varphi(x) \): "Object \( x \) has property \( \varphi \)"  
  (Notation for **First-order logic** predicates)

- \( \Rightarrow \): "Implies"  
  (Material **implication**)

- \( \forall x \): "For every \( x \)", or "for all \( x \)"  
  (**Universal quantification**)

- \( \exists x \): "There exists an \( x \)", or "for some \( x \)"  
  (**Existential quantification**)

- \( \neg \varphi \): "The **negation** of \( \varphi \)"  
  (i.e., not \( \varphi \))

### Modal Operators (used in **modal logic**):

- \( \Diamond \): "It is possible that...", or "in at least one **possible world**, it is true that..."  
  (Modal operator for **possibility**)

- \( \Box \): "It is necessary that...", or "in all **possible worlds**, it is true that..."  
  (Modal operator for **necessity**)

### Primitive Predicate in This Argument:

- \( P(\varphi) \): "Property \( \varphi \) is positive"  
  (Since it applies to properties, "being positive" is a **second-order logic** property)

### Derived Predicates (Defined in Terms of Other Predicates):

- \( G(x) \): "\( x \) is God-like". (**Definition 1**)

- \( \varphi \text{ ess } x \): "\( \varphi \) is an essential property of \( x \)"  
  (**Definition 2**)

- \( E(x) \): "Object \( x \) exists necessarily"  
  (**Definition 3**)


## Translation of Full Argument with Possible Justification

* **Axiom 1**: If \( \varphi \) is a positive property, and if it is necessarily true (true in all possible worlds) that every object \( x \) with property \( \varphi \) also has property \( \psi \), then \( \psi \) is also a positive property. 
   $$
   \begin{aligned}
   \text{Ax. 1.} & \quad \left(P(\varphi) \wedge \Box \forall x (\varphi(x) \Rightarrow \psi(x))\right) \Rightarrow P(\psi)
   \end{aligned}
   $$
   - It seems, it does not define what a positive property is. However, if a positive property means purely good property (property that is purely in accordance with a being/object), then Axiom 1 is valid. This is possibly because, if a positive property includes another property that is negative (purely good includes not good), then it is contradiction, which is logically impossible. For instance, if benevolence (good) is a positive property, and every benevolent being must also be wise, then wisdom is also a positive property (good property). 
   
&nbsp;
* **Axiom 2**: The negation of a property \( \varphi \) is positive if, and only if, \( \varphi \) is not positive.
   $$
   \begin{aligned}
   \text{Ax. 2.} & \quad P(\neg \varphi) \Leftrightarrow \neg P(\varphi)
   \end{aligned}
   $$
   - This is possibly because of the following:
      1. A property that is both positive and negative is logically impossible if Godel means positive as purely good property (property that is purely in accordance with a being/object), which means classical logic must apply (such as law of excluded middle, A or not A).
      2. So if P is not positive, then negation of P is positive or not P(not positive) is positive. [1]
      3. So if the negation of P is positive, then P is not positive, as not P(not positive) is positive. [1]
      4. Therefore, the negation of a property \( \varphi \) is positive if, and only if, \( \varphi \) is not positive. [2,3]
   * For example: If not being unwise (negation) could be a positive property, then being unwise is not a positive property. If being unwise is not positive, then not being unwise (negation) could be a positive property (because it implies wise which is a better). 
   
&nbsp;
* **Theorem 1**: If a property \( \varphi \) is positive, then it is possible that there exists an object \( x \) that has this property (in at least one possible world, there exists an object \( x \) that has this property).
   $$
   \begin{aligned}
   \text{Th. 1.} & \quad P(\varphi) \Rightarrow \Diamond \exists x \varphi(x)
   \end{aligned}
   $$
   - This is base from Axiom 1 that positivity is logically consistent as any property derived from a positive one must also be positive. Furthermore, from Axiom 2, there cannot be a contradiction between positive properties and their negations, which reinforces the logical consistency of positive properties. Therefore, if a property 𝜑 is positive, it must be possible that an object exists with that property in at least some world, because positive properties are logically coherent and do not lead to contradictions.  For instance, Imagine we are considering the property of "being omniscient" (having complete knowledge). This is a positive property, so according to Axiom 1 and Axiom 2, the logical consistency of this property implies that it must be possible for an object (e.g., a being) to have this property. In at least one possible world, there must be a being with the property of omniscience, because the property itself does not lead to any contradiction or impossibility in any world.
   
&nbsp;
* **Definition 1**: Object \( x \) has the godlike property if and only if for every property \( \varphi \), if \( \varphi \) is a positive property, then \( x \) has property \( \varphi \). (In other words, an object \( x \) is God-like if, and only if, \( x \) has all positive properties).
   $$
   \begin{aligned}
   \text{Df. 1.} & \quad G(x) \Leftrightarrow \forall \varphi (P(\varphi) \Rightarrow \varphi(x))
   \end{aligned}
   $$
   
&nbsp;
* **Axiom 3**: The property of being God-like is itself a positive property.
   $$
   \begin{aligned}
   \text{Ax. 3.} & \quad P(G)
   \end{aligned}
   $$
   - Base from definition 1, it means that a God-like being does not only have positive property but also have all positive properties or all of it's property is positive.

&nbsp;
* **Theorem 2**: It is possible that there exists a God-like object \( x \)  (in at least one possible world, there exists a God-like object \( x \)).
   $$
   \begin{aligned}
   \text{Th. 2.} & \quad \Diamond \exists x G(x)
   \end{aligned}
   $$
   - This is base from theorem 1, that in at least one possible world, there exists an object \( x \) that has positive property. Plus, from Axiom 3, the property of being God-like is itself a positive property.
   
&nbsp;
* **Definition 2**:  \( \varphi \) is an essential property of \( x \) if and only if object \( x \) has the property \( \varphi \) and –  for every \( \psi \), if object \( x \) has property \( \psi \) then it is necessary that for every \( y \) if object \( y \) has property \( \varphi \) then object \( y \) has property \( \psi \).
   $$
   \begin{aligned}
   \text{Df. 2.} & \quad \varphi \text{ ess } x \Leftrightarrow \varphi(x) \wedge \forall \psi \left(\psi(x) \Rightarrow \Box \forall y (\varphi(y) \Rightarrow \psi(y))\right)
   \end{aligned}
   $$
   - An essential property is a property that defines an object. If an object has this property, then this property and all other properties derive from it must logically follow from it, regardless of the world or object.
   - For instance:
      - Triangle is an essential property of x if and only if object x has the property of triangle and –  for every other property like "3 side property", if object x has property of "3 side" then it is necessary that for every y if object y has property of triangle then object y has property of "3 side".
      - Benevolent is an essential property of x if and only if object x has the property of benevolent and –  for every other property like "knowledge and capacity for good property", if object x has property of "knowledge and capacity for good" then it is necessary that for every y if object y has property of benevolent then object y has property of "knowledge and capacity for good".
   
&nbsp;
* **Axiom 4**: If a property \( \varphi \) is positive, then it is necessarily positive (positive in all possible worlds).
   $$
   \begin{aligned}
   \text{Ax. 4.} & \quad P(\varphi) \Rightarrow \Box P(\varphi)
   \end{aligned}
   $$
   - Base on definition 2, If property \( \varphi \) is positive, then "positive" is an essential property of \( x \) if and only if object \( x \) has the property "positive" and –  for every "positive", if object \( x \) has property "derived from positive" then it is necessary that for every \( y \) if object \( y \) has property "positive" then object \( y \) has property "derived from positive". In other words, if a property \( \varphi \) is positive, then it is necessarily positive (positive in all possible worlds) or a positive property is necessarily a positive property. This is possibly because, it is tautologically true or true by logical law of identity, which is necessarily true (Like A is A, all bachelors are unmarried men, triangle has three sides, etc are true in all possible worlds). 
   
&nbsp;
* **Theorem 3**: If \( x \) is God-like, then being God-like is an essential property of \( x \).
   $$
   \begin{aligned}
   \text{Th. 3.} & \quad G(x) \Rightarrow G \text{ ess } x
   \end{aligned}
   $$
   - This is possibly because,  a positive property is necessarily a positive property as we can see on the Axiom 4, plus the property of being God-like is itself a positive property as we can see on the Axiom 3, then God-like is an essentially a God-like or an essential property of \( x \).
   
&nbsp;
* **Definition 3**: An object \( x \) "exists necessarily" if and only if for every property \( \varphi \), if \( \varphi \) is an essential property of \( x \) then it is necessary that there exists an object \( y \) that has property \( \varphi \)
   $$
   \begin{aligned}
   \text{Df. 3.} & \quad E(x) \Leftrightarrow \forall \varphi (\varphi \text{ ess } x \Rightarrow \Box \exists y \varphi(y))
   \end{aligned}
   $$
   - The definition formalizes the idea of **necessary existence**: an object exists necessarily if its defining (essential) properties are guaranteed to exist in all possible worlds, and vice versa. If an essential property fails to exist in any world, the object \( x \) cannot exist necessarily
   - If \( x \) exists necessarily, then its essential properties exist in all possible worlds. If the essential properties of \( x \) exist in all possible worlds, then \( x \) exists necessarily.
   - For example:
      - "Laws of logic" exists necessarily if its defining (essential) properties, such as law of identity, are guaranteed to exist in all possible worlds, and vice versa. It means law of identity or A must be A, triangle must be a triangle, etc must follow in all possible worlds if "Laws of logic" exists necessarily, and vice versa.
      - "Mathematical Laws" exists necessarily if its defining (essential) properties, such as basic arithmetic, are guaranteed to exist in all possible worlds, and vice versa. Its means basic arithmetic such as  1 + 1 is 2, 2 + 3 is 5, etc must be true in all possible worlds if "Mathematical Laws" exists necessarily, and vice versa.
      - "Positive or God-like" object exists necessarily if its defining (essential) properties, such as all good, all knowing, all powerful, etc are guaranteed to exist in all possible worlds, and vice versa. Its means all good, all knowing, all powerful, etc exist in all possible worlds if "Positive or God-like" object exists necessarily, and vice versa.
   
&nbsp;
* **Axiom 5**: "Necessary existence" is a positive property.
   $$
   \begin{aligned}
   \text{Ax. 5.} & \quad P(E)
   \end{aligned}
   $$
   - As we can see on the definition 3, the axiom 5 means that if the object's defining (essential) properties are guaranteed to exist in all possible worlds, then that object exists necessarily, and vice versa, which means it is a positive property (purely good property  or a property that is purely in accordance with a being/object). This is possibly because of the following:
      1. Necessary existence is a property that is purely in accordance with a being/object. *For without necessary existence, an object cannot have properties at all or in all possible worlds, which contradicts or not in accordance to an object that has property in all possible worlds.
      2. If a positive property means property that is purely in accordance (not contradicting) with a being/object.
      3. Then, "Necessary existence" is a positive property. [1,2]
      
&nbsp;
* **Theorem 4**: It is necessary (true in all possible worlds) that there exist an object \( x \) that has the God-like property. 
   $$
   \begin{aligned}
   \text{Th. 4.} & \quad \Box \exists x G(x)
   \end{aligned}
   $$
   - This is possibly because of the following:
      * **Theorem 2**: It is possible that there exists a God-like object \( x \)  (in at least one possible world, there exists a God-like object \( x \)).  
      * **Theorem 3**: If \( x \) is God-like, then being God-like is an essential property of \( x \): This is the object that has all positive properties or all of it's property is positive (Definition 1).
      * **Axiom 5**: "Necessary existence" is a positive property.
      * **Therefore,**  It is necessary that there exist an object \( x \) that has the God-like property. 
   
&nbsp;
## Computationally Verified Versions (According to Wikipedia as of 25.1.13)

Christoph Benzmüller and Bruno Woltzenlogel-Paleo formalized Gödel's proof to a level that is suitable for [automated theorem proving](https://github.com/FormalTheology/GoedelGod) or at least computational verification via [proof assistants](https://github.com/FormalTheology/GoedelGod). The effort made headlines in German newspapers. According to the authors of this effort, they were inspired by [Melvin Fitting's book](https://www.amazon.com/Mathematical-Logic-Philosophical-Philosophy-ebook/dp/B0077ZY9KY).

In 2014, they computationally verified Gödel's proof (in the [above version](http://page.mi.fu-berlin.de/cbenzmueller/papers/C40.pdf)). They also proved that this version's axioms are consistent, but imply modal collapse, thus confirming Sobel's 1987 argument. In the same paper, they suspected Gödel's original version of the axioms to be inconsistent, as they failed to prove their consistency.

In 2016, they gave an automated proof that the original version implies `◊ ◻ ⊥`, i.e., is inconsistent in every modal logic with a reflexive or symmetric accessibility relation. Moreover, they gave an argument that this version is inconsistent in every logic at all, but failed to duplicate it by automated provers. However, they were able to verify Melvin Fitting's reformulation of the argument and guarantee its consistency.

### References
1. Benzmüller, Christoph, and Woltzenlogel-Paleo, Bruno. *Automating Gödel's Ontological Proof of God's Existence with Higher-Order Automated Theorem Provers*. European Conference on Artificial Intelligence (2014). [PDF Link](http://page.mi.fu-berlin.de/cbenzmueller/papers/C40.pdf).
2. Benzmüller, Christoph, and Woltzenlogel-Paleo, Bruno. *The Inconsistency in Gödel's Ontological Argument: A Success Story for AI in Metaphysics*. International Joint Conference on Artificial Intelligence (2016). [PDF Link](http://www.ijcai.org/Proceedings/16/Papers/137.pdf).
3. Benzmüller, Christoph, and Fuenmayor, David. *Types, Tableaus and Gödel's God in Isabelle/HOL*. Archive of Formal Proofs (May 2017). [Link](https://www.isa-afp.org/entries/Types_Tableaus_and_Goedels_God.html).


## Scrutiny

* For axiom 1 and 2, is it not possible that good (postive) includes not good (not positive) at the same time but in different context? For instance, if its possible that many parts of that property is good and other part of that property is not good. If so, is it truly a logical contradiction? If not, then positive can includes not positive, right?
   - Positive with negative is not purely positive, it cannot be considered positive only in absolute sense, it is both positive and negative but in different context or parts. If Godel is talking about purely positive, then it will still not include flaws or defect (not positive), right? if an purely property includes another property that is negative (purely good includes not good), then it is contradiction in the same context, which is logically impossible, right?

* Some argue that good includes not good if its necessary for the greater good. For instance, removing some parts of the body for some cases is necessary for survival. If so, good includes not good, which means that positive includes not positive, right? If so, Axiom 1 is invalid, right? If so, does the argument fails by this?
   - In your example, the appears "not-good" act (e.g., amputation) is only justified because it serves a higher positive property (e.g., preserving life). Therefore, the appears "not-good" action can be instrumentally good, not inherently positive or negative. 
   - Furthermore, instrument or way is different from property. While the way can appear as not good is some sense, but the inherent reason (like will, intention, or characteristic) that cause that is good/positive. An inherent will, intention, or characteristic can be considered property of something/someone. So it still considered a positive property, does it not? The act of removing a body part might be "not good" as an action in isolation. However, if the intention behind the act is to save a life, this intention embodies benevolence or compassion, which are inherently positive properties, does it not?

* Ambiguity of Positive Properties: Gödel never explicitly defines what constitutes a "positive property." The argument hinges on the assumption that positivity is an intuitively understood and objective notion, but critics argue that it is subjective or culturally influenced.
   - If positive property means purely good or purely in accordance with a being/object, then it is demonstrated above that the conclusion will follow, right?

* Dependency on Modal Logic: Gödel's proof heavily relies on modal logic (S5 specifically), which is not universally accepted. Critics argue that the validity of the proof depends on the correctness of this logical framework.
   -  A is A. S5 is tautologically correct or true by logical law of identity. If something necessary exist in at least some possible world, then it is necessary (exist in all possible worlds). Like if laws of logic is necessary and can exist in at least some possible world, then it is not only possible but necessary. So If something is possibly necessary, then it is necessary, which is the implication of modal logic S5, right?

* **Modal Collapse From Sobel:** Jordan Howard Sobel, showing that if the axioms are accepted, they lead to a "modal collapse" where every statement that is true is necessarily true. Here is Sobel’s proof of modal collapse: first, we prove that all of God’s properties are necessarily instantiated. Suppose that a Godlike being exists and has property F. Call the Godlike being j. We know, from theorem 2, that G is the essence of j. This means that G necessitates all of j’s actual properties. Since j has F, G must necessitate F, and since G is necessarily instantiated, F must also be necessarily instantiated. In fact, the conjunction of F and being identical to j is necessarily instantiated: so j has F in every possible world. For the proof of modal collapse, let Q be some arbitrary truth. We will show that □Q. We know, from Gödel’s theorem 3, that a Godlike being exists: call it j again. So, we know G(j). We also know, from theorem 2, that G is the essence of j. This means that G necessitates all of j’s actual properties. Since Q is true, j has the property of being such that Q (i.e., from (Q&j = j), we can deduce that j has the property x̂[Q&x = x]). Thus, being G must necessitate being such that Q. Since G is instantiated in every world, it follows that something is such that Q is true in every world. Hence, □Q.
   - The problem on the argument is in the notion that "Since Q is true, j has the property of being such that Q". It does not follow, even in the actual world, if horse and lion exist, does it mean that the lion is the property of horse?
   * Let say this is what Sobel means:
   1. Let say Q is arbitrary or contingent truth.
   2. If G exist in all possible worlds, then it exist where Q exist, and vice versa. [1]
   3. So Q is part of or included in G existence in at least some possible world . [2]
   4. But G exist in all possible world.
   5. So Q (contingent truth) exist in all possible world also. [3,4]
   * So as we can see, it will produce modal colapse, right?
   - Q is part of or included in G existence in at least some possible world is different from Q is part of or included in G existence in all possible world, right? Let say I exist in a virtual world as a character of a game and the spaghetti dragon exist on that also. If I exist in the actual world also as an actual, does it mean that the spaghetti dragon exist in the actual world also? it does not follow, right? If its shown in the basis that Q is part of or included in G existence in all possible world, then it is valid, however, basis 3 does not shown as that, right?
   * In 2014, they computationally verified Gödel's proof (in the above version). They also proved that this version's axioms are consistent, but imply modal collapse, thus confirming Sobel's 1987 argument. How about this?
   - As far as we researched, computationally verified system will only check if logic will follow from the basis or axiom. However, it is not checking weather the axiom is justified or valid, itself. So it is not enough to say that something is verified by this, isn't it?

* In 2016, they gave an automated proof that the original version implies `◊ ◻ ⊥`, i.e., is inconsistent in every modal logic with a reflexive or symmetric accessibility relation. Moreover, they gave an argument that this version is inconsistent in every logic at all.
   - From the axiom 1 and 2 of Godel, it shows that positive properties cannot have negative, which implies it cannot have falsehood properties, which means falsehood object or subject x is not possible. So why it will produce falsehood if that's the case?
   - Plus, there are no justification why automated proof that the original version implies `◊ ◻ ⊥`, i.e., is inconsistent in every modal logic with a reflexive or symmetric accessibility relation and also no justification on why it is inconsistent in every logic at all, right?
   - Furthermore, is it not modal logic with a reflexive or symmetric accessibility relation system a questionable logic? is it truly logic? Does a possible world can truly access each other? 

## Conclusion

**In summary,** Is it necessary (true in all possible worlds) that there exist an object \( x \) that has the God-like property?

## References

* Translation from Mind-Maatters-AI [Mind Matters AI: Gödel Says God Exists and Proves It](https://mindmatters.ai/2021/06/godel-says-god-exists-and-proves-it/): 

* Wiki pedia [Wiki pedia](https://en.wikipedia.org/wiki/G%C3%B6del%27s_ontological_proof)
