---
layout: post
title: Signing Lemon
date: 2022-11-02 20:42:50 +0300
tags: linguistics ssw
giscus_comments: true
---

Originally posted as part of the [CMPE58H](https://cmpe.boun.edu.tr/courses/cmpe58h) course at `https://furkanakkurt5204.gitlab.io/personal/linguistics/2022/11/02/signing-lemon`.

---

Last week, we talked about a possible ontology for sign languages (SL) during the 58H project proposals. I searched if there were any attempts at it. There is a paper in 2022 working on just that, [Towards a new Ontology for Sign Languages](https://aclanthology.org/2022.lrec-1.423) (Declerck, LREC 2022). In the paper, the authors talk about their ongoing work on including multimodal lexical data in [the OntoLex-Lemon framework](https://www.w3.org/2019/09/lexicog) with the result of [the first edition of their ontology](https://github.com/Declerck/sl-onto). An excerpt from the ontology is at the end.

Integrating multimodality of natural languages, like sign languages, into the framework of OntoLex-Lemon is quite on point. Although modalities may differ between spoken and signed languages, they share quite a lot and can be represented with a single model.

Still, _sign language_ represented quite a challenge for them, as it's quite concentrated on the movements of a person, since the framework was created specifically for written or phonetic representations of lexical data. Starting the work, they realized that a comprehensive study of "LD (Linked Data) compliant description of the constitutive elements of sign languages" is necessary. They also mention that discussions regarding "the representation of multimodal language data", first focus being on SLs, started in [the “Ontology Lexica” W3C Community](https://www.w3.org/community/ontolex), a good sign.

## Excerpt from the ontology

```turtle
sldc:BackAndForth
  rdf:type sldc:PathMovement ;
  dc:source "https://asl-lex.org/" ;
  rdfs:label "\"back and forth\""@en ;
.
sldc:BackOfHand
  rdf:type sldc:Location_DGS_Vertical ;
  dc:source "DGS" ;
  rdfs:label "\"back of the hand\""@en ;
.
```
