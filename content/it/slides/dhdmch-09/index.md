---
title: DHDMCH - L'oltretesto
summary: Introduzione al corso di Digital Humanities e Data Management per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2023-11-24T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# L'oltretesto

## Lezione 09 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

## RDF

---

### Resource Description Framework

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/rdf.png" height="auto" width="700"/>
      <figcaption>
          Fonte: Bernard, C. (2019). Immersing evolving geographic divisions in the semantic Web (Doctoral dissertation, Université Grenoble Alpes). <a href="https://theses.hal.science/tel-02524361v1">https://theses.hal.science/tel-02524361v1</a>. 
      </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Modello di dati standard che permette di rappresentare, descrivere, e pubblicare i dati sul Web in un formato accessibile e interpretabile dalle macchine tramite l'utilizzo di triple soggetto-predicato-oggetto.
    </p>
  </div>
</div>

<div class="footer">
Jonathan Blaney, "Introduction to the Principles of Linked Open Data," Programming Historian 6 (2017), <a href="https://doi.org/10.46430/phen0068">https://doi.org/10.46430/phen0068</a>. 
</div>

---

###  L’unità minima nei LOD: la tripla RDF

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
    <img src="img/triple.png" height="auto" width="700"/>
      <figcaption>
          Fonte: Jonathan Blaney, "Introduction to the Principles of Linked Open Data," Programming Historian 6 (2017), <a href="https://doi.org/10.46430/phen0068">https://doi.org/10.46430/phen0068</a>.
      </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
      <p>
        Costrutto astratto minimo di modellazione dei LOD.
      </p>
      <p>
        <ul>
          <li>Soggetto: un'entità (sempre identificata da un URI);</li>
          <li>Predicato: una caratteristica del soggetto (sempre identificata da un URI);</li>
          <li>Oggetto: un'entità (identificata da un URI) o un valore (letterale, numerico, temporale, ecc.).</li>
        </ul>
      </p>
      <p>
        Le triple si collegano tra loro, formando un grafo di dati.
      </p>
  </div>
</div>

<div class="footer">
Jonathan Blaney, "Introduction to the Principles of Linked Open Data," Programming Historian 6 (2017), <a href="https://doi.org/10.46430/phen0068">https://doi.org/10.46430/phen0068</a>. 
</div>

---

### ESEMPIO CON NEUROMANTE

---

### RDF COME GRAFO

---

### Un piccolo limite di RDF in quanto modello di dati

Dice _cosa_ fare, ma non dice:
- _Come scrivere triple_: per questo ci sono le **serializzazioni** (es. RDF/XML, Turtle, ecc.) che specificano la **sintassi** da usare;
- _Come esprimere entità e proprietà_: per questo esistono i **modelli semantici** (es. vocabolari controllati, ontologie, ecc.) che specificano il **lessico** da usare.

---

### Un esempio di serializzazione RDF: Turtle

```
@prefix dhdmch: <http://example.org/> .
@prefix ex: <http://example.org/data/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .

ex:neuromante a dhdmch:Book ;
    dhdmch:publicationDate "1984" ;
    dhdmch:genre dhdmch:cyberpunk ;
    dhdmch:creator ex:william-gibson ;
    dhdmch:pages "271" .

ex:william-gibson a dhdmch:Person .
```

---

### Turtle: prefissi

Per ogni modello, dicitura `@prefix` + prefisso (a vostra scelta, esistono convenzioni tacite) + URI del modello tra caporali + punto

```
@prefix dhdmch: <http://example.org/> .
@prefix ex: <http://example.org/data/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .

...
```

---

### Turtle: prefissi

I prefissi ci evitano di dover ripetere l'URI completo ogni volta (ricordate: per riferirci a risorse e proprietà _dobbiamo_ usare gli URI).

```
@prefix dhdmch: <http://example.org/> .
@prefix ex: <http://example.org/data/> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .

ex:neuromante rdf:type dhdmch:Book .
```

