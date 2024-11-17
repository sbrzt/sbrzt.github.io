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

  ```
  tesi brutta.docx
  tesi brutta2.docx
  tesi vera.docx
  tesi vera finale.docx
  ```

---

### Un buon sistema di versionamento è sistematico

Aggiungere le date rende leggermente più facile seguire quando sono state apportate le modifiche.

  ```
  tesi_20-03-2024.docx
  tesi_06-05-2024.docx
  tesi_10-05-2024.docx
  tesi_30-05-2024.docx
  ```

---

### Un ottimo sistema di versionamento è descrittivo, permissivo, collaborativo

Monitora sviluppi e modifiche nei tuoi documenti, registra le modifiche apportate al tuo documento in un modo che tu possa comprenderle in seguito, permette di annullare le modifiche e tornare a verisoni precedenti, e facilita la collaborazione tra diverse persone per lavorare sullo stesso documento.

<div class="footer">
Perez-Riverol, Y., Gatto, L., Wang, R., Sachsenberg, T., Uszkoreit, J., Leprevost, F. D. V., ... & Vizcaíno, J. A. (2016). Ten simple rules for taking advantage of Git and GitHub. PLoS computational biology, 12(7), e1004947. <a href="https://doi.org/10.1371/journal.pcbi.1004947">https://doi.org/10.1371/journal.pcbi.1004947</a>.
</div>

---

### Git è un ottimo sistema di versionamento distribuito

Permette di tenere traccia delle modifiche apportate ai file in un progetto. 

In pratica, consente di salvare diverse versioni di un file o di un intero progetto nel tempo, così puoi vedere cosa è cambiato, chi ha fatto le modifiche e quando.

<div class="footer">
Ram, K. (2013). Git can facilitate greater reproducibility and increased transparency in science. Source code for biology and medicine, 8, 1-8. <a href="https://doi.org/10.1186/1751-0473-8-7">https://doi.org/10.1186/1751-0473-8-7</a>.
</div>

---

### Glossario Git

Git (e sistemi costruiti su Git, come GitHub) è basato su una serie di concetti identificati con una terminologia particolare che bisogna riconoscere, studiare e ricordare.

---

### Repository ("repo")

> Cartella contenente tutti i file di un progetto, insieme alla cronologia completa delle modifiche che sono state fatte su di essi.

---

### Commit

> Operazione che registra le modifiche apportate ai file in una repository (simile ad una "fotografia" dello stato del progetto in un determinato momento).

---

### Branch

> Copia indipendente del progetto ma collegata ad esso, utile per apportare modifiche senza influire sui file originali.

---

### Merge

> Operazione che unisce le modifiche fatte in un branch con un'altro branch (di solito quello principale).

---

### Clone

> Copia locale di una repository.

---

### Pull

> Operazione che scarica le modifiche da una repository remota ad un clone sul tuo computer.

---

### Push

> Operazione che invia le modifiche da un clone sul tuo computer ad una repository remota.

---

### Conflict

> Evento che si verifica quando si cerca di unire due modifiche incompatibili fatte sugli stessi file in branch diversi.

---

### Fork

> Copia online di una repository.

---

### Pull request

> Proposta di modifica inviata ad una repository remota.

---

### GitHub è una piattaforma online per repository Git

https://github.com/

Permette di caricare, condividere e collaborare su progetti Git con altre persone.

Strumento fondamentale per la comunità open-source e per i progetti aziendali.

Sempre più importante anche per gestire i flussi di lavoro della pubblicazione di riviste, dei libri di testo aperti, e di altri progetti di natura più "umanistica".

<div class="footer">
Blischak, J. D., Davenport, E. R., & Wilson, G. (2016). A quick introduction to version control with Git and GitHub. PLoS computational biology, 12(1), e1004668. <a href="https://doi.org/10.1371/journal.pcbi.1004668">https://doi.org/10.1371/journal.pcbi.1004668</a>.
</div>

---

## Una panoramica veloce

---

### 1. Registriamoci su GitHub

Registriamo un account su GitHub: https://github.com/signup.

---

### 2. Dalla home iniziale si può accedere a tutto

![](img/0201.png)

---

### 3. La barra laterale destra si riferisce al nostro profilo

![](img/0202.png)

---

### 4. Dal nostro profilo possiamo accedere alle nostre repository

![](img/0203.png)

---

### 5. Dal nostro profilo possiamo accedere alle nostre repository

![](img/0204.png)

---

### 6. In una repository vediamo le cartelle e i file che contiene

![](img/0205.png)

---

### 7. Cliccando su una cartella o file, ne vediamo i contenuti

![](img/0206.png)

---

### 8. Cliccando su _Settings_, vediamo le impostazioni della repository

![](img/0207.png)

---

### 9. Possiamo creare una nuova repository direttamente su GitHub o caricandola da locale

![](img/0208.png)

---

### 10. Proviamo a crearne una nuova direttamente

![](img/0209.png)

---

### 11. La nuova repository appena creata

![](img/0210.png)

---

### 12. Vediamo un file della repository (es. README.md)

![](img/0211.png)

---

