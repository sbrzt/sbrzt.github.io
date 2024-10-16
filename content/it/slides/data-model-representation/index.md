---
title: Dati e modelli per il patrimonio culturale e la loro rappresentazione
summary: I casi del Rinascimento digitale di Ulisse Aldrovandi e del Progetto SIRIUS
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2022-12-31T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light
---

# Dati e modelli per il patrimonio culturale e la loro rappresentazione

## I casi del _Rinascimento digitale di Ulisse Aldrovandi_ e del _Progetto SIRIUS_

###### Sebastian Barzaghi | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/) | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527)

---

### Outline

1. Concetti chiave
  * Dato
  * Modello (di dati)
  * FAIRness
2. Casi di studio
  * Aldrovandi (Spoke 4)
  * SIRIUS (Spoke 6)

---

{{< slide background-image="img/data-intro.jpg" class="section-slide">}}

## Partiamo dai dati

<!--
Photo by <a href="https://unsplash.com/@gregbecker?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Greg Becker</a> on <a href="https://unsplash.com/photos/body-of-water-under-clear-blue-sky-sYzFIusQp3Q?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

<section>
  <h3>Si parte sempre dai dati</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/data.png" height="auto" width="700"/>
          <figcaption>
              Fonte: Noppe, N., Vanvelk, J., & Callens, N. (2023). The hands-on guide to research data management for KU Leuven researchers, students, and research support staff in the humanities and social sciences. Zenodo. <a href="https://doi.org/10.5281/zenodo.8010618">https://doi.org/10.5281/zenodo.8010618</a>.
          </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
        <p>
          I dati sono record fattuali raccolti, generati o riutilizzati come base di analisi, ragionamenti, discussioni o calcoli.
        </p>
        <p>
          Fare ricerca implica lavorare con i dati, tanto come oggetti di studio ed analisi, quanto come prodotti del processo stesso di ricerca.
        </p>
    </div>
  </div>
  <div class="footer">
    OECD (2007), OECD Principles and Guidelines for Access to Research Data from Public Funding, OECD Publishing, Paris. <a href="https://doi.org/10.1787/9789264034020-en-fr">https://doi.org/10.1787/9789264034020-en-fr</a>.
  </div>
</section>

<section>
  <h3>Le sfide dei dati culturali</h3>
  <p>
    I processi della ricerca in ambito culturale sono ancora dominati da paradigmi tradizionali.
  </p>
  <p>
    I dati culturali sono complessi e raramente documentati in modo da facilitarne l'integrazione, la comprensione e il riutilizzo da parte di altri.
  </p>
  <div class="footer">
    Erzsébet Tóth-Czifra (2019). DARIAH Pathfinder to Data Management Best Practices in the Humanities. Version 1.0.0. DARIAH-Campus. [Pathfinder]. <a href="https://campus.dariah.eu/id/yR8mHfs3eW-ibu58LerCt">https://campus.dariah.eu/id/yR8mHfs3eW-ibu58LerCt</a>.
  </div>
</section>

---

{{< slide background-image="img/model-intro.jpg" class="section-slide">}}

## Semplifichiamo

<!--
Photo by <a href="https://unsplash.com/@spaceboy?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Henrik Dønnestad</a> on <a href="https://unsplash.com/photos/abstract-painting-t2Sai-AqIpI?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

<section>
  <h3>I dati sono rappresentati da modelli</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
      <img src="img/model.png" height="auto" width="700"/>
        <figcaption>
            Fonte: Kučerová, H. (2018). The concept of model and conceptual model in information science. <a href="https://knihovnarevue-en.nkp.cz/archives/2018-2/reviewed-articles/the-concept-of-model-and-conceptual-model-in-information-science ">https://knihovnarevue-en.nkp.cz/archives/2018-2/reviewed-articles/the-concept-of-model-and-conceptual-model-in-information-science</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
        <p>
          Astrazioni che descrivono i dati per renderli comprensibili a umani e macchine.
        </p>
    </div>
  </div>
  <div class="footer">
    Flanders, J., & Jannidis, F. (2015). Data modeling. A new companion to digital humanities, 229-237. <a href="https://doi.org/10.1002/9781118680605.ch16">https://doi.org/10.1002/9781118680605.ch16</a>.
  </div>
