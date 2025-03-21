---
title: ABINF - Internet e World Wide Web
summary: Lezione di "Internet e World Wide Web" del corso di Abilità Informatiche per i Beni Culturali
authors: [Sebastian Barzaghi]
tags: [Digital Humanities]
categories: [Digital Humanities]
date: '2024-01-27T00:00:00Z'
slides:
  theme: white
  highlight_style: github-light

---

# Internet e World Wide Web

## Lezione 05 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)

---

{{< slide background-image="img/0500.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## HTTP

<!--
Photo by <a href="https://unsplash.com/@thisisjlaw?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Justin Lawrence</a> on <a href="https://unsplash.com/photos/cn-tower--Y9XT1-5LL8?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

### Cos'è un protocollo?

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0501.jpg" height="auto" width="200"/>
        <figcaption>
            Fonte: Di <a href="https://unsplash.com/@thealmani?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">almani ماني</a> su <a href="https://unsplash.com/photos/red-stop-light-on-green-background-g6mxlM-h0jQ?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Per comunicare, gli elementi all’interno di un sistema devono seguire regole comuni.
    </p>
    <p>
      Un protocollo è un insieme di regole e di messaggi che governano la comunicazione tra due entità.
    </p>
    <p>
      La definizione di ogni protocollo consiste nel fornire un insieme di regole non ambigue, definendo i messaggi che possono essere scambiati tra entità, il loro significato e le azioni da intraprendere in ogni situazione (es. semaforo).
    </p>
  </div>
</div>

<div class="footer">
An Overview of HTTP. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview">https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview</a>.
</div>

---

### Cos'è un protocollo?

Un protocollo deve essere espresso in un particolare linguaggio, un insieme di segnali e/o simboli comprensibili alle entità al fine di avviare e gestire la comunicazione.

Un linguaggio di questo tipo deve avere:

* Una **sintassi** da seguire per costruire i messaggi;
* Delle regole interpretative del messaggio, per definire la **semantica** dei messaggi;
* Dei **meccanismi per sincronizzare** la comunicazione;
* Dei **meccanismi per correggere e/o gestire** eventuali errori che possono intercorrere nello scambio dei messaggi.

<div class="footer">
An Overview of HTTP. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview">https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview</a>.
</div>

---

### Il protocollo HTTP

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/0502.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.ionos.it/digitalguide/hosting/tecniche-hosting/protocollo-http/">https://www.ionos.it/digitalguide/hosting/tecniche-hosting/protocollo-http/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Protocollo di comunicazione utilizzato per il trasferimento di dati tra un client e un server su una rete.
    </p>
    <p>
      HTTP standardizza come client e server comunicano tramite il metodo richiesta-risposta, in cui il client invia una richiesta al server e il server risponde con una risposta contenente i dati richiesti.
    </p>
  </div>
</div>

<div class="footer">
An Overview of HTTP. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview">https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview</a>.
</div>

---

### Tra client e server esistono _proxy_

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/0503.svg" height="auto" width="700"/>
        <figcaption>
            Fonte: Di H2g2bob - Opera propria basata su: <a href="//commons.wikimedia.org/wiki/File:Proxy_concept_en.svg" title="File:Proxy concept en.svg">Proxy concept en.svg</a>, <a href="http://creativecommons.org/publicdomain/zero/1.0/deed.en" title="Creative Commons Zero, Public Domain Dedication">CC0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=124743074">Collegamento</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Tra il client e il server ci sono numerosi intermediari, collettivamente chiamati <strong>proxy</strong>, che eseguono diverse operazioni per migliorare le prestazioni e la sicurezza (gateway, cache, ecc.).
    </p>
  </div>
</div>

<div class="footer">
An Overview of HTTP. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview">https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview</a>.
</div>

---

### Ricordiamoci che esistono due tipi di messaggi

**Richiesta**: messaggio mandato dal client per richiedere una determinata azione da parte del server;

**Risposta**: messaggio mandato dal server come risposta alla richiesta del client.

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### La struttura di un messaggio secondo HTTP

- Una **testa** composta da:
  * Una **riga iniziale** (di richiesta o di risposta);
  * Un insieme di **intestazioni opzionali** (o header) che specificano la richiesta o descrivono il corpo del messaggio;
- Una **riga vuota** che separa la testa dal corpo del messaggio;
- Un **corpo opzionale** (o body o payload) con il contenuto del messaggio.

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### La struttura di un messaggio HTTP

<figure>
  <img src="img/0504.png" height="auto" width="1000"/>
    <figcaption>
        Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messagesg</a>.
    </figcaption>
</figure>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### La richiesta HTTP

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0505.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview">https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Testa: una riga di richiesta (contenente il <strong>metodo</strong>, il percorso e la versione di HTTP utilizzata) e le intestazioni (headers) contenenti varie informazioni (es. nome del dominio del server, lingua del messaggio, ecc.).
    </p>
    <p>
      Un'eventuale riga vuota (nell'immagine non c'è).
    </p>
    <p>
      Un eventuale corpo (nell'immagine non c'è).
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### Il metodo GET

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      GET /contact HTTP/1.1<br/>
      Host: example.com<br/>
      User-Agent: curl/8.6.0<br/>
      Accept: */*
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      Permette di richiedere informazioni sulla risorsa definita dall’URL specificato.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### Il metodo POST

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      POST /contact HTTP/1.1<br/>
      Host: example.com<br/>
      User-Agent: curl/8.6.0<br/>
      Accept: application/json<br/>
      Content-Type: application/json<br/>
      Content-Length: 74<br/>
      </br>
      {</br>
        "name": "John Doe",<br/>
        "email": "john.doe@example.com",<br/>
        "message": "I'd like to get in touch regarding your services."<br/>
      }
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      POST permette di creare sul server Web la risorsa specificata dall’URL utilizzato e di associare informazioni incluse nella richiesta.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### Il metodo DELETE

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      DELETE /contact/12345 HTTP/1.1</br>
      Host: example.com</br>
      User-Agent: curl/8.6.0</br>
      Accept: application/json</br>
      Authorization: Bearer your-access-token
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      DELETE permette di rimuovere dal server web contattato tutte le informazioni relative alla risorsa specificata nella richiesta tramite l’URL.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### Il metodo PUT

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      PUT /contact/12345 HTTP/1.1</br>
      Host: example.com</br>
      User-Agent: curl/8.6.0</br>
      Accept: application/json</br>
      Content-Type: application/json</br>
      Content-Length: 89</br>
      </br>
      {</br>
        "name": "John Doe",</br>
        "email": "john.doe@example.com",</br>
        "message": "I'd like to update my contact information with new details."</br>
      }
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      PUT permette di specificare informazioni aggiuntive, incluse nella richiesta, ad una risorsa esistente che già risiede sul server.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### La risposta HTTP

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0506.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview">https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Tutte le risposte, oltre che a contenere metadati nell’header (e talvolta dati) nel corpo, specificano anche un codice di stato (un numero di tre cifre che specifica la classe di risposta.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### I codici di stato: 1XX

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      HTTP/1.1 100 Continue</br>
      Date: Sat, 17 Feb 2025 10:52:00 GMT</br>
      Server: Apache/2.4.41 (Unix)</br>
      Content-Length: 0
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      Risposta informativa preliminare o di diagnostica (molto raro, di solito non usato).
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### I codici di stato: 2XX

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      HTTP/1.1 200 OK</br>
      Date: Sat, 17 Feb 2025 10:53:00 GMT</br>
      Server: Apache/2.4.41 (Unix)</br>
      Content-Type: application/json</br>
      Content-Length: 123</br>
      </br>
      {</br>
        "status": "success",</br>
        "message": "Request processed successfully."</br>
      }
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      La richiesta è stata ricevuta, compresa, accettata e elaborata con successo dal server.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

### I codici di stato: 3XX

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      HTTP/1.1 301 Moved Permanently</br>
      Location: https://www.example.com/new-contact</br>
      Date: Sat, 17 Feb 2025 10:55:00 GMT</br>
      Server: Apache/2.4.41 (Unix)</br>
      Content-Length: 0
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      Il client deve effettuare ulteriori azioni per completare la richiesta.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div> 

---

### I codici di stato: 4XX

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      HTTP/1.1 404 Not Found</br>
      Date: Sat, 17 Feb 2025 10:57:00 GMT</br>
      Server: Apache/2.4.41 (Unix)</br>
      Content-Type: application/json</br>
      Content-Length: 85</br>
      </br>
      {</br>
        "status": "error",</br>
        "message": "Not found. The requested resource could not be found on this server."</br>
      }
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      C'è stato un errore che dipende dalla richiesta del client (spesso derivante da errori nell'URL della richiesta).
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div> 

---

### I codici di stato: 5XX

<div style="display: flex; align-items: center;">
  <div style="flex: 1; font-size: 20px; text-align: left;">
    <code>
      HTTP/1.1 500 Internal Server Error</br>
      Date: Sat, 17 Feb 2025 11:00:00 GMT</br>
      Server: Apache/2.4.41 (Unix)</br>
      Content-Type: application/json</br>
      Content-Length: 95</br>
      </br>
      {</br>
        "status": "error",</br>
        "message": "An unexpected error occurred. Please try again later."</br>
      }
    </code>
  </div>
  <div style="flex: 1;">
    <p>
      C'è stato un errore che dipende dal server durante il tentativo di elaborazione della richiesta del client.
    </p>
  </div>
</div>

<div class="footer">
HTTP Messages. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages">https://developer.mozilla.org/en-US/docs/Web/HTTP/Messages</a>.
</div>

---

{{< slide background-image="img/0507.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## Le tecnologie Web

<!--
Photo by <a href="https://unsplash.com/@afgprogrammer?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Mohammad Rahmani</a> on <a href="https://unsplash.com/photos/black-flat-screen-computer-monitor-8qEB0fTe9Vw?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

### Pagine e siti Web

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0508.png" height="auto" width="700"/>
        <figcaption>
            Fonte: Di <a href="https://en.wikipedia.org/wiki/User:Lulzmango" class="extiw" title="en:User:Lulzmango">Lulzmango</a> - <a href="https://en.wikipedia.org/wiki/Web_page" class="extiw" title="en:Web page">en:Web_page</a>, <a href="https://creativecommons.org/licenses/by-sa/4.0" title="Creative Commons Attribution-Share Alike 4.0">CC BY-SA 4.0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=16944315">Link</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Una pagina Web è un documento ipertestuale pubblicato sul World Wide Web e visualizzato dall’utente tramite un client (browser, app, ecc.).
    </p>
    <p>
      Quindi, un sito Web consiste in un insieme di pagine Web (più altri file correlati) che il client richiede ad uno o più server per elaborarli e generarne la visualizzazione sullo schermo del dispositivo.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### La marcatura del testo

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/0512.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://basic-inf.github.io/2024-2025/chapters/08.pdf">https://basic-inf.github.io/2024-2025/chapters/08.pdf</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Annotazione del testo per definire esplicitamente i ruoli strutturali e semantici delle parti di cui è costituito.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### La marcatura del testo

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/0513.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://basic-inf.github.io/2024-2025/chapters/08.pdf">https://basic-inf.github.io/2024-2025/chapters/08.pdf</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      La marcatura trasforma il testo in una struttura ad albero.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### La marcatura del testo

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/0516.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Diversi linguaggi di marcatura (es. SGML, XML).
    </p>
    <p>
      Metalinguaggi che definiscono regole sintattiche per specificare la marcatura, ma non impongono alcun vocabolario.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### La marcatura: l'elemento

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/0514.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://basic-inf.github.io/2024-2025/chapters/08.pdf">https://basic-inf.github.io/2024-2025/chapters/08.pdf</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Termine informativo che esprime la semantica della porzione di testo a cui si riferisce.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### La marcatura: l'attributo

<div style="display: flex; align-items: center;">
  <div style="flex: 2;">
    <figure>
      <img src="img/0515.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://basic-inf.github.io/2024-2025/chapters/08.pdf">https://basic-inf.github.io/2024-2025/chapters/08.pdf</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Informazione aggiuntiva che si riferisce all’elemento a cui viene assegnata, sotto forma di coppia chiave-valore inserita nel marcatore di apertura.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### Marcatura di un pezzo di testo: esempio

```
<book language="english">  
  <chapter>  
    <paragraph>  
      Alice was beginning to get very tired of sitting by her  
      sister on the bank, and of having nothing to do: once or  
      twice she had peeped into the book her sister was  
      reading, but it had no pictures or conversations in it,  
      <quotation>“and what is the use of a book,”</quotation>  
      thought Alice, <quotation>“without pictures or  
      conversations?”</quotation>  
    </paragraph>  
  </chapter>  
</book>  
```

<div class="footer">
How the web works. In MDN Web Docs.   
 <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

### Introduzione a HTML

Linguaggio che segue una sintassi simile a XML e che inoltre utilizza uno specifico vocabolario costituito da elementi ed attributi per identificare i vari ruoli strutturali e semantici di una pagina Web.

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### HTML può essere semplicissimo

<figure>
  <img src="img/0517.png" height="auto" width="700"/>
    <figcaption>
        Fonte: <a href="https://www.w3schools.com/html/html_editors.asp">https://www.w3schools.com/html/html_editors.asp</a>.
    </figcaption>
</figure>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### HTML può essere semplicissimo

<figure>
  <img src="img/0518.png" height="auto" width="700"/>
    <figcaption>
        Fonte: <a href="https://www.w3schools.com/html/html_editors.asp">https://www.w3schools.com/html/html_editors.asp</a>.
    </figcaption>
</figure>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### Struttura base di un documento HTML

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0519.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.codewithharry.com/tutorial/html-page-structure/">https://www.codewithharry.com/tutorial/html-page-structure/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      <code>!DOCTYPE</code>: informazione per il client riguardante il tipo di documento che si deve aspettare
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### Struttura base di un documento HTML

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0519.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.codewithharry.com/tutorial/html-page-structure/">https://www.codewithharry.com/tutorial/html-page-structure/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      <code>html</code>: inizio e fine del documento HTML.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### Struttura base di un documento HTML

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0519.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.codewithharry.com/tutorial/html-page-structure/">https://www.codewithharry.com/tutorial/html-page-structure/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      <code>head</code>: sezione di intestazione del documento, contenente metadati e altre informazioni tecniche (invisibile all'utente).
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### Struttura base di un documento HTML

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0519.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.codewithharry.com/tutorial/html-page-structure/">https://www.codewithharry.com/tutorial/html-page-structure/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      <code>body</code>: sezione di contenuto del documento, contenente titoli, paragrafi, immagini, video, ecc. (tutto ciò che è visibile all'utente).
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### Cascading Style Sheets

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0510.svg" height="auto" width="200"/>
        <figcaption>
            Fonte: Di Rudloff - <a href="//commons.wikimedia.org/wiki/File:CSS3_and_HTML5_logos_and_wordmarks.svg" title="File:CSS3 and HTML5 logos and wordmarks.svg">CSS3 and HTML5 logos and wordmarks.svg</a>, <a href="https://creativecommons.org/licenses/by/3.0" title="Creative Commons Attribution 3.0">CC BY 3.0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=49121103">Link</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Linguaggio per definire lo stile delle pagine Web.
    </p>
    <p>
      Separazione tra contenuto e la sua rappresentazione: <a href="https://csszengarden.com/">https://csszengarden.com/</a>.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

### JavaScript

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0511.png" height="auto" width="200"/>
        <figcaption>
            Fonte: Di JavaScript Corp. - The JavaScript foundation, <a href="https://creativecommons.org/licenses/by-sa/4.0" title="Creative Commons Attribution-Share Alike 4.0">CC BY-SA 4.0</a>, <a href="https://commons.wikimedia.org/w/index.php?curid=103235118">Link</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Linguaggio di programmazione usato per aggiungere interattività alle pagine Web.
    </p>
    <p>
      Esecuzione di determinate azioni in seguito allo scatenarsi di specifici eventi.
    </p>
  </div>
</div>

<div class="footer">
Introduction to HTML. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML">https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML</a>.
</div>

---

{{< slide background-image="img/0520.jpg" class="section-slide">}}

<div class="dark-overlay"></div>

## Le tecnologie di rete

<!--
Photo by <a href="https://unsplash.com/@alinnnaaaa?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Alina Grubnyak</a> on <a href="https://unsplash.com/photos/low-angle-photography-of-metal-structure-ZiQkhI7417A?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
-->

---

### Come fa il client a trovare il server?

URL e HTTP forniscono le istruzioni necessarie ad ottenere una rappresentazione della risorsa cercata (ovvero, una copia della pagina HTML che visualizziamo).

Prendiamo un URL come questo: `http://<dominio>/<percorso>?<parametri>#<ancora>`:
* Il client richiede al server `/<percorso>?<parametri>#<ancora>`;
* Il server restituisce un messaggio con la copia della risorsa richiesta.

Ma manca il punto 1:
* Il client cerca uno degli indirizzi IP del dominio usando il DNS.

<div class="footer">
IP Address. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Glossary/IP_Address">https://developer.mozilla.org/en-US/docs/Glossary/IP_Address</a>.
</div>

---

### L'indirizzo IP

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0521.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.giovannicirillo.it/definizione-indirizzo-ip/">https://www.giovannicirillo.it/definizione-indirizzo-ip/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
    Pur usando l’URL per accedere ad una risorsa, in realtà il server web che la ospita non è direttamente raggiungibile usando il suo nome ma attraverso un indirizzo specifico.
    </p>
    <p>
    Un indirizzo IP è un identificativo numerico assegnato a ogni dispositivo connesso a Internet.
    </p>
  </div>
</div>

<div class="footer">
IP Address. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Glossary/IP_Address">https://developer.mozilla.org/en-US/docs/Glossary/IP_Address</a>.
</div>

---

### L'indirizzo IP

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0521.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.giovannicirillo.it/definizione-indirizzo-ip/">https://www.giovannicirillo.it/definizione-indirizzo-ip/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Una serie di numeri separati da punti, utilizzata per instradare il traffico di rete tra i dispositivi.
    </p>
    <p>
      Essenziali per la comunicazione su Internet, poiché consentono ai dispositivi di identificarsi e di scambiarsi informazioni tra di loro.
    </p>
  </div>
</div>

<div class="footer">
IP Address. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Glossary/IP_Address">https://developer.mozilla.org/en-US/docs/Glossary/IP_Address</a>.
</div>

---

### Il Domain Name System

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0522.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.geeksforgeeks.org/working-of-domain-name-system-dns-server/">https://www.geeksforgeeks.org/working-of-domain-name-system-dns-server/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Quando un utente inserisce un URL o clicca su un link, il browser deve scoprire l'indirizzo IP associato a quel dominio per stabilire una connessione.
    </p>
    <p>
      Il DNS è un sistema di nomenclatura utilizzato per tradurre i nomi di dominio degli indirizzi Web in indirizzi IP numerici.
    </p>
  </div>
</div>

<div class="footer">
DNS. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Glossary/DNS">https://developer.mozilla.org/en-US/docs/Glossary/DNS</a>.
</div>

---

### Il Domain Name System

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0522.png" height="auto" width="700"/>
        <figcaption>
            Fonte: <a href="https://www.geeksforgeeks.org/working-of-domain-name-system-dns-server/">https://www.geeksforgeeks.org/working-of-domain-name-system-dns-server/</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      In pratica, è come un elenco telefonico per Internet, dove i nomi di dominio come "google.com" vengono tradotti in indirizzi IP numerici come "172.217.168.78" che i computer possono usare per connettersi ai server Web corrispondenti.
    <p>
      Permette agli utenti di trovare i siti web desiderati utilizzando nomi di dominio, invece di usare gli indirizzi IP numerici.
    </p>
  </div>
</div>

<div class="footer">
DNS. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Glossary/DNS">https://developer.mozilla.org/en-US/docs/Glossary/DNS</a>.
</div>

---

### Il Transmission Control Protocol

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0523.png" height="auto" width="300"/>
        <figcaption>
            Fonte: <a href="https://basic-inf.github.io/2024-2025/chapters/06.pdf">https://basic-inf.github.io/2024-2025/chapters/06.pdf</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Un protocollo che garantisce una trasmissione affidabile dei dati attraverso una rete.
    <p>
      Basato sulla commutazione di pacchetto: suddivisione dei dati in pacchetti, aggiunta di un'intestazione che contiene informazioni sui dati, e garanzia che i pacchetti siano consegnati senza errori e nell'ordine corretto.
    </p>
  </div>
</div>

<div class="footer">
TCP. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Glossary/TCP">https://developer.mozilla.org/en-US/docs/Glossary/TCP</a>.
</div>

---

### Il Transmission Control Protocol

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0523.png" height="auto" width="300"/>
        <figcaption>
            Fonte: <a href="https://basic-inf.github.io/2024-2025/chapters/06.pdf">https://basic-inf.github.io/2024-2025/chapters/06.pdf</a>.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Gli indirizzi IP vengono utilizzati per instradare i pacchetti di dati attraverso la rete da un dispositivo all’altro.
    <p>
      Insieme, TCP e IP costituiscono il protocollo TCP/IP, che è diventato lo standard de facto per la comunicazione di rete su Internet.
    </p>
  </div>
</div>

<div class="footer">
TCP. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Glossary/TCP">https://developer.mozilla.org/en-US/docs/Glossary/TCP</a>.
</div>

---

## Ricapitolando

---

### Il Web è una strada, e noi dobbiamo andare ad un negozio

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0524.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Ad un’estremità c’è il client (casa), all’altra il server (un negozio).
    <p>
      Durante la navigazione tramite browser, digitare un URL o cliccare su un link equivale a camminare dalla casa verso il negozio.
    </p>
  </div>
</div>

<div class="footer">
How the web works. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

### Chiediamo l'indirizzo

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0525.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Il browser si collega al server DNS e trova l'indirizzo reale del server su cui risiede il sito Web.
    </p>
    <p>
      In pratica, cerchiamo e troviamo l'indirizzo del negozio.
    </p>
  </div>
</div>

<div class="footer">
How the web works. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

### Troviamo l'indirizzo

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0526.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Il browser si collega al server DNS e trova l'indirizzo reale del server su cui risiede il sito Web.
    </p>
    <p>
      In pratica, cerchiamo e troviamo l'indirizzo del negozio.
    </p>
  </div>
</div>

<div class="footer">
How the web works. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

### Trovato il negozio, facciamo il nostro ordine

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0527.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      l browser invia un messaggio di richiesta HTTP al server, chiedendogli di inviare una copia del sito Web al client.
    </p>
    <p>
      In pratica, una volta arrivati al negozio, ordiniamo quello che ci serve.
    </p>
  </div>
</div>

<div class="footer">
How the web works. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

### Il nostro ordine va a buon fine e ci vengono consegnati i prodotti

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0528.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Se il server approva la richiesta del client, invia al client un messaggio "200 OK", che significa "Certo, puoi guardare quel sito web! Eccolo qui", e inizia quindi a inviare i file del sito Web al browser sotto forma di pacchetti di dati.
    </p>
    <p>
      In pratica, il negozio ci consegna i prodotti che abbiamo ordinato, e noi li riportiamo a casa.
    </p>
  </div>
</div>

<div class="footer">
How the web works. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

### Durante tutto questo

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0529.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Il messaggio e tutti i dati in esso contenuti, inviati tra il client e il server, vengono trasmessi attraverso la connessione Internet utilizzando il protocollo TCP/IP.
    </p>
  </div>
</div>

<div class="footer">
How the web works. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

### Infine, ritorniamo a casa

<div style="display: flex; align-items: center;">
  <div style="flex: 1;">
    <figure>
      <img src="img/0530.png" height="auto" width="700"/>
        <figcaption>
            Fonte: propria.
        </figcaption>
    </figure>
  </div>
  <div style="flex: 1;">
    <p>
      Il browser assembla i pacchetti in una pagina Web completa e la visualizza a schermo.
    </p>
    <p>
      In pratica, ritorni a casa con i prodotti in mano, pronti per essere usati.
    </p>
  </div>
</div>

<div class="footer">
How the web works. In MDN Web Docs. <a href="https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works">https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works</a>.
</div>

---

# Fine

## Lezione 05 del corso di _Abilità Informatiche_ (2024/2025)

###### Sebastian Barzaghi | [sebastian.barzaghi2@unibo.it](mailto:sebastian.barzaghi2@unibo.it) | [https://orcid.org/0000-0002-0799-1527](https://orcid.org/0000-0002-0799-1527) | [https://www.unibo.it/sitoweb/sebastian.barzaghi2/](https://www.unibo.it/sitoweb/sebastian.barzaghi2/)