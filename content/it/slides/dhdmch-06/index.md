---
title: DHDMCH - L'oggetto bibliografia
summary: Introduzione al corso di Digital Humanities e Data Management per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2023-11-24T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# L'oggetto bibliografia

## Lezione 06 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

## Zotero

---

### Alcune attività fondamentali di ricerca

- Raccogliere letteratura scientifica;
- Costruire bibliografie;
- Citare risorse bibliografiche.

---

### Un flusso di lavoro classico...

![](img/0601.png)

---

### Un flusso di lavoro classico...

![](img/0602.png)

---

### Un flusso di lavoro classico...

![](img/0603.png)

---

### ... Con i soliti problemi

- Un sacco di PDF con nomi di file incomprensibili;
- Nessun collegamento tra metadati, file, note;
- Quando si cita, la migliore opzione è copiare e incollare;
- Difficile condividere articoli con metadati;
- Riformattazione a mano delle citazioni;
- Collaborazione difficile.

---

### Usiamo Zotero

Link: <https://www.zotero.org/>

Zotero è un servizio e un software gratuito e open-source per la gestione dei riferimenti bibliografici e dei metadati. 

Consente di raccogliere, organizzare, citare e condividere fonti bibliografiche in modo semplice e veloce.

In particolare, serve per:
- **Raccolta dei dati**: consente di raccogliere automaticamente metadati da articoli, libri, siti web e altre risorse online;
- **Organizzazione**: permette di organizzare i riferimenti in collezioni, aggiungere tag, note e allegare file PDF;
- **Citazioni e riferimenti**: genera citazioni in vari stili (APA, MLA, Chicago, ecc.) e crea bibliografie in modo automatico;
- **Condivisione**: facilita la collaborazione, permettendo di condividere raccolte di riferimenti con altri ricercatori.

---

### 1. Home page di Zotero.org

![](img/0604.png)

---

### 2. Login 

![](img/0605.png)

---

### 3. Registrazione

![](img/0606.png)

---

### 4. Interfaccia principale

![](img/0607.png)

---

### 5. Aggiunta di un nuovo item alla collezione

![](img/0608.png)

---

### 6. Colonna dei metadati bibliografici

![](img/0609.png)

---

### 7. Selezione di item e export

![](img/0610.png)

---

### 8. Produzione di citazioni inline

![](img/0611.png)

---

### 9. Produzionme di riferimenti bibliografici

![](img/0612.png)

---

## Attività pratica

---

### Scopriamo qualche dato di Mythologiae

Il dataset di Mythologiae è costituito da ~4389 righe e 31 colonne: 
* Ogni riga corrisponde ad un'opera d'arte;
* Ogni colonna orrisponde ad un metadato riferito all'opera d'arte (es. autore, tema mitologico, data di creazione, ecc.);

Tra le colonne, c'è anche `cho_sources_classic`, che indica le fonti classiche associate al tema mitologico individuato nell'opera.

---

### Oggi lavoriamo solo su un piccolo sottoinsieme di dati: le citazioni canoniche

Le citazioni canoniche sono un sistema di riferimento utilizzato principalmente nella letteratura classica, per citare testi antichi in modo breve e standardizzato. Esse indicano il titolo dell’opera, seguita dal libro e dalla sezione specifica.

- Opera: nome del testo (ad esempio, Apollodoro, Odissea, Erodoto);
- Libro: il numero del libro o della parte dell'opera;
- Sezione: il numero della sezione, capitolo o verso specifico.

Esempi:
- `Apollod. 3.5.8`, che equivale a "Apollodoro, _Biblioteca_, libro 3, capitolo 5, sezione 8";
- `Hom. Od. 11.273`, che equivale a "Omero, _Odissea_, libro 11, verso 273";
- `Hdt. 2.175`, che equivale a "Erodoto, _Storie_, libro 2, paragrafo 175".

---

### Cosa farete

- Esaminerete il dataset disponibile qui: ...
    - Due colonne: una contenente una serie di citazioni canoniche, l'altra i rispettivi link a Perseus;
- Cercherete su Perseus i dati contestuali della citazione (ove possibile), come l'editore, il luogo di pubblicazione, ecc.;
- Nella collezione `DHDMCH_2024-2025` condivisa su Zenodo, inserirete i dati bibliografici estratti dalla citazione e da Perseus;
    - La tipologia dell'opera sarà `Book` oppure `Book section`, a seconda che venga citato l'intero libro oppure solo una parte;
    - Nel campo `Extra` inserirete l'informazione specifica sulla parte dell'opera che viene citata:
        - Esempio: per `Apollod. 3.5.8` inserirete nel campo Extra "Libro 3, capitolo 5, sezione 8" (capirete cosa scrivere dal contesto).

---

## Altri lati di Zotero (che vi consiglio di esplorare)

---

### Zoterobib

![](img/0613.png)

---

### Zoterobib

![](img/0614.png)

---

### Zotero (software) e Zotero Connector (plugin per browser)

![](img/0615.png)

---

# Fine

## Lezione 06 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)