</section>

<section>
  <h3>Dati e modelli devono parlare</h3>
  <p>
    Un modello deve rappresentare una visione chiara e condivisa del significato dei dati.
  </p>
  <p>
    I dati rappresentati da modelli uguali (o formalmente allineati) parlano la stessa lingua.
  </p>
  <p>
    Questa rappresentazione è fondamentale per l'apertura dei dati.
  </p>
</section>

---

{{< slide background-image="img/open-sesame.jpg" class="section-slide">}}

## Apriti, Scienza

<!--
Photo by <a href="https://unsplash.com/@ilmissile?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Jacopo Tarantini</a> on <a href="https://unsplash.com/photos/bottom-view-of-rocks-GUwwV5l2QNk?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

<section>
  <h3>La scienza fatta bene</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
        <img src="img/fair.png" height="auto" width="700"/>
        <figcaption>
            MBezjak, S., Clyburne-Sherin, A., Conzett, P., Fernandes, P. L., Görögh, E., Helbig, K., ... & Tennant, J. (2018). The Open Science Training Handbook. <a href="https://open-science-training-handbook.gitbook.io/book">https://open-science-training-handbook.gitbook.io/book</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
        <p>
          La Scienza Aperta è un insieme di movimenti e pratiche che ha l'obiettivo di rendere la conoscenza scientifica più trasparente, accessibile e riutilizzabile per tutti.
        </p>
    </div>
  </div>
  <div class="footer">
    Edmond, J., & Tóth-Czifra, E. (2018). Open data for humanists, a pragmatic guide. <a href="https://shs.hal.science/halshs-02115443">https://shs.hal.science/halshs-02115443</a>.
  </div>
</section>

<section>
  <h3>La FAIRificazione</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
        <img src="img/fairification.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.go-fair.org/fair-principles/fairification-process/">https://www.go-fair.org/fair-principles/fairification-process/</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        Processo di trasformazione di dati non-FAIR in una loro versione FAIR.
      </p>
      <p>
        Include la definizione di un modello semantico e la sua applicazione per collegare i dati tra loro.
      </p>
      <p>
        Per fare questo, si utilizzano tecnologie legate al paradigma dei Linked Open Data.
      </p>
    </div>
  </div>
  <div class="footer">
    Jacobsen, A., Kaliyaperumal, R., da Silva Santos, L. O. B., Mons, B., Schultes, E., Roos, M., & Thompson, M. (2020). A generic workflow for the data FAIRification process. Data Intelligence, 2(1-2), 56-65. <a href="https://doi.org/10.1162/dint_a_00028">https://doi.org/10.1162/dint_a_00028</a>.
  </div>
</section>

<section>
  <h3>Dati aperti e contestualizzati</h3>
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
        I Linked Open Data (LOD) sono dati semi-strutturati, pubblicati in formato aperto e descritti tramite modelli semantici. 
      </p>
      <p>
        Sono rappresentati tramite triple soggetto-predicato-oggetto su cui si basa RDF (Resource Description Framework).
      </p>
    </div>
  </div>
  <div class="footer">
    Blaney, J. (2017). Introduction to the Principles of Linked Open Data. The Programming Historian. <a href="https://doi.org/10.46430/phen0068">https://doi.org/10.46430/phen0068</a>.
  </div>
</section>

