---
title: DHDMCH - Tutto è rivelato
summary: Introduzione al corso di Digital Humanities e Data Management per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2023-12-09T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# Tutto è rivelato

## Lezione 13 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

## Voyant Tools: attività pratica

---

### Carichiamo un file tratto da Mythologiae

Link al sotto-dataset: <https://docs.google.com/spreadsheets/d/1v-H6uYEuJUE_1Jh7SOq4Dyhh6So1tdQU9kN7PuAFFGk/edit?usp=sharing>.
- Su GitHub: `tutorial` > `data` > `csv` > `README.md` > 4. Dataset Note e Descrizioni > Fonti > Selezione di colonne.

Link a Voyant Tools: <https://voyant-tools.org/>.

Scaricate il sotto-dataset in CSV, ed effettuate l'upload di questo su Voyant Tools.

---

### 1. Parole chiave e frequenze

Scopriamo quali sono le 10 parole più frequenti utilizzate.

- Di quali dati si tratta?
- Quale/i visualizzazione/i usereste?
- Cosa notate (qualsiasi cosa, anche "ovvio" o "banale")?
- Ci sono parole che potrebbero essere escluse (cioé aggiunte alla lista di stopwords)? Come cambia l'analisi?

---

### Aggiungere le _stopword_

Su alcune skin (es. `Cirrus`), è possibile cliccare sulle opzioni (la terza icona nell'angolo in alto a destra della skin).

Tra le opzioni, abbiamo le _stopword_. Di default, l'opzione attiva è l'auto-detect (cioé le stopword sono individuate in automatico, sulla base della lingua del testo). 

Per modificare manualmente l'elenco di stopword, è sufficiente cliccare su `Edit List` e aggiungere o togliere parole (ad ogni parola deve corrispondere una riga!).

Una volta salvate e confermate le modifiche, cosa succede?

---

### 2. Relazioni tra parole

Scopriamo come le parole sono collegate tra loro in base alla loro co-occorrenza, utilizzando anche le funzioni di ricerca testuale.

- Di quali dati si tratta?
- Quale/i visualizzazione/i usereste?
- Cosa notate (qualsiasi cosa, anche "ovvio" o "banale")?

---

### Effettuare le ricerche

- `pestilenza`: trova il termine esatto;
- `pestilen*`: trova termini che iniziano con "pestilen";
- `"marito e moglie"`: cerca l'intera espressione;
- `"opera misericordia"~5`: "opera" e "misericordia" co-occorrono
entro 5 termini;
- `@Personaggi`: ricerca raggruppata di tutti i termini inclusi in una
categoria;
- `^@Personaggi`: ricerca dei singoli termini inclusi in una categoria.

---

### Aggiungere categorie

Gruppi di parole semanticamente connesse (es. personaggi, luoghi, emozioni) da usare per ricerche mirate.

- Cliccate su opzioni;
- Vicino alla voce _Categories_, cliccate su _Edit_;
- Potete rimuovere le categorie esistenti;
- Cliccate su _Add Category_;
- Scrivete un nome per la categoria, e.g. _Personaggi_ e cliccate su _Add_;
- Trascinate i nomi dei personaggi dalla lista _Terms_ alla lista _Personaggi_;
- Salvare cliccando su _Save_.

---

### Esplorate!

---

### Esportate le visualizzazioni

- Cliccate sull'icona per l'esportazione (la prima in alto a destra nel riquadro della skin);
- Cliccate su _Export Visualization_ e poi _Export a PNG image of this visualization_;
- Sincronizzate, caricate le immagini nel vostro clone della repo, dentro `tutorial` > `doc` > `img` > `viz`, e fate il pull request.

---

# Fine

## Lezione 13 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)
