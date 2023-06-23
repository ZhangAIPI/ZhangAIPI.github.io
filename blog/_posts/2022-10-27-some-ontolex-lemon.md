---
layout: post
title: Some OntoLex-Lemon
date: 2022-10-27
tags: linguistics ssw
giscus_comments: true
---

Originally posted as part of the [CMPE58H](https://cmpe.boun.edu.tr/courses/cmpe58h) course at `https://medium.com/@furkanakkurt7642/some-ontolex-lemon-798779392f0a`.

---

OntoLex-Lemon<sup>[1](#references)</sup> is a model for representing lexicographical ontologies, _lemon_ being short for _lexicon model for ontologies_. It was developed because ontology languages, OWL and RDF(S), didn’t allow furnishing ontologies with linguistic information so a resource like [WordNet](https://wordnet.princeton.edu) wasn’t possible. They mention in their community report that "OWL and RDF(S) rely on a property [named] _rdfs:label_" to show a relation between a vocabulary element and its lexicalization. This single property is not in the least sufficient for a human language.<sup>[1](#references)</sup>

Thanks to OntoLex-Lemon, WordNet has powered so many NLP applications of English and made them possible. Many languages lack a wordnet as creation of one requires manual annotation of thousands upon thousands entries as well as consistent and accurate lexical data collection. Because human languages are results of the human brain, they share a lot in common and all of their needs can be fulfilled by a single lexicon model. Also, the OntoLex-Lemon model is open to extensions and its vocabulary can be augmented on an application basis. Human languages are very similar but since linguistic theories vary, the model has been made sure to be abstracted from specific theories.<sup>[1](#references)</sup>

<div class="row">
    <div class="col-sm mt-3 mt-md-0 text-center">
        {% include figure.html path="/assets/img/lemon-core-model.webp" title="Core Model" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Core Model
</div>

A representative image of the model is provided in their document, which I’ve provided just above. In the image, boxes represent classes, filled arrows represent object properties and non-filled arrows are for subclass relations. Main class of the model is _Lexical Entry_ which is further specialized into three: word, multiword expression and an affix (prefix, suffix, etc.). For a word example, we can represent the word _cat_ in [Turtle RDF Syntax](http://www.w3.org/TR/turtle) as the triple: _:cat a ontolex:Word_.<sup>[1](#references)</sup>

For more information, please see the community report, dated 5/10/2016.<sup>[1](#references)</sup>

## References

1. [https://www.w3.org/2016/05/ontolex/](https://www.w3.org/2016/05/ontolex)
