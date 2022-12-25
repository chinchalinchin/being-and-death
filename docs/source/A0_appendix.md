# Appendix I: Propositional Calculus

In what follows, you will find the definitions and explanations for the author's [Markdown]() compliant variation of propositional calculus. This variant was adopted for ease of use with webpages. Solutions exist for JavaScript based _LaTeX_ through libraries like [MathJAX](), and perhaps if the content of this work is ever completed to the author's satisfaction, he will refactor the syntax to be more in line with general conventions, but for now, this will suffice.

## Definitions 

### Symbols

- `P()` represents a predicate function
- `#` represents the quantifier for existence
- `@` represents the quantifier for universality
- `!` represents negation
- `|` represents denotion
- `~` represents set membership.
- `%` represents set exclusion.
- `->` represents implication.
- `&` represents conjunction.
- `v` represents disjunction.
- `<->` represents equivalence
- `=` represents equality
- `n(S)` represents the cardinality of a set _S_
- `[]` represent content separation, i.e. the "_comma_".

### Variables

- uppercase letters, such as _A_ and _B_, represents sets. 
    - `{}` also denotes a set.
- lowercase letters, such as _a_ and _b_, represents unquantified, indeterminate set members

## Propositions

TODO

### Excluded Middle

The law of the excluded middle simply states that it must either be the case that _P_ or its negation is true,

`P v !P`

For example, it cannot be the case that both propositions, _12 is even_ and _12 is odd_, are simultaneously true, because the concepts of even and odd are negations of one another with respect to the natural numbers (i.e., `odd <-> !even`). The set theoretic definitions of even and odd partition the natural numbers into non-overlapping sets, therefore a number must be contained in one or the other, but not both. This is what is captured in the law of the excluded middle.

### Quantification 

The following list shows how the English language can be mapped to the semantics of propositional calculus. Examples are given letting _x_ represent an indefinite but distinct bunny rabbit, the propositional function `P(-)` represent the predicate _is fluffy_, and _A_ represents the set of bunnies which have the property of being fluffy,

- (Q1) **Universal**: `@x | P(x)`
    - _General_: all _x_ that satisfy _P_
    - _Particular_: all bunnies are fluffy
- (Q2) **Negated Universal**: `![ @x | P(x) ]`
    - _General_:  not all _x_ satisfy _P_
    - _Particular_: not all bunnies are fluffy
- (Q3) **Existential**: `#x | P(x)`
    - _General_: atleast one _x_ exists that satisifes P_ 
    - _Particular_: some bunnies are fluffy
- (Q4) **Negated Existential**: `![ #x | P(x) ]`
    - _General_: no _x_ exists that satifies _P_
    - _Particular_: no bunnies are fluffy
- (Q5) **Universal Membership** `@x | x ~ A`
    - _General_: all _x_ in the set _A_
    - _Particular_: all things in the concept _fluffy bunnies_
- (Q6) **Universal Exclusion**: `@x | x % A`
    - _General_: all x not in the set _A_
    - _Particular_: all things not in the concept _fluffy bunnies_

## Sets


In the preceding, we have written `#x | P(x)` as a way of abstracting from the general proposition contained in the English sentence _there is an x that is P_ its purely formal characteristics. 

This formulation implies when a proposition is asserted, it is equivalent to applying a function to a subject, embodied in the term `P(x)`. When a subject is predicated by a descriptive clause, the predicate is transferred to the subject in its entirety, without meditation. This implies the subject _is_ the predicate. Rather, when we write `P(x)`, what we really mean is the subject _x_ has the property of having the predicate _P_. It is in their belonging to a set that objects are predicated by a property _P_. In mathematics, the thing which has a property has that property by virtue of its inclusion in a set. Sets are analogous to concepts; they are collections of objects that share the same property, and it is because they belong to this collection that predication is possible. In other words, when we write `#x | P(x)`, we are implicitly writing,

(D1) `#x | x ~ A & P(x)`

where _A_ is the set of things having the property _P_.

A set can be understood intuitively as a collection of objects. More formally, using the above definitions, a set _A_ can be defined through the symbolic proposition,

(D2) `#A | [ @x | x ~ A v A = 0 ]`

This translate roughly into the sentence: _there exists a set A such that for all x, x belongs to A or A is empty_.

### Axiom of Separation

In the first attempt to formalize the foundations of mathematics, before the concept of _sets_ was well defined in its lexicon, **Frege** proposed the following _axiom of separation_,

(A1.1) `#A | [ @x | x ~ A <-> P(x) ]`

This translate into _there exists an A such that for all x, if and only if x belongs to A, then x has the property of belong to that set.

**Zermelo** modified the _axiom of separation_ so as to remove the possibility of **Russell**'s paradox from the possibilities of its application in the following way,


(A1.2) `#A | [ @x | x ~ A <-> x ~ B & P(x)]`

Roughly speaking, this axioms says, _given a set B, there exists a set A such that for all x, if and only if x is a member of A, then x is a member of B and has the property of belonging to the set A_.

The existence of set _B_ must be given prior to the application of the axiom, or else 
TODO

### Axiom of Extensionability

TODO

### Theorems

1. Individuation: 

