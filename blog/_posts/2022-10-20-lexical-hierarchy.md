---
layout: post
title: Lexical Hierarchy
date: 2022-10-20
tags: linguistics ssw
giscus_comments: true
---

Originally posted as part of the [CMPE58H](https://cmpe.boun.edu.tr/courses/cmpe58h) course at `https://medium.com/@furkanakkurt7642/lexical-hierarchy-85943cd4c0b6`.

---

WordNet is a lexical database of English. It groups its lexemes by synonymy and calls the groups _synsets_. There are more than a hundred thousand _synsets_.<sup>[1](#references)</sup> A synset also has some kind of a definition and optionally an example usage. It serves for many people as a dictionary and a thesaurus together.<sup>[2](#references)</sup> The structure of the grouping resembles a hierarchy where a word of a distinct conceptual idea has mostly a small set of connections.<sup>[1](#references)</sup> It seems to me even a single semantic conception of a surface form of a word should have more connections, it definitely does for a human brain; however, probably it’s not possible to create such a web just now.

Some third parties also consider WordNet itself as an ontology that’s used in computer science.<sup>[2](#references)</sup> [In another project](http://wordnet-rdf.princeton.edu/about), its database has been converted to [RDF](https://www.w3.org/RDF) and its data has been restructured according to [Lexicon Model for Ontologies](https://www.w3.org/2016/05/ontolex) of W3C, making it a more accurate ontology.

I wonder if WordNet can be used to _semanticize_ the web. Language learning in a semantic web would be helpful as there would be applications that would show a word’s translation in the context of the paragraph, not just the most immediate usage. Even translations of whole sentences could be done, as semantic information would definitely help a machine translation tool to more accurately do its job. I believe the convenience it would provide would make a lot of people interested in its applications. Many people can’t find time to learn a language, even though they want to for their career, as a heritage language, or just as a hobby. Duolingo just taps into this and helps many people learn a language in small bites. Recently, I started using it "actively" _again_.

As an example application that could use WordNet, I know of an extension, [Toucan](https://jointoucan.com), that changes the words in a text to a desired language. Semanticization of web would make this extension a whole lot better, while making the process of adding other languages to the extension a whole lot easier.

## References

1. [WordNet](https://wordnet.princeton.edu)
2. [WordNet - Wikipedia](https://en.wikipedia.org/wiki/WordNet)
