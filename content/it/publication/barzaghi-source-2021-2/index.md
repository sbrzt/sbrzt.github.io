---
# Documentation: https://hugoblox.com/docs/managing-content/

title: Source code for generating the National Edition of Aldo Moro's works DOIs
subtitle: ''
summary: ''
authors:
- Sebastian Barzaghi
tags:
- digital edition
- national edition of aldo moro's works
- python
- datacite
- digital object identifier
categories: []
date: '2021-11-01'
lastmod: 2023-12-20T14:33:24+01:00
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
publishDate: '2023-12-20T13:33:23.286508Z'
publication_types:
- '0'
abstract: A collection of the source codes used to automatically register the Digital
  Object Identifiers of the works published on the National Edition of Aldo Moro's
  works. The software connects to both an external MongoDB database and the DataCite
  API in order to assign to each document its respective DOI and register it on DataCite
  Fabrica. To start the program, fill in the blanks in the code (marked with '@')
  accordingly, then run `python doifier.py` in the command prompt, and select the
  HTTP method to run.
publication: '*Zenodo*'
doi: 10.5281/zenodo.5651219
links:
- name: URL
  url: https://zenodo.org/record/5651219
---
