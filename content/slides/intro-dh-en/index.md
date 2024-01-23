---
title: The Literacy of Now
summary: A soft introduction to Digital Humanities
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2022-12-31T00:00:00Z'
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: white
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: github-light
---

# A Literacy of Building (part 1)

#### A soft introduction to Digital Humanities and digital research projects 

Sebastian Barzaghi

[sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it)

[https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527)


---

## Information technology is structural
Information technology is systemic, embedded in our societal structures, especially in scientific research

It is used to collect, present, analyze, and draw conclusions from data

It also encourages an increasing collaboration among professionals specialized in very diverse fields

<div class="footer">
  Goble, C., & De Roure, D. (2009). Data Intensive Computing: The Fourth Paradigm of Scientific Discovery. ISBN: 978-0-9825442-0-4
</div>

---

## This is also valid for the Humanities
Availability of digital resources and software tools to support:

* existing research questions
* existing methodologies
* new research questions
* new methodologies

<div class="footer">
  Borgman, C. L. (2010). The digital future is now: A call to action for the humanities. Digital humanities quarterly, 3(4). Retrieved from https://escholarship.org/uc/item/0fp9n05s
</div>

---

## Enter Digital Humanities
A rapidly growing field exploring the potential of digital methods and techniques in humanities research projects

Coined in the early 2000s, the term describes a multitude of academic realities working at the interface between technology and the humanities

Still difficult to define

<div class="footer">
  Kirschenbaum, M. G. (2016). What is digital humanities and what’s it doing in English departments?. In Defining digital humanities (pp. 211-220). Routledge. http://dx.doi.org/10.1632/ade.150.55 
</div>

---

## A double definition
Kathleen Fitzpatrick offers an insightful definition:

> […] a nexus of fields within which scholars use **computing technologies to investigate the kinds of questions that are traditional to the humanities**, or […] ask traditional kinds of humanities-oriented questions about computing technologies.

<div class="footer">
  Fitzpatrick, K. (2012). The humanities, done digitally. Debates in the digital humanities, 12-15. https://doi.org/10.5749/minnesota/9780816677948.003.0002
</div>

---

## A double definition
Kathleen Fitzpatrick offers an insightful definition:

> […] a nexus of fields within which scholars use computing technologies to investigate the kinds of questions that are traditional to the humanities, or […] **ask traditional kinds of humanities-oriented questions about computing technologies**.

<div class="footer">
  Fitzpatrick, K. (2012). The humanities, done digitally. Debates in the digital humanities, 12-15. https://doi.org/10.5749/minnesota/9780816677948.003.0002
</div>

---

## Still...
There has always been a divergence in nature (and thus in approaches):
- _digital_: implementation, creation, programming = practice
- _humanities_: interpretation, speculation, comparative approaches = theory

<div class="footer">
  Warwick, C. (2015). Building theories or theories of building? A tension at the heart of digital humanities. A new companion to digital humanities, 538-552. http://dx.doi.org/10.1002/9781118680605.ch37
</div>

---

## DH as "literacy of building"
Task of encouraging (= "educating") in the "construction" (intellectual, social, ideological process) of something that generates knowledge within academic, public, and private discourse

* Practical skills
* Interpretive approaches
* Valorization, dissemination, and use of research results

<div class="footer">
  Endres, B. (2017). A literacy of building: making in the digital humanities. Making Things and Drawing Boundaries: Experiments in the Digital Humanities, 44-54. https://doi.org/10.5749/j.ctt1pwt6wq.7
</div>

---

## Digital projects

A project that uses digital methods and technologies as an integral part of the research process, dissemination of research results, and interaction with a wide audience of users

There are various types: e.g., digital editions, bibliographic databases, data analysis applications, GIS applications, etc.

<div class="footer">
  Dubrovina, L., Lobuzina, K., Onyshchenko, O., & Boriak, H. (2021). Digital Humanitarian Project as a component of digital humanities. Science and Innovation, 17(1), 54-63.  https://doi.org/10.15407/scine17.01.054
</div>

---

## Common characteristics