<section>
  <h3>I nostri due casi di FAIRificazione</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
        <img src="img/samod.png" height="auto" width="700"/>
        <figcaption>
            Fonte: Peroni, S. (2016). SAMOD: an agile methodology for the development of ontologies. figshare. <a href="http://dx.doi.org/10.6084/m9.figshare.3189769">http://dx.doi.org/10.6084/m9.figshare.3189769</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        La digitalizzazione di una mostra temporanea, e la valorizzazione di dati di valutazione dei rischi in ambito culturale.
      </p>
      <p>
        Definizione, sviluppo e implementazione di un modello semantico che "FAIRifica" i dati esistenti.
      </p>
    </div>
  </div>
  <div class="footer">
    Peroni, S. (2016). A Simplified Agile Methodology for Ontology Development. In Proceedings of the 13th OWL: Experiences and Directions Workshop and 5th OWL reasoner evaluation workshop (OWLED-ORE 2016). <a href="https://w3id.org/people/essepuntato/papers/samod-owled2016.html">https://w3id.org/people/essepuntato/papers/samod-owled2016.html</a>.
  </div>
</section>

---

{{< slide background-image="img/aldrovandi.png" class="section-slide">}}

## Caso 1: Il Rinascimento Digitale di Ulisse Aldrovandi

<!--

-->
---

<section>
  <h3>Digitalizzare una mostra temporanea</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
        <img src="img/aldrovandi-intro.png" height="auto" width="700"/>
        <figcaption>
            Fonte: Balzani, R., Barzaghi, S., Bitelli, G., Bonifazi, F., Bordignon, A., Cipriani, L., ... & Vittuari, L. (2024). Saving temporary exhibitions in virtual environments: The Digital Renaissance of Ulisse Aldrovandi–Acquisition and digitisation of cultural heritage objects. Digital Applications in Archaeology and Cultural Heritage, 32, e00309. <a href="https://doi.org/10.1016/j.daach.2023.e00309">https://doi.org/10.1016/j.daach.2023.e00309</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        Progetto pilota per raccogliere linee guida di acquisizione e digitalizzazione del patrimonio culturale, da applicare ai casi core dello Spoke 4.
      </p>
    </div>
  </div>
</section>

<section>
  <h3>I dati: oggetti culturali</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
        <img src="img/aldrovandi-data.png" height="auto" width="700"/>
        <figcaption>
            Fonte: Barzaghi, S., Bordignon, A., Gualandi, B., & Peroni, S. (2024, June 5). Thinking Outside the Black Box: Insights from a Digital Exhibition in the Humanities. MeTe digitali. Mediterraneo in rete tra testi e contesti (AIUCD 2024), Catania, Italy. Zenodo. <a href="https://doi.org/10.5281/zenodo.11487997">https://doi.org/10.5281/zenodo.11487997</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
        <p>
          Descrizione strutturata per ogni oggetto, definita da una serie di metadati bibliografici estratti dal catalogo del museo.
        </p>
    </div>
  </div>
</section>

<section>
  <h3>I dati: processo di digitalizzazione</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
        <img src="img/aldrovandi-process.png" height="auto" width="700"/>
        <figcaption>
            Fonte: Barzaghi, S., Bordignon, A., Gualandi, B., Heibi, I., Massari, A., Moretti, A., ... & Renda, G. (2024). A Proposal for a FAIR Management of 3D Data in Cultural Heritage: The Aldrovandi Digital Twin Case. arXiv preprint arXiv:2407.02018. <a href="https://doi.org/10.48550/arXiv.2407.02018">https://doi.org/10.48550/arXiv.2407.02018</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        Descrizione strutturata per il processo di digitalizzazione di ogni oggetto, definita da una serie di metadati assegnati ad ogni fase prevista dal flusso di lavoro.
      </p>
    </div>
  </div>
</section>

<section>
  <h3>Il modello: CHAD-AP</h3>
  <figure>
    <img src="img/chad-ap-object.png" height="auto" width="500"/>
    <figcaption>
        Fonte: Barzaghi, S., Heibi, I., Moretti, A., & Peroni, S. (2024). Developing Application Profiles for Enhancing Data and Workflows in Cultural Heritage Digitisation Processes. arXiv preprint arXiv:2404.12069. <a href="https://doi.org/10.48550/arXiv.2404.12069">https://doi.org/10.48550/arXiv.2404.12069</a>.
    </figcaption>
  </figure>
