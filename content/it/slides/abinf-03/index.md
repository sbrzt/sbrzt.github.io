---
title: ABINF - Rappresentare l'informazione
summary: Lezione di "Rappresentare l'informazione" del corso di Abilità Informatiche per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2024-01-27T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# Rappresentare l'informazione

## Lezione 03 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

### Una sonda nell'orbita di Marte

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0301.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.bbc.co.uk/bitesize/guides/zp92mp3/revision/1">https://www.bbc.co.uk/bitesize/guides/zp92mp3/revision/1</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      1988, Cape Canaveral, 2 settimane a Natale.
    </p>
    <p>
      La NASA lancia la missione Mars Climate Orbiter, con l'obiettivo di inserire una sonda nell'orbita di Marte per effettuare investigazioni scientifiche sul clima del pianeta rosso e per fare da ponte radio con la Terra.
    </p>
  </div>
</div>

<div class="footer">
Novelli, A. (2023). Il disastro del Mars Climate Orbiter. Astrospace.
 <a href="https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/">https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/</a>.
</div>

---

### L'errore da 125 milioni di dollari

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0302.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.bbc.co.uk/bitesize/guides/zp92mp3/revision/1">https://www.bbc.co.uk/bitesize/guides/zp92mp3/revision/1</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Il 23 settembre 1999, dopo 283 giorni di viaggio nello spazio, la sonda, dal valore di 125 milioni di dollari, eseguì una manovra ad alta quota nell'orbita di Marte con 49 secondi di anticipo: in altre parole, non stava seguendo la traiettoria prevista.
    </p>
    <p>
      Alle 2:27 del mattino, la sonda scompare dietro Marte per non riapparire mai più.
    </p>
  </div>
</div>

<div class="footer">
Novelli, A. (2023). Il disastro del Mars Climate Orbiter. Astrospace.
 <a href="https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/">https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/</a>.
</div>

---

### Il motivo del fallimento

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0303.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.bbc.co.uk/bitesize/guides/zp92mp3/revision/1">https://www.bbc.co.uk/bitesize/guides/zp92mp3/revision/1</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Una settimana dopo la perdita della sonda, la NASA rilascia una dichiarazione, attribuendo l'incidente a un errore legato al sistema usato per ricalcolare la posizione della sonda nello spazio. 
    </p>
    <p>
      Tra la sonda e la NASA c'era uno scambio continuo di dati, che permetteva il ricalcolo della traiettoria della sonda rispetto all'obiettivo finale.
    </p>
  </div>
</div>

<div class="footer">
Novelli, A. (2023). Il disastro del Mars Climate Orbiter. Astrospace.
 <a href="https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/">https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/</a>.
</div>

---

### Due lingue diverse

La Lockheed Martin, azienda incaricata di realizzare la sonda e alcuni strumenti usati dai tecnici per gestirla, aveva adottato la **libbra-forza per secondo** come unità di misura per il ricalcolo.

La NASA, invece, utilizzava il **Newton per secondo**.

<div class="footer">
Novelli, A. (2023). Il disastro del Mars Climate Orbiter. Astrospace.
 <a href="https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/">https://www.astrospace.it/2022/09/23/il-disastro-del-mars-climate-orbiter/</a>.
</div>

---

### Tra codifiche e metadati

Senza le unità di misura, i dati numerici non hanno significato, e assumere erroneamente determinate unità può portare a gravi problemi.

I comandi di navigazione dovevano essere codificati correttamente nelle unità appropriate per essere compresi da entrambi i sistemi.

---

