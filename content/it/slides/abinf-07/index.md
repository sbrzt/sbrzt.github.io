---
title: ABINF - Intelligenza Artificiale
summary: Lezione di "Intelligenza Artificiale" del corso di Abilità Informatiche per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2024-01-27T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# Intelligenza Artificiale

## Lezione 07 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

### Dal profilo psicologico a Cambridge Analytica

Nel 2007 viene creata un'applicazione Facebook chiamata MyPersonality, che permette agli utenti di compilare dei brevi questionari psicometrici

Sulla base di questo, crea un piccolo profilo psicologico (basato sui Big Five).

https://it.wikipedia.org/wiki/Big_Five_(psicologia)#/media/File:Wiki-grafik_peats-de_big_five_ENG.png

---

### Dal profilo psicologico a Cambridge Analytica

Nell'ecosistema di Facebook, diventa possibile confrontare i risultati di questi test con tutti i tipi di altri dati online dei soggetti (likes, pagine seguite, informazioni di profilo, ecc.).

Diventa molto semplice trovare delle correlazioni tra cose a cui hanno messo un "like", cose che hanno condiviso o pubblicato, sesso, età, luogo di residenza, ecc.

https://www.nbcnews.com/health/health-news/can-facebook-assess-your-personality-n284736

---

### Dal profilo psicologico a Cambridge Analytica

Ciò ha permesso ai ricercatori di fare correlazioni e trarre deduzioni molto affidabili.

Esempi: gli uomini a cui piaceva il marchio di cosmetici MAC avevano leggermente più probabilità di essere gay; uno dei migliori indicatori per l'eterosessualità era "gradire" il Wu-Tang Clan; i seguaci di Lady Gaga erano tendenzialmente estroversi, mentre quelli che amavano la filosofia erano più introversi.

---

### Dal profilo psicologico a Cambridge Analytica

Ogni informazione di questo tipo è troppo debole per produrre una previsione affidabile su una persona, dove prevale l’individualità del singolo.

Quando migliaia di singoli dati vengono combinati, le previsioni risultanti diventano molto più accurate.

---

### Dal profilo psicologico a Cambridge Analytica

Questo ha permesso di comprendere un fenomeno (il comportamento social delle persone), ma ha anche aperto la strada ad altre applicazioni, che hanno creato un database di profili di utenti associati a differenze individuali (giovane conservatore; democratico divorziato; etc) che sono poi stati usati per indirizzare campagne elettorali.

