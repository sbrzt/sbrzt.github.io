---
title: Cleaning data with OpenRefine
summary: A soft introduction to Data Cleaning with OpenRefine
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2024-07-01T00:00:00Z'
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: white
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: github-light
---

# Humanities Data Cleaning

#### A soft introduction to Data Cleaning with OpenRefine

Sebastian Barzaghi | 
[sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | 
[https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527)

---

## What is humanities data?

Any value assigned to something that can be quantified, qualified or interpreted in some way to be used as an informative evidence

Numbers, words, images, videos, photos, audio records, interviews, manuscripts, notes, collections...

<div class="footer">
  Gualandi, B., Pareschi, L., & Peroni, S. (2023). What do we mean by “data”? A proposed classification of data types in the arts and humanities. Journal of Documentation, 79(7), 51-71. <a href="https://doi.org/10.1108/JD-07-2022-0146">https://doi.org/10.1108/JD-07-2022-0146</a>.
</div>

---

## To be useful, data should be organized

To be understood by yourself in the future

To be machine-readable (Interoperable in FAIR)

To be understood by others (Reusable in FAIR)

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## All data is messy

Never take your data at face value

80% of data analysis is spent on the process of cleaning data and preparing it for further manipulation and analysis

Cleaning and preparation must be iterative

Necessary for working with datasets

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## A dataset is a collection of data

Every value belongs to a variable and an observation

Every variable forms a column

Every observation forms a row

<div class="footer">
  S. Ciston, “A CRITICAL FIELD GUIDE FOR WORKING WITH MACHINE LEARNING DATASETS”, K. Crawford and M. Ananny, Eds., Knowing Machines project, Feb. 2023. <a href="https://knowingmachines.org/critical-field-guide">https://knowingmachines.org/critical-field-guide</a>.
</div>

---

## Data cleaning is hard (but worth it)!
* Prepare the data
* Eliminate redundancy
* Separate or combine values
* Fix errors and inconsistencies (e.g. duplicates, empty values, inconsistent spelling or formatting, etc.)
* Standardize when possible
* Treat NULL values

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Common mistakes

---

## Never modify your original data

Always make a copy before making changes

Back up your files

Keep track of all the steps

Save your files in the `UTF-8` encoding 

<div class="footer">
  Seth van Hooland, Ruben Verborgh, and Max De Wilde, "Cleaning Data with OpenRefine," Programming Historian 2 (2013), <a href="https://doi.org/10.46430/phen0023">https://doi.org/10.46430/phen0023</a>.
</div>

---

## Always describe your data
Document everything necessary to understand what is in the dataset and how to use it

Consider:
* The who, what, when, where, and how of data collection
* How to find and access the data
* Suggestions on the suitability of the data for answering specific questions
* Warnings about known problems or inconsistencies in the data
* Information to check that the data are properly imported

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Use standard table formats

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="tidy-1.png" alt="https://r4ds.had.co.nz/tidy-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Every variable must have a separate column</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Use standard table formats

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="tidy-2.png" alt="https://r4ds.had.co.nz/tidy-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Every observation must have a separate row</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Use standard table formats

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="tidy-3.png" alt="https://r4ds.had.co.nz/tidy-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Every cell should contain a single data value</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Avoid aggregating comments and other information with data

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="multiple-info.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Examples: comments placed within data cells, measurement units included in data cells, entering more than one type of information in a cell, including metadata in the table, etc.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Avoid aggregating comments and other information with data

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="single-info.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Add units to the column title or into a separate column</p>
        <p>Add information to a separate column</p>
        <p>Add metadata in a separate document</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Do not use formatting to convey information

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="formatting.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Example: highlighting cells, rows or columns that should be excluded from an analysis, leaving blank rows to indicate separations in data.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Do not use formatting to convey information

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="good-formatting.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Add units to the column title or into a separate column</p>
        <p>Add information to a separate column</p>
        <p>Add metadata in a separate document</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Do not use multiple tables nor tabs

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="multiple-tables.jpg" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Multiple data tables or tabs within a single spreadsheet</p>
        <p>If possible, combine everything into one table, or store each table in a separate file</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Do not use special characters

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="special-characters.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Whenever possible, avoid special characters in column headings and text: / \: * . ? ‘ < > [ ] ( ) & $ æÆøØåÅäÄ</p>
        <p>Always avoid using spaces in column headings - instead, use underscores or CamelCase</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Be consistent

* Dates displayed in many different formats (e.g. "12 July 2024", "12/07/2024", "12-07-2024", etc.)
* Names displayed in many different variants (e.g. "Alessandro Manzoni", "A. Manzoni", "Manzoni", "Manzoni, Alessandro", etc.)
* Use international standard formats (e.g. `YYYY-MM-DD` for dates)
* Use authority records for names (e.g. [VIAF](http://viaf.org/viaf/14356))
* Be consistent in your capitalization of words, choice of delimiters, and naming conventions for variables
* Avoid using your delimiter in the data itself

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Eliminate redundancy (with caution!)

Includes:
* Duplicates
* Irrelevant observations
* Incomplete data
* Invalid data
* Conflicting data

It's all **interpretation**: consider whether an observation or a column should be removed or not!

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Always treat NULL values

Use a consistent way that is compatible and unlikely to cause errors (e.g. blank)

Consider that:
* It can be difficult to know if a value is missing or was overlooked during data entry
* Blanks can be confusing when spaces or tabs are used as delimiters in text files

`NA` and `NULL` are reasonable null values

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Perform basic quality control

Check for: 
* Grammatical errors
* Inconsistent use of upper and lowercase
* Inconsistent titles for columns 
* Inconsistent units of measurement, data types (e.g., numeric, character), naming schemes, etc.
* Out-of-range values

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Export and share

Use an established and open license to let others know exactly what they can and cannot do with the data (e.g. [Creative Commons Zero (CC0)](https://creativecommons.org/publicdomain/zero/1.0/)) 

Use open formats to make the data interoperable (e.g. [CSV](https://en.wikipedia.org/wiki/Comma-separated_values)), when possible

Consider sharing your data on GitHub and/or publishing it on a repository (e.g. [Zenodo](https://zenodo.org/), [Figshare](https://figshare.com/), etc.) to make it visible, accessible and stable

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## OpenRefine

---

## A tool for tabular data cleaning

* Easy to identify and fix errors
* Easy to combine data from different sources
* Does not change the original file
* All actions are reversible and tracked
* Documentation can be published alongside the data
* Workflow can be saved and applied to new datasets

<div class="footer">
  Baker, J., Moore, C., Priego, E., Alegre, R., Cope, J., Price, L., ... & Wilson, G. (2016). Library Carpentry: software skills training for library professionals. Liber Quarterly: The Journal of European Research Libraries, 26(3), 141-162. <a href="http://dx.doi.org/10.18352/lq.10176">http://dx.doi.org/10.18352/lq.10176</a>
</div>

---

## Some common scenarios

You want to:
* Know how many times a particular value appears in a column in your data 
* Know how values are distributed across your whole data set 
* Normalize dates which are formatted in different ways, and want to change all the dates in the list to a single common date format
* Normalize names or terms that differ from each other but refer to the same people, places or concepts
* Separate bits of data combined together into individual data
* Align your data to an external data source

<div class="footer">
  Baker, J., Moore, C., Priego, E., Alegre, R., Cope, J., Price, L., ... & Wilson, G. (2016). Library Carpentry: software skills training for library professionals. Liber Quarterly: The Journal of European Research Libraries, 26(3), 141-162. <a href="http://dx.doi.org/10.18352/lq.10176">http://dx.doi.org/10.18352/lq.10176</a>
</div>

---

## Installing OpenRefine

* Download OpenRefine: [https://openrefine.org/download.html](https://openrefine.org/download.html)
  * It should already come with Java Runtime Environment
  * If it does not work, also download and install Java Runtime Environment: [https://www.java.com/it/](https://www.java.com/it/)

* Unzip the downloaded file
* Double-click on `openrefine.exe` or `refine.bat`
* Access the interface on a web browser at [http://127.0.0.1:3333](http://127.0.0.1:3333)

---

## Creating a project

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-1.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Download the Mythologiae dataset (link in chat)</li>
        <li><em>Create Project</em> > <em>This computer</em></li>
        <li>Click on <em>Choose files</em> > <code>mythologiae-dataset.csv</code></li>
        <li>Click on <em>Next</em></li>
      </ul>
    </div>
</div>

---

## Creating a project

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-2a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><em>Parse data as</em> > <em>CSV / TSV / separator-based files</em></li>
        <li><em>Character encoding</em> > <code>UTF-8</code></li>
        <li>Select <em>Columns are separated by</em> > <em>commas (CSV)</em></li>
        <li>Flag <em>Use character <code>"</code> to enclose cells containing column separators</em></li>
        <li>Flag <em>Trim leading & trailing whitespace from strings</em></li>
      </ul>
    </div>
</div>

---

## Creating a project

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-2b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Select <em>Parse next <code>1</code> line(s) as column headers</em></li>
        <li>Flag <em>Store blank rows</em></li>
        <li>Flag <em>Store blank cells as nulls</em></li>
        <li>Click on <em>Create project</em></li>
      </ul>
    </div>
</div> 

---

## The project screen

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-3a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><code>Permalink</code> allows you to return to a project at a specific view state, with facets and filters applied, by putting view-specific information directly into the URL</li>
      </ul>
    </div>
</div>

---

## The project screen

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-3b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><code>Open</code> opens up a new browser tab showing the Create Project screen to change settings, start a new project, or open an existing project</li>
        <li><code>Export</code> allows you to pick a format for exporting a dataset</li>
        <li><code>Help</code> will open up a new browser tab and bring you to this user manual on the web</li>
      </ul>
    </div>
</div> 

---

## The grid screen

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-4.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Where the data of your project is displayed in a tabular format</li>
        <li>Number of total rows</li>
        <li>Rows mode vs. records mode</li>
        <li>Number of rows / records visible on screen at one time</li>
      </ul>
    </div>
</div> 

---

## Facet/Filter

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-5.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <p>Main ways to explore your data, by displaying patterns, trends and subgroups</p>
      <ul>
        <li><code>Refresh</code> updates each facet with the latest information</li>
        <li><code>Reset all</code> resets all facets without removing them</li>
        <li><code>Remove all</code> removes all facets</li>
      </ul>
    </div>
</div> 

---

## Undo/Redo

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-6.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Project's history as a list of changes in order</li>
        <li>Autosave every 5 minutes and when closing with <code>CTRL + C</code></li>
        <li>Any activity that changes the data can be undone</li>
        <li>The change history of each project is saved with the project itself</li>
      </ul>
    </div>
</div> 

---

## Row mode, record mode

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-7a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><strong>Row</strong>: a series of cells, one cell per column</li>
        <li>Sometimes, there are multiple pieces of information in one cell (e.g. <code>dcho_keyword</code>)</li>
        <li>In those cases, if you successfully split these values, you can use OpenRefine's <strong>records mode</strong> to visualize them correctly</li>
      </ul>
    </div>
</div>

---

## Row mode, record mode

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-7b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><strong>Record</strong>: a collection of one or more rows</li>
        <li>The multiple pieces of information in one cell (e.g. <code>dcho_keyword</code>), once split, are visualized each in a different row, but belong to the same record</li>
      </ul>
    </div>
</div>

---

## Explore data with Facets

**Facet**: an aspect of data variance in a column

Gives a big picture look at the data

Allows further operations, like filtering and clustering

---

## Explore data with Facets

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Typically, you create a facet on a particular column</li>
        <li>Click on the <em>triangle</em> in front of the column name (e.g. <code>dcho_theme</code>)</li>
        <li>Select <em>Facet</em></li>
        <li>Select a Facet of your choice (e.g. <em>Text facet</em>)</li>
      </ul>
    </div>
</div>

---

## Text facet

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Takes the total contents of the cells of the column in question and matches them up</li>
        <li>Sort by name or count</li>
        <li>Mass-edit every identical cell in the column</li>
        <li>Great way to have a look at the data and fix typos, whitespace, etc.</li>
      </ul>
    </div>
</div>

---

## Text facet

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8c.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Multiple facets are stacked on the top of each other (e.g. <code>cho_author</code> is added)</li>
      </ul>
    </div>
</div>

---

## Filter

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8d.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Filters can be added on a column</li>
        <li>Useful for identifying precise pieces of data</li>
        <li>Click on the arrow and select <em>Text filter</em></li>
      </ul>
    </div>
</div>

---

## Filter

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8e.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>The filter share the same space with the facets</li>
        <li>Type in the text you are searching for (e.g. "edipo")</li>
        <li>Case-insensitive by default</li>
      </ul>
    </div>
</div>

---

## Filter with Facets

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8f.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>You can also filter through facets</li>
        <li>Click on any entry in a filter (e.g. "Allston, Washington" in the <code>cho_author</code> facet)</li>
        <li>Only the rows with that value are shown</li>
      </ul>
    </div>
</div>

---

## Filter with Facets

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8g.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>You can use multiple facets to enhance filtering</li>
      </ul>
    </div>
</div>

---

## Filter with facets

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8h.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>You can use customized facets for certain effects (e.g. filter in rows with blank cells)</li>
      </ul>
    </div>
</div>

---

## Sorting

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8i.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Determine the order in which rows are shown based on certain conditions</li>
        <li>Click on the arrow and select <em>Sort</em></li>
      </ul>
    </div>
</div>

---

## Sorting

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8l.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Select how to treat the cell values during sorting (e.g. if they are dates, you most likely want to select <em>dates</em>)</li>
        <li>You can also select the sorting order</li>
        <li>Click on <em>OK</em></li>
      </ul>
    </div>
</div>

---

## Clustering

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8m.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>A great way to fix inconsistencies found with facets</li>
        <li>Uses a variety of comparison methods to find text entries that are similar but not exact, then shares those results with you so that you can merge the cells that should match</li>
        <li>Create a facet</li>
        <li>Click on <em>Cluster</em></li>
      </ul>
    </div>
</div> 

---

## Clustering

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8n.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Click on <em>Cluster</em></li>
        <li>Experiment with different algorithms to detect different clusters</li>
        <li>For each cluster, you can merge the values by replacing them with a single consistent value</li>
        <li>By default, the most common value in the cluster is used as the new value, but you can change it</li>
      </ul>
    </div>
</div> 

---

## Clustering

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-8o.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Experiment with different algorithms to detect different clusters</li>
        <li>For each cluster, you can merge the values by flagging <em>Merge?</em></li>
        <li>Click on <em>Merge selected & re-cluster</em> to check, and <em>Merge selected & Close</em> to finish</li>
      </ul>
    </div>
</div> 

---

## Cell editing

OpenRefine offers a number of features to edit and improve the contents of cells automatically and efficiently

* Editing through a text facet: click on _Edit_ to the right of the facet, and type in a new value
* Using a find/replace function: select _Edit cells_ > _Replace_ to input a string to search and a string to replace it with
* Editing individual cells: hover over a cell and click on _Edit_

---

## Splitting

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-9a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Sometimes a cell can contain multiple values (e.g. <code>dcho_keyword</code> column: multiple values separated by commas <code>,</code>)</li>
        <li>Click on the arrow and select <em>Edit cells</em></li>
        <li>Select <em>Split multi-valued cells</em></li>
      </ul>
    </div>
</div>

---

## Splitting

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-9b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>You can decide how to split the cells</li>
        <li>Ideally, you should always use a separator (e.g. <code>,</code>, <code>|</code>, <code>;</code>, etc.)</li>
        <li>Click on <em>OK</em></li>
      </ul>
    </div>
</div>

---

## Transforming

A powerful way to enforce changes that cannot be achieved through simple facets, filters or clusters

* trimming leading and trailing whitespaces
* splitting data into multiple columns
* removing punctuation
* standardising a data format
* extracting a particular type of data from a textual string

Can be either preset or written ad-hoc in a language called GREL

---

## Reconciliation

Semi-automated process of matching data with external sources

External sources must offer a compliant web service in order to work

Useful for:
* Fixing spelling or variations in proper names
* Cleaning up manually-entered values against authority files
* Linking your data to an existing dataset

Human judgment is required to review and approve the results

Happens by default through string searching

Clean and cluster data before reconciling

---

## Reconciliation

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-9c.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Click on the arrow and select <em>Reconcile</em></li>
        <li>Select <em>Start reconciling</em></li>
      </ul>
    </div>
</div>

---

## Reconciliation

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-9d.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Select the reconciliation service (e.g. <code>VIAF</code>)</li>
        <li>Click on <em>Next</em></li>
      </ul>
    </div>
</div>

---

## Reconciliation

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-9e.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Depending on the column and the reconciliation service selected, choose the type of entity you want to reconcile (e.g. <code>Person</code>)</li>
        <li>Click on <em>Start reconciling</em></li>
      </ul>
    </div>
</div>

---

## Reconciliation

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="openrefine-9f.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Some cell values are reconciled directly (e.g. <em>Houdon, Jean Antoine</em>)</li>
        <li>Others need manual validation (e.g. <em>Gérard, Francois Baron</em>)</li>
        <li>Click on the <em>single check</em> to reconciliate only in that cell, or the <em>double check</em> to extend it to all identical cells</li>
      </ul>
    </div>
</div>

---

## What to do

---

## dcho_theme

* Set a common separator (`|`)
* Split
* Cluster
* Edit (e.g. keep only the last value if there is a hierarchy, delete "Non categoria", etc.)
* Standardize when possible (see [Iconclass]())
  * sign in Iconclass
  * search for the theme
  * choose the most appropriate option 
  * replace the existing theme in the dataset with the ID of the option found
  * e.g. L'Enigma della Sfinge &rarr; `94T33`
  * e.g. Eracle cattura il cinghiale di Erimanto &rarr; `94L324`

---

## cho_century

* Set a common separator (`|`)
* Edit
* Standardize (see [EDTF](https://www.loc.gov/standards/datetime/))
  * e.g. II century &rarr; `0100-01-01/0199-12-31`
  * e.g. II century B.C. &rarr; `-0199-01-01/-0100-12-31`

---

## cho_date

* Set a common separator (`|`)
* Edit (e.g. remove "ca.", "circa", etc.)
  * Uncertainty ("ca.", "circa", etc.) has to be expressed in a separate column `cho_date_uncertainty` which only accepts `True` (yes) or `False` (no)
* Standardize (see [EDTF](https://www.loc.gov/standards/datetime/))
  * e.g. 460 B.C. &rarr; `-0460`
  * e.g. 550-530 B.C. &rarr; `-0550/-0530`
  * e.g. 1705-1706 &rarr; `1705/1706`

---

## cho_sources_classic

* Set a common separator (`|`)
* Edit (e.g. remove citations that are not in canonical form)
  * Non-canonical citations should be saved in a separate column `cho_sources_other`
* Standardize
  * Look for the citation on [Perseus](https://www.perseus.tufts.edu/hopper/)
  * e.g. Apollodoro, Biblioteca, II 5 &rarr; `Apollod. 2.5`
  * e.g. Omero, Odissea, XI vv.601-604 &rarr; `Hom. Od. 11.601`

---

## Other data

* All: check for NULL values, fix typos, replace separators with `|`
* `dcho_keyword`: Split, Cluster, Edit
* `cho_title`: Edit
* `cho_author`: Cluster, Edit, Reconcile with VIAF (Person)
* `cho_period`: Cluster, Edit
* `cho_type`: Cluster, Edit
* `cho_location`: Cluster, Edit, Reconcile with VIAF (Organization)

---

## Conclusion

There is already a lot you can do to increase data quality
* Explore data by using facets, filters and sorting
* Transform data by single- and mass-editing, clustering and replacing
* Reconcile data with external sources

Try and experiment! You are working on a copy, and you can alyaws trace back