{{< slide background-image="img/0304.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## Una questione di linguaggio

<!--

-->

---

### Un linguaggio naturale è quello parlato da noi

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0305.jpg" height="auto" width="700"/>
        <figcaption>
            Fonte: Foto di <a href="https://unsplash.com/@mikham?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Mikayla Storms</a> su <a href="https://unsplash.com/photos/man-in-black-helmet-riding-brown-horse-during-daytime-9h_bJdGqzCk?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Linguaggio caratterizzato da ricchezza espressiva, ambiguità e ridondanza, per cui un qualsiasi costrutto formulato è potenzialmente polisemico.
    </p>
    <p>
      Esempio: "Sposto il cavallo".
    </p>
  </div>
</div>

<div class="footer">
Formal and Natural Languages. In How To Think Like A Computer Scientist: Interactive Edition.  
 <a href="https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html">https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html</a>.
</div>

---

### Un linguaggio naturale è quello parlato da noi

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0306.jpg" height="auto" width="700"/>
        <figcaption>
            Fonte: Foto di <a href="https://unsplash.com/@vdphotography?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">VD Photography</a> su <a href="https://unsplash.com/photos/a-group-of-chess-pieces-sitting-on-top-of-a-chess-board-qHv3EowYEk0?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Linguaggio caratterizzato da ricchezza espressiva, ambiguità e ridondanza, per cui un qualsiasi costrutto formulato è potenzialmente polisemico.
    </p>
    <p>
      Esempio: "Sposto il cavallo".
    </p>
  </div>
</div>

<div class="footer">
Formal and Natural Languages. In How To Think Like A Computer Scientist: Interactive Edition.  
 <a href="https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html">https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html</a>.
</div>

---

### Un linguaggio formale è quello usato per ridurre al minimo l'incertezza

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0307.jpg" height="auto" width="700"/>
        <figcaption>
            Fonte: Foto di <a href="https://unsplash.com/@thisisengineering?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">ThisisEngineering</a> su <a href="https://unsplash.com/photos/woman-in-black-long-sleeve-shirt-GzDrm7SYQ0g?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
      .
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Linguaggio per formulare costrutti dotati di significato in modo preciso e non ambiguo.
    </p>
    <p>
      Per comunicare con un computer, l'ambiguità del linguaggio naturale è un problema (servono altre informazioni relative al contesto e alla pragmatica che un computer, di base, non recepisce), quindi vengono usati linguaggi formali.
    </p>
  </div>
</div>

<div class="footer">
Formal and Natural Languages. In How To Think Like A Computer Scientist: Interactive Edition.  
 <a href="https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html">https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html</a>.
</div>

---

### Un linguaggio formale è costituito da tre elementi

* **Alfabeto**: insieme finito di simboli;
  * Esempio: `{a, b, c}` (un alfabeto costituito da tre simboli: `a`, `b` e `c`);
* **Grammatica**: insieme di regole sintattiche che specificano combinazioni valide di simboli;
  * Esempio: `G → a ∣ b ∣ c` (`G` è una grammatica che stabilisce che possiamo solo usare `a`, `b` o `c` separatamente);
* **Semantica**: insieme di significati attribuiti ai simboli e alle loro combinazioni;
  * Esempio: `a: "rosso" ; b: "blu" ; c: "verde"` (ad ogni simbolo ed eventuali combinazioni viene associato un significato).

<div class="footer">
Formal and Natural Languages. In How To Think Like A Computer Scientist: Interactive Edition.  
 <a href="https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html">https://runestone.academy/ns/books/published/thinkcspy/GeneralIntro/FormalandNaturalLanguages.html</a>.
</div>

---

{{< slide background-image="img/0308.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

### Il linguaggio di un semaforo!

<!--
Photo by <a href="https://unsplash.com/@thealmani?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">almani ماني</a> on <a href="https://unsplash.com/photos/red-stop-light-on-green-background-g6mxlM-h0jQ?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

{{< slide background-image="img/0309.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## La codifica

<!--
Photo by <a href="https://unsplash.com/@gabiontheroad?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Gabriella Clare Marino</a> on <a href="https://unsplash.com/photos/gray-and-white-abstract-painting-J5zIt97NYxQ?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

### Una codifica è il processo di trasformazione di un'informazione da un alfabeto ad un altro

Tecnica con la quale un dato viene rappresentato mediante un definito insieme di simboli.

Con tali simboli è possibile formare sequenze che possono essere messe in relazione biunivoca con gli elementi costituenti l'informazione.

Esempi:
* Numero di matricola
* Braille
* Codice fiscale
* Morse
* ...

---

### La codifica dei numeri

---

### Partiamo dalla notazione decimale posizionale

La codifica più comunemente adottata oggi per la rappresentazione dei numeri interi.

Il termine **decimale** indica il numero di simboli utilizzati (**cifre**): `{0, 1, 2, 3, 4, 5, 6, 7, 8, 9}`.

Il termine **posizionale** indica che il significato dei simboli cambia in base alla loro posizione. Il numero rappresentato da ogni simbolo è moltiplicato per una potenza di 10 (il numero di simboli che cotituiscono l'alfabeto, la **base**).

Con `n` cifre è possibile rappresentare 10<sup>n</sup> numeri naturali: da 0 a 10<sup>n</sup>-1.

Es. con 4 cifre possiamo rappresentare 10<sup>4</sup> numeri (da 0 a 9999).

<div class="footer">
Rappresentazione posizionale degli interi. <a href="http://www-dft.ts.infn.it/~pastore/DIDA/MNF/posizionale.html">http://www-dft.ts.infn.it/~pastore/DIDA/MNF/posizionale.html </a>.
</div>

---

### Esempio: il numero 2465

Il significato di ogni simbolo dipende dalla posizione di questo all'interno della sequenza di simboli creata in base alla loro combinazione. 

<code>2 X 10<sup>3</sup> + 4 X 10<sup>2</sup> + 6 X 10<sup>1</sup> + 5 X 10<sup>0</sup></code>

Che equivale a 2 _migliaia_ + 4 _centinaia_ + 6 _decine_ + 5 _unità_.

<div class="footer">
Rappresentazione posizionale degli interi. <a href="http://www-dft.ts.infn.it/~pastore/DIDA/MNF/posizionale.html">http://www-dft.ts.infn.it/~pastore/DIDA/MNF/posizionale.html</a>.
</div>

---

### Esistono codifiche non posizionali?

Il sistema di numerazione romano!

Si tratta di un **sistema additivo** basato su:

* Un alfabeto di simboli letterari a ciascuno dei quali viene assegnato un valore numerico;
* Un numero è rappresentato da una sequenza di tali simboli;
* Il valore di un numero è dato dalla somma dei valori corrispondenti ai simboli ottenuti, se in ordine decrescente; altrimenti, li si sottrae.

Esempi:
* `VIII = 5 + 1 + 1 + 1 = 8`;
* `IV = 5 - 1 = 4`.

---

### Esistono codifiche non decimali?

---

### L'informazione va codificata per il computer

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0310.jpg" height="auto" width="700"/>
        <figcaption>
            Fonte: Foto di <a href="https://unsplash.com/@aler?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">alerkiv</a> su <a href="https://unsplash.com/photos/close-up-photography-of-green-motherboard--9jmFkN-_U4?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Il computer memorizza ed elabora vari tipi di informazioni (numeri, testi, immagini, suoni, ecc.).
    </p>
    <p>
      Occorre rappresentare tale informazione in un formato facilmente manipolabile dal computer.
    </p>
  </div>
</div>

---

### Di fatto, un computer è una grande collezione di dispositivi _bistabili_

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0311.jpg" height="auto" width="700"/>
        <figcaption>
            Fonte: Foto di <a href="https://unsplash.com/@mk__s?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">mk. s</a> su <a href="https://unsplash.com/photos/a-light-switch-cover-on-a-white-wall-Ual1Obieofc?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      "Bistabile" indica qualcosa che può assumere nel tempo solo due stati stabili (es. interruttore). Nel caso del computer, si tratta della presenza / assenza di corrente elettrica.
    </p>
    <p>
       Per ogni tipo di informazione (numerica, testuale, grafica, sonora, ecc.) che vogliamo trattare con un computer, dobbiamo individuare una codifica che si avvalga esclusivamente di questa caratteristica.
    </p>
  </div>
</div>

---

### Consideriamo un alfabeto binario

Alfabeto: `{0, 1}`.

**Bit**: cifra binaria, ovvero uno dei due simboli del sistema numerico binario, classicamente chiamati _zero_ (0) e _uno_ (1).

Allo _zero_ sono spesso associate le idee di "chiuso", "spento", "assente", "falso".

All'_uno_ sono spesso associate le idee di "aperto", "acceso", "presente", "vero".

<div class="footer">
History of the Binary System. In Cut The Knot.
 <a href="https://www.cut-the-knot.org/do_you_know/BinaryHistory.shtml">https://www.cut-the-knot.org/do_you_know/BinaryHistory.shtml</a>.
</div>

---

### Con 1 bit rappresentiamo poco...

Solo 2 diverse informazioni:

* 0 → No / Falso / Off;
* 1 → Si / Vero / On.

---

### ... Ma se usassimo più bit?

Proviamo a rappresentare le stagioni con una codifica binaria. Le stagioni sono 4, quindi ci servono 2 bit (2<sup>2</sup> sequenze possibili).

* 00 → Primavera;
* 10 → Estate;
* 01 → Autunno; 
* 11 → Inverno.

Mettendo insieme più bit possiamo rappresentare più informazioni e quindi più complessità.

---

### La binarietà è conveniente

2 bit : 4 (2<sup>2</sup>) sequenze possibili: 00, 01, 10, 11.

3 bit: 8 (2<sup>3</sup>) sequenze possibili: 000, 001, 010, 100, 011, 101, 110, 111.

...

Con `n bit` possiamo rappresentare 2<sup>n</sup> sequenze: da 0 a 2<sup>n</sup>-1.

8 bit costituiscono un **byte**.

---

### Codifica numerica da base 2 a base 10

Moltiplicare ogni bit per il suo peso (attenzione a partire da 2<sup>n</sup>-1!) e sommare le potenze.

10100  

1 X 2<sup>4</sup> + 0 X 2<sup>3</sup> + 1 X 2<sup>2</sup> + 0 X 2<sup>1</sup> + 0 X 2<sup>0</sup>  
= 1 X 16 + 0 X 8 + 1 X 4 + 0 X 2 + 0 X 1  
= 16 + 0 + 4 + 0 + 0  

= 20  

---

### Codifica numerica da base 10 a base 2

Dividere il numero per 2 ripetutamente fino ad arrivare a zero e disporre i resti in ordine inverso.

12

12 / 2 → resto 0
= 6 / 2 → resto 0
= 3 / 2 → resto 1
= 1 / 2 → resto 1 

Prendiamo i resti dall'ultimo al primo:

= 1100

---

### Quindi…

* Conosciamo la numerazione in base 2;
* Conosciamo la numerazione in base 10;
* Sappiamo passare da una base di numerazione all'altra (cioé convertire i numeri in bit).

Come digitalizziamo invece la lettera `a`?

---

## La codifica del testo

---

### I caratteri corrispondono a codici binari

L'alfabeto anglosassone ha circa 120 caratteri (maiuscole + minuscole + numeri + interpunzione + ...)

Quanti bit ci servono per coprirli tutti?

Bastano 7 bit = 2<sup>7</sup> = 128 sequenze.

---

### American Standard Code for Information Interchange (ASCII)

Codifica secondo la quale ogni carattere è rappresentato da una sequenza di 7 bit.

Esempi:

* `A` → `1000001`;
* `B` → `1000010`;
* `BABA` → `1000010 1000001 1000010 1000001`.

---

### ASCII esteso

* Estensione di ASCII a 8 bit (2<sup>8</sup> = 256 simboli);
* Codifica quasi tutti i linguaggi occidentali;
* Include molti altri simboli utili.

Esempi:

* `CAT` → `01000011 01000001 01010100`;
* `cat` → `01100011 01100001 01110100`.

---

### Un altro esempio

<figure>
  <img src="img/0312.png" height="auto" width="700"/>
    <figcaption>
        Fonte: <a href="https://computerscienceiseasy.com/an-introduction-to-ascii-and-unicode/">https://computerscienceiseasy.com/an-introduction-to-ascii-and-unicode/</a>.
    </figcaption>
</figure>

---

### L'altra metà del problema

La digitalizzazione - cioé codificare contenuto informativo in binario - è solo metà del problema.

Dobbiamo anche codificare le caratteristiche del contenuto, cioé contestualizzarlo ("specificare le unità di misura", nel caso della sonda spaziale).

---

## I dati sopra (e oltre) i dati

---

### Cosa sono i metadati?

<figure>
  <img src="img/0313.png" height="auto" width="700"/>
    <figcaption>
        Fonte: <a href="https://dataedo.com/kb/data-glossary/what-is-metadata">https://dataedo.com/kb/data-glossary/what-is-metadata</a>.
    </figcaption>
</figure>

---

### Cosa sono i metadati?

<figure>
  <img src="img/0314.png" height="auto" width="600"/>
    <figcaption>
        Fonte: <a href="https://dataedo.com/kb/data-glossary/what-is-metadata">https://dataedo.com/kb/data-glossary/what-is-metadata</a>.
    </figcaption>
</figure>

---

### Cosa sono i metadati?

<figure>
  <img src="img/0315.png" height="auto" width="400"/>
    <figcaption>
        Fonte: <a href="https://dataedo.com/kb/data-glossary/what-is-metadata">https://dataedo.com/kb/data-glossary/what-is-metadata</a>.
    </figcaption>
</figure>

---

### Dati su dati

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0316.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://medium.com/towards-data-science/what-is-metadata-800403c0767b">https://medium.com/towards-data-science/what-is-metadata-800403c0767b</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      I metadati possono essere visti come l'insieme di tutto ciò che si può dire su un dato (oggetto informativo) in un determinato momento, a qualsiasi livello di aggregazione.
    </p>
  </div>
</div>

<div class="footer">
Baca, M. (Ed.). (2016). Introduction to metadata. Getty Publications.
 <a href="https://www.getty.edu/publications/intrometadata/">https://www.getty.edu/publications/intrometadata/</a>.
</div>

---

### Sembra roba complicata...

<figure>
  <img src="img/0320.png" height="auto" width="700"/>
    <figcaption>
        Fonte: Margaritopoulos, Merkourios & Margaritopoulos, Thomas & Mavridis, Ioannis & Manitsaris, Athanasios. (2012). Quantifying and Measuring Metadata Completeness. Journal of the American Society for Information Science and Technology. 63. <a href="http://dx.doi.org/10.1002/asi.21706">http://dx.doi.org/10.1002/asi.21706</a>. 
    </figcaption>
</figure>

---

### I metadati dovrebbero riflettere tre caratteristiche di ciò che descrivono

* **Contenuto**: ciò che l'oggetto contiene o rappresenta (intrinseco all'oggetto);
* **Contesto**: informazioni su chi, cosa, quando, dove e come l'oggetto è stato creato e utilizzato (estrinseco all'oggetto):
* **Struttura**: le relazioni formali tra gli oggetti informativi, che possono essere intrinseche, estrinseche o entrambe.

<div class="footer">
Baca, M. (Ed.). (2016). Introduction to metadata. Getty Publications.
 <a href="https://www.getty.edu/publications/intrometadata/">https://www.getty.edu/publications/intrometadata/</a>.
</div>

---

### Funzioni dei metadati

* Organizzazione e descrizione;
* Validazione e autenticazione;
* Ricerca e recupero;
* Utilizzo e conservazione.

<div class="footer">
Baca, M. (Ed.). (2016). Introduction to metadata. Getty Publications.
 <a href="https://www.getty.edu/publications/intrometadata/">https://www.getty.edu/publications/intrometadata/</a>.
</div>

---

### Caratteristiche (non ovvie) dei metadati

- Non devono essere per forza digitali;
- Sono più di semplici descrizioni dei dati;
- Possono provenire da diverse fonti;
- Continuano ad accumularsi durante tutto il ciclo di vita di un dato;
- Possono essere metadati per qualcuno e dati per qualcun'altro.

<div class="footer">
Baca, M. (Ed.). (2016). Introduction to metadata. Getty Publications.
 <a href="https://www.getty.edu/publications/intrometadata/">https://www.getty.edu/publications/intrometadata/</a>.
</div>

---

### Esistono diverse tipologie di metadati (e diversi modi di classificarli)

- **Descrittivi**: permettono la scoperta, l'identificazione e la selezione della risorsa. Includono elementi come "titolo", "autore", ecc.;
- **Tecnici**: forniscono informazioni sul funzionamento o comportamento della risorsa. Includono elementi come "formato", "compressione", "password", ecc.;
- **Amministrativi**: facilitano la gestione della risorsa. Includono elementi come "identificativo", "licenza", "provenienza", ecc.

<div class="footer">
Australian Research Data Commons (ARDC). (2020). ARDC Metadata Guide. Zenodo. <a href="https://doi.org/10.5281/zenodo.6459832">https://doi.org/10.5281/zenodo.6459832</a>. 
</div>

---

### In cosa dovrebbero consistere dei metadati per essere "buoni" metadati?

I metadati dovrebbero focalizzarsi su:
* Cosa
* Quando
* Dove
* Chi
* Come
* Da quale fonte
* Perché

<div class="footer">
Ram, Sudha & Liu, Jun. (2008). A Semiotics Framework for Analyzing Data Provenance Research. JCSE. 2. 221-248. <a href="http://dx.doi.org/10.5626/JCSE.2008.2.3.221">http://dx.doi.org/10.5626/JCSE.2008.2.3.221</a>. 
</div>

---

### In principio, l'idea è semplice

L'applicazione dei metadati in un caso concreto, però, è complessa: da dove partiamo? Come descriviamo i dati in modo tale da renderli consistenti e gestibili da me e altre persone? Come lo facciamo in una maniera scalabile?

Fortunatamente, esistono gli **schemi di metadati**.

<div class="footer">
Saux, L. (2024). What is metadata and why is it as important as the data itself? Opendatasoft. <a href="https://www.opendatasoft.com/en/blog/what-is-metadata-and-why-is-it-important-data/">https://www.opendatasoft.com/en/blog/what-is-metadata-and-why-is-it-important-data/</a>. 
</div>

---

### I metadati seguono degli schemi

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0317.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://project-thor.readme.io/docs/datacite-metadata-schema">https://project-thor.readme.io/docs/datacite-metadata-schema</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Strutture concettuali che specificano quali metadati utilizzare e secondo quali regole.
    </p>
    <p>
      Stabiliscono un significato unico e non ambiguo per i metadati, costituendo una sorta di lingua semplificata comune per caratterizzare i dati.
    </p>
  </div>
</div>

<div class="footer">
Australian Research Data Commons (ARDC). (2020). ARDC Metadata Guide. Zenodo. <a href="https://doi.org/10.5281/zenodo.6459832">https://doi.org/10.5281/zenodo.6459832</a>. 
</div>

---

### Esempio: decidiamo di descrivere un libro

Per farlo, usiamo una serie di metadati come:

* Titolo
* Autore
* Data di pubblicazione
* Genere
* ...

I termini, molto comuni, li abbiamo decisi noi.

Volendo, li possiamo ri-utilizzare per descrivere anche altri libri.

Abbiamo creato uno schema di metadati per i libri.

---

### Se formalmente validati e riconosciuti, diventano standard

* [MARC](https://www.loc.gov/marc/bibliographic/) (standard per la rappresentazione di informazioni bibliografiche);
* [Dublin Core](https://www.dublincore.org/) (standard per la rappresentazione di risorse sul Web);
* [CIDOC-CRM](https://cidoc-crm.org/) (standard per la documentazione di beni culturali).

---

### Esempio: Dublin Core

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0318.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://project-thor.readme.io/docs/datacite-metadata-schema">https://project-thor.readme.io/docs/datacite-metadata-schema</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Schema di metadati per descrivere risorse pubblicate sul Web.
    </p>
    <p>
      Include quindici elementi (poi estesi ulteriormente) ritenuti fondamentali.
    </p>
  </div>
</div>

---

### Altri standard rilevanti

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0319.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://metadataetc.org/metadatabasics/standards.htm">https://metadataetc.org/metadatabasics/standards.htm</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <ul>
    <li>
      <strong>Standard per i contenuti dei dati</strong>: definiscono come rappresentare uno specifico tipo di dati a partire dal formato (es. <a href="https://www.ionos.it/digitalguide/siti-web/programmazione-del-sito-web/iso-8601/">ISO 8601</a> per le date, o <a href="https://it.wikipedia.org/wiki/ISO_639-1">ISO 639-1</a> per le lingue);
    </li>
    <li>
      <strong>Standard per i valori dei dati</strong>: definiscono come rappresentare uno specifico tipo di dati a partire da un insieme finito e controllato di opzioni (es. <a href="https://en.wikipedia.org/wiki/Art_%26_Architecture_Thesaurus">AAT</a>);
    </li>
    </ul>
  </div>
</div>

---

### L'elemento umano

---

### Il rapimento a Chibok

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0321.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://fivethirtyeight.com/features/nigeria-kidnapping/">https://fivethirtyeight.com/features/nigeria-kidnapping/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <ul>
    <li>
      Aprile 2014: 76 ragazze vengono rapite da una scuola a Chibok, nell'est della Nigeria, dal gruppo terroristico Boko Haram.
    </li>
    <li>
      Poco dopo, FiveThirtyEight esamina la situazione in un articolo.
    </li>
    </ul>
  </div>
</div>

<div class="footer">
Pitfalls in metadata: 3 stories. <a href="https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
">https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
</a>. 
</div>

---

### Rapimenti o _notizie_ sui rapimenti?

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0322.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://fivethirtyeight.com/features/nigeria-kidnapping/">https://fivethirtyeight.com/features/nigeria-kidnapping/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <ul>
    <li>
      L'articolo ha subito critiche per la fonte utilizzata per i dati nel grafico e per l'analisi nel contenuto.
    </li>
    <li>
      I numeri provengono dal Global Database of Events, Language and Tone (GDELT), un database che raccoglie dati su eventi e località da migliaia di fonti di notizie, tra cui televisione, stampa e online.
    </li>
    <li>
      Invece di mostrare i "rapimenti giornalieri in Nigeria", il grafico mostra i "rapporti giornalieri di notizie sui rapimenti in Nigeria".
    </li>
    </ul>
  </div>
</div>

<div class="footer">
Pitfalls in metadata: 3 stories. <a href="https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
">https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
</a>. 
</div>

---

### Due metriche diverse

Una tendenza in aumento potrebbe essere dovuta a un numero maggiore di rapimenti, ma anche a un numero maggiore di notizie in generale o a una maggiore attenzione dei media verso il fenomeno.

Il problema maggiore è l'assunzione che un singolo evento o luogo nel database corrisponda a un singolo rapimento. 

È molto probabile che più rapporti di notizie nel database facciano riferimento allo stesso evento.

<div class="footer">
Pitfalls in metadata: 3 stories. <a href="https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
">https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
</a>. 
</div>

---

### Di nuovo, un'interpretazione sbagliata

Di conseguenza, l'articolo è stato aggiornato, precisando: "Questo post dovrebbe fare riferimento ai rapporti dei media sui rapimenti, non ai rapimenti stessi".

Il giornalista di FiveThirtyEight ha preso i dati nel database GDELT per ciò che erano, senza considerare come i dati vengano raccolti e cosa rappresenta ogni record nel database. 

Questa è un'informazione cruciale sui dati (= metadati) per interpretare correttamente le informazioni.

<div class="footer">
Pitfalls in metadata: 3 stories. <a href="https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
">https://data.europa.eu/apps/data-visualisation-guide/pitfalls-in-metadata-3-stories
</a>. 
</div>

---

<!--
https://www.cambridge.org/core/books/privacy-and-power/metadeath/A0943FA90B2F321B10F83EB2629D4AFB
-->

# Fine

## Lezione 03 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)