</section>

<section>
  <h3>Il modello: CHAD-AP</h3>
  <figure>
    <img src="img/chad-ap-process.png" height="auto" width="500"/>
    <figcaption>
        Fonte: Barzaghi, S., Heibi, I., Moretti, A., & Peroni, S. (2024). Developing Application Profiles for Enhancing Data and Workflows in Cultural Heritage Digitisation Processes. arXiv preprint arXiv:2404.12069. <a href="https://doi.org/10.48550/arXiv.2404.12069">https://doi.org/10.48550/arXiv.2404.12069</a>.
    </figcaption>
  </figure>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
  <figure>
    <img src="img/aldrovandi-example-1.png" height="auto" width="1200"/>
  </figure>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-2.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-2.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-3.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-4.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-4.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-5.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-6.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-6.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-7.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-8.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-8.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-9.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-10.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-10.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-11.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-1.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-1.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-example-12.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section>
  <h3>Risultati</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/aldrovandi-qr.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        Un profilo applicativo totalmente documentato, estendibile, allineato a standard internazionali, e <a href="https://github.com/dharc-org/chad-ap/tree/main">pubblicamente disponibile</a>, per rappresentare oggetti culturali e il loro processo di digitalizzazione.
      </p>
      <p>
        Opportunità: trattamento dei modelli 3D come veri e propri dati della ricerca.
      </p>
    </div>
  </div>
</section>

---

{{< slide background-image="img/sirius.jpg" class="section-slide">}}

## Caso 2: SIRIUS

<!--
Photo by <a href="https://unsplash.com/@joshuakettle?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Joshua Kettle</a> on <a href="https://unsplash.com/photos/a-large-building-with-a-blue-dome-on-top-of-it-94JPfJ-1Hl4?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

<section>
  <h3>Promuovere una cultura del rischio</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 2;">
      <figure>
        <img src="img/sirius-intro.png" height="auto" width="700"/>
        <figcaption>
            Fonte: Fiorentino, S., Chinni, T., Cornaglia, M., Iannucci, A., Vandini, M. (2024). From data interrelationships to capacity building and public awareness: the instance of Ravenna (Italy) and project SIRIUS - management strategies for cultural heritage at risk. PROCULTHER-NET 2 Project. Technical Bulletin N. 3, pp 18-27. <a href="https://civil-protection-knowledge-network.europa.eu/system/files/2024-07/tb_3_final.pdf">https://civil-protection-knowledge-network.europa.eu/system/files/2024-07/tb_3_final.pdf</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        Progetto che punta all'implementazione su scala locale di linee guida internazionali per la prevenzione di rischi ambientali e antropici che impattano sul patrimonio culturale.
      </p>
    </div>
  </div>
  <div class="footer">
    Barzaghi, S., Fiorentino, S., Mecozzi, A., Iannucci, A., & Vandini, M. (2024). The SIRIUS Project: Integrating Data Modeling and Citizen Engagement for Heritage Risk Management. In Karajgikar, J., Janco, A., & Otis, J. (Eds.), DH2024 Book of Abstracts (p. 48-50). Zenodo. <a href="https://doi.org/10.5281/zenodo.13834936">https://doi.org/10.5281/zenodo.13834936</a>.
  </div>
</section>

