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

# Intelligenza Artificiale (2)

## Lezione 08 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

{{< slide background-image="img/0800.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## Come funziona l'IA

<!--

-->

---

### IA debole (o ristretta)

L'IA debole, anche chiamata IA ristretta, è focalizzata su un compito specifico (ad esempio, il riconoscimento di oggetti). 

Risolve una classe di problemi specifici attraverso alcune capacità cognitive.

Esempi: recommendation systems, assistenti virtuali, ecc.

https://www.miquido.com/wp-content/uploads/2023/07/Hybrid-Recommendation-System-in-Netflix-700x492.png

---

### Esempio: AlphaGo

Nel 2015-16 DeepMind sviluppa AlphaGo, un programma che batte il campione umano di Go, un famosissimo gioco da tavolo cinese.

Documentario: https://www.youtube.com/watch?v=WXuK6gekU1Y.

https://ichef.bbci.co.uk/ace/branded_news/1200/cpsprodpb/0D9B/production/_88738430_pic1go.jpg

---

### IA forte (o estesa)

L'IA forte è un tipo di intelligenza artificiale le cui capacità imitano le proprietà adattive e generalizzabili del cervello umano, comprese il ragionamento, la pianificazione e l'intuizione.

Conosciuta anche come IA Generale (AGI), _per ora_ è pura speculazione.

https://www.vox.com/the-highlight/23779413/silicon-valleys-ai-religion-transhumanism-longtermism-ea

---

### Pseudo-esempio: Watson

Nel 2011 sconfigge campioni umani nel gioco televisivo statunitense Jeopardy.

Usa conoscenza ad ampio spettro, comprensione e generazione di linguaggio naturale, forme di ragionamento e apprendimento.

Analizza dati da molte fonti, pari a 1 milione di libri al secondo.

“Customizzabile” per diverse applicazioni specifiche:
* Supporto alle decisioni in diagnosi e terapie;
* Servizi al cliente;
* Assistenza nei processi legali;
* ...

https://www.youtube.com/watch?v=P18EdAKuC1U

---

### Tipologie e approcci diversi

* IA **simbolica**: si basa sull'uso di simboli e regole esplicite per rappresentare e manipolare la conoscenza, tipicamente utilizzata in sistemi esperti;
* IA **sub-simbolica**: si basa sull'uso di modelli matematico-probabilistici per rappresentare i processi cognitivi;
  * **Reti neurali artificiali**: ispirate al funzionamento del cervello umano, utilizzate per riconoscere pattern e fare previsioni su grandi quantità di dati;
  * **Deep Learning**: sottocategoria delle reti neurali che utilizza strutture più complesse (come reti profonde) per affrontare compiti più complessi;
  * **Large Language Models**: addestrati su enormi quantità di testi per comprendere, generare e rispondere in linguaggio naturale.

---

### Approccio simbolico

Le AI simboliche rappresentano la conoscenza in modo chiaro e definito tramite simboli (parole, numeri, segni, etc.) che hanno un significato ben preciso, e seguono regole definite per manipolare questi simboli.

Per esempio, un programma che "ragiona" su come risolvere un problema di logica (come "Se piove, allora prendo l'ombrello") lavora usando sequenze di simboli come "piove" e "ombrello" e segue regole di inferenza logica per prendere una decisione.

Un sistema esperto di medicina potrebbe usare simboli come "febbre", "tosse", "mal di testa" per fare diagnosi, applicando regole logiche per determinare quale malattia potrebbe corrispondere a questi sintomi.

https://miro.medium.com/v2/resize:fit:1400/1*xYZrAXZi6Iq3c1Z_CxW6ZA.png

---

### Approccio simbolico

Vantaggi: l'approccio simbolico è molto potente per risolvere problemi complessi in ambienti ben definiti, come la logica formale, la pianificazione e la manipolazione di concetti astratti. È facile da controllare, correggere e interpretare, e permette di costruire modelli molto trasparenti.

Svantaggi: la sua principale limitazione è che dipende da una conoscenza predefinita. Inoltre, la rappresentazione simbolica è rigida, e richiede notevoli sforzi nella sua definizione (in termini di simboli da utilizzare e di regole da applicare per la loro manipolazione). Non è particolarmente adattabile o capace di gestire l'incertezza o i contesti ambigui, come quelli che si trovano nel mondo reale.

---

### Approccio sub-simbolico

La conoscenza non è rappresentata da simboli visibili o comprensibili dall'uomo (come "mela", "albero", "rosso"), ma è distribuita attraverso le connessioni tra elementi informativi atomizzati (come i neuroni in un cervello umano).

In altre parole, la conoscenza è codificata in modo implicito attraverso pattern di attivazione. In un cervello, ogni neurone e la sua connessione ad altri neuroni rappresentano in modo molto più astratto la conoscenza.

Una rete neurale "impara" a riconoscere pattern, ma non lo fa in modo esplicito con simboli: non ha un concetto formale di "mela" in termini simbolici, ma riconosce pattern di dati che, per esempio, corrispondono ad una mela in una foto.

https://miro.medium.com/v2/resize:fit:1400/1*q3lZ7tRz1vf48uL6PNmeSg.png

---

### Approccio sub-simbolico

Vantaggi: l'approccio sub-simbolico è molto più performante per compiti percettivi (es. riconoscimento vocale o visivo) in cui è necessario gestire l'incertezza. È molto flessibile e può essere addestrato per adattarsi a nuovi dati senza essere riprogrammato esplicitamente, rendendolo quindi molto più facile da scalare.

Svantaggi: una rete neurale non è facilmente interpretabile, perché non esiste una rappresentazione esplicita e comprensibile per l'uomo di cosa "sa" la rete. Inoltre, l'AI sub-simbolica tendenzialmente richiede enormi quantità di dati e di potenza hardware per allenarsi e può fare errori in scenari non previsti durante l'addestramento.

---

### Esempio di approccio sub-simbolico: Machine learning

IA che impara dai dati e fa previsioni sulla base di quello che ha imparato, in assenza di istruzioni esplicite (cioé simboliche).

https://miro.medium.com/v2/resize:fit:1400/1*uB8f6JncIQwhSVnh5DjiTA.png

---

### Unità della rete neurale: il Percettrone

Le cellule del cervello umano, i neuroni, formano una rete complessa e altamente interconnessa.

Inviano segnali elettrici l'uno all'altro per elaborare informazioni provenienti dal mondo esterno.

https://natureofcode.com/static/472369e80e00d3edb93dae98f30c1ebf/ddecd/10_nn_2.webp

---

### Unità della rete neurale: il Percettrone

Analogamente, una rete neurale artificiale è fatta di neuroni artificiali che prendono dati esterni come input e producono un risultato.

Il modello più semplice è il **percettrone**, proposto da Rosenblatt nel 1958.

https://natureofcode.com/static/cf5195820637396bd5e310f20411a82a/e4512/10_nn_4.webp

---

### Unità della rete neurale: il Percettrone

Un percettrone consiste in:
* Uno o più **input** (dati in entrata);
* Un'**unità di calcolo**;
* Un **output** (dati in uscita).

Il percettrone prende gli input (numeri), li soppesa, somma i risultati e decide se dare come output un 1 o un 0 in base a una soglia predefinita.

https://natureofcode.com/static/cf5195820637396bd5e310f20411a82a/e4512/10_nn_4.webp

---

### Unità della rete neurale: il Percettrone

Ogni dato ha un certo valore numerico.

Il valore di ogni dato di input viene moltiplicato con un **peso** (un altro valore numerico, generalmente tra 0 e 1, che ne rappresenta l'importanza rispetto al risultato finale).

Tutti i valori pesati vengono **sommati** insieme, producendo un unico numero (una somma pesata).

https://www.w3schools.com/ai/img_perceptron.jpg

---

### Unità della rete neurale: il Percettrone

Questa somma pesata viene passata attraverso una **funzione di attivazione**, che decide se il perceptrone si "attiva" (come un neurone che si accende). 

Il percettrone base utilizza una **funzione a gradino**: se la somma è maggiore di una certa soglia, l'output sarà 1 (vero); se è minore della soglia, l'output sarà 0 (falso).

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

Nota ancora più importante: abbiamo completamente ignorato il concetto di **bias**, un aggiustamento che ci permette di spostare la soglia di decisione in maniera più flessibile ed adattabile a seconda della situazione. Nella pratica, si tratta di un altro valore numerico da aggiungere alla somma pesata, per evitare di rimanere limitati alle sole funzioni lineari.

---

### Reti neurali multistrato

Sono composte da gruppi di neuroni artificiali organizzati in livelli. 

Tipicamente sono presenti: 
* un **livello di input**: il punto in cui i dati entrano nel sistema;
* uno o più **livelli intermedi**: strati di neuroni che elaborano i dati in modo complesso;
* un **livello di output**: il risultato finale.

Ogni neurone in un livello fa un calcolo sui dati che riceve e poi decide se attivarsi o meno, sulla base degli elementi che abbiamo già visto.

https://upload.wikimedia.org/wikipedia/commons/thumb/4/46/Colored_neural_network.svg/800px-Colored_neural_network.svg.png

---

### Reti neurali multistrato

Ogni neurone rappresenta una piccola parte di un concetto, un suo **microtratto**. 

Non ha senso guardare un singolo neurone e pensare che rappresenti qualcosa di definito come "gatto", "cane", "mela", "rosso", "peso", "10cm". 

Per esempio, se stiamo cercando di riconoscere una foto di un gatto, un singolo neurone ha il compito di riconoscere la presenza di un angolo, un altro la curvatura di un orecchio, un altro ancora la presenza di linee verticali.

https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Neural-Network-Example-What-Is-A-Neural-Network-Edureka.png

---

### Reti neurali multistrato

I neuroni nei primi strati potrebbero identificare caratteristiche di base come bordi, angoli e forme semplici. 

I neuroni in strati più profondi potrebbero combinare queste informazioni per identificare forme più complesse, come occhi, orecchie o il corpo di un animale. 

Infine, gli strati finali della rete neurale potrebbero combinare tutte queste informazioni per decidere se l'immagine rappresenta un "gatto" o un "cane".

https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2019/08/Neural-Network-Example-What-Is-A-Neural-Network-Edureka.png

---

### Reti neurali multistrato

Anche se noi progettiamo la rete, i neuroni nei layer nascosti non sono "programmati" per compiere operazioni specifiche come accade in un programma tradizionale. 

Invece, attraverso il processo di addestramento, i pesi dei neuroni vengono aggiustati in modo che la rete impari a riconoscere pattern nei dati. 

Ogni neurone nei layer nascosti impara a rappresentare una piccola parte di un concetto. Tuttavia, questi pattern non sono immediatamente interpretabili.

Non sappiamo esattamente cosa ogni neurone sta "vedendo", ma piuttosto possiamo osservare come il risultato finale si adatti correttamente al nostro obiettivo.

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

### Torniamo a parlare di apprendimento

---

### Tipi di ML

L'apprendimento è un processo iterativo che consiste nell'ottimizzazione progressiva dei parametri che definiscono il modello di IA, attraverso la misurazione ciclica dell'errore tra il risultato prodotto e il risultato atteso.

* **Supervisionato**: l'IA viene addestrata su dati preventivamente etichettati da un essere umano;
* **Non supervisionato**: l'IA viene addestrata su dati non etichettati;
* **Per rinforzo**: l'IA apprende sulla base di penalità o ricompense ricevute dall'ambiente in cui si trova ad agire.

---

### Tipi di ML

L'addestramento consiste nel provare, fare errori, e correggerli tramite la **retropropagazione**, un meccanismo per cui la rete regola i vari pesi tra neuroni per migliorare il proprio risultato.

Il training è poi seguito da una fase successiva di testing, in cui la rete svolge l’attività per cui è stata addestrata su nuovi dati che non aveva mai visto prima.

https://www.researchgate.net/publication/354960266/figure/fig1/AS:11431281251915131@1718389091562/The-main-types-of-machine-learning-Main-approaches-include-classification-and-regression.tif

---

### Apprendimento supervisionato

In fase di addestramento della rete, vengono forniti sia i dati su cui allenarsi (es. immagini da classificare a seconda che contengano gatti oppre cani) e la risposta corretta (es. a tutte le immagini di cani è associata l’etichetta "cane"; a tutte le immagini di gatti è associata l’etichetta "gatto").

https://miro.medium.com/v2/1*Iz7bCLrPTImnBDOOEyE3LA.png

---

### Apprendimento non-supervisionato

In fase di apprendimento della rete, vengono forniti solo dati senza la risposta corretta.

L'IA individua da sola regolarità statistiche presenti nei dati (es. la conformazione del muso, la dimensione, i colori, ecc.). 

Sulla base di questo, è possibile creare un insieme di dati (_cluster_) omogeneo contenente le immagini di "cane" e un altro contenente le immagini di "gatto".

https://static.javatpoint.com/tutorial/machine-learning/images/unsupervised-machine-learning-1.png

---

### Apprendimento per rinforzo

In fase di apprendimento, l'IA apprende a compiere delle azioni in un ambiente al fine di massimizzare una ricompensa cumulativa nel tempo.

L'IA esegue azioni e riceve feedback sotto forma di ricompense o penalizzazioni. L'obiettivo dell'agente è imparare a scegliere le azioni che massimizzano la ricompensa complessiva nel lungo periodo.

Una IA impara a giocare a Pokémon: https://www.youtube.com/watch?v=DcYLT37ImBY.

Una IA impara a camminare: https://www.youtube.com/watch?v=L_4BPjLBF4E.

---

### Un'ulteriore categorizzazione: IA discriminativa vs. IA generativa

---

### IA discriminativa

Finalizzata all'analisi delle informazioni ricevute e alla classificazione di tali informazioni in categorie predefinite: “discrimina” i dati secondo alcuni criteri predefiniti. 

Modelli di IA di tipo discriminativo vengono addestrati per distinguere tra categorie di dati (es. come riconoscere immagini di oggetti diversi).

https://vitalflux.com/wp-content/uploads/2023/03/discriminative-modeling-example.png

---

### IA generativa

Finalizzata alla generazione di nuovo contenuto (testi, immagini, musica, video, ecc.) sulla base di determinate informazioni di partenza (_prompt_). 

I modelli di tipo generativo imparano a produrre nuovi dati con caratteristiche simili ai dati originali, utilizzando modelli di apprendimento automatico per identificare i pattern e le relazioni nei dati esistenti.

https://vitalflux.com/wp-content/uploads/2023/03/generative-modeling-example.png

---

### Un esempio ibrido: Generative Adversarial Networks

Un modello che usa due reti diverse: un discriminatore e un generatore.

Durante il training, il discriminatore apprende a riconoscere immagini reali (es. apprendimento non supervisionato o supervisionato per specifiche classi, come i gatti).

Alla fine dell'apprendimento, è in grado di dire se uno stimolo appartiene alla classe di immagini di training (fotografie reali, volti, gatti, etc.) o no.

Il generatore, invece, crea immagini sulla base di dati casuali: inizialmente, le immagini create saranno senza senso.

---

### Un esempio ibrido: Generative Adversarial Networks

L'output del generatore viene dato in pasto al discriminatore, che verifica che i dati prodotti dal generatore siano accettabili rispetto ai dati di addestramento su cui il discriminatore si è allenato.

Se i dati non sono accettabili, il generatore deve correggere i pesi; se invece i dati sono accettabili, il discriminatore è stato "ingannato", e l’immagine è presa come risultato valido.

* https://thispersondoesnotexist.com/
* https://thiscatdoesnotexist.com/

---

### Large Language Model

Un modello di IA generativa basato su reti neurali multistrato e addestrato su enormi quantità di testo per imparare a riconoscere schemi e associazioni propri del linguaggio naturale.

Un utente interroga il modello con un _prompt_ e riceve dal modello una risposta. Sia il prompt che la risposta vengono aggiunti iterativamente ad una "finestra contestuale" che riproduce una forma di "memoria" tenuta dal modello.

https://dx1ienyxpbg1x.cloudfront.net/index_dev/articles/gallery_images/1721733661397675395_3_blob

---

### Large Language Model

Il processo di addestramento di un LLM si divide in due fasi principali:
* **Pre-training**: in questa fase, il modello viene addestrato su un grande corpus di testo per imparare a riconoscere le relazioni tra le parole e tra le frasi;
* **Fine-tuning**: in questa fase, il modello viene addestrato su un nuovo corpus di testo specifico per migliorare la sua capacità di generare testo in un contesto specifico.

https://miro.medium.com/v2/resize:fit:720/format:webp/0*MjVPWxOiEgjK12Be.png

---

### Large Language Model

I pesi delle connessioni tra neuroni che il modello impara durante il processo di addestramento vengono chiamati **parametri**. 

Conme già visto, si tratta di valori numerici che definiscono il comportamento del modello e che il modello stesso ottimizza per affinare la sua capacità di predire o generare output in modo coerente.

---

### Large Language Model

I parametri vengono inizializzati (spesso in modo casuale) e successivamente ottimizzati per riconoscere le relazioni linguistiche generali presenti nei dati (es. prevedere la parola successiva in una frase o per completare una sequenza di testo).

Nel fine-tuning, i parametri già ottimizzati durante il pre-training vengono adattati ulteriormente su un corpus di testo specifico e più mirato.

---

### Large Language Model

Man mano che i parametri aumentano, aumentano le capacità del modello, ma anche le risorse di calcolo richieste. 

Es. l'evoluzione dei modelli GPT per la creazione di testo: 
* GPT-1 ha 117 milioni di parametri;
* GPT2 ne ha 1.5 miliardi;
* GPT3 ne ha 175 miliardi.

---

### Large Language Model

Vantaggi: elevatissima scalabilità e flessibilità; resistenza a informazioni incerte, danneggiate o lacunose.

Svantaggi: performance fortemente influenzata dai dati di addestramento, potenziale presenza di allucinazioni (palesi errori nell'output generato), costi di sviluppo e addestramento elevati (legati alle risorse hardware e alla quantità di dati richieste), mancanza di trasparenza, incertezze legate all'AI Act. 

---

{{< slide background-image="img/0700.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## I problemi

<!--

-->

---

### Uso di dati nella IA

L’IA si basa su **dati storici** e **dati sintetici**.

I dati storici sono raccolti in dataset "reali": le canzoni che ho ascoltato, le temperature raccolte negli ultimi 200 anni, i post su Twitter su un determinato argomento, i testi estratti da articoli di giornale digitalizzati dalla Library of Congress, ecc.

I dati sintetici sono generati da un'altra IA e possono aiutare a rappresentare un problema, se ne danno una rappresentazione affidabile.

---

### IA discriminatoria?

Bias presenti nei dati possono produrre distorsioni nel funzionamento delle IA allenate su questi (es. alcuni sistemi di riconoscimento facciale trattano alcune persone in modo più impreciso rispetto alle altre, sulla base della pigmentazione della pelle o della loro struttura facciale).

https://www.bbc.com/news/technology-68655429

---

### IA e overfitting

Fenomeno che si verifica quando un'IA impara troppo bene i dettagli dei dati di addestramento, al punto da diventare troppo specifico per quel dataset.

Questo significa che, invece di generalizzare e fare previsioni accurate su nuovi dati, il modello diventa "troppo adattato" a quelle specifiche informazioni e quindi perde la capacità di adattamento.

---

### Una minaccia?

* Protezione dei dati?
* Copyright?
* Creazione di monopoli?
* Impatto sul mercato del lavoro?
* Disinformazione?
* Ambiente?

---

### Una minaccia?

L'intelligence sudcoreana ha accusato DeepSeek di raccolta eccessiva dei dati personali della propria utenza, compresi i pattern di input dalla tastiera (che permettono il riconoscimento dell'individuo), e di invio di questi ad altre aziende cinesi.

https://www.reuters.com/technology/artificial-intelligence/south-korea-spy-agency-says-deepseek-excessively-collects-personal-data-2025-02-10/

---

### Una minaccia?

Anthropic viene denunciata da un gruppo di autori per aver allenato i propri LLM su dati testuali, tra cui centinaia di migliaia di libri protetti da copyright. 

https://www.corrierecomunicazioni.it/digital-economy/intelligenza-artificiale-anthropic-denunciata-per-violazione-di-copyright/

---

### Una minaccia?

La stragrande maggioranza di startup di IA è vincolata in esclusiva alle big tech come Amazon, Google e Microsoft, in cambio di finanziamenti ingenti e accesso a enormi risorse di calcolo e dati. 

https://www.tomshw.it/hardware/ia-a-rischio-monopolizzazione-lantitrust-comincia-le-indagini-2025-01-18

---

### Una minaccia?

Bp pianifica di licenziare il 5% della propria forza lavoro (circa 7700 persone) sulla base di valutazioni di ridimensionamento effettuate da una IA.

https://www.wired.it/article/intelligenza-artificiale-licenziamenti-bp-tagli-rinnovabili-investimenti-lavoro/

---

### Una minaccia?

Grok, il chatbot della piattaforma X, permette di generare direttamente in loco testi, immagini e video non sottoposti ad alcun tipo di controllo (eccetto quelli previsti dalla piattaforma stessa).

https://www.franzrusso.it/condividere-comunicare/ia-possibili-rischi-disinformazione-il-caso-grok/

---

### Una minaccia?

In media, ChatGPT consuma 519 millilitri d'acqua per generare un testo di 100 parole.

https://fortune.com/article/how-much-water-does-ai-use/

---

### Questioni etiche

Le IA rischiano di essere:
* Imperscrutabili: non è dato sapere in base a cosa abbiano favorito una decisione;
* Fuorvianti: hanno preso una decisione in base a dati distorti da bias;
* Ingiuste: generano effetti iniqui sulle persone;
* Trasformative: portano a trasformazioni dell'output che minacciano l'autonomia, la privacy o altri diritti individuali;
* Non-tracciabili: difficoltà nel rintracciare la persona o organizzazione responsabile dell'output.

---

### AI Act

Nel 2024, il Parlamento Europeo ha approvato l'AI Act, il primo Regolamento al mondo esplicitamente e totalmente dedicato all'IA.

Il testo contiene norme che disciplinano l'attività delle IA, obbligando le aziende che le sviluppano e distribuiscono al rispetto dei diritti e dei valori fondamentali dell'Unione Europea.

https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R1689

https://artificialintelligenceact.eu/

---

### AI Act

Saranno **vietati** i sistemi di IA che determinano un rischio inaccettabile per la sicurezza, la sussistenza e i diritti delle persone. 

In questa categoria rientrano i sistemi che possono manipolare il comportamento umano (es. _social scoring_ e polizia predittiva).

https://scenarieconomici.it/wp-content/uploads/2021/08/scs5.png

---

### AI Act

Il regolamento considera **ad alto rischio** un numero limitato di sistemi di IA che possono avere ripercussioni negative sulla sicurezza delle persone o sui loro diritti fondamentali (es. identificazione biometrica; riconoscimento delle emozioni; valutazione dell'occupazione; determinare l'accesso a servizi e a prestazioni pubblici e privati essenziali).

Prima di immettere un sistema di IA ad alto rischio sul mercato dell'UE, o di farlo entrare in servizio, i fornitori dovranno sottoporlo, in particolare, a una valutazione.

---

### AI Act

I sistemi di IA **a basso rischio** (come videogiochi o filtri spam) saranno esenti da obblighi, ferma restando l'adesione volontaria a codici di condotta, da parte dei fornitori di tali sistemi, ad esempio laddove esista un evidente rischio di manipolazione. 

Gli utenti dovranno essere consapevoli del fatto che stanno interagendo con una macchina.

---

### IA e cultura

Nell'AI Act europeo, la cultura è espressamente menzionata fra gli ambiti al cui sviluppo l'IA è chiamata a concorrere. 

A livello nazionale si richiamano le potenzialità dell'IA, ma si evidenzia anche come "digitalizzare beni non metadatati e/o descritti sia fortemente sconsigliato".

Vengono ripresi e rivisti concetti fondamentali come l'**originalità** (con ripercussioni anche sul concetto di _bene digitale come replica o copia dell'originale fisico_) e il **copyright**.

---

### IA e cultura

I fornitori dovranno assicurarsi che gli output siano esplicitamente etichettati come prodotti di IA.

I fornitori dovranno pubblicare una descrizione sufficientemente dettagliata dei dati utilizzati per l'addestramento dei propri modelli.

I detentori dei diritti potranno espressamente riservarsi il diritto di utilizzo delle proprie opere (in teoria)... ma come si fa con i modelli già addestrati?

---

# Fine

## Lezione 08 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)