Es. il microtargeting psicografico operato da [Cambridge Analytica](https://www.dirittoconsenso.it/2021/12/21/il-caso-cambridge-analytica/) durante le elezioni americane del 2016 e la Brexit, grazie a modelli di Machine Learning, una forma di Intelligenza Artificiale.

---

{{< slide background-image="img/0700.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## Introduzione

<!--

-->

---

### Cos'è l'IA?

La scienza che studia tecniche computazionali in grado di emulare l’intelligenza umana.

L’abilità di una macchina di mostrare capacità umane quali il ragionamento, l’apprendimento, la pianificazione e la creatività.

---

### Cos'è l'IA?

L’intelligenza artificiale permette ai sistemi di capire il proprio ambiente, mettersi in relazione con quello che percepisce e risolvere problemi, e agire verso un obiettivo specifico. 

I sistemi di IA sono capaci di adattare il proprio comportamento analizzando gli effetti delle azioni precedenti e lavorando in autonomia.

---

### Cos'è l'IA?

L'IA è già parte della trasformazione digitale del mondo.

Quali lavori/comportamenti/attività sarà possibile far svolgere alle IA, e con quali conseguenze nelle relazioni tra e con gli esseri umani?

https://chatgpt.com/

https://aidungeon.com/

https://perchance.org/ai-text-to-image-generator

https://suno.com/home

https://text-to-cad.zoo.dev/

https://invideo.io/make/ai-video-generator/

---

### Applicazioni dell'IA

* **Informatica** (sistemi operativi, programmazione, reti, user interface, filtri anti-spam, sistemi di suggerimento, motori di ricerca, ecc.);
* **Medicina** (formulazione di farmaci, immagini radiologiche, trasporto, supporto alla diagnosi e terapia, ecc.);
* **Robotica** (guida autonoma, robot trasportatori, Kiva robot, ristorazione, Boston Dynamics, droni, ecc.);
* **Marketing** (pubblicità mirata):
* **Finanza** (algoritmi di trading);
* **Filosofia**;
* **Legge**;
* ...

---

### Applicazioni dell'IA

Il campo della IA è diviso in un insieme di aree specializzate, per ciascuna delle quali esistono sistemi molto efficienti nel compiere una azione ma totalmente inadatti alle altre aree.

Si tratta di una delle principali differenze rispetto all'intelligenza umana, che per definizione è in grado di adattarsi a diversi tipi di problemi.

---

### Applicazioni dell'IA

Ad esempio, i programmi di machine translation spesso raggiungono risultati pari o migliori degli umani nella traduzione di un altissimo numero di lingue.

Tuttavia, non riescono a tradurre il senso di espressioni idiomatiche o astratte (umorismo, metafore) se non espressamente pre-programmate.

---

{{< slide background-image="img/0700.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## Origini dell'IA

<!--

-->

---

### Radici in discipline diverse

* **Filosofia** (intelligenza, conoscenza, ragionamento, apprendimento, linguaggio, ecc.);
* **Matematica** (logica, probabilità, statistica, teoria degli algoritmi, ecc.);
* **Psicologia** (modelli cognitivi, esperimenti psicologici);
* **Informatica** (software, hardware, algoritmi);
* **Linguistica** (sintassi, semantica e pragmatica del linguaggio naturale, rappresentazione della conoscenza);
* **Economia** (teoria delle decisioni, teoria dei giochi, ricerca operativa);
* **Neuroscienze** (neuroni, sinapsi, elaborazione delle informazioni nel cervello).

---

### Filosofia

* **Aristotele** (384-322 a.C.) fu il primo a formulare un insieme preciso di leggi che governano la parte razionale della mente. Sviluppò un sistema informale di sillogismi per il ragionamento corretto, che in linea di principio permetteva di generare conclusioni meccanicamente, date delle premesse iniziali;
* **Llull** (1315) teorizzò che il ragionamento potesse essere eseguito tramite artefatti meccanici;
* **Hobbes** (1588-1679) teorizzò il ragionamento come calcolo numerico;
* **Leibniz** (1646-1717) costruì una macchina per eseguire operazioni su concetti piuttosto che su numeri.

---

### Matematica

* **Boole** (1815-1864) elaborò i dettagli della logica proposizionale, o logica booleana;
* **Lovelace** (1840) previde l’avvento dell'AI simbolica (basata cioè su simboli/significati e le loro manipolazioni da parte di operazioni logiche);
* **Frege** (1848-1925) estese la logica di Boole per includere oggetti e relazioni (Logica del primo ordine);
* **Russel** (1919) dimostrò che proposizioni complesse e argomenti deduttivi possono essere rappresentati da valori vero/falso e operatori se/allora/non;
* **Turing** (1912-1954) dimostrò che qualsiasi operazione può essere eseguita da un calcolatore binario, che accetta cioè solo i simboli 0 e 1.

---

### La nascita dell'IA (1943-1955)

Il primo lavoro che ora è generalmente riconosciuto come IA fu svolto da Warren McColluch e Walter Pitts (1943).

Si basarono su tre fonti:
* La conoscenza della fisiologia di base e della funzione dei neuroni nel cervello;
* Un'analisi formale della logica proposizionale di Russel;
* La teoria della computazione di Turing.

https://natureofcode.com/static/472369e80e00d3edb93dae98f30c1ebf/ddecd/10_nn_2.webp

---

### La nascita dell'IA (1943-1955)

Proposero un modello di neuroni artificiali in cui ogni neurone è caratterizzato come "acceso" o "spento", con un passaggio a "acceso" che avviene in risposta alla stimolazione di un numero sufficiente di neuroni adiacenti.

Lo stato di un neurone fu concepito come "fattualmente equivalente a una proposizione che proponeva il suo stimolo adeguato".

Dimostrarono che qualsiasi funzione può essere calcolata da una rete di neuroni connessi.

https://natureofcode.com/static/cf5195820637396bd5e310f20411a82a/e4512/10_nn_4.webp

---

### Entusiasmo iniziale, grandi aspettative (1952-1969)

L'intelligenza artificiale (IA) fu definita, per la prima volta, nel 1956, da John McCarthy come "la scienza e l'ingegneria di costruire macchine intelligenti". 

Più o meno nello stesso periodo, Alan Turing, nel suo articolo "Computing Machinery and Intelligence" (1950), proponeva come test per considerare una macchina intelligente l'abilità di emulare così bene il comportamento umano da diventare indistinguibile.

https://www.masswerk.at/elizabot/

---

### Una dose di realtà (1966-1973)

I primi sistemi si rivelarono un fallimento quando furono messi alla prova su una gamma più ampia di problemi più difficili.

Il primo tipo di difficoltà emerse perché la maggior parte dei primi programmi funzionava solo seguendo un insieme di istruzioni fisse per arrivare a una conclusione.

Esempio: "Quando piove, la strada si bagna" -> "Sta piovendo", quindi "La strada è bagnata".

---

### Una dose di realtà (1966-1973)

Il secondo tipo di difficoltà fu l'irrisolvibilità di molti dei problemi che l'IA stava cercando di risolvere (es. il Problema del Commesso Viaggiatore).

https://www.astronomia.com/wp-content/uploads/2010/12/percorsi-citta.jpg

---

### Sistemi basati sulla conoscenza (1969-1979)

I metodi di risoluzione dei problemi emersi durante il primo decennio di IA erano meccanismi di ricerca a scopo generale che cercavano di mettere insieme passaggi elementari di ragionamento per trovare soluzioni complete.

Tali approcci sono stati chiamati deboli perché, sebbene generali, non sono in grado di scalare per affrontare istanze di problemi più grandi o difficili.

---

### Sistemi basati sulla conoscenza (1969-1979)

L'alternativa ai metodi deboli è utilizzare conoscenze più potenti e specifiche per il dominio, che permettano passaggi di ragionamento più ampi e possano gestire più facilmente i casi tipicamente ricorrenti in aree di competenza ristrette. Questi tipi di sistemi sono anche chiamati sistemi esperti.

Questi sistemi funzionano in due parti principali:
* Base di conoscenza: una grande raccolta di informazioni su un certo argomento (ad esempio, malattie e trattamenti per un sistema medico);
* Motore di inferenza: il "cervello" del sistema, che usa la base di conoscenza per fare ragionamenti e trovare soluzioni.

Esempio: https://www.forbes.com/sites/gilpress/2020/04/27/12-ai-milestones-4-mycin-an-expert-system-for-infectious-disease-therapy/

---

### Inverno della IA (1980-1993)

L'industria dell'IA esplose da pochi milioni di dollari nel 1980 a miliardi di dollari nel 1988, includendo centinaia di aziende che costruivano sistemi esperti, sistemi di visione, robot e software e hardware specializzati per questi scopi.

Poco dopo arrivò un periodo chiamato “inverno dell'IA”, in cui molte aziende fallirono, poiché non riuscirono a mantenere le promesse fatte.

Motivi:
* Dipendenza da regole fisse: i metodi di ragionamento utilizzati dai sistemi basati sulla conoscenza non funzionavano di fronte all'incertezza;
* Impossibilità di aggiornare autonomamente le conoscenze: i sistemi di questo tipo non potevano apprendere dall'esperienza.

---

### Reti neurali e apprendimento automatico (1986 - presente)

Questi metodi hanno la capacità di apprendere dall'esperienza.

Possono confrontare il valore di output previsto con il valore reale rispetto ad un problema e modificare i loro parametri per ridurre la differenza, rendendoli più propensi a performare bene su esempi futuri.

La fragilità dei sistemi esperti portò a un nuovo approccio, più scientifico, che incorporava la probabilità anziché la logica booleana, e l'apprendimento automatico anziché la programmazione manuale.

---

### Big data (2001 - presente)

Nel corso della storia di 60 anni dell'informatica, l'enfasi è stata sull'algoritmo come principale oggetto di studio.

Alcuni lavori recenti nell'IA suggeriscono che, per molti problemi, ha più senso preoccuparsi dei dati e essere meno selettivi riguardo all'algoritmo da applicare.

---

### Big data (2001 - presente)

Uno studio influente in questa direzione è stato il lavoro di Yarowsky sulla disambiguazione del senso delle parole: dato l'uso della parola "plant" in una frase, ci si riferisce a una pianta o a una fabbrica?

* Gli approcci precedenti si basavano su esempi etichettati dall'uomo combinati con algoritmi di apprendimento automatico;
* Yarowsky mostrò che questa attività può essere svolta senza alcun esempio etichettato, con una precisione del 96%, analizzando un corpus molto grande con le definizioni del dizionario dei due sensi (cioè "plant, flora" e "plant, impianto industriale").

---

### Deep learning (2011–presente)

Il deep learning si riferisce all'apprendimento automatico che utilizza più livelli di elementi computazionali semplici e regolabili.

Esperimenti con tali reti furono condotti già negli anni '70, e sotto forma di reti neurali convoluzionali ottennero alcuni successi nel riconoscimento di cifre scritte a mano negli anni '90.

Tuttavia, fu solo nel 2011 che i metodi di deep learning decollarono veramente. Questo avvenne inizialmente nel riconoscimento vocale e poi nel riconoscimento visivo di oggetti.

https://getthematic.com/insights/content/images/2023/02/image-1.png

---

### Deep learning (2011–presente)

Nel 2012, in una competizione per classificare le immagini in una delle mille categorie (armadillo, libreria, cavatappi, ecc.), un sistema di deep learning creato da Geoffrey Hinton dimostrò un miglioramento drammatico rispetto ai sistemi precedenti, che si basavano in gran parte su caratteristiche realizzate a mano.

Il deep learning dipende da hardware potente e dalla disponibilità di grandi quantità di dati di addestramento.

---

### Lo stato dell'arte

La Stanford University riunisce panel di esperti per fornire report sullo stato dell'arte nell'IA, e produce anche un AI Index su aiindex.org per monitorare i progressi.

Le ultime tendenze: https://aiindex.stanford.edu/report/#individual-chapters.

---

{{< slide background-image="img/0700.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## Come funziona l'IA

<!--

-->

---

### IA debole (o ristretta)

L'IA debole, anche chiamata IA ristretta, è focalizzata su un compito specifico (ad esempio, il riconoscimento di oggetti). Mira a imitare come gli esseri umani eseguono azioni di base come ricordare, percepire e risolvere problemi semplici.

Risolve una classe di problemi specifici attraverso alcune
capacità cognitive.

Esempi: recommendation systems, assistenti virtuali, ecc.

---

### Esempio: AlphaGo

Nel 2015-16 DeepMind sviluppa AlphaGo, un programma che batte il campione umano di Go utilizzando algoritmi di “deep learning” e tecniche di ragionamento automatico.

https://ichef.bbci.co.uk/ace/branded_news/1200/cpsprodpb/0D9B/production/_88738430_pic1go.jpg

---

### IA forte (o estesa)

L'IA forte è un tipo di intelligenza artificiale le cui capacità imitano le capacità adattive e generalizzabili del cervello umano, comprese il ragionamento, la pianificazione e l'intuizione.

Conosciuta anche come AI Generale, per ora è pura speculazione.

---

### Pseudo-esempio: Watson

Nel 2011 sconfigge campioni umani nel gioco televisivo Jeopardy.

Usa “conoscenza” ad ampio spettro, comprensione e generazione di linguaggio naturale, forme di ragionamento e apprendimento.

Hardware potente e costoso (RAM di 16 Terabyte, > 1M$)

Analizza dati da molte fonti, pari a 1 milione di libri al secondo

“Customizzabile” per diverse applicazioni specifiche:
* Sanità (supporto alle decisioni in diagnosi e terapie);
* Servizi al cliente;
* Call center per grandi aziende;
* Assistenza nei processi legali;
* ...

---

### Tipologie e approcci diversi

* IA simbolica: si basa sull'uso di simboli e regole esplicite per rappresentare e manipolare la conoscenza, tipicamente utilizzata in sistemi esperti;
* IA sub-simbolica: si basa sull'uso di modelli matematico-probabilistici per rappresentare i processi cognitivi;
  * Reti neurali artificiali: ispirati al funzionamento del cervello umano, utilizzati per riconoscere pattern e fare previsioni su grandi quantità di dati;
  * Deep Learning: sottocategoria delle reti neurali che utilizza strutture più complesse (come reti profonde) per affrontare compiti più complessi;
  * Large Language Models: addestrati su enormi quantità di testi per comprendere, generare e rispondere in linguaggio naturale.

---

### Approccio simbolico

Usare simboli significa rappresentare la conoscenza o le informazioni in modo chiaro e definito tramite simboli (parole, numeri, segni, etc.) che hanno un significato ben preciso, e seguire regole definite per manipolare questi simboli.

In un sistema simbolico, ogni elemento di conoscenza è rappresentato esplicitamente con simboli e la logica del sistema si basa su regole formali di manipolazione di questi simboli, come in un linguaggio di programmazione o in un sistema esperto. 

Per esempio, un programma che "ragiona" su come risolvere un problema di logica, come "Se piove, allora prendo l'ombrello", lavora usando simboli come "piove" e "ombrello" e segue regole di inferenza per prendere una decisione.

https://miro.medium.com/v2/resize:fit:1400/1*xYZrAXZi6Iq3c1Z_CxW6ZA.png

---

### Approccio simbolico

* Facile da controllare;
* Facile da correggere;
* Facile da spiegare;
- Notevole impegno necessario per definire i simboli;
- Notevole impegno necessario per progettare regole e metodi per manipolare i simboli e risolvere i problemi.

---

### Approccio sub-simbolico

La conoscenza non è rappresentata da simboli visibili o comprensibili dall'uomo (come "gatto" o "mela"), ma è distribuita attraverso le connessioni tra i neuroni e i pesi di queste connessioni. 

La rete neurale "impara" a riconoscere pattern, ma non lo fa in modo esplicito con simboli: non ha un concetto formale di "gatto" o "mela" in termini simbolici, ma riconosce pattern di dati che, per esempio, corrispondono a un gatto o ad una mela in una foto.

https://miro.medium.com/v2/resize:fit:1400/1*q3lZ7tRz1vf48uL6PNmeSg.png

---

### Approccio sub-simbolico

* Migliore performance per compiti percettivi;
* Più robusto contro l'incertezza;
* Più facile da scalare;
* Meno conoscenza iniziale richiesta;
- Difficile da spiegare;
- Necessita di una grande quantità di esempi per apprendere la forza ottimale.

---

### Esempio di approccio sub-simbolico: Machine learning

IA che impara dai dati e fa previsioni sulla base di quello che ha imparato, in assenza di istruzioni esplicite (cioé simboliche).

Basato sull'idea di rete neurale.

https://miro.medium.com/v2/resize:fit:1400/1*uB8f6JncIQwhSVnh5DjiTA.png

---

### Unità della rete neurale: il Percettrone

Le cellule del cervello umano, i neuroni, formano una rete complessa e altamente interconnessa e inviano segnali elettrici l'uno all'altro per aiutare gli esseri umani a elaborare informazioni.

https://natureofcode.com/static/472369e80e00d3edb93dae98f30c1ebf/ddecd/10_nn_2.webp

---

### Unità della rete neurale: il Percettrone

Analogamente, una rete neurale artificiale è fatta di neuroni artificiali (battezzati da Rosenblatt "percettroni") che collaborano per risolvere un problema.

https://natureofcode.com/static/cf5195820637396bd5e310f20411a82a/e4512/10_nn_4.webp

---

### Unità della rete neurale: il Percettrone

Un percettrone consiste in:
* Uno o più input (dati in entrata);
* Un'unità di calcolo;
* Un output (dati in uscita).

Il perceptrone prende gli input (numeri), li soppesa, somma i risultati e decide se dare come output un 1 o un 0 in base a una soglia predefinita.

https://natureofcode.com/static/cf5195820637396bd5e310f20411a82a/e4512/10_nn_4.webp

---

### Unità della rete neurale: il Percettrone

Ogni dato ha un certo valore numerico.

Il valore di ogni dato di input viene moltiplicato con un peso (un valore numerico, generalmente tra 0 e 1, che ne rappresenta l'importanza rispetto al risultato finale).

Tutti i valori pesati vengono sommati insieme, producendo un unico numero.

https://www.w3schools.com/ai/img_perceptron.jpg

---

### Unità della rete neurale: il Percettrone

Questa somma pesata viene passata attraverso una funzione di attivazione, che decide se il perceptrone si "attiva" (cioè produce un output). 

Una funzione semplice, chiamata "step function" (funzione a gradino), dice semplicemente: se la somma è maggiore di una certa soglia, l'output sarà 1 (vero); se è minore della soglia, l'output sarà 0 (falso).

https://www.sharpsightlabs.com/wp-content/uploads/2023/07/perceptron_structure_v1.png

---

### Unità della rete neurale: il Percettrone

Il percettrone, in origine, era pensato per prendere input binari (0 e 1) e generare output binari (0 e 1).

Molto utile per decisioni semplici.

---

### Esempio di Percettrone: il concerto

Dobbiamo decisere se andare ad un concerto. 

Di solito, dobbiamo considerare una serie di fattori: l'artista è bravo? Il tempo è buono? 

Per prendere questa decisione, decidiamo di usare un percettrone.

---

### Esempio di Percettrone: il concerto

I fattori da considerare sono i dati di input, ad ognuno dei quali possiamo assegnare un valore binario (0 equivale a "NO", 1 equivale a "SI").

* L'artista è bravo? = 0 o 1
* Il tempo è buono? = 0 o 1
* Siamo con amici? = 0 o 1
* Servono cibo? = 0 o 1
* Servono bevande? = 0 o 1

---

### Esempio di Percettrone: il concerto

Ognuno di questi fattori, però, ha per noi un'importanza diversa. 

Quindi, ad ogni input assegnamo anche un peso numerico che rappresenti questa importanza (dove 0 è "importanza nulla" e 1 è "importanza essenziale").

* L'artista è bravo? = 0 o 1, con peso = 0.7
* Il tempo è buono? = 0 o 1, con peso = 0.6
* Siamo con amici? = 0 o 1, con peso = 0.5
* Servono cibo? = 0 o 1, con peso = 0.3
* Servono alcolici? = 0 o 1, con peso = 0.4

---

### Esempio di Percettrone: il concerto

Ora, diciamo che:

* L'artista è bravo = 1
* Il tempo non è buono = 0
* Siamo con amici = 1
* Non servono cibo = 0
* Servono alcolici = 1

E diciamo che la nostra soglia da considerare per prendere la decisione sia 1.5: sotto la soglia, l'output è 0 ("non vado al concerto"); sopra la soglia, l'output è 1 ("vado al concerto").

---

### Esempio di Percettrone: il concerto

Moltiplichiamo ogni input per il peso che gli abbiamo assegnato:

* L'artista è bravo = 1 * 0.7 = 0.7
* Il tempo non è buono = 0 * 0.6 = 0
* Siamo con amici = 1 * 0.5 = 0.5
* Non servono cibo = 0 * 0.3 = 0
* Servono alcolici = 1 * 0.4 = 0.4

Sommandoli, otteniamo: 0.7 + 0 + 0.5 + 0 + 0.4 = 1.6

---

### Esempio di Percettrone: il concerto

La somma dei valori pesati è 1.6, e la soglia che abbiamo stabilito è 1.5.

Dato che 1.6 > 1.5, l'output è 1, quindi andrò al concerto.

Nota: il criterio per stabilire la soglia dipende dal dominio del problema e dalle preferenze di chi sviluppa. Si tratta di una decisione arbitraria effettuata su basi empiriche (esperienza), su dati (in un processo di addestramento), ecc.

---

### Reti neurali multistrato

Sono composte da gruppi di neuroni artificiali organizzati in livelli. 

Tipicamente sono presenti: 
* un livello di input: il punto in cui i dati entrano nel sistema;
* uno o più livelli intermedi: strati di neuroni che elaborano i dati in modo complesso;
* un livello di output: il risultato finale.

Ogni neurone in un livello fa un calcolo sui dati che riceve e poi decide se attivarsi o meno.

https://upload.wikimedia.org/wikipedia/commons/thumb/4/46/Colored_neural_network.svg/800px-Colored_neural_network.svg.png

---

### Reti neurali multistrato

Ogni neurone rappresenta una piccola parte di un concetto. 

Non ha senso guardare un singolo neurone e pensare che rappresenti qualcosa di grande come "gatto" o "cane". 

Piuttosto, molti neuroni insieme contribuiscono a formare un concetto più grande, come "gatto" o "cane". 

Quindi, ogni neurone è come un microtratto, una piccolissima caratteristica di qualcosa.

https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Neural-Network-Example-What-Is-A-Neural-Network-Edureka.png

---

### Esempio: capire se una foglia è malata

Prendiamo l'immagine di una foglia. Vogliamo capire se la foglia è sana o malata. Decidiamo di utilizzare una rete neurale.

L'immagine è fatta di pixel, e ogni pixel ha un valore numerico che rappresenta il colore del pixel stesso. Quindi, un'immagine può essere convertita in un insieme strutturato di valori numerici.

https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Neural-Network-Example-What-Is-A-Neural-Network-Edureka.png


---

### Esempio: capire se una foglia è malata

Una volta che l'immagine è trasformata in numeri, questi numeri vengono passati come input alla rete neurale.

La rete neurale ha livelli nascosti (strati intermedi) che si occupano di elaborare e trasformare questi numeri in informazioni più utili.

Ogni neurone nei layer nascosti prende i numeri in ingresso (che sono i pixel dell'immagine), li combina con i pesi (numeri che determinano quanto ogni input è importante), e poi applica una funzione di attivazione per determinare se quel neurone deve attivarsi o meno.

https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Neural-Network-Example-What-Is-A-Neural-Network-Edureka.png

---

### Esempio: capire se una foglia è malata

I layer nascosti quindi trasformano questi numeri di input in rappresentazioni più astratte. 

Ad esempio, mentre nel primo strato la rete potrebbe rilevare semplici caratteristiche come i bordi della foglia, nei layer successivi la rete potrebbe iniziare a riconoscere caratteristiche più complesse come la forma della foglia o eventuali macchie che indicano malattia.

https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Neural-Network-Example-What-Is-A-Neural-Network-Edureka.png

---

### Esempio: capire se una foglia è malata

L'output finale viene prodotto dal livello di output, che di solito è un singolo neurone (o più neuroni, a seconda del tipo di classificazione). 

Nel caso della classificazione della foglia come sana o malata, l'output sarà una probabilità tra 0 e 1, che indica quanto è probabile che l'immagine della foglia sia sana (ad esempio, 0.8 = 80% di probabilità che la foglia sia sana).

https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Neural-Network-Example-What-Is-A-Neural-Network-Edureka.png

---

### Torniamo a parlare di Machine Learning

---

### Tipi di ML

L'apprendimento è un processo iterativo che consiste nell'ottimizzazione progressiva dei parametri che definiscono il modello di IA, attraverso la misurazione ciclica dell'errore tra il risultato atteso e il risultato prodotto.

* **Supervisionato**: i dati di esempio sono preventivamente etichettati da un essere umano;
* **Non supervisionato**: cerca autonomamente di individuare relazioni tra i dati;
* **Per rinforzo**: apprende sulla base di penalità o ricompense ricevute dall'ambiente in cui si trova ad agire.

---

### Tipi di ML

Richiedono una fase di addestramento (training), che rende la rete in grado di adattarsi al tipo di attività da svolgere.

L'addestramento consiste nel provare, fare errori, e correggerli tramite la retropropagazione, un meccanismo per cui la rete regola i vari pesi tra neuroni per migliorare il proprio risultato.

Il training è poi seguito da una fase successiva di testing, in cui la rete svolge l’attività per cui è stata addestrata su nuovi dati che non aveva mai visto prima.

https://www.researchgate.net/publication/354960266/figure/fig1/AS:11431281251915131@1718389091562/The-main-types-of-machine-learning-Main-approaches-include-classification-and-regression.tif

---

### Apprendimento supervisionato

In fase di addestramento della rete, vengono forniti sia gli stimoli su cui operare (es. immagini da classificare come cani o gatti) e la risposta corretta (es. a tutte le immagini di cani è associata l’etichetta «cane»; a tutte le immagini di gatti è associata l’etichetta «gatto»).

https://miro.medium.com/v2/1*Iz7bCLrPTImnBDOOEyE3LA.png

---

### Apprendimento non-supervisionato

Il training non prevede che siano fornite le risposte corrette.

Invece, vengono individuate regolarità statistiche presenti nei dati: ad esempio, la conformazione del muso, la dimensione, i colori, ecc. 

Sulla base di questo, è possibile creare un cluster omogeneo contenente le immagini di «cane» e un altro contenente le immagini di «gatto».

https://static.javatpoint.com/tutorial/machine-learning/images/unsupervised-machine-learning-1.png

---

### Apprendimento per rinforzo

Come nell’apprendimento per rinforzo umano, è possibile guidare l’addestramento di una macchina assegnando premi o punizioni in base alle azioni svolte.

Questo premio/punizione può riferirsi a una catena complessa di azioni svolte dalla macchina, a volte in tempi diversi (es., scacchi), o ad azioni semplici.

---

### IA discriminativa

Finalizzata all'analisi delle informazioni ricevute e alla classificazione di tali informazioni in categorie predefinite: “discrimina” i dati secondo alcuni criteri predefiniti. 

Modelli di IA di tipo discriminativo vengono addestrati per distinguere tra categorie di dati (es. come riconoscere immagini di oggetti diversi).

I modelli apprendono una funzione matematica in grado di separare i dati.

---

### IA generativa

Finalizzata alla generazione di nuovo contenuto (testi, disegni, immagini, ecc.) sulla base di determinate informazioni di partenza (PROMPT). 

I modelli di tipo generativo imparano a produrre nuovi dati con caratteristiche simili ai dati originali (ad es. come produrre testi o immagini di un certo tipo), utilizzando modelli di apprendimento automatico per identificare i pattern e le relazioni nei dati esistenti.

I modelli apprendono una funzione matematica che rappresenta la distribuzione di probabilità dei dati.

---

### Un esempio ibrido: Generative Adversarial Networks

Durante il training, il discriminatore apprende a riconoscere immagini reali (es. apprendimento non supervisionato o supervisionato per specifiche classi, come gatti).

Alla fine dell'apprendimento è in grado di dire se uno stimolo appartiene alla classe di immagini di training (fotografie reali, volti, gatti, etc.) o no.

---

### Un esempio ibrido: Generative Adversarial Networks

Un generatore crea immagini sulla base di dati casuali: inizialmente, le immagini create saranno senza senso.

È come le immagini di training?
* NO-> il generatore deve correggere i pesi
* SI-> il discriminatore è stato «ingannato», e l’immagine è presa come risultato valido

---

### Un esempio ibrido: Generative Adversarial Networks

Per ogni contenuto che il «discriminatore» sa riconoscere, è possibile creare un esempio.

È necessario che il sistema riesca a discriminare con esattezza le caratteristiche (features) di ciascun contenuto!

• https://thispersondoesnotexist.com/
• https://thiscatdoesnotexist.com/
• https://www.craiyon.com/

---

### Large Language Model

Modelli generativi generati da tecniche di deep-learning addestrati su enormi quantità di testo per imparare a riconoscere schemi e associazioni propri del linguaggio naturale.

---

### Large Language Model

Il processo di addestramento di un Large Language Model si divide in due fasi principali:
* Pre-training: in questa fase, il modello viene addestrato su un grande corpus di testo per imparare a riconoscere le relazioni tra le parole e le frasi;
* Fine-tuning: in questa fase, il modello viene addestrato su un nuovo corpus di testo specifico per migliorare la sua capacità di generare testo in un contesto specifico.

---

### Large Language Model

L'IA generativa produce risultati statisticamente probabili, ma non necessariamente veri, reali. 

La qualità e la rumorosità dei dati così come le caratteristiche stesse dei modelli, possono far apprendere una distribuzione di probabilità alterata o distorta; in questi casi, il modello potrebbe non essere in grado di distinguere le relazioni causali da quelle spurie o coincidentali, proponendo risposte inesatte, travisanti la realtà.

La risposta di un modello generativo è confezionata in una argomentazione, formulata aggregando un numero limitato di fonti emergenti.

---

### Large Language Model

Man mano che i parametri aumentano, aumentano le capacità del modello, ma anche le risorse di calcolo richieste. 

Se consideriamo, ad esempio, l'evoluzione dei modelli GPT per la creazione di testo, il GPT-1 del 2018 possedeva 117 milioni di parametri, il GPT2 del 2019 ne aveva 1,5 miliardi, e il GPT3 del 2020 raggiungeva i 175 miliardi. 

Per addestrare un nuovo modello, oggi occorrono centinaia di migliaia di unità di elaborazione grafica ciascuna delle quali ha un costo di decine di migliaia di dollari.

---

### Large Language Model

Secondo i dati dell'Osservatorio del Politecnico di Milano, lo scalpore suscitato dai risultati dall'IA generativa ha ravvivato l'interesse nell'IA in generale e il mercato dell'IA, nel 2023, in Italia ha raggiunto una crescita del 52%, rispetto al 2022, pari a 760 mln di euro. 

Di questi, per ora, solo il 5% riguarda le soluzioni basate sull'IA generativa (principalmente assistenti virtuali per sintetizzare documenti, scrivere codice informatico, interrogare basi di dati). 

---

### Large Language Model

Alta flessibilità e resistenza ad informazione danneggiata o lacunosa

Tuttavia, la loro decisione è sempre probabilistica, anche quando questo non è richiesto: 1+1 = forse 2

La performance è fortemente influenzata dalle caratteristiche dei dati di training -> rischio di BIAS

A frenare gli investimenti in questo settore sono soprattutto la potenziale inattendibilità delle risposte (allucinazioni), i costi di sviluppo elevati, le incertezze legate all'AI act. 

---

{{< slide background-image="img/0700.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## I problemi

<!--

-->

---

### Uso di dati della IA

L’IA si basa su dati storici e sintetici.

I dati storici sono raccolti da database “reali”: le canzoni che ho ascoltato, le temperature raccolte negli ultimi 200 anni, i post su un determinato argomento.

Si trata di “big data” ampi ma non necessariamente omogenei al loro interno.

I dati sintetici sono generati dal sistema e possono aiutare a rappresentare un problema, se ne danno una rappresentazione affidabile.

In questo caso, non ci sono dati reali su cui basare l’apprendimento ma solo dati generati da un’altra IA.

---

### IA discriminatoria?

Confound presenti nei dati possono produrre distorsioni nel funzionamento; ad esempio, alcuni sistemi di riconoscimento facciale trattano alcune persone in modo più impreciso rispetto alle altre.

La numerosità dei dati di training può produrre distorsioni.

---

### Una minaccia?

Protezione dei dati?

Copyright?

Creazione di monopoli?

Impatto sul mercato del lavoro?

Disinformazione?

---

### Questioni etiche

Legate alla gestione dei dati (prove) usati dai sistemi IA (legate alla conoscenza della realtà):

Possibilità che siano:
* Inconcludenti: non permettono di prendere alcuna decisione;
* Imperscrutabili: non è dato sapere in base a cosa abbiano favorito una decisione;
* Fuorvianti: hanno preso una decisione in base a dati distorti;
* Ingiusti: generano effetti iniqui sulle persone;
* Trasformativi: trasformazioni nel processo decisionale che minacciano l'autonomia o la privacy individuale;
* Non-tracciabilità: difficoltà nel rintracciare la persona/organizzazione responsabile di un determinato evento o comportamento.

---

### Questioni etiche

I LLM richiedono grandi quantità di dati per funzionare, che possono includere informazioni personali: problema legato alla privacy nella raccolta, archiviazione e utilizzo dei dati.

L'uso di modelli di grandi dimensioni richiede risorse computazionali significative, limitando l'accesso a tali tecnologie a poche organizzazioni o individui con risorse sufficienti e generando un impatto significativo a livello ecologico.

---

### Questioni etiche

Non esiste una soluzione certa a questo problema, se non quella di indagare il tipo di training a cui un sistema è soggetto, e il suo comportamento in fase di produzione.

• Supervisionare i processi normativi
• Europa: AI act (2024)

---

### AI Act

Nel 2024, il Parlamento Europeo ha approvato l'AI Act, il primo Regolamento al mondo esplicitamente e totalmente dedicato all'Intelligenza Artificiale.

Il testo contiene norme che disciplinano l'attività dei software di obbligando gli operatori al rispetto dei diritti e dei valori fondamentali dell'Unione Europea.

---

### AI Act

Saranno vietati i sistemi di IA che determinano un rischio inaccettabile per la sicurezza, i mezzi di sussistenza e i diritti delle persone. 

In questa categoria rientrano i sistemi che possono manipolare il comportamento umano come quelli che consentono di attribuire un "punteggio sociale" (social scoring), per finalità pubbliche e private, classificando le persone in base al loro comportamento sociale o alle loro caratteristiche personali, e determinate applicazioni di polizia predittiva.

---

### AI Act

Il regolamento considera ad alto rischio un numero limitato di sistemi di IA che possono potenzialmente avere ripercussioni negative sulla sicurezza delle persone o sui loro diritti fondamentali (tutelati dalla Carta dei diritti fondamentali dell'UE) (es. identificazione biometrica remota, categorizzazione biometrica e riconoscimento delle emozioni; valutazione dell'occupazione; determinare l'accesso a servizi e a prestazioni pubblici e privati essenziali).

Prima di immettere un sistema di IA ad alto rischio sul mercato dell'UE, o di farlo entrare in servizio, i fornitori dovranno sottoporlo, in particolare, a una valutazione della conformità.

---

### AI Act

I sistemi di IA a rischio minimo (come videogiochi o filtri spam) saranno esenti da obblighi, ferma restando l'adesione volontaria a codici di condotta, da parte dei fornitori di tali sistemi, ad esempio laddove esista un evidente rischio di manipolazione. 

Gli utenti dovranno essere consapevoli del fatto che stanno interagendo con una macchina.

---

### IA e cultura

Nell'AI Act europeo, la cultura è espressamente menzionata fra gli ambiti al cui sviluppo l'intelligenza artificiale è chiamata a concorrere; la diversità culturale è un fattore che dovrebbe essere preservato nella progettazione e nell'uso dell'AI. 

A livello nazionale, nell'ambito delle politiche per la digitalizzazione dei beni culturali, se per un verso si richiamano le potenzialità dell'AI, per altro verso si evidenzia come «digitalizzare beni non metadatati e/o descritti è fortemente sconsigliato.

Questa eventualità potrebbe essere ammissibile [ad esempio nel caso di] campagne sperimentali orientate a una descrizione del bene eseguita online da una comunità di riferimento adeguatamente identificata (possibili progetti di crowdsourcing) o alla descrizione del soggetto con l'uso di algoritmi di intelligenza artificiale» (cfr. Linee guida per la digitalizzazione del patrimonio culturale). 

---

### IA e cultura

Il tema della "novità" dell'opera riadattata con nuovi linguaggi divulgativi e comunicativi rispetto all'originale è adombrato, con specifico riferimento al digitale, anche nel Piano nazionale di digitalizzazione del patrimonio culturale 2022–2023 là dove si evoca il superamento della «funzione ancillare del bene digitale come replica o copia dell'originale fisico e afferma la legittimità di un percorso di conoscenza autonomo, peculiare e connotato da originalità. 

Originalità che non discende dall'oggetto ma dalla relazione intellettuale da cui il bene digitale prende forma e da cui attinge nuovi significati trasmissibili e non solo "pensabili". 

Il patrimonio culturale digitale è costituito da oggetti, la cui natura può essere definita sulla base delle relazioni informative che sono in grado di generare. 

Essi, anche quando collegati ai beni culturali fisici, possiedono un'autonomia ontologica, come ormai attestato da un'ampia letteratura. 

L'esistenza di tale quid novi fra opera originale e sue rielaborazioni sembra alla base della disposizione in commento e potrebbe assumere rilievo anche in caso di rielaborazioni operate dall'AI.

---

### IA e copyright

L'AI Act europeo impone ai fornitori di servizi di offrire adeguate informazioni dei materiali utilizzati per l'addestramento dell'intelligenza artificiale, anche al fine di consentire la tutela del diritto d'autore e del copyright ai soggetti interessati.

Nel proprio addestramento, i sistemi d'intelligenza artificiale attingono a una grande massa di dati e contenuti presenti in rete (c.d. webscraping), in alcuni casi protetti da copyright o altri diritti che ne limitano l'accesso o l'utilizzo senza autorizzazione. 

[New York Times contro Open A.I.]

---

### IA e copyright

La configurabilità di un diritto di proprietà intellettuale in caso di opera creata dall'AI. 

Lo United States Copyright Office ha adottato nel 2023 apposite linee guida (Copyright Registration Guidance: Works Containing Material Generated by Artificial Intelligence) al fine di valutare se un'opera realizzata mediante strumenti d'intelligenza artificiale generativa possa o meno essere coperta da diritto d'autore. 

In questa prospettiva, secondo un giudizio caso per caso, l'ufficio valuta «se l'"opera" sia fondamentalmente di paternità umana, con il computer [o altro dispositivo] come mero strumento di supporto, o se gli elementi tradizionali di paternità dell'opera (espressione letteraria, artistica o musicale o elementi di selezione, arrangiamento, ecc.) siano concepiti ed eseguiti non dall'uomo ma dalla macchina». 

la «protezione del diritto d'autore postula il requisito dell'originalità e della creatività, consistente non già nell'idea che è alla base della sua realizzazione, ma nella forma della sua espressione, ovvero dalla sua soggettività, presupponendo che l'opera rifletta la personalità del suo autore, manifestando le sue scelte libere e creative; la consistenza in concreto di tale autonomo apporto forma oggetto di una valutazione destinata a risolversi in un giudizio di fatto» per poi aggiungere, ai fini che qui interessano, come  l' «aver utilizzato un software per generare l'immagine […] è pur sempre compatibile con l'elaborazione di un'opera dell'ingegno con un tasso di creatività che andrebbe solo scrutinato con maggior rigore». La pronuncia, pur non sciogliendo la questione in via definitiva e compiuta, non conclude a priori che il concorso dell'intelligenza artificiale alla realizzazione dell'opera escluda in ogni caso la configurabilità del diritto d'autore, dovendo valutarsi caso per caso.

---


### Il test di Turing

The Turing Test, proposed by Alan Turing (1950), was designed to provide a satisfactory operational definition of intelligence.
• A computer passes the test if a human interrogator, after posing some written questions,
cannot tell whether the written responses come from a person or from a computer.

GPT-4 was considered human 54% of the time, closely mimicking real human interactions

---

# Fine

## Lezione 06 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)