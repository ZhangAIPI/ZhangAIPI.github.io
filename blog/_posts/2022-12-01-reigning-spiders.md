---
layout: post
title: Reigning spiders
date: 2022-12-01 13:00:00 +0300
tags: ontology ssw
giscus_comments: true
---

Originally posted as part of the [CMPE58H](https://cmpe.boun.edu.tr/courses/cmpe58h) course at `https://furkanakkurt5204.gitlab.io/personal/ontology/2022/12/01/reigning-spiders`.

---

I wondered about reasoners. W3C has the [Semantic Web Rule Language](https://www.w3.org/Submission/SWRL) (SWRL). Its syntax is similar to a notation I learned during CMPE260: [Extended Backus–Naur form](https://en.wikipedia.org/wiki/Extended_Backus%E2%80%93Naur_form) (EBNF). They define rules as axioms: `axiom ::= rule`.

The axioms have _antecedents_ (body) and _consequents_ (head), each composed of _atoms_. The rule may be defined as: `if antecedent, then consequent`. Basic atoms are of the forms:

1. `C(x)`: descriptions
    - Example: `ontolex:LexicalConcept(:hebûn_v_ku_sense_concept)`
2. `P(x, y)`: relations
    - Example: `skos:definition(:hebûn_v_en_sense_concept, "assets"@en)`
3. `sameAs(x, y)`: equalization
    - Example: `sameAs(foaf:Person, wd:Q5)`

Compositing atoms, one can construct very complex rules. One such rule would be, informally: parent(?x, ?y) ∧ parent(?y, ?z) ⇒ grandparent(?x, ?z).

Sidenote: In the specification, they mention that `sameAs` and `differentFrom` atoms do not increase the expressivity of the language since OWL and rules together without these atoms are capable of the same expressions.