* Use of data-driven analysis methods
* Management of digital resources (e.g., a set of documents or data saved in one or more files in a specific format)
* Structured, informative, and interpretable organization of resources
* Digital publication of resources

<div class="footer">
  Dubrovina, L., Lobuzina, K., Onyshchenko, O., & Boriak, H. (2021). Digital Humanitarian Project as a component of digital humanities. Science and Innovation, 17(1), 54-63.  https://doi.org/10.15407/scine17.01.054
</div>

---

## Digital project lifecycle

Scientifically valid, reliable, reusable tool capable of addressing research questions, methodologies, and themes pertinent to humanistic disciplines (text, interpretation, uncertainty, human experience, etc.)

![Lifecycle schema of a digital project (Source: https://localcontexts.org/traditional-digital-content-lifecycle/)](figure-1.png)

---

## Production

* Resource selection
* Digital acquisition and/or transcription of resources, with awareness of
  * different formats
  * license types
  * quality of the acquisition action

Example: collection and transcription of a series of documents for digitization for a digital edition

---

## Description

* Content, context, users analysis
* Selection and/or design of metadata schemes, controlled vocabularies, and other standards
* Modeling and production of metadata

Example: defining the markup schema for document structure and ontologies for content and relationships

---

## Management

* Processing of resources
* Analysis and querying of resources
* Reasoning at the infrastructure level to host the results

Example: semi-automatic conversion of documents into formats suitable for semantic publishing through a custom-developed application and a set of scripts

---

## Archiving

* Reflecting on the storage service
* Defining preservation metadata
* Establishing data preservation policies, including for the application and often the entire environment
* Ensuring their long-term accessibility

Example: choosing the server to host the digital edition, publishing the dataset dump on Zenodo

---

## Sharing

* Designing and developing interfaces to facilitate user interaction
* Developing data and application sharing policies

Example: implementing search mechanisms, data visualizations, downloads, etc.

---

## Reuse

* Facilitating access and ensuring the reuse of data and applications
* Ensuring the viability of data in contexts beyond the native one
* Designing and developing technical documentation for the project

Example: project documentation development, publishing each research output following Open Science practices

---

## Summary

DH = building reusable and scientifically valid digital objects and processes in humanities research through projects

Every digital project has its life cycle: production, description, manipulation, archiving, sharing, reuse

The cycle can vary, is not strictly linear, and is often iterative

---

## Objective

Design, implement, and publish a DH project

We will start with a dataset

We will create a digital object to formally describe a certain domain, manage it, and share it according to a set of fundamental standards to ensure scientific validity

Document it in a white paper that will be published in an open format

---

## Bibliography

* Borgman, C. L. (2010). The digital future is now: A call to action for the humanities. Digital humanities quarterly, 3(4). Retrieved from https://escholarship.org/uc/item/0fp9n05s
* Dubrovina, L., Lobuzina, K., Onyshchenko, O., & Boriak, H. (2021). Digital Humanitarian Project as a component of digital humanities. Science and Innovation, 17(1), 54-63. DOI: https://doi.org/10.15407/scine17.01.054
* Endres, B. (2017). A literacy of building: making in the digital humanities. Making Things and Drawing Boundaries: Experiments in the Digital Humanities, 44-54. DOI: https://doi.org/10.5749/j.ctt1pwt6wq.7  
* Fitzpatrick, K. (2012). The humanities, done digitally. Debates in the digital humanities, 12-15. DOI: https://doi.org/10.5749/minnesota/9780816677948.003.0002

---

## Bibliography

* Goble, C., & De Roure, D. (2009). Data Intensive Computing: The Fourth Paradigm of Scientific Discovery. ISBN: 978-0-9825442-0-4
* Kirschenbaum, M. G. (2016). What is digital humanities and what’s it doing in English departments?. In Defining digital humanities (pp. 211-220). Routledge. DOI: http://dx.doi.org/10.1632/ade.150.55 
* Warwick, C. (2015). Building theories or theories of building? A tension at the heart of digital humanities. A new companion to digital humanities, 538-552. DOI: http://dx.doi.org/10.1002/9781118680605.ch37