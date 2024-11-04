---
title: DHDMCH - Primi passi
summary: Lezione 02 del corso di Digital Humanities e Data Management per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2023-11-18T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# Primi passi

## Lezione 02 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527)

---

## Versionamento

---

### Il versionamento è la gestione delle modifiche nei file

La maggior parte delle persone utilizza una qualche forma di versionamento per gestire i propri file.

  > tesi_brutta.docx
    tesi_brutta2.docx
    tesi_vera.docx
    tesi_vera_finale.docx

---

### Un buon sistema di versionamento è sistematico

Aggiungere le date rende leggermente più facile seguire quando sono state apportate le modifiche.

  > tesi-20-03-2024.docx
    tesi-06-05-2024.docx

---

### Un ottimo sistema di versionamento è descrittivo, permissivo, collaborativo

Monitora sviluppi e modifiche nei tuoi documenti, registra le modifiche apportate al tuo documento in un modo che tu possa comprenderle in seguito, permette di annullare le modifiche e tornare a verisoni precedenti, e facilita la collaborazione tra diverse persone per lavorare sullo stesso documento.



Perez-Riverol, Y., Gatto, L., Wang, R., Sachsenberg, T., Uszkoreit, J., Leprevost, F. D. V., ... & Vizcaíno, J. A. (2016). Ten simple rules for taking advantage of Git and GitHub. PLoS computational biology, 12(7), e1004947. https://doi.org/10.1371/journal.pcbi.1004947.

---

### Git è un ottimo sistema di versionamento distribuito


Concetti chiave: commit, branch, merge.

Vantaggi: tracciamento delle modifiche, gestione di progetti complessi, collaborazione.


Ram, K. (2013). Git can facilitate greater reproducibility and increased transparency in science. Source code for biology and medicine, 8, 1-8. https://doi.org/10.1186/1751-0473-8-7.

---

### GitHub è una piattaforma per repository Git

Funzionalità di collaborazione (pull request, issue tracking).

Importanza nella comunità open-source e per i progetti aziendali.

Sempre più importante anche per gestire i flussi di lavoro della pubblicazione di riviste, dei libri di testo aperti e di altri progetti umanistici.

Blischak, J. D., Davenport, E. R., & Wilson, G. (2016). A quick introduction to version control with Git and GitHub. PLoS computational biology, 12(1), e1004668. https://doi.org/10.1371/journal.pcbi.1004668.

---

### GitHub Desktop è un'applicazione per facilitare l'uso di Git e GitHub

Offre un'interfaccia grafica per usare Git.



Van Strien, D. (2016). An Introduction to Version Control Using GitHub Desktop. The Programming Historian. https://doi.org/10.46430/phen0051.

---

### Installazione

1. Registriamo un account su GitHub: https://github.com/signup;

2. Scarichiamo GitHub Desktop: https://desktop.github.com/download/;

3. Installiamo GitHub Desktop seguendo le istruzioni.

---

### Una panoramica



---

## Creiamo

---

### Creating a Document

We can begin with a very simple document.

---

### Creare un nuovo repository

There are a number of different ways to add files for GitHub Desktop to track. We can drag the folder containing the file onto GitHub Desktop. When you do this you will be asked whether you want to create a repository for this folder. Alternatively we can click on the ‘plus’ icon to open a finder window to choose folders we want to add

Once we have added our folder we will be able to see it in a list of repositories on the left column.

If we choose the repository we just added we will see the files contained in that repository. From this menu we can choose which files we want to version control. (There might be times when we are working on projects in which files are produced which we don’t need or want to version control.) On the right we will see the current document.

If we show hidden folders in the folder we have just added to GitHub you will see that the folder now contains an extra folder with the name ‘.git’. This folder is how GitHub desktop tracks changes we make within our version controlled folder whether these changes be adding new files or modifying existing ones.

---

Lets go back to the document in our text editor and add something new.

Hello world!
a second line

Save the changes to your file and go back to GitHub Desktop. You will see that these new lines of text appear. This lets us know that GitHub is able to see changes in your file but at the moment these changes haven’t been recorded in an official ‘snapshot’ of your repository.

To do this we need to commit our changes.

---

### Effettuare il primo commit

A commit tells Git that you made some changes which you want to record. Though a commit seems similar to saving a file, there are different aims behind ‘committing’ changes compared to saving changes. Though people sometimes save different versions of a document, often you are saving a document merely to record the version as it is when it is saved. Saving the document means you can close the file and return to it in the same state later on. Commits, however, take a snapshot of the file at that point and allow you to document information about the changes made to the document.

To commit changes you must give a summary of the changes and include an optional message. It is important that you think carefully about when to make commits. The advantages of version control taking snapshots of your changes regularly relies on you making commits. It is often tempting to just commit changes when you have finished working on a document but this might not reflect when important changes occurred.

A useful way to think about commits is as the ‘history’ of your document. Each commit records a development or change made to the documents in your repository; the history of the document can be traced by looking at all of the commits. For this history to be useful later on, either for ourselves or for someone else, it is important that this history is recorded at relevant points. Trying to make commits ‘atomic’ is an important consideration. What this means is that each commit ‘makes sense’ on its own. The changes in the commit and the message are understandable without having to look at surrounding commits.

Esercizio pratico: fare un commit delle modifiche e scrivere un messaggio significativo.

---

### Building a good repository

Focusing on making both your messages and your commits ‘atomic’ will make it easier to ‘move’ through different stages of your repositories history. A good repository will allow you to easily understand changes that were made at different stages, will be understood by other people and will help you reflect on the changes you make to a document.

There is some difference between how you would manage a repository primarily focused on code and one focused on text. Both, however, benefit from clear and logical organisation. This is something that is important to do with your research data regardless of whether you are version controlling it and/or making it public. For a useful introduction to managing research data see James Baker’s lesson Preserving Your Research Data.

---

### Rollback e Revert

Spiegazione delle operazioni di rollback.

Esercizio: annullare una modifica e ripristinare una versione precedente.

---

### Pubblicare il repository su GitHub

At the moment we are only recording our changes locally. We may be happy to only store our changes locally (it is still important to back our files up) but we may want to upload our repository onto GitHub to make it public or to have it stored outside of our computer. The process of doing this through GitHub Desktop is straightforward. On GitHub desktop you ‘publish’ repositories. This will push your repository from your computer to the GitHub website and set up a remote repository in the process.

Once your document is online, you can continue to make local changes to your file. But you will have to sync your local changes to reflect these changes in the published GitHub repository. GitHub stores changes both locally (on your computer) and remotely (on their servers). It is important to keep these changes in sync. On GitHub Desktop this process is simplified by using a sync option rather than by using the push and pull commands used on the command line. You will see a ‘sync’ button on GitHub Desktop. This will ensure your local (computer) and remote (GitHub server) repositories are the same.

---

### Clonare un repository esistente

Come clonare un repository pubblico da GitHub.

Esercizio: clonare un repository di esempio.

---

### Branching e Merging

Spiegazione del concetto di branch e della loro importanza.

Come creare e gestire branch in GitHub Desktop.

---

### Pull Requests

Introduzione al concetto di pull request.

Esercizio pratico: simulare una pull request per modifiche su un branch.

---

## Esercizio

---

### Attività pratica

Creare un repository, aggiungere file, effettuare commit, e sincronizzare con GitHub.
