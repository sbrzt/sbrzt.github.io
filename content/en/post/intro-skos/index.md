---
title: SKOS and Roll
subtitle: Navigating Knowledge with Taxonomy
summary: A crash course on Simple Knowledge Organization System (SKOS).
date: 2023-12-21
math: false
image:
  placement: 2
  caption: '"Linked Open Data", deepai.org'
slides: introduction-lod-it
draft: true
---

## What is a controlled vocabulary?
A controlled vocabulary is a list of standardized terms that can be used for indexing, cataloguing, and retrieving information during activities related to navigation and search. In particular, a controlled vocabulary defines standardized terms that are used in a specific application domain, maps them to variants and synonyms, and organizes them in logical structures ordered according to specific conceptual categories. A concrete example of a controlled vocabulary would be the subject index used in a library to describe its bibliographic resources.

```markmap
- Pet
  - Mammal
    - Dog
    - Cat
    - Ferret
  - Rodent
    - Mice
    - Rat
    - Gerbil
  - Reptile
    - Turtle
    - Lizard
    - Snake
```

We developed three controlled vocabularies to model the roles held by Aldo Moro, the subjects of his works, and their types. Similarly to the classification scheme Iconclass, the concepts contained in our vocabularies – being for the most part long and complex – are identified by alphanumeric codes and accompanied by textual labels written in natural language that document their meaning (for example, the term `role01` denotes "Aspiring delegate of Catholic Youth", `role02` denotes "Student", and so on).

The following figure illustrates an example of how we structured the roles vocabulary. In particular, the vocabulary is made up by:
- Information about the vocabulary itself, such as its documentation, access point (also known as top concept), and metadata;
- The top concept, which acts as the access point of the vocabulary that gathers all the other concepts under itself. The top concept is identified by natural language labels, documented by its definition and explanatory notes, and connected to the other concepts in the vocabulary;
- A series of concepts that make up the vocabulary. Each concept is identified by natural language labels, documented by a description, and characterized by relations with other vocabulary concepts and external resources as well.

## What is SKOS?
SKOS is not just a fancy acronym; it's a common data model for knowledge organization systems such as thesauri, classification schemes, subject heading systems, and taxonomies. Using SKOS, a knowledge organization system or controlled vocabulary can be expressed as machine-readable data. Once expressed in SKOS, data can then be exchanged between computer applications and published in a machine-readable format on the web. Think of it as a translator that helps computers and humans communicate more effectively about the relationships between different terms and concepts.

### Concepts
At the heart of SKOS are concepts. They represent the abstract objects that constitute a knowledge organization system. "Abstract object" may seem as a very vague notion, and in a way it is. A concept can be virtually anything that can exist in the human mind: a pet, a role interpreted in a theatre play, an architecture style, a type of amino acid. It just needs two things: to be abstract, and to be separate from the term(s) identifying it.

In SKOS, a concept is instantiated by identifying it with a Uniform Resource Identifier (URI) and asserting that it is of type `skos:Concept`.

```turtle
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix ex: <http://www.example.com/> .

ex:cat a skos:Concept .
```

### Labels
In SKOS, a label is the element that is the descriptor of a concept, and consists in a textual label written in natural language. Simply put, it is the text "Cat" for the concept of cat. It may seem obvious, even silly, but keep in mind that in knowledge organization and computer science taking things for granted is prohibited. Giving a readable label to a piece of data means everything: to you (the creator) and to other agents (researchers, softwares, and so on).

In SKOS, there are three ways to attach labels to a concept:

- `skos:prefLabel`: a preferred label for the concept (e.g. "Cat");
- `skos:altLabel`: an alternative label for the concept, e.g. a synonym, abbreviation or acronym ("Kitten");
- `skos:hiddenLabel`: a variant of some sort (a misspelling, an outdated form, etc.) that we want to be accessible for indexing by applications, but not visible for the human user (e.g. "katze").

```turtle
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix ex: <http://www.example.com/> .

ex:cat a skos:Concept ;
    skos:prefLabel "Cat"@en ;
    skos:prefLabel "Katze"@de ;
    skos:altLabel "kitten"@en ;
    skos:hiddenLabel "katze"@de .
```

### Semantic relationships
In a knowledge organization system, it's important to establish relationships between concepts. For example, if you are creating a vocabulary about literary genres, you want to represent somehow the fact that "Slasher" is a sub-genre of "Horror" and is related to "Thriller".

