---
title: DHDMCH - Diario di bordo
summary: Introduzione al corso di Digital Humanities e Data Management per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2023-11-21T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# Diario di bordo

## Lezione 04 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

## Markdown

---

### Un linguaggio di markup leggero

Markdown consente di scrivere testi formattati utilizzando una sintassi semplice e facilmente leggibile.

Viene utilizzato in vari contesti, come la scrittura di documentazione tecnica, blog, README files su piattaforme come GitHub, e anche per creare contenuti in sistemi di gestione dei contenuti (CMS) o piattaforme di blogging come Jekyll e Hugo.

Markdown serve per semplificare la scrittura di documenti formattati, permettendo agli utenti di concentrarsi sul contenuto senza doversi preoccupare della complessità del codice. La sua sintassi intuitiva lo rende ideale per scrivere in modo rapido e strutturato, ed è facilmente convertibile in HTML o altri formati, rendendolo perfetto per la pubblicazione su web o la condivisione di documenti tecnici in modo efficiente.

<div class="footer">
Gruber, J. (2012). Markdown: Syntax. URL <a href="http://daringfireball.net/projects/markdown/syntax">http://daringfireball.net/projects/markdown/syntax</a>.
</div>

---

### Per visualizzare il risultato

Generalmente, visualizzare immediatamente la resa di un testo in Markdown non è difficile, ma nel nostro caso non è immediato...

Intanto usiamo questo: https://markdownlivepreview.com/

---

## La sintassi

---

### Corsivo

Per rendere una frase in corsivo in Markdown, puoi racchiudere le parole con un trattino basso `_`.

`Una parola _in corsivo_.` 

Una parola in _corsivo_.

---

### Grassetto

Allo stesso modo, per rendere una frase in grassetto in Markdown, puoi racchiudere le parole con due asterischi `**`. 

`Una parola **in grassetto**.`

Una parola in **grassetto**.

---

### Grassetto + corsivo

Naturalmente, puoi usare _sia il corsivo che il **grassetto**_ nella stessa riga. Puoi anche applicarli **su più parole**.

In generale, non importa in quale ordine metti gli asterischi o i trattini bassi.

---

### Intestazioni

In Markdown, le intestazioni sono precedute da uno o più cancelletti `#`.

Esistono sei livelli di intestazioni in Markdown:

`# Intestazione 1`

`## Intestazione 2`

`### Intestazione 3`

`#### Intestazione 4`

`##### Intestazione 5`

`###### Intestazione 6`

---

### Link

Esistono due tipi di link in Markdown (link inline e reference link), ma entrambi vengono visualizzati nello stesso modo. 

---

### Link inline

Per creare un link inline, racchiudi il testo del link tra parentesi quadre `[ ]`.

Poi racchiudi l'URL tra parentesi tonde `( )`.

`Link al mio [sito](https://sbrzt.netlify.app).`

