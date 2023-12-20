---
# Documentation: https://hugoblox.com/docs/managing-content/

title: Source code for processing the National Edition of Aldo Moro's works data
subtitle: ''
summary: ''
authors:
- Sebastian Barzaghi
tags:
- semantic web
- digital humanities
- digital edition
- national edition of aldo moro's works
- data cleaning
- data wrangling
- python
categories: []
date: '2021-10-01'
lastmod: 2023-12-20T14:33:18+01:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2023-12-20T13:33:17.983372Z'
publication_types:
- '0'
abstract: "A series of Python scripts that have been used to process the documents\
  \ in the National Edition of Aldo Moro's works.  In particular, the scripts are:\
  \ recast.py, for refactoring the documents code, correcting possible errors, normalizing\
  \ and finalizing resource URIs, and so on; TEIfy.py, for generating TEI documents\
  \ from the HTML code. The TEI structure imitates the source code as closely as possible,\
  \ and in addition integrates bibliographic metadata in the document header as well;\
  \ PDFfy.py, for generating PDF documents from the HTML code. The PDF pagination\
  \ and visualization is regulated by a CSS stylesheet (stylesheet.css); generate.py,\
  \ for converting metadata into semantic statements collected in a knowledge base\
  \ and organized on the basis of the standards defined in the data modelling phase;\
  \ align.py, for integrating document markup in the knowledge base; main.py, for\
  \ gathering and managing the functions defined in the other scripts; utils.py, for\
  \ choosing which script to run and in which local directory. To start the program,\
  \ run `python main.py` in the command prompt, then select the function you want\
  \ to run and the directory you intend to use. You will either need a `config.json`\
  \ file containing some variables in order to make it work (such as your local paths\
  \ and names of the directories), or write them directly into the code as variables."
publication: '*Zenodo*'
doi: 10.5281/zenodo.5592470
links:
- name: URL
  url: https://zenodo.org/record/5592470
---
