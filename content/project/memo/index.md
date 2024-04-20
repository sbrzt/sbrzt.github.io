---
title: Medieval Manuscript Ontology (MeMO)
summary: The Medieval Manuscripts Ontology (MeMO) is an OWL 2 DL ontology that aims to provide a framework for the formal description of the collection of medieval codices and manuscripts. It has been developed in the context of Progetto IRNERIO, according to certain requirements and with the possibility to extend it for representing similar resources that exist in other collections.
tags:
  - Knowledge Management
  - Data Documentation
date: '2020-03-20T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Medieval manuscript. deepai.org
  focal_point: Smart

url_code: 'https://w3id.org/irnerio/ontology/memo'
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

MeMO, the Medieval Manuscripts Ontology, is an OWL 2 DL ontology that aims to provide a framework for the formal description of the medieval codices and manuscripts described in the Project IRNERIO catalogue and the relations that exist between them. It is centered on a set of concepts (codex, manuscript, folio, text and gloss), which have been precisely defined via the Functional Requirements for Bibliographic Records (FRBR) standard in order to model such complexity in an accurate and logically consistent structure. The model thus becomes able to cover multiple use cases and scenarios in proportion to how many requirements have been adequately met.

While developing MeMO, a high priority has been given to the goal of reaching a sound balance between precision (to satisfy the user’s needs) and coverage (to ensure a certain degree of extensibility and reuse) of the model. Ultimately, the idea behind the development of MeMO has been to provide a data model for representing the aforementioned collection of medieval codices and manuscripts according to certain requirements and with the possibility to extend it for representing similar resources that exist in other collections.

FRBR allows a holistic perspective about the resource, on multiple levels of conceptualization, by breaking down the semantic and conceptual ambiguities related to objects created by human hands into different but related and layered concepts and by allowing the description of an artifact and its relations with other entities to be more expressive, precise and dynamic. Nonetheless, FRBR has some limitations. Even though the definitions of its concepts are quite straightforward, FRBR is not easily understood by the common user, who finds the terms work, expression, manifestation and item not very clear.

According to FRBR, any object (such as a manuscript, for example) has to be described by taking into consideration all the four levels in order to have a complete overview of it. This multi-leveled conceptualization is difficult for an average user to comprehend, because it is much more intuitive to expect the concept of that object to exist at a single FRBR level. In order to avoid this issue without giving up the expressivity of FRBR, a good solution is to place that object at the level that is deemed more appropriate in relation to the scenario taken into consideration.

This approach has been used systematically for the FRBR-aligned Bibliographic Ontology (FaBiO) (Peroni and Shotton 2012), with which MeMO has been aligned. Being an ontology focused on entities that are published, textual in nature, and/or referred to by bibliographic references, FaBiO defines its own set of entities that are subclasses of the original FRBR entities by taking advantage of the FRBRcore RDF vocabulary (FRBRcore, http://purl.org/vocab/frbr/core#). In order to embrace this approach and be consistent with the scenarios that are present in the case study, MeMO reuses FaBiO interpretations of FRBR entities as superclasses of its entities. In particular: manuscript, text and gloss are conceptualized as subclasses of fabio:Expression (since they are carry a content and are not inherently related to a precise format), while codex and folio are conceptualized as subclasses of fabio:Manifestation, since they carry a format that functions as a container for both text and glosses, and thus for manuscripts as well.