Link al mio [sito](https://sbrzt.netlify.app).

---

### Link veloci

Per trasformare rapidamente un URL o un indirizzo email in un link, racchiudilo tra caporali `< >`.

`<sebastian.barzaghi2@unibo.it>`

<sebastian.barzaghi2@unibo.it>

---

### Reference link

L'altro tipo di link si chiama reference link, poiché fa riferimento a un altro punto nel documento. 

```
    Ecco [un link a qualcos'altro][altro luogo].
    Ecco [un altro link][altro-link].
    E ora torniamo a [primo link][altro luogo].

    [altro luogo]: www.github.com
    [altro-link]: www.google.com
```

Ecco [un link a qualcos'altro][altro luogo].  
Ecco [un altro link][altro-link].  
E ora torniamo a [primo link][altro luogo].  

[altro luogo]: www.github.com  
[altro-link]: www.google.com

---

### Link interni

Per linkare ad un altro elemento (di solito un'intestazione) all'interno dello stesso documento, è sufficiente riprendere il testo dell'intestazione in minuscolo, sostituire gli eventuali spazi con il trattino `-`, e precederlo con il cancelletto `#`.

```
###### Intestazione sei

[Link all'intestazione sei](#intestazione-sei)
```

###### Intestazione sei

[Link all'intestazione sei](#intestazione-sei)

---

### Immagini

Se sai come creare link in Markdown, puoi creare anche immagini. La sintassi è quasi la stessa.

Per creare un'immagine, inserisci un punto esclamativo `!`, racchiudi il testo alternativo tra parentesi quadre `[ ]`, e poi racchiudi il link dell'immagine tra parentesi tonde `( )` (Il testo alternativo è una frase o una frase che descrive l'immagine per le persone con disabilità visive).

`![Benjamin Bannekat](http://octodex.github.com/images/founding-father.jpg)`

---

### Citazioni

Per creare una citazione, tutto quello che devi fare è precedere la linea con il simbolo "maggiore di" `>`.

`> Questa è una citazione.`

> Questa è una citazione.

---

### Liste

Esistono due tipi di liste: ordinate e non ordinate.

---

### Liste non ordinate

Per creare una lista non ordinata, precedi ogni elemento della lista con un asterisco `*`, seguito da uno spazio. Ogni elemento della lista deve essere su una propria linea.

```
* Primo elemento
* Secondo elemento
* Terzo elemento
```

* Primo elemento
* Secondo elemento
* Terzo elemento

---

### Liste ordinate

Una lista ordinata è preceduta da numeri, anziché asterischi.

```
1. Primo elemento
2. Secondo elemento
3. Terzo elemento
```

1. Primo elemento
2. Secondo elemento
3. Terzo elemento

---

### Indentazione

A volte, potresti aver bisogno di annidare una lista all'interno di un'altra. 

La sintassi è uguale, con l'aggiunta di quattro spazi (o un tab) prima dell'asterisco o numero dell'elemento indentato.

In alcune variazioni di Markdown, è sufficiente uno spazio.

```
* Primo elemento
  * Secondo elemento
  * Terzo elemento
```

* Primo elemento
  * Secondo elemento
  * Terzo elemento

---

### Paragrafi

I paragrafi sono delimitati dal newline (a capo + invio).

```
Primo paragrafo.

Secondo paragrafo.
```

Primo paragrafo.

Secondo paragrafo.

---

### Paragrafi 

Altrimenti, è possibile mantenere le righe vicine, ma separate da due spazi `  `.

```
Primo paragrafo.  
Secondo paragrafo.  
```

Primo paragrafo.  
Secondo paragrafo.  

---

### Codice

Per indicare un pezzo di testo come parte di un codice, racchiudilo tra backtick ```.

```
Questo è un pezzo di `codice`
```

QUesto è un pezzo di `codice`.

---

### Blocco di codice

Per creare blocchi di codice, indenta ogni linea del blocco di almeno quattro spazi o un tab.

```
    Questo è un blocco di codice
    che continua per molteplici
    righe.
```

---

### Separatori

Per creare un separatore orizzontale (una linea, in pratica), usa tre o più asterischi `***`, trattini `---` o trattini bassi `___`, da soli.

---

### Tabelle

Per aggiungere una tabella, usa tre o più trattini (---) per creare l'intestazione di ogni colonna, e usa il simbolo pipe `|` per separare ogni colonna e definire l'inizio e la fine di ogni riga.

```
| Intestazione 1            | Intestazione 2  |
| ------------------------- | --------------- |
| Intestazione              | Titolo          |
| Paragrafo                 | Testo           |
```

| Intestazione 1            | Intestazione 2  |
| ------------------------- | --------------- |
| Intestazione              | Titolo          |
| Paragrafo                 | Testo           |

---

## Esercizio pratico

---

### Obiettivo 1: sistemiamo i nostri README.txt, facendoli diventare README.md

* Tornate sul clone della repo su cui avete lavorato l'altra volta;
* Sincronizzate il vostro fork con la repo originale (sulla repo clonata: `Synch fork` > `Update branch`); 
* In `data`, create un nuovo file `README.md`;
* In `README.md`, copia-incollate i contenuti dai `README.txt`;
* Formattate il contenuti in Markdown, come mostrato nella prossima slide;
* Eliminate il `README.txt`;
* Fate un `pull request`, come l'altra volta.

---

### Come formattare il testo del README in `data`

- I testi in maiuscolo sono intestazioni (da organizzare in livelli);
- Le voci nell'indice devono essere elementi di una lista ordinata;
- Le voci nell'indice devono essere link interni che si riferiscono alle rispettive intestazioni;
- Il nome del file deve essere in codice;
- Le voci in Struttura devono essere elementi di liste non ordinate;
- Le voci in Struttura devono essere in grassetto;
- Link e mail 

---

### Obiettivo 2: stiliamo un DMP per il nostro progetto su Mythologiae

```
# Mythologiae - Data Management Plan

| Versione | Data       | Note                    |
| -------- | ---------- | ----------------------- |
| v0.1.0   | 21-11-2024 | Creazione del documento |

## Autori

- Sebastian Barzaghi -- ORCID -- AFFILIAZIONE -- RUOLO
- ...

## Sommario esecutivo

...

## Introduzione

...

## Descrizione dei dati

- Quali dati (ad esempio il tipo, i formati e i volumi) verranno raccolti o prodotti?
- Come verranno raccolti o prodotti i nuovi dati e/o come verranno riutilizzati i dati esistenti?

## Documentazione e qualità dei dati

- Quali metadati e documentazione (ad esempio la metodologia di raccolta dei dati e il modo di organizzare i dati) accompagneranno i dati?
- Quali misure di controllo della qualità dei dati saranno utilizzate?

## Backup e archiviazione

- Come saranno archiviati e salvati i dati e i metadati durante la ricerca?
- Come sarà gestita la sicurezza dei dati e la protezione dei dati sensibili durante la ricerca?

## Requisiti legali ed etici

- Come saranno gestite altre questioni legali, come i diritti di proprietà intellettuale e la proprietà? Quale legislazione si applica?
- Quali questioni etiche e codici di condotta ci sono e come saranno presi in considerazione?

## Condivisione dei dati e conservazione a lungo termine

- Come e quando i dati saranno condivisi? Ci sono possibili restrizioni alla condivisione dei dati o motivi di embargo?
- Come saranno selezionati i dati per la conservazione e dove saranno conservati a lungo termine (ad esempio un repository di dati o un archivio)?
- Quali metodi o strumenti software sono necessari per accedere e utilizzare i dati?
- Come sarà garantita l'applicazione di un identificatore unico e persistente (come un Digital Object Identifier (DOI)) a ciascun set di dati?

```

---

### Salviamo la nostra bozza di DMP in `docs`

---

# Fine

## Lezione 04 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)