<section>
  <h3>I dati: assessment del rischio</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/risk-assessment.png" height="auto" width="300"/>
        <figcaption>
            Fonte: WARREDOC. (2022). Study on risk assessment and management of cultural heritage across Europe: Risk Management for Cultural Heritage (Agreement n° 2021-1-IT01-KA220-VET-000034797, Project Result N.1). RMCH Steering Committee. <a href="https://www.charisma-academy.eu/wp-content/uploads/2022/11/CHARISMA_PR1_Study-on-risk-assessment-and-management-of-cultural-heritage-across-Europe.docx.pdf">https://www.charisma-academy.eu/wp-content/uploads/2022/11/CHARISMA_PR1_Study-on-risk-assessment-and-management-of-cultural-heritage-across-Europe.docx.pdf</a>.
        </figcaption>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        Processo scientifico complesso che coinvolge svariate attività di raccolta, analisi, valutazione e produzione di dati, spesso sparsi e non strutturati.
      </p>
    </div>
  </div>
  <div class="footer">
    Barzaghi, S. (2024). Towards a FAIR Ontology Pattern for Describing Heritage Risk Assessment Activities. In: Antonacopoulos, A., et al. Linking Theory and Practice of Digital Libraries. TPDL 2024. Lecture Notes in Computer Science, vol 15178. Springer, Cham. <a href="https://doi.org/10.1007/978-3-031-72440-4_15">https://doi.org/10.1007/978-3-031-72440-4_15</a>.
  </div>
</section>

<section>
  <h3>Il modello: HeRO</h3>
  <figure>
    <img src="img/hero.png" height="auto" width="500"/>
      <figcaption>
          Fonte: Barzaghi, S. (2024). Towards a FAIR Ontology Pattern for Describing Heritage Risk Assessment Activities. In: Antonacopoulos, A., et al. Linking Theory and Practice of Digital Libraries. TPDL 2024. Lecture Notes in Computer Science, vol 15178. Springer, Cham. <a href="https://doi.org/10.1007/978-3-031-72440-4_15">https://doi.org/10.1007/978-3-031-72440-4_15</a>.
      </figcaption>
  </figure>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <p>
        Durante un'attività di identificazione dei rischi relativi al Battistero degli Ariani, condotta a Ravenna da Laura Rossi tra l'1 marzo e l'1 aprile 2024, viene identificato quanto segue: "Inondazioni e piogge forti, di cadenza annuale, posso causare l'erosione delle mura del battistero".
      </p>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <p>
        Durante un'attività di identificazione dei rischi relativi al Battistero degli Ariani, condotta a Ravenna da Laura Rossi tra l'1 marzo e l'1 aprile 2024, viene identificato quanto segue: "Inondazioni e piogge forti, di cadenza annuale, posso causare l'erosione delle mura del battistero".
      </p>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/sirius-example-1.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <p>
        Durante un'attività di analisi dei rischi che interessano il Battistero degli Ariani, condotta tra l'1 aprile e l'1 maggio, Laura individua quanto segue: "Un evento di alluvione è previsto nel battistero circa una volta ogni 25 anni, colpendo molto probabilmente l'intero valore del patrimonio per evento, con conseguente perdita parziale". Per trarre queste conclusioni, Laura usa come fonte il dataset "dati_alluvione_2011-2016.zip", e assegna una serie di punteggi che determinano il calcolo del rischio. 
      </p>
    </div>
    <div style="flex: 1;">
    </div>
  </div>
</section>

<section data-auto-animate>
  <h3>Esempio</h3>
    <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <p>
        Durante un'attività di analisi dei rischi che interessano il Battistero degli Ariani, condotta tra l'1 aprile e l'1 maggio, Laura individua quanto segue: "Un evento di alluvione è previsto nel battistero circa una volta ogni 25 anni, colpendo molto probabilmente l'intero valore del patrimonio per evento, con conseguente perdita parziale". Per trarre queste conclusioni, Laura usa come fonte il dataset "dati_alluvione_2011-2016.zip", e assegna una serie di punteggi che determinano il calcolo del rischio. 
      </p>
    </div>
    <div style="flex: 1;">
      <figure>
        <img src="img/sirius-example-2.png" height="auto" width="700"/>
      </figure>
    </div>
  </div>
</section>

