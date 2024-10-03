---
title: Data Cleaning nelle Scienze Umane
summary: Introduzione alla pulizia dei dati con OpenRefine
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2024-07-01T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light
---

# Data Cleaning nelle Scienze Umane

#### Laboratorio introduttivo alla pulizia dei dati con OpenRefine

Sebastian Barzaghi | 
[sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | 
[https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527)

---

{{< slide background-image="img/section-01.jpg" class="section-slide">}}

## Partiamo dai dati

Immagine: Redon, O. (1905–1916). *The Chariot of Apollo* [Oil on canvas, 26 x 32 in. (66 x 81.3 cm)]. Anonymous Gift, 1927. Accession No. 27.29.


---

## Cosa sono i dati nelle scienze umane?

Un dato è qualsiasi valore assegnato a qualcosa che può essere quantificato, qualificato o interpretato in qualche modo per essere utilizzato come prova informativa.

Numeri, parole, immagini, video, foto, registrazioni audio, interviste, manoscritti, appunti, collezioni...

<div class="footer">
  Gualandi, B., Pareschi, L., & Peroni, S. (2023). What do we mean by “data”? A proposed classification of data types in the arts and humanities. Journal of Documentation, 79(7), 51-71. <a href="https://doi.org/10.1108/JD-07-2022-0146">https://doi.org/10.1108/JD-07-2022-0146</a>.
</div>

---

## Per essere utili, i dati devono essere organizzati...

... per essere compresi da te in futuro.

... per essere leggibili dalle macchine (_Interoperable_ secondo [FAIR](https://sba.unibo.it/it/almadl/open-access-e-open-science/dati-della-ricerca-aperti)).

... per essere compresi dagli altri (_Reusable_ secondo [FAIR](https://sba.unibo.it/it/almadl/open-access-e-open-science/dati-della-ricerca-aperti)).

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Tutti i dati sono disordinati

Non dare mai la qualità dei tuoi dati per scontato.

L'80% dell'analisi dei dati è dedicato al processo di pulizia dei dati e alla loro preparazione per ulteriori manipolazioni e analisi.

La pulizia e la preparazione devono essere iterative.

La pulizia e la preparazione sono necessarie per lavorare con i dataset.

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Un dataset è una raccolta di dati

Ogni **valore** appartiene a una **variabile** e a un'**osservazione**.

Ogni **variabile** forma una **colonna**.

Ogni **osservazione** forma una **riga**.

<div class="footer">
  S. Ciston, “A CRITICAL FIELD GUIDE FOR WORKING WITH MACHINE LEARNING DATASETS”, K. Crawford and M. Ananny, Eds., Knowing Machines project, Feb. 2023. <a href="https://knowingmachines.org/critical-field-guide">https://knowingmachines.org/critical-field-guide</a>.
</div>

---

{{< slide background-image="img/section-01.jpg" class="section-slide">}}

## Mythologiae

---

## Un dataset di fonti iconografiche mitologiche (1/3)

Link: https://mythologiae.unibo.it/

Obiettivo: raccogliere un insieme di fonti iconografiche, classificarle, localizzarle rispetto agli istituti fisici di conservazione e creare
un collegamento fra rappresentazione iconografica e fonti testuali di riferimento.

La collezione è il frutto di attività laboratoriali, in cui gli studenti sono stati chiamati a scegliere e interpretare opere d’arte eterogenee, provenienti da diverse realtà di conservazione.

---

## Un dataset di fonti iconografiche mitologiche (2/3)

Il filo conduttore che lega fra di loro le opere della collezione è la scena mitologica che esse raffigurano. 

Gli annotatori, dunque, non solo hanno compiuto un’analisi ermeneutica di ciascuna opera, assegnando una categoria concettuale (tema ricorrente) concordata sulla base di una tassonomia interna, ma hanno anche associato al tema, dove possibile, le opere letterarie da cui il tema ha tratto origine o quelle opere che lo hanno, in una qualche forma, ripreso.

---

## Un dataset di fonti iconografiche mitologiche (3/3)

Ogni opera è descritta da una serie di metadati, per lo più con valori testuali, come _titolo_, _autore_, _periodo_, _collocazione_, e _note_.

Questo rende i dati contenuti in Mythologiae estremamente ricchi da una parte, ed estremamente poco strutturati dall'altra.

Inoltre, essendo stato compilato manualmente da diverse persone, alcuni dati contenuti nel dataset tendono ad essere disomogenei in termini di formato, separatori, ecc.

---

{{< slide background-image="img/section-01.jpg" class="section-slide">}}

## Errori comuni

---

## La pulizia dei dati è difficile (ma ne vale la pena)!

Può essere riassunta in una serie di attività:
* Preparare i dati;
* Eliminare inutili ridondanze;
* Separare o combinare i valori;
* Gestire errori e incoerenze (esempio: duplicati, valori nulli, errori di ortografia o formattazione incoerenti, ecc.);
* Standardizzare quando possibile.

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>
</div>

---

## Non modificare mai i dati originali

Fai sempre una copia prima di apportare modifiche.

Esegui il backup dei file.

Tieni traccia di tutti i passaggi.

Salva i tuoi file nella codifica `UTF-8`.

<div class="footer">
  Seth van Hooland, Ruben Verborgh, and Max De Wilde, "Cleaning Data with OpenRefine," Programming Historian 2 (2013), <a href="https://doi.org/10.46430/phen0023">https://doi.org/10.46430/phen0023</a>.
</div>

---

## Descrivi sempre i dati

Documenta tutto il necessario per capire cosa c'è nel dataset e come utilizzarlo

Considera di indicare almeno:
* Il "chi", "cosa", "quando", "dove" e "come" dei dati;
* Modalità di reperimento e accesso ai dati;
* Suggerimenti sull'idoneità dei dati per rispondere a domande specifiche;
* Avvertenze sui problemi o le incoerenze note nei dati;
* Informazioni per verificare che i dati siano importati correttamente.

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Usa formati standard per le tabelle (1/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/tidy-1.png" alt="https://r4ds.had.co.nz/tidy-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Una colonna per ogni variabile.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Usa formati standard per le tabelle (2/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/tidy-2.png" alt="https://r4ds.had.co.nz/tidy-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Una riga per ogni osservazione.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Usa formati standard per le tabelle (3/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/tidy-3.png" alt="https://r4ds.had.co.nz/tidy-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Una cella per ogni valore.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Evita di aggregare commenti e altre informazioni con i dati (1/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/multiple-info.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Inserimento di più di un tipo di informazione in una cella (esempi: commenti, unità di misura, metadati, ecc.).</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Evita di aggregare commenti e altre informazioni con i dati (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/single-info.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Aggiungi le informazioni aggiuntive al titolo della colonna o in una colonna separata.</p>
        <p>Aggiungi i metadati in un documento separato.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Non utilizzare la formattazione per trasmettere informazioni (1/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/formatting.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Esempi: evidenziare celle, righe o colonne che dovrebbero essere escluse da un'analisi; lasciare righe vuote per indicare separazioni nei dati, ecc.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Non utilizzare la formattazione per trasmettere informazioni (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/good-formatting.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/02-common-mistakes.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Aggiungi le unità al titolo della colonna o in una colonna separata.</p>
        <p>Aggiungi le informazioni in una colonna separata.</p>
        <p>Aggiungi i metadati in un documento separato.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Non utilizzare più tabelle o più schede

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/multiple-tables.jpg" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Esempio: più di una tabella o scheda all'interno di un singolo foglio di calcolo.</p>
        <p>Se possibile, combina tutto in una tabella unica o mantieni ogni tabella in un file separato.</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Non utilizzare caratteri speciali

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/special-characters.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
        <p>Se possibile, evita <a href="https://www.edatlas.it/scarica/1836/Capitolo5/ContenutiDigitali/2EntitaCarattere.pdf">caratteri speciali</a> nei titoli delle colonne e nel testo: <code>/</code> <code>\</code> <code>:</code> <code>*</code> <code>.</code> <code>?</code> <code>‘</code> <code><</code> <code>></code> <code>[</code> <code>]</code> <code>(</code> <code>)</code> <code>&</code> <code>$</code> <code>æ</code> <code>Æ</code> ...</p>
        <p>Evita sempre di utilizzare spazi nei titoli delle colonne: invece, utilizza underscore (<code>_</code>) o CamelCase (esempio: <code>TitoloPrincipale</code>).</p>
    </div>
</div>

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Sii coerente

* Scenario 1: date visualizzate in molti formati diversi (esempi: "12 luglio 2024", "12/07/2024", "12-07-2024", ecc.);
  * Utilizza **standard internazionali** (esempi: [EDTF](https://www.loc.gov/standards/datetime/));
* Scenario 2: nomi visualizzati in molte varianti diverse (esempi: "Alessandro Manzoni", "A. Manzoni", "Manzoni", "Manzoni, Alessandro", ecc.);
  * Utilizza **record di autorità** (esempi: [VIAF](https://viaf.org/));
* Sii coerente anche nella **capitalizzazione** delle parole, nella scelta dei **delimitatori** e nelle convenzioni di **denominazione** per le variabili;
* Evita di utilizzare il delimitatore usato dal dataset (esempi: `,`, `;`, `/`, ecc.) nei dati stessi;
* Fai attenzione agli **spazi**!

<div class="footer">
  UiT The Arctic University of Norway. (2023). Data Cleaning. Zenodo. <a href="https://doi.org/10.5281/zenodo.8375643">https://doi.org/10.5281/zenodo.8375643</a>.
</div>

---

## Elimina la ridondanza (con cautela!)

Nell'eliminazione includi:
* Duplicati;
* Osservazioni irrilevanti;
* Dati incompleti;
* Dati non validi;
* Dati in conflitto.

Sono tutte **interpretazioni**: considera sempre se un'osservazione o una colonna debbano essere eliminate o meno!

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Tratta sempre i valori NULL

Usa un metodo coerente che sia compatibile e che non causi errori (come lasciare la cella vuota).

Considera che:
* Può essere difficile sapere se un valore è mancante o è stato trascurato durante l'inserimento dei dati;
* Gli spazi vuoti possono essere confusi quando spazi (`  `) o tabs (`/`) sono usati come delimitatori;
* `NA` e `NULL` sono valori nulli ragionevoli.

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Esegui sempre un controllo di qualità

Verifica:
* Errori grammaticali;
* Uso incoerente di maiuscole e minuscole;
* Titoli incoerenti per le colonne;
* Unità di misura incoerenti, tipi di dati incoerenti (esempio: numero, stringa), schemi di denominazione, ecc.;
* Valori fuori intervallo.

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

## Quando hai finito, esporta e condividi

Utilizza una licenza aperta per far sapere agli altri esattamente cosa possono e non possono fare con i dati (esempio: [Creative Commons Zero (CC0)](https://creativecommons.org/publicdomain/zero/1.0/)).

Utilizza formati aperti per rendere i dati interoperabili (esempio: [CSV](https://en.wikipedia.org/wiki/Comma-separated_values)), quando possibile.

Considera di condividere i tuoi dati su [GitHub](https://github.com/) e/o di pubblicarli su un repository (esempio: [Zenodo](https://zenodo.org/), [Figshare](https://figshare.com/), ecc.) per renderli visibili, accessibili e stabili.

<div class="footer">
  White, E. P., Baldridge, E., Brym, Z. T., Locey, K. J., McGlinn, D. J., & Supp, S. R. (2013). Nine simple ways to make it easier to (re)use your data (e7v2). PeerJ Inc. <a href="https://doi.org/10.7287/peerj.preprints.7v2">https://doi.org/10.7287/peerj.preprints.7v2</a>.
</div>

---

{{< slide background-image="img/section-01.jpg" class="section-slide">}}

## OpenRefine

---

## Uno strumento per la pulizia dei dati

OpenRefine permette di:
* Identificare e correggere errori;
* Combinare dati da diverse fonti;
* Non modifica il file originale;
* Tutte le azioni sono reversibili e tracciate;
* La documentazione può essere pubblicata insieme ai dati;
* Il flusso di lavoro può essere salvato e applicato a nuovi dataset.

<div class="footer">
  Baker, J., Moore, C., Priego, E., Alegre, R., Cope, J., Price, L., ... & Wilson, G. (2016). Library Carpentry: software skills training for library professionals. Liber Quarterly: The Journal of European Research Libraries, 26(3), 141-162. <a href="http://dx.doi.org/10.18352/lq.10176">http://dx.doi.org/10.18352/lq.10176</a>.
</div>

---

## Alcuni scenari di utilizzo

* Vuoi sapere quante volte un particolare valore appare in una colonna nei tuoi dati;
* Vuoi sapere come i valori sono distribuiti in tutto il dataset;
* Vuoi normalizzare date formattate in modi diversi ad un unico formato comune;
* Vuoi normalizzare nomi o termini che, pur riferendosi alle stesse entità, differiscono tra loro;
* Vuoi separare frammenti di dati combinati insieme in dati individuali;
* Vuoi allineare i dati a una fonte esterna.

<div class="footer">
  Baker, J., Moore, C., Priego, E., Alegre, R., Cope, J., Price, L., ... & Wilson, G. (2016). Library Carpentry: software skills training for library professionals. Liber Quarterly: The Journal of European Research Libraries, 26(3), 141-162. <a href="http://dx.doi.org/10.18352/lq.10176">http://dx.doi.org/10.18352/lq.10176</a>.
</div>

---

## Installazione di OpenRefine

* Scarica OpenRefine: [https://openrefine.org/download.html](https://openrefine.org/download.html);
  * Dovrebbe già includere Java Runtime Environment;
  * Se non funziona, scarica e installa anche Java Runtime Environment: [https://www.java.com/it/](https://www.java.com/it/);
* Decomprimi il file scaricato;
* Fai doppio clic su `openrefine.exe` (su Windows), `openrefine.dmg` (su OS) o `refine.bat`;
* Accedi all'interfaccia su un browser web all'indirizzo [http://127.0.0.1:3333](http://127.0.0.1:3333).

---

## Creazione di un progetto (1/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-1.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Scarica il dataset Mythologiae (link in chat);</li>
        <li>In <em>Create Project</em> > <em>This computer</em>, clicca su <em>Choose files</em> e carica <code>mythologiae-dataset.csv</code>;</li>
        <li>Clicca su <em>Next</em>.</li>
      </ul>
    </div>
</div>

---

## Creazione di un progetto (2/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-2a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>In <em>Parse data as</em> > <em>CSV / TSV / separator-based files</em>;</li>
        <li><em>Character encoding</em> deve avere <code>UTF-8</code> come valore;</li>
        <li>Seleziona <em>Columns are separated by</em> > <em>commas (CSV)</em>;</li>
        <li>Spunta <em>Use character <code>"</code> to enclose cells containing column separators</em>;</li>
        <li>Spunta <em>Trim leading & trailing whitespace from strings</em>.</li>
      </ul>
    </div>
</div>

---

## Creazione di un progetto (3/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-2b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Seleziona <em>Parse next <code>1</code> line(s) as column headers</em>;</li>
        <li>Spunta <em>Store blank rows</em>;</li>
        <li>Spunta <em>Store blank cells as nulls</em>;</li>
        <li>Clicca su <em>Create project</em>.</li>
      </ul>
    </div>
</div>

---

## Schermata del progetto (1/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-3a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><code>Permalink</code> ti consente di tornare ad uno stato di visualizzazione specifico del progetto, con filtri e faccette applicati, inserendo informazioni specifiche della visualizzazione direttamente nell'URL.</li>
      </ul>
    </div>
</div>

---

## Schermata del progetto (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-3b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><code>Open</code> apre una nuova scheda del browser mostrando la schermata di creazione del progetto per modificare le impostazioni, avviare un nuovo progetto o aprire un progetto esistente;</li>
        <li><code>Export</code> ti consente di selezionare un formato per esportare il dataset;</li>
        <li><code>Help</code> apre una nuova scheda del browser contenente un manuale utente.</li>
      </ul>
    </div>
</div>

---

## Schermata della griglia

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-4.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Visualizzazione dei dati in formato tabellare;</li>
        <li>Numero totale di righe;</li>
        <li>Modalità rows vs modalità records;</li>
        <li>Numero di righe/record visibili su schermo contemporaneamente.</li>
      </ul>
    </div>
</div>

---

## Facet/Filter

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-5.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <p>Modi principali per esplorare i dati, mostrando pattern, tendenze e sottogruppi;</p>
      <ul>
        <li><code>Refresh</code> aggiorna ciascuna facet con le informazioni più recenti;</li>
        <li><code>Reset all</code> resetta tutte le faccette senza rimuoverle;</li>
        <li><code>Remove all</code> rimuove tutte le faccette.</li>
      </ul>
    </div>
</div>

---

## Undo/Redo

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-6.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Storico del progetto come elenco di modifiche in ordine cronologico;</li>
        <li>Salvataggio automatico ogni 5 minuti e alla chiusura con <code>CTRL + C</code>;</li>
        <li>Ogni attività che modifica i dati può essere annullata;</li>
        <li>La cronologia delle modifiche di ciascun progetto è salvata insieme al progetto stesso.</li>
      </ul>
    </div>
</div>

---

## Modalità rows

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-7a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><strong>Row</strong>: una serie di celle, una cella per colonna;</li>
        <li>A volte, ci sono più informazioni in una singola cella (esempio: <code>dcho_keyword</code>);</li>
        <li>In questi casi, se riesci a dividere correttamente questi valori, puoi utilizzare la modalità <strong>records</strong> di OpenRefine per visualizzarli correttamente.</li>
      </ul>
    </div>
</div>

---

## Modalità records

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-7b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li><strong>Record</strong>: una collezione di una o più righe;</li>
        <li>Le molteplici informazioni in una singola cella (esempio: <code>dcho_keyword</code>), una volta divise, vengono visualizzate ognuna in una riga diversa, ma appartengono allo stesso record;</li>
        <li>Funziona dopo aver eseguito uno <emph>split</emph>, un'operazione che vedremo tra poco.</li>
      </ul>
    </div>
</div>

---

## Esplora i dati con le Facet (1/2)

**Facet**: un aspetto della varianza dei dati in una colonna.

Fornisce una visione d'insieme dei dati.

Consente ulteriori operazioni, come il filtraggio e il clustering.

---

## Esplora i dati con le Facet (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Tipicamente, crei una facet su una particolare colonna;</li>
        <li>Fai clic sul <em>triangolo</em> davanti al nome della colonna (esempio: <code>dcho_theme</code>);</li>
        <li>Seleziona <em>Facet</em>;</li>
        <li>Seleziona una facet a tua scelta (esempio: <em>Text facet</em>).</li>
      </ul>
    </div>
</div>

---

## Text facet (1/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Prende il contenuto totale delle celle della colonna in questione e le abbina;</li>
        <li>Ordina per nome o conteggio;</li>
        <li>Modifica in massa ogni cella identica nella colonna;</li>
        <li>Ottimo per esaminare i dati e correggere errori di battitura, spazi in eccesso, ecc.</li>
      </ul>
    </div>
</div>

---

## Text facet (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8c.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Molteplici facet sono impilate una sopra l'altra (esempio: nell'immagine viene aggiunta <code>cho_author</code>).</li>
      </ul>
    </div>
</div>

---

## Filter (1/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8d.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>I filtri possono essere aggiunti su una colonna;</li>
        <li>Utili per identificare più precisamente dei dati;</li>
        <li>Clicca sulla freccia e seleziona <em>Text filter</em>.</li>
      </ul>
    </div>
</div>

---

## Filter (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8e.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>I filtri condividono lo stesso spazio con le facet;</li>
        <li>Digita il testo da cercare (esempio: "edipo") per restituire le righe con quel testo contenuto in quella colonna;</li>
        <li>Sensibilità alle maiuscole e minuscole disattivata di default.</li>
      </ul>
    </div>
</div>

---

## Filtrare con i Facet (1/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8f.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>È possibile filtrare anche tramite facet;</li>
        <li>Clicca su qualsiasi voce in un filtro (esempio: "Allston, Washington" nella facet <code>cho_author</code>);</li>
        <li>Vengono visualizzate solo le righe con quel valore in quella colonna.</li>
      </ul>
    </div>
</div>

---

## Filtrare con i Facet (2/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8g.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Puoi usare più facet per migliorare il filtraggio.</li>
      </ul>
    </div>
</div>

---

## Filtrare con i Facet (3/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8h.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Puoi usare facet personalizzati per ottenere determinati effetti (esempio: filtrare le righe con celle vuote).</li>
      </ul>
    </div>
</div>

---

## Sort (1/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8i.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Puoi determinare l'ordine in cui vengono mostrate le righe in base ad alcune condizioni.</li>
        <li>Clicca sulla freccia e seleziona <em>Sort</em>.</li>
      </ul>
    </div>
</div>

---

## Sort (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8l.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Seleziona come trattare i valori delle celle durante l'ordinamento (esempio: se sono date, molto probabilmente vorrai selezionare <em>date</em>);</li>
        <li>Puoi anche selezionare l'ordine effettivo (esempio: prima tutti i valori validi, poi quelli errati, poi quelli mancanti);</li>
        <li>Clicca su <em>OK</em>.</li>
      </ul>
    </div>
</div>

---

## Cluster (1/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8m.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Un ottimo modo per correggere le incongruenze trovate con le facet;</li>
        <li>Utilizza una varietà di metodi di confronto per trovare diciture simili ma non identiche, e mostrarle in modo da rendere possibile l'allineamento dei valori che dovrebbero essere uguali;</li>
        <li>Crea una facet;</li>
        <li>Clicca su <em>Cluster</em>.</li>
      </ul>
    </div>
</div>

---

## Cluster (2/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8n.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Clicca su <em>Cluster</em>;</li>
        <li>Prova diversi algoritmi per rilevare vari cluster;</li>
        <li>Per ogni cluster, puoi unire i valori sostituendoli con un valore unico e coerente;</li>
        <li>Per impostazione predefinita, il valore più comune nel cluster viene utilizzato come nuovo valore, ma puoi cambiarlo.</li>
      </ul>
    </div>
</div> 

---

## Cluster (3/3)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-8o.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Prova diversi algoritmi per rilevare vari cluster;</li>
        <li>Per ogni cluster, puoi unire i valori spuntando <em>Merge?</em>;</li>
        <li>Clicca su <em>Merge selected & re-cluster</em> per verificare e su <em>Merge selected & Close</em> per terminare.</li>
      </ul>
    </div>
</div>

---

## Modifica delle celle

OpenRefine offre numerose funzionalità per modificare e migliorare il contenuto delle celle in modo automatico ed efficiente.

* Modifica tramite una facet di testo: clicca su _Edit_ a destra della facet e inserisci un nuovo valore;
* Utilizzo della funzione trova/sostituisci: seleziona _Edit cells_ > _Replace_ per inserire una stringa da cercare e una stringa da sostituire;
* Modifica delle singole celle: passa il mouse su una cella e clicca su _Edit_.

---

## Split (1/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-9a.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>A volte una cella può contenere più valori (esempio: colonna <code>dcho_keyword</code>, con più valori separati da virgole <code>,</code>);</li>
        <li>Fondamentale per la modalità <emph>records</emph>;</li>
        <li>Fai clic sulla freccia e seleziona <em>Edit cells</em>;</li>
        <li>Seleziona <em>Split multi-valued cells</em>.</li>
      </ul>
    </div>
</div>

---

## Split (2/2)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-9b.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Puoi decidere come dividere le celle;</li>
        <li>Idealmente, dovresti sempre usare nel testo un separatore (esempio: <code>,</code>, <code>|</code>, <code>;</code>, ecc.), e indicarlo qui;</li>
        <li>Clicca su <em>OK</em>.</li>
      </ul>
    </div>
</div>

---

## Transform

Un meccanismo potente per applicare modifiche che non possono essere ottenute tramite semplici facet, filtri o cluster.

* Eliminare spazi bianchi iniziali e finali;
* Dividere i dati in più colonne;
* Rimuovere la punteggiatura;
* Standardizzare un formato di dati;
* Estrarre un particolare tipo di dati da una stringa di testo.

Possono essere preimpostate o scritte ad hoc in un linguaggio chiamato GREL.

---

## Reconcile (1/5)

Processo semi-automatico di allineamento dei dati a fonti esterne.

Utile per:
* Correggere errori di ortografia o variazioni nei nomi propri;
* Pulire i valori inseriti manualmente confrontandoli con file di autorità;
* Collegare i tuoi dati a un dataset esistente.

È necessario il giudizio umano per rivedere e approvare i risultati.

Avviene di default tramite ricerca di stringhe, quindi pulisci e raggruppa i dati prima di riconciliarli!

---

## Reconcile (2/5)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-9c.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Clicca sulla freccia e seleziona <em>Reconcile</em>;</li>
        <li>Seleziona <em>Start reconciling</em>.</li>
      </ul>
    </div>
</div>

---

## Reconcile (3/5)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-9d.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Seleziona il servizio di riconciliazione (esempio: <code>VIAF</code>);</li>
        <li>Clicca su <em>Next</em>.</li>
      </ul>
    </div>
</div>

---

## Reconcile (4/5)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-9e.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>A seconda della colonna e del servizio di riconciliazione selezionato, scegli il tipo di entità che desideri riconciliare (esempio: <code>Person</code>);</li>
        <li>Clicca su <em>Start reconciling</em>.</li>
      </ul>
    </div>
</div>

---

## Reconcile (5/5)

<div style="display: flex; align-items: center;">
    <div style="flex: 1;">
        <img src="img/openrefine-9f.png" alt="https://datacarpentry.org/spreadsheet-ecology-lesson/01-format-data.html" style="max-width: 100%;">
    </div>
    <div style="flex: 1; padding-left: 20px;">
      <ul>
        <li>Alcuni valori delle celle vengono riconciliati direttamente (esempio: <em>Houdon, Jean Antoine</em>);</li>
        <li>Altri richiedono una validazione manuale (esempio: <em>Gérard, Francois Baron</em>);</li>
        <li>Cliccare sul <em>segno di spunta singolo</em> per riconciliare solo quella cella, o sul <em>segno di spunta doppio</em> per estenderlo a tutte le celle identiche.</li>
      </ul>
    </div>
</div>

---

{{< slide background-image="img/section-01.jpg" class="section-slide">}}

## Cosa fare

---

## Cosa fare

Abbiamo individuato quattro colonne problematiche che richiedono particolare attenzione in termini di qualità e pulizia dei dati.

* `dcho_theme`: il tema mitologico individuato nell'opera;
* `cho_century`: il secolo a cui risale l'opera;
* `cho_date`: la data di creazione dell'opera;
* `cho_sources_classic`: le fonti classiche associate al tema mitologico individuato nell'opera.

---

## dcho_theme (1/2)

* Impostare un separatore comune (`|`);
* Dividere i valori (_split_);
* Raggruppare i valori (_cluster_);
* Mantenere solo l'ultimo valore a destra se c'è una gerarchia, solitamente indicata da una sequenza di termini separati da `>`. Esempio: "Gli dèi>Efeso" &rarr; `Efeso`;
* Normalizzare i valori NULL (esempio: "Non categoria" &rarr; `NULL`).

---

## dcho_theme (2/2)

* Standardizzare quando possibile (vedi [Iconclass](https://iconclass.org/)):
  * Iscriviti e accedi a Iconclass;
  * Cerca il tema;
  * Scegli l'opzione più appropriata;
  * Sostituisci il tema esistente nel dataset con l'ID dell'opzione trovata:
    * Esempio: "L'Enigma della Sfinge" &rarr; `94T33`;
    * Esempio: "Eracle cattura il cinghiale di Erimanto" &rarr; `94L324`.

---

## cho_century

* Modificare (esempio: eliminare le virgole);
* Normalizzare i valori NULL (esempio: cella vuota &rarr; `NULL`).
* Standardizzare (vedi [EDTF](https://www.loc.gov/standards/datetime/)):
  * Rappresentazione delle date CE: `[year][“-”][month][“-”][day]`;
    * Esempio: "20 giugno 1992" &rarr; `1992-06-20`;
  * Rappresentazione delle date BCE: `["-"][year][“-”][month][“-”][day]`;
    * Esempio: "1800 a.C." &rarr; `-1800`;
  * Rappresentazione dei periodi: `[beginning]["/"][end]`;
    * Esempio: "II secolo" &rarr; `0100-01-01/0199-12-31`;
    * Esempio: "II secolo a.C." &rarr; `-0199-01-01/-0100-12-31`.

---

## cho_date (1/2)

* Impostare un separatore comune (`|`);
* Modificare (esempio: rimuovi "ca.", "circa", ecc.);
* Normalizzare i valori NULL (esempio: cella vuota &rarr; `NULL`).
* Standardizzare (vedi [EDTF](https://www.loc.gov/standards/datetime/)):
  * Rappresentazione delle date CE: `[year][“-”][month][“-”][day]`;
    * Esempio: "1992" &rarr; `1992`;
  * Rappresentazione delle date BCE: `["-"][year][“-”][month][“-”][day]`;
    * Esempio: "460 a.C." &rarr; `-0460`
  
---

## cho_date (2/2)

* Standardizzare (vedi [EDTF](https://www.loc.gov/standards/datetime/)):
  * Rappresentazione dei periodi CE: `[beginning]["/"][end]`;
    * Esempio: "1705-1706" &rarr; `1705/1706`
  * Rappresentazione dei periodi BCE: `["-"][beginning]["/"]["-"][end]`;
    * Esempio: "550-530 a.C." &rarr; `-0550/-0530`
  * Rappresentazione dell'incertezza: `[date]["%"]`;
    * Esempio: "1590 circa" &rarr; `1590%`.

---

## cho_sources_classic

* Impostare un separatore comune (`|`);
* Normalizzare i valori NULL (esempio: "Non categoria" &rarr; `NULL`).
* Modificare (esempio: rimuovere le citazioni che non sono in forma canonica):
  * Le citazioni non canoniche devono essere salvate così come sono in una colonna separata `cho_sources_other`;
* Standardizzare (vedi [Perseus](https://www.perseus.tufts.edu/hopper/)):
  * Cerca la citazione su Perseus;
  * Scegli l'opzione più appropriata;
  * Sostituisci la citazione esistente nel dataset con l'opzione trovata:
    * Esempio: "Apollodoro, Biblioteca, II 5" &rarr; `Apollod. 2.5`;
    * Esempio: "Omero, Odissea, XI vv.601-604" &rarr; `Hom. Od. 11.601`.

---

## Altre colonne

* Tutte: normalizzare i valori NULL, correggere i refusi, sostituire i separatori con `|`;
* `dcho_keyword`: dividere, raggruppare, modificare (mantenere solo italiano);
* `cho_author`: raggruppare, modificare, riconciliare con VIAF ("Person");
* `cho_period`: raggruppare, modificare;
* `cho_type`: raggruppare, modificare;
* `cho_location`: raggruppare, modificare, riconciliare con VIAF ("Organization").

---

## Conclusioni

Potete già fare molto per aumentare la qualità dei dati! Riassumendo:

* Esplorate i dati utilizzando _facet_, filtri e _sorting_;
* Trasformate i dati tramite modifiche singole e di massa, raggruppamenti (_cluster_), divisioni (_split_) e sostituzioni;
* Riconciliate i dati con fonti esterne, quando possibile, automaticamente o manualmente.

Provate! Ricordate che potete sempre tornare indietro.

---

# Data Cleaning nelle Scienze Umane

#### Fine

Sebastian Barzaghi | 
[sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | 
[https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527)