Volendo "Neuromante", "è un" e "Libro" possiamo scriverli anche così:

`http://example.org/data/neuromante http://www.w3.org/1999/02/22-rdf-syntax-ns#type http://example.org/libro`

---

### Turtle: triple

Una tripla in Turtle è scritta sequenziando soggetto, predicato e oggetto uno dopo l'altro e separati da uno spazio.

Una tripla finisce sempre con un punto.

```
ex:neuromante rdf:type dhdmch:Book .  
ex:neuromante dhdmch:publicationDate "1984" .  
ex:neuromante dhdmch:genre dhdmch:cyberpunk ;  
ex:neuromante dhdmch:creator ex:william-gibson ;  
ex:neuromante dhdmch:pages "271" .
```

---

### Turtle: triple

Se abbiamo più triple con lo stesso soggetto, possiamo utilizzare una sintassi più elegante, con una prima tripla che esprime il soggetto e tutte le altre indentate sotto la prima che sottointendono il soggetto. 

Ogni tripla che non è l'ultima finisce con il punto e virgola.

```
ex:neuromante rdf:type dhdmch:Book ;  
    dhdmch:publicationDate "1984" ;  
    dhdmch:genre dhdmch:cyberpunk ;  
    dhdmch:creator ex:william-gibson ;  
    dhdmch:pages "271" .  
```

---

### Però non c'è interoperabilità

Il nostro `dhdmch` è in sostanza la reinvenzione della ruota: esistono già molteplici modelli in grado di descrivere libri (e il dominio bibliografico in senso lato). 

Inoltre, ci servono il modello anche per rappresentare "Persona" e il vocabolario controllato da cui attingere il valore "cyberpunk".

A patto di rispettare le costrizioni logiche dei vari modelli, li possiamo combinare per fare una descrizione interoperabile dei dati.

Alcuni modelli:
- [FaBiO]()
- [Dublin Core Terms]()
- [PRISM]()
- [FOAF]()
- [Wikidata]()

---

### Le triple, riscritte con modelli esistenti

- `dhdmch:Book` diventa ... (abbreviato in `fabio:Book`);
- dhdmch:publicationDate
- dhdmch:genre
- `dhdmch:cyberpunk` diventa `https://www.wikidata.org/wiki/Q174526` (abbreviato in `wd:Q174526`);
- `dhdmch:creator` diventa ... (abbreviato in `dct:creator`);
- dhdmch:pages
- `dhdmch:Person` diventa ... (abbreviato in `foaf:Person`).

Libro → http://purl.org/spar/fabio/Book 
Genere → http://www.w3.org/2004/02/skos/core#Concept 
Persona → http://xmlns.com/foaf/0.1/Person 
è un/una → http://www.w3.org/1999/02/22-rdf-syntax-ns#type 
pubblicato nel → http://prismstandard.org/namespaces/basic/2.0/publicationDate 
ha genere → http://purl.org/dc/terms/type 
scritto da → http://purl.org/dc/terms/creator 
ha pagine → http://purl.org/spar/fabio/hasPageCount 

---

### Le triple, riscritte con modelli esistenti

```
@prefix ex: <http://example.org/data/> .
@prefix fabio: <> .
@prefix dct: <> .
@prefix foaf: <> .
@prefix XXX: <> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .

ex:neuromante rdf:type fabio:Book ;  
    XXX:publicationDate "1984" ;  
    XXX:genre wd:Q174526 ;  
    dct:creator ex:william-gibson ;  
    XXX:pages "271" .

ex:william-gibson a foaf:Person .
```

---

## ALTRE INDICAZIONI SU MODELLAZIONE

---

### non esiste un unico modello

Ipotizziamo che non abbiamo interesse a modellare le persone come entità, ma ci basta sapere i nomi delle persone coinvolte nel ciclo di vita del libro

IMG

---

