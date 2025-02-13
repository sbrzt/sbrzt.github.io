---
title: Source code for processing the National Edition of Aldo Moro's works data
authors:
- Sebastian Barzaghi
date: '2021-10-01'
publishDate: '2025-02-13T15:40:36.836984Z'
publication_types:
- manuscript
publication: '*Zenodo*'
doi: 10.5281/zenodo.5592470
abstract: "A series of Python scripts that have been used to process the documents
  in the National Edition of Aldo Moro's works.  In particular, the scripts are: recast.py,
  for refactoring the documents code, correcting possible errors, normalizing and
  finalizing resource URIs, and so on; TEIfy.py, for generating TEI documents from
  the HTML code. The TEI structure imitates the source code as closely as possible,
  and in addition integrates bibliographic metadata in the document header as well;
  PDFfy.py, for generating PDF documents from the HTML code. The PDF pagination and
  visualization is regulated by a CSS stylesheet (stylesheet.css); generate.py, for
  converting metadata into semantic statements collected in a knowledge base and organized
  on the basis of the standards defined in the data modelling phase; align.py, for
  integrating document markup in the knowledge base; main.py, for gathering and managing
  the functions defined in the other scripts; utils.py, for choosing which script
  to run and in which local directory. To start the program, run `python main.py`
  in the command prompt, then select the function you want to run and the directory
  you intend to use. You will either need a `config.json` file containing some variables
  in order to make it work (such as your local paths and names of the directories),
  or write them directly into the code as variables."
tags:
- data cleaning
- data wrangling
- digital edition
- digital humanities
- national edition of aldo moro's works
- python
- semantic web
links:
- name: URL
  url: https://zenodo.org/record/5592470
---