In SKOS, there are many relationships that can be expressed between concepts:
- hierarchical
  - `skos:broader`
  - `skos:narrower`
  - `skos:broaderTransitive`
  - `skos:narrowerTransitive`
- associative
  - `skos:related`

the relationship is transitive if concept A is related to concept B. Concept B is related to concept C. That implies that concept A is related to concept C.

Important to not mix hierarchical and associative relationships: if two concepts are in broader/narrower relationships between each other then they are explicitly in hierarchical relationships, therefore, don’t need to be related via skos:related property. Similarly, if two concepts are related via skos:related property we can infer that they are related in some other distinct hierarchical relationships (e.g. a concept representing a tangible object is related to a concept describing a method that uses that object).

```turtle
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix ex: <http://www.example.com/> .

ex:cat a skos:Concept ;
  skos:prefLabel "cat"@en ;
  skos:prefLabel "Katze"@de ;
  skos:altLabel "kitten"@en ;
  skos:narrower ex:wildcat .

ex:wildcat a skos:Concept ;
  skos:prefLabel "wildcat"@en ;
  skos:broader ex:cat .
```

### Concept Documentation
SKOS defines properties to add human-readable documentation about concept. It is strongly recommended to add documentation properties for each concept.

The following properties can be used:

- skos:note - general documentation purposes
- skos:scopeNote - partial information about the intended meaning of a concept
- skos:definition - complete explanation of the intended meaning of a concept
- skos:example - example of the use of a concept
- skos:historyNote - significant changes to the meaning or the form of a concept
- skos:editorialNote - administrative information for editors
- skos:changeNote - changes for the purposes of administration and maintenance

### Mapping concepts
Concepts can be semantically reconciled to concepts in different Concept Schemes (=vocabularies) or LOD resources on the Web for the purposes of data interoperability and integration.

SKOS provides the following properties to link concepts with external resources:

- skos:exactMatch - the local term is an exact match to a term in an external vocabulary
- skos:closeMatch - not exact but close match to a term in an external vocabulary
- skos:broadMatch - the local term has a broader match in an external vocabulary
- skos:narrowMatch - the local term has a narrower term in an external vocabulary
- skos:relatedMatch - the related term in an external vocabulary

```turtle
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix ex: <http://www.example.com/> .

ex:europeanWildcat rdf:type skos:Concept;
    skos:prefLabel "European wildcat"@en;
    skos:exactMatch <https://www.wikidata.org/wiki/Q148833>;
    skos:broadMatch <https://www.wikidata.org/wiki/Q43576>.
```

### Concept Scheme
As mentioned above, CV forms a schema of data descriptors. Therefore SKOS introduces a Concept Scheme class to express the notion of CV itself. Concepts are compiled in one Concept Scheme with an explicitly defined scope.

The following statements define the purpose and usage of Concept Scheme class:

skos:ConceptScheme is a class for representing a controlled vocabulary.
Concepts have to be linked to ConceptScheme via skos:inScheme property.
skos:hasTopConcept is used to define entry points of a hierarchy.
Metadata about Concept Scheme can be expressed using Dublin Core properties such as dct:creator, dct:contributor, dct: title, dct:rightHolder …

```turtle
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix ex: <http://www.example.com/> .
@prefix dct: <http://purl.org/dc/terms/> .

ex:animalsVocabulary rdf:type skos:ConceptScheme;
  dct:title "Animals Vocabulary"@en;
  skos:hasTopConcept ex:animals.

ex:animals rdf:type skos:Concept;
  skos:prefLabel "animals"@en;
  skos:prefLabel "Tiere"@de;
  skos:inScheme ex:animalsVocabulary;
  skos:topConceptOf ex:animalsVocabulary.
```

