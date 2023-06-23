---
layout: post
title: Qualifiers among Triples
date: 2022-11-10 13:15:00 +0300
tags: ontology ssw
giscus_comments: true
---

Originally posted as part of the [CMPE58H](https://cmpe.boun.edu.tr/courses/cmpe58h) course at `https://furkanakkurt5204.gitlab.io/personal/ontology/2022/11/10/qualifiers-among-triples`.

---

Last week, we went over some ontologies brought up by our classmates. Browsing Toykan's ontology, [Ontology Lookup Service](https://www.ebi.ac.uk/ols/index) (OLS), the keyword _some_ had caught my eye as independent of the usual triples (subject, predicate and object). Reading this week's paper, _Wikidata: A large-scale collaborative ontological medical database_, I realized those are _qualifiers_ that we also see in Wikidata.

The paper mentions that Wikidata items have claims "in the form of triples". The subject refers to the item the claim is referring to. The predicate is used in place of the ontology concept _property_. Lastly, the object represents a value. Claims are then made more precise through _qualifiers_.

## Example Qualifier from OLS

The item [_Acetaminophen_](http://purl.obolibrary.org/obo/CHEBI_46195) has a relation: _has role_ <span style="color:purple">some</span> xenobiotic. _has role_ is the property; the purple part is a qualifier; _xenobiotic_ is the value (object).