### 13. Proviamo a modificarlo...

![](img/0212.png)

---

### 14. ... Aggiungendo del testo

![](img/0213.png)

---

### 15. Facciamo un _commit_ delle modifiche appena fatte

![](img/0214.png)

---

### 16. Le modifiche sono state salvate correttamente

![](img/0215.png)

---

### 17. Ora proviamo ad interagire con una repository di qualcun'altro

![](img/0216.png)

---

### 18. Potete clonare l'intera repository in vari modi, incluso un download in formato _.zip_

![](img/0217.png)

---

### 19. Ora proviamo a _forkare_ la repository

![](img/0218.png)

---

### 20. Eseguire un _fork_ è simile a creare una nuova repository

![](img/0219.png)

---

### 21. La repository da cui abbiamo _forkato_ può subire modifiche nel frattempo...

![](img/0220.png)

---

### 22. ... Ma possiamo ri-allineare il nostro _fork_ molto facilmente

![](img/0221.png)

---

### 23. Ora il nostro _fork_ è allineato con la repository di origine

![](img/0222.png)

---

### 24. Potete creare nuovi file in almeno due modi

![](img/0223.png)

---

### 25. Potete creare un nuovo file direttamente su GitHub

![](img/0224.png)

---

### 26. Per confermare la creazione del file, è sufficente eseguire un _commit_

![](img/0225.png)

---

### 27. Ora il file è stato creato ed è visualizzabile

![](img/0226.png)

---

### 28. In alternativa, potete anche caricare un file esistente sul vostro computer

![](img/0231.png)

---

### 29. Una volta caricato il file, eseguite il _commit_

![](img/0232.png)

---

### 30. Di nuovo, ora il file è stato caricato ed è visualizzabile

![](img/0233.png)

---

### 31. Potete ovviamente eliminare i file

![](img/0227.png)

---

### 32. Prima di eliminare i file, prima avrete un'anticipazione...

![](img/0228.png)

---

### 33. ... E poi dovrete confermare l'operazione con un _commit_

![](img/0229.png)

---

### 34. Ora il file è stato correttamente eliminato

![](img/0230.png)

---

## Attività pratica

---

### Obiettivo: creare un file README per il nostro progetto su Mythologiae

Un README è un file di testo che introduce e spiega un progetto, fornendo informazioni necessarie a contestualizzare e comprendere i contenuti, le metodologie, e i risultati. 

Si tratta di uno strumento molto semplice ed efficace per comunicare con altre persone potenzialmente interessate al vostro progetto.

Solitamente, è il primo file che viene creato (rigorosamente nella cartella principale), ed è uno dei file da aggiornare in continuazione nel corso del tempo.

Può essere scritto in qualsiasi formato di testo. Solitamente viene usato il Markdown (`.md`), ma lo vedremo nella prossima puntata. Per ora, limitiamoci ad utilizzare il formato `.txt`.

---

### 1. Troviamo la repo del tutorial

Link: https://github.com/dhdmch/tutorial

Questa sarà la repo di riferimento per le nostre lezioni pratiche.

---

### 2. Creiamo un nuovo file e chiamiamolo README.txt

---

### 3. Stabiliamo la struttura del nostro README

```
# Nome

## Descrizione
Il cosa, perché e come del progetto. Qual'è la motivazione? Quale problema stiamo risolvendo? Cosa abbiamo imparato?

## Fonti
Link alle fonti dei dati utilizzati

## Metodi e strumenti
Metodologie e/o strumenti utilizzati

## Credits
Contatti di tutte le persone coinvolte

## Licenza
Etichetta e link alla licenza

## Changelog
Sezione dove teniamo traccia di quello che abbiamo fatto e delle modifiche avvenute (prima la più recente)
```

---

### 4. Facciamo un _commit_ per salvare il file

---

### 5. Ora creiamo due cartelle: una chiamata `data`, l'altra `docs`

Non è possibile creare cartelle direttamente su GitHub, quindi le creeremo in locale e le caricheremo.

GitHub non accetta cartelle vuote, quindi dobbiamo riempirle con qualcosa per poterle caricare con successo.

---

### 6. Per ora, `docs` e `data` conterranno altri README (vuoti)

---

### 7. Finalizziamo il caricamento di `docs` e `data` con un _commit_

---

## Oltre la semplice interfaccia

---

### 1. GitHub Desktop

Applicazione ufficiale che offre un'interfaccia grafica per facilitare l'uso di Git e GitHub.

<div class="footer">
Van Strien, D. (2016). An Introduction to Version Control Using GitHub Desktop. The Programming Historian. https://doi.org/10.46430/phen0051.
</div>

---

### Installazione

1. Scaricate GitHub Desktop: https://desktop.github.com/download/;

2. Installate GitHub Desktop seguendo le istruzioni fornite.

---

### Git su linea di comando

Decisamente il metodo migliore, soprattutto per gli sviluppatori.

Richiede un certo tipo di sforzo, ma una volta compresi i concetti di Git e il funzionamento della linea di comando, diventa parte naturale del flusso di lavoro.

```

git add .

git commit -m "Testo del commit"

git push origin main

---