## Integrity Conditions
The SKOS Reference document includes several integrity conditions. Integrity conditions are statements that help determine whether or not given data (for example, a vocabulary) are consistent with respect to the SKOS data model. The purpose of SKOS integrity conditions is to encourage the construction of well-formed and consistent data and to promote interoperability between data represented in SKOS.
skos:ConceptScheme is disjoint with skos:Concept
This condition states that SKOS concept schemes, or groups of SKOS concepts, must not be on the same hierarchical level as SKOS concepts and vice versa. For example, in the veggie vocab, Vegetables is a skos:ConceptScheme. This means that Vegetables must not also be a skos:Concept and one of the concepts, like Lima Bean, may not be a skos:ConceptScheme.
skos:prefLabel, skos:altLabel and skos:hiddenLabel are pairwise disjoint properties
This condition states that no SKOS concept may be a member of more than one preferred label, alternate label, and hidden label.
A resource has no more than one value of skos:prefLabel per language tag
This condition states that no SKOS concept may have more than one preferred label for each language tag. For example, the concept summer_squash has the preferred label of “Summer Squash” in English and of “Cucurbita pepo” in Latin, and there may not be any other preferred labels in English or Latin.
skos:related is disjoint with the property skos:broaderTransitive
This condition states that no two SKOS concepts may be connected by both related and broader transitive relationships.
skos:Collection is disjoint with each of skos:Concept and skos:ConceptScheme
This condition states that SKOS collections, or labeled or ordered groups of SKOS concepts, must not be on the same hierarchical level as SKOS concepts and vice versa. For example, in the veggie vocab, Vegetables is a skos:Collection. This means that Vegetables must not also be a skos:Concept and one of the concepts, like Lima Bean, may not be a skos:Collection.
skos:exactMatch is disjoint with each of the properties skos:broadMatch and skos:relatedMatch
This condition states that no two SKOS concepts may be related by more than one of exact match, broader match, and related match.

## SKOS checklist
The future retrieval and search functionality will directly depend on the quality of CV, therefore, it is important to follow W3C recommendations for SKOS and check a vocabulary against the most common errors before using it in an application or publishing on the Web. The most common reasons for errors and bad practices are the following:
Omitted or invalid language tags (e.g.: skos:prefLabel “stone”@english)
Label conflicts (e.g. two concepts have the same preferred lexical label in a given language when they belong to the same concept scheme)
Orphan concepts (e.g. concepts without any associative or hierarchical relationships)
Undocumented concepts (concept should have one of the documentary notes)
Valueless associative relations
Omitted top concepts => no starting points of the concept hierarchy
Top concept having broader concepts
Creating a new concept for each synonym
Ambiguous label for a concept
Flat data (no hierarchy and associative relationships among concepts)

## Task: Model Music styles vocabulary
There are many styles used to categorize music. Consider the following styles: pop music, alternative rock, electronic music, punk rock, techno, rock, heavy metal.
Structure/draw your own vocabulary called “Music styles”
Model this vocabulary in a SKOS record:
model in RDF turtle format
add at least one documentary note for each concept
add labels in other languages
feel free to add more music styles
establish relationships to external LOD resources (dbpedia, wikidata)
save file in .ttl format
Visualize “Music styles” using web tool SKOS play. Try out different visualization types.

## Conclusion
In the ever-expanding digital landscape, effective knowledge organization is not a luxury but a necessity. SKOS stands as a reliable companion in this journey, providing a standardized and interoperable framework for expressing, sharing, and connecting knowledge. As you delve into the world of semantic web technologies, consider the power that SKOS brings to the table, opening up new possibilities for more efficient and meaningful information organization.

## References
- Harpring, Patricia. Introduction to controlled vocabularies: terminology for art, architecture, and other cultural works. Getty Publications, 2010.
- "SKOS: A Guide for Information Professionals", American Library Association, May 18, 2015. http://www.ala.org/alcts/resources/z687/skos (Accessed December 21, 2023). Document ID: df364f20-e2ad-4b0e-bc8e-9b4eff9bc777
- Ksenia Zaytseva and Matej Ďurčo (2020). Controlled Vocabularies and SKOS. Version 1.1.0. Edited by Matej Ďurčo and Tanja Wissik. DARIAH-Campus. [Training module]. https://campus.dariah.eu/id/D8d6OrLdpLlGRqBSQDVN0
- https://www.w3.org/TR/skos-primer/
- https://www.w3.org/TR/skos-reference/
- Mader, Christian, Bernhard Haslhofer, and Antoine Isaac. “Finding quality issues in SKOS vocabularies.” In International Conference on Theory and Practice of Digital Libraries, pp. 222-233. Springer, Berlin, Heidelberg, 2012.
- https://arxiv.org/ftp/arxiv/papers/2012/2012.02325.pdf
- https://fairvocabularies.github.io/examples/index.html

### Did you find this page helpful? Consider sharing it 🙌