<section>
  <h3>Risultati</h3>
  <div style="display: flex; align-items: center;">
    <div style="flex: 1;">
      <figure>
        <img src="img/sirius-qr.png" height="auto" width="700"/>
      </figure>
    </div>
    <div style="flex: 1;">
      <p>
        Un design pattern facilmente integrabile, estendibile, documentato su <a href="https://github.com/sirius-org/hero">GitHub</a> e archiviato ad ogni update su <a href="https://doi.org/10.5281/zenodo.13857430">Zenodo</a>, per rappresentare le attività coivolte nella valutazione dei rischi a cui sono soggetti i beni culturali.
      </p>
      <p>
        Opportunità: pubblicazione di dati sparsi e ricchi di complessità e un loro riutilizzo per un impatto potenzialmente più significativo sulla comunità.
      </p>
    </div>
  </div>
</section>

<section>
  <h3>Nel prossimo futuro</h3>
  <div style="display: flex; align-items: center;">
      <div style="flex: 2;">
        <figure>
          <img src="img/atlas.png" height="auto" width="700"/>
          <figcaption>
              Fonte: Barzaghi, S. (2024). sirius-org/risk-atlas: Version 0.1.0 (v0.1.0). Zenodo. <a href="https://doi.org/10.5281/zenodo.13857449">https://doi.org/10.5281/zenodo.13857449</a>.
          </figcaption>
        </figure>
      </div>
      <div style="flex: 1;">
        <p>
          Al momento stiamo sviluppando un'applicazione Web per la visualizzazione interattiva dei dati e il monitoraggio di eventi di rischio.
        </p>
        <p>
          Un'altra attività riguarderà lo sviluppo di (almeno) un vocabolario controllato per definire una "terminologia del rischio" per i beni culturali.
        </p>
      </div>
  </div>
</section>

---

{{< slide background-image="img/conclusion.jpg" class="section-slide">}}

## Per concludere

---

<section>
  <h3>Dati + modelli + FAIRness = buona rappresentazione</h3>
  <p>
    Una rappresentazione FAIR dei dati attraverso modelli semantici adeguati è essenziale per una gestione scientifica del patrimonio culturale.
  </p>
  <p>
    Se ben concertato, questo approccio ha impatti significativi non solo sulla ricerca, ma anche sull'industria e sulla cittadinanza.
  </p>    
</section>

<section>
  <h3>Rendiamo i nostri dati più aperti e FAIR</h3> 
  <p>
    I modelli semantici non solo facilitano la comunicazione tra diversi dati e servizi, ma sono anche essenziali per documentarli e renderli più comprensibili.
  </p>
  <p>
    Metadati e documentazione relativi ai processi e alle metodologie devono essere raccolti e valorizzati, soprattutto durante lo svolgimento del progetto.
  </p>
  <p>
    Le metodologie sono dati, quindi trattiamole come tali: come facciamo le cose è importante tanto quanto (o più de)le cose che facciamo!
  </p>
</section>

<section>
  <h3>Facciamoci le domande giuste</h3>
  <p>
    Nella nostra ricerca, integriamo pratiche di Open Science per assicurare l'interoperabilità e il riutilizzo dei dati? Quali? Come?
  </p>
  <p>
    Che tipo di dati e di metodologie utilizziamo? Quanto sono FAIR? 
  </p>
  <p>
    Con quali modelli li rappresentiamo? Sono comprensibili?
  </p>
  <p>
    Cosa altro ci serve per contribuire ad una base di conoscenza del nostro patrimonio culturale più aperta e condivisa?
  </p>
  <div class="footer">
    Jones, S., & Grootveld, M. (2017). How FAIR are your data?. <a href="https://doi.org/10.5281/zenodo.5111307">https://doi.org/10.5281/zenodo.5111307</a>.
  </div>
</section>

---

# Grazie!

# Dati e modelli per il patrimonio culturale e la loro rappresentazione

## I casi del _Rinascimento digitale di Ulisse Aldrovandi_ e del _Progetto SIRIUS_

###### Sebastian Barzaghi | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/) | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527)