### non esiste un unico modello

Non abbiamo più la classe Persona
“scritto da” diventa un attributo di Libro
Modello più semplice, ma perdiamo espressività ed elasticità

---

### non esiste un unico modello

Ipotizziamo che abbiamo interesse a modellare il tempo come periodo caratterizzato da un inizio e una fine

---

### non esiste un unico modello

Abbiamo una nuova entità “1984” appartenente alla nuova classe “Intervallo di tempo” con due attributi “data di inizio” e “data di fine”
“pubblicato nel” diventa una relazione
Modello più complesso ed espressivo

---

### non esiste un unico modello

Ipotizziamo che abbiamo interesse a modellare le pagine singole

---

### non esiste un unico modello

Abbiamo 271 nuove entità appartenente alla nuova classe “Pagina”
“ha pagine” diventa una relazione
Modello più espressivo, interessato all'aspetto strutturale

---

### Ereditarietà 

Esiste anche una graphic novel di Neuromante

Siamo interessati a modellare anche questa entità e le sue caratteristiche

Quale classe le assegnamo?

---

Potremmo trattarla come istanza della classe “Libro”, dato che ci interessano le stesse caratteristiche

Ma ci interessa modellare anche una caratteristica particolare della graphic novel: chi l’ha illustrata (Bruce Jensen, una nuova entità appartenente a “Persona”)

---

Creiamo una classe “Graphic novel”, le assegnamo la nuova entità “Neuromante: la Graphic Novel, Vol. 1”, stabiliamo una relazione “illustrato da” tra la graphic novel e la nuova entità “Bruce Jensen”

Ma ricordiamoci che ci interessano anche altre caratteristiche, tipiche di un Libro: chi l’ha scritta? quante pagine ha? di quale genere fa parte?

---

Una sottoclasse eredita tutte le proprietà della propria superclasse e (solitamente) ha proprietà aggiuntive che ne giustificano l’esistenza 

“Graphic novel” eredita TUTTE le proprietà di “Libro” (in questo caso stiamo utilizzando solo “ha pagine”), e in aggiunta ha anche “illustrato da”

---

### Proprietà o classe: tipizzazione

I concetti di Libro e Graphic novel sono Classi

Molteplici classi particolari (maggiore espressività, molto difficile da mantenere)


I concetti di Libro e Graphic novel sono Tipi: ci servono per classificare oggetti bibliografici

Stessa differenziazione, ma con meno classi e nessuna informazione particolare (minore espressività, molto più facile da gestire)


---

### Proprietà o classi: eventi

Il concetto di creazione di un Libro è reso da una relazione “scritto da” tra Libro e Agente

Impossibile capire chi ha pubblicato quando


Il concetto di creazione di un Libro è una classe “Creazione” che rappresenta l’evento in cui un’istanza di libro è stata creata da un’istanza di Agente

Il concetto di “Pubblicazione” (inteso come attività o evento) permette di disambiguare (rendendo il modello più complesso e più corretto)


---

## Attività pratica

---

### CONTESTO

dcho_id	dcho_title	dcho_publication_date	dcho_permalink	dcho_image_related	dcho_image_title	dcho_image_description	dcho_image_alt_text	dcho_image_url

cho_title	cho_author	cho_description	cho_period	cho_century	cho_date	cho_type	cho_location	cho_note	cho_related	cho_sources_classic	cho_sources_other	cho_sources_classic_link

---

### ATTIVITA
fate un piccolo modello di una parte (CAPIRE QUALE)
prima grafico (MAGARI QUESTO GLIELO FORNISCO IO)?
poi scritto in turtle
usando una riga di dati
e riusando queste ontologie

---

salvate il file in ttl
salvate il tutto in `data` > `rdf`
salvate l'immagine in `docs` > `assets` > `img` 

---

# Fine

## Lezione 09 del corso di _Digital Humanities e Data Management per i Beni Culturali_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)
