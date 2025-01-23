---
title: ABINF - Pensiero Computazionale
summary: Lezione di Pensiero Computazionale del corso di Abilità Informatiche per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2024-01-27T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# Pensiero Computazionale

## Lezione 02 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

##  ALGORITMI

---

### Cos'è? (1/3)

IMG PAD THAI

---

### Cos'è? (2/3)

IMG ISTRUZIONI

---

### Cos'è? (3/3)

IMG MINDMAP

---

### Cosa hanno in comune?

IMG COMPOSITA

* Sequenziali
* Finiti
* Generali
* Non ambigui
* Corretti
* Efficienti

---

### In altre parole, sono **algoritmi**

---

### Un algoritmo è un insieme di istruzioni per fare qualcosa

Una sequenza finita di procedure precise per produrre un risultato (output) a partire da uno stato iniziale (input)

https://www.lospaziodirosanna.it/testo-e-testi/algoritmi-diagrammi-di-flusso-esempi-e-attivita/ 

---

### Esempio di algoritmo implementato

num1 = 1.5
num2 = 6.3

def function (n1, n2):
    sum = n1 + n2
    return sum

function(num1,num2)

---

### Un programmatore implementa algoritmi interpretabili dal computer

Quindi, un linguaggio di programmazione è un modo particolare per scrivere algoritmi e istruire un computer ad eseguirli

Un programma è un algoritmo (o insieme di algoritmi) scritto/i con un particolare linguaggio di programmazione che esegue delle particolari funzioni orientate allo svolgimento di alcuni compiti

---

## COMPUTER

---

### The kilo-girls

Prima degli anni ‘40: il computer è una _persona_ che effettua calcoli numerici a mano (es. posizioni dei pianeti, conversioni al sistema metrico)

https://www.messynessychic.com/2021/11/02/human-computer-the-forgotten-womens-profession/

Copeland, B. Jack, "The Modern History of Computing", The Stanford Encyclopedia of Philosophy (Winter 2020 Edition), Edward N. Zalta (ed.), URL: https://plato.stanford.edu/archives/win2020/entries/computing-history/. 


---

### Machine of the year

Dopo gli anni '40: sistema elettronico (programmabile o non programmabile) di elaborazione delle informazioni

https://www.computerhistory.org/timeline/1982/

Copeland, B. Jack, "The Modern History of Computing", The Stanford Encyclopedia of Philosophy (Winter 2020 Edition), Edward N. Zalta (ed.), URL: https://plato.stanford.edu/archives/win2020/entries/computing-history/. 

---

### La nostra definizione

Un agente che, se istruito correttamente, esegue calcoli a partire da qualche informazione iniziale (detta input) per produrre una risposta (detta output)

https://www.computerhistory.org/timeline/1982/

Copeland, B. Jack, "The Modern History of Computing", The Stanford Encyclopedia of Philosophy (Winter 2020 Edition), Edward N. Zalta (ed.), URL: https://plato.stanford.edu/archives/win2020/entries/computing-history/. 

---

### Componenti: Hardware

L'insieme delle componenti fisiche, non modificabili (alimentatori, elementi circuitali fissi, unità di memoria, ecc.), di un computer

Scheda madre
Central Processing Unit (CPU)
Graphics Processing Unit (GPU)
Random Access Memory (RAM)
Solid State Drive (SSD)
Hard Disk Drive (HDD)
Periferiche


Hemmendinger, D. , Pottenger, . William Morton , Freiberger, . Paul A. and Swaine, . Michael R. (2023, December 28). computer. Encyclopedia Britannica. https://www.britannica.com/technology/computer 

---

### Componenti: Software

L’insieme delle componenti digitali, modificabili (es. programmi, procedure, applicativi), di un computer

Google Chrome
Microsoft Word
Photoshop
Whatsapp
Windows
Elden Ring
…

Hemmendinger, D. , Pottenger, . William Morton , Freiberger, . Paul A. and Swaine, . Michael R. (2023, December 28). computer. Encyclopedia Britannica. https://www.britannica.com/technology/computer

---

## Computational thinking

---

### Mindstorms (Papert, 1980)

Impariamo costruendo iterativamente conoscenza

Rappresentazioni potenti consentono un apprendimento efficace

Computer come meta-strumento per “rendere l’astratto concreto” tramite un apprendimento per tentativi, sbagli, e correzioni

Pensiero computazionale come strumento di apprendimento basato sulla costruzione socialmente ed emotivamente partecipata di un artefatto

Lodi, M., & Martini, S. (2021). Computational thinking, between Papert and Wing. Science & education, 30(4), 883-908. https://doi.org/10.1007/s11191-021-00202-5 

---

### Computational Thinking (Wing, 2006)

Disponibilità di strumenti digitali, soprattutto sul World Wide Web

La maggior parte delle discipline diventano “computazionali”

Il pensiero computazionale è un atteggiamento e un insieme di competenze universalmente applicabili che vanno oltre l'informatica

Consiste in un approccio all’astrazione che aiuta a risolvere problemi e progettare soluzioni

Lodi, M., & Martini, S. (2021). Computational thinking, between Papert and Wing. Science & education, 30(4), 883-908. https://doi.org/10.1007/s11191-021-00202-5 

---

### Il computational thinking è un approccio di risoluzione dei problemi basato sui concetti della computazione

