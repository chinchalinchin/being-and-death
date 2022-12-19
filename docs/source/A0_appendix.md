# Appendix 1: Propositional Calculus

In what follows, you will find the definitions and explanations for the author's [Markdown]() compliant variation of propositional calculus. This variant was adopted for ease of use.

## Definitions

- `P()` represents a predicate
- `#` represents the quantifier for existence
- `@` represents the quantifier for universality
- `!` represents negation
- `|` represents denotion
- `~` represents set membership
- `->` represents implication.
- `&` represents conjunction.
- `||` represents disjunction.
- `<->` represents logical equivalence
- uppercase letters, such as _A_ and _B_, represents sets. **NOTE**: `{}` also denote sets, when set builder notation is employed.
- lowercase letters, such as _a_ and _b_, represents unquantified, or indeterminate, set members
- `n(S)` represents the cardinality of a set _S_, i.e. its countability[^13]
- `[]` are placeholders to separate content, i.e. the "_comma_".

## Examples
- _for all x such that x satisfies P_ : `@ x | P(x)`
- _for not all x such that x satisfies P_: `~ [ @ x | P(x) ]`
- _there exists an x such that x satisifes P_ : `# x | P(x)`
- _there does not exist an x such that x satifies P_: `~ [ # x | P(x) ]`

**NOTE**: I have been careful to remove any linguistic ambiguities in the preceding that might arise through the conjugation of `to be`, i.e instead of saying _x is P_ we say _x satisfies P_. Notice we may phrase all of these forms in terms of existence, not Being. In logic, where precision is of the utmost importance, we be careful not to let our subjective intrepretation of Being influence our understanding of existence and universals.

## Negating A Universal Quantification



## Negating An Existential Quantification