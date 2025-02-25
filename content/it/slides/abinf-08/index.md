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

Questo premio/punizione può riferirsi a una catena complessa di azioni svolte dalla macchina, a volte in tempi diversi (es. scacchi), o ad azioni semplici.

---

### IA discriminativa

Finalizzata all'analisi delle informazioni ricevute e alla classificazione di tali informazioni in categorie predefinite: “discrimina” i dati secondo alcuni criteri predefiniti. 

Modelli di IA di tipo discriminativo vengono addestrati per distinguere tra categorie di dati (es. come riconoscere immagini di oggetti diversi).

I modelli apprendono una funzione matematica in grado di separare i dati.

https://vitalflux.com/wp-content/uploads/2023/03/discriminative-modeling-example.png

---

### IA generativa

Finalizzata alla generazione di nuovo contenuto (testi, disegni, immagini, ecc.) sulla base di determinate informazioni di partenza (PROMPT). 

I modelli di tipo generativo imparano a produrre nuovi dati con caratteristiche simili ai dati originali (ad es. come produrre testi o immagini di un certo tipo), utilizzando modelli di apprendimento automatico per identificare i pattern e le relazioni nei dati esistenti.

I modelli apprendono una funzione matematica che rappresenta la distribuzione di probabilità dei dati.

https://vitalflux.com/wp-content/uploads/2023/03/generative-modeling-example.png

---

### Un esempio ibrido: Generative Adversarial Networks

Un modello che usa due reti diverse: un discriminatore e un generatore.

Durante il training, il discriminatore apprende a riconoscere immagini reali (es. apprendimento non supervisionato o supervisionato per specifiche classi, come i gatti).

Alla fine dell'apprendimento, è in grado di dire se uno stimolo appartiene alla classe di immagini di training (fotografie reali, volti, gatti, etc.) o no.

---

### Un esempio ibrido: Generative Adversarial Networks

Il generatore, invece, crea immagini sulla base di dati casuali: inizialmente, le immagini create saranno senza senso.

L'output del generatore viene dato in pasto al discriminatore, che verifica che i dati prodotti dal generatore siano accettabili rispetto ai dati di addestramento su cui il discriminatore si è allenato.

Se i dati non sono accettabili, il generatore deve correggere i pesi; se invece i dati sono accettabili, il discriminatore è stato "ingannato", e l’immagine è presa come risultato valido.

---

### Un esempio ibrido: Generative Adversarial Networks

* https://thispersondoesnotexist.com/
* https://thiscatdoesnotexist.com/

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

## Lezione 08 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)