Definisce i processi mentali che coinvolgiamo quando formuliamo un certo problema ed esprimiamo le relative soluzioni usando un linguaggio che un computer (sia esso umano o macchina) può comprendere e, conseguentemente, eseguire

Lodi, M., & Martini, S. (2021). Computational thinking, between Papert and Wing. Science & education, 30(4), 883-908. https://doi.org/10.1007/s11191-021-00202-5 

---

### Principi della computazione

* Logica: prevedere e analizzare
* Algoritmi: Formulare sequenze e regole
* Pattern: Individuare e utilizzare similitudini
* Decomposizione: Suddividere in parti più piccole e gestibili
* Astrazione: Rimuovere dettagli non necessari
* Valutazione: Formulare giudizi

---

### Focus sull'astrazione

* Logica: prevedere e analizzare
* Algoritmi: Formulare sequenze e regole
* Pattern: Individuare e utilizzare similitudini
* Decomposizione: Suddividere in parti più piccole e gestibili
* **Astrazione: Rimuovere dettagli non necessari**
* Valutazione: Formulare giudizi

---

## Non possediamo nient'altro che metafore

---

### Il dilemma del porcospino

Quanto più due esseri umani si avvicinano tra loro per cercare calore e conforto, tanto più si feriranno a vicenda

Metafora sulle complessità delle relazioni e dell’intimità umana

Schopenhauer, A. (2000). Parerga and paralipomena: Short philosophical essays (Vol. 1). OUP UK.

---

### Cos'è una metafora?

Figura retorica che consiste nell’uso di un termine o concetto per rappresentare un altro termine o concetto

Una rappresentazione che aiuta a rendere più comprensibili concetti complessi

---

### Astrazione

Processo di rimozione dei dettagli trascurabili di una situazione in modo da semplificarla e focalizzare l’attenzione sulle sue caratteristiche principali

https://it.wikipedia.org/wiki/Metropolitana_di_Milano

---

### Astrazione

Usiamo queste astrazioni in modo intenzionale o inconscio nella vita quotidiana

Cosa hanno in comune le situazioni qui sotto?

https://unsplash.com/it/foto/spilla-da-balia-dargento-su-carta-bianca-Sl69Jw-o0rU

https://unsplash.com/it/foto/persone-che-camminano-in-un-centro-commerciale-JWEwaHqSAHU

---

### La mappa non è il territorio

Un’astrazione, che rappresenta qualcosa, non è quella cosa (ma può essere utile)

Korzybski, A. (1958). Science and sanity: An introduction to non-Aristotelian systems and general semantics. Institute of GS.

---

### La mappa è un'interpretazione

Quando facciamo un'astrazione, stiamo esplicitando le nostre assunzioni sulla natura della cosa che stiamo semplificando

ES: TESTO come OGGETTO LINGUISTICO, OGGETTO MATERICO, OGGETTO CONCETTUALE, ELENCO DI SIMBOLI...

---

### Astrazione nel CT

Dare nuovamente forma alle astrazioni che abbiamo già immagazzinato in passato come conseguenza della nostra esperienza personale – e che, spesso, riutilizziamo inconsciamente

Essere nuovamente e interamente coscienti di queste astrazioni significa doverle ridefinire usando un linguaggio appropriato per renderle comprensibili a un computer

Permettere alle persone di pensare come se fossero computer scientist, anche quando bisogna affrontare attività del quotidiano

---

### Una struttura dati è una specie di contenitore di informazioni

Descrizione delle informazioni presenti in una certa situazione secondo un’organizzazione generica e riutilizzabile in più contesti come parte del processo di astrazione

Esempi: liste, code, pile, insiemi, dizionari, alberi e grafi

Qualche idea di cosa possano essere questi oggetti?

---

### Lista

Sequenza ordinata di elementi potenzialmente ripetibili e numerabili

https://unsplash.com/it/foto/persona-che-scrive-la-lista-dei-desideri-sul-libro-RLw-UC03Gwc

---

### Pila

Lista in cui le operazioni di aggiunta e rimozione seguono una strategia last in first out (LIFO)

https://unsplash.com/it/foto/assorted-books-on-wooden-table-eMP4sYPJ9x0

---

### Coda

Un tipo di lista in cui le operazioni di aggiunta e rimozione seguono una strategia first in first out (FIFO)

https://unsplash.com/it/foto/persone-in-piedi-sul-pavimento-di-cemento-grigio-durante-il-giorno-ZAbIO5eas9Q

---

### Insieme

Una collezione di elementi non ordinati e non ripetibili che si possono contare

https://unsplash.com/it/foto/una-pila-di-barre-colorate-diverse-0Yi5hg61omY

---

### Dizionario

Una collezione non ordinata di elementi definiti da coppie chiave-valore non ripetibili

https://unsplash.com/it/foto/carta-bianca-per-stampante-con-testo-nero-1UDjq8s8cy0

---

### Albero

Un insieme di nodi collegati tra loro da una relazione gerarchica genitore-figlio

https://unsplash.com/it/foto/libro-di-fiabe-su-superficie-grigia-qtUAV-_yWZc

---

### Grafo

Un insieme di nodi di una rete collegati da archi (che possono essere orientati)

https://maa.org/press/periodicals/convergence/leonard-eulers-solution-to-the-konigsberg-bridge-problem

---

### Quiz

...

---

# Fine

## Lezione 02 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)