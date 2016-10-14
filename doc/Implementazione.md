# Case Arduino, implementazione

1. [Introduzione](#introduzione)

  - [Informazioni sul progetto](#informazioni-sul-progetto)

  - [Scopo](#scopo)

1. [Implementazione](#implementazione)

1. [Test](#test)

  - [Protocollo di test](#protocollo-di-test)

  - [Risultati test](#risultati-test)

  - [Mancanze/limitazioni conosciute](#mancanze/limitazioni-conosciute)

1. [Consuntivo](#consuntivo)

1. [Conclusioni](#conclusioni)

  - [Sviluppi futuri](#sviluppi-futuri)

  - [Considerazioni personali](#considerazioni-personali)

1. [Sitografia](#sitografia)

1. [Allegati](#allegati)



## Introduzione

### Informazioni sul progetto

  Progetto: Case per Arduino

  Allievo: Jonathan Fassora

  Docenti: Adriano Barchi, Luca Muggiasca

  Scuola Arti e Mestieri Trevano, Informatica, Modulo 306 + progetti

  Inizio: 09.09.2016

  Consegna: 21.10.2016

## Implementazione

### Taglio del legno
Per fare il taglio del legno ho disegnato le parti del case direttamente sul compensato a misura giusta. Al momento del taglio ho lasciato un margine che sono poi andato a rifinire con la carta vetrata per una maggiore precisione. Per praticare i buchi necessari (sul fronte 2 prese, sul coperchio fori per i cavi) ho sfruttato un trapano per inserire la lama del traforo e tagliare "dall'interno".
### Assemblaggio
Una volta ricavati i pezzi (coperchio, fronte, retro, doppia base) ho assemblato il case. Per fare ciò ho prima di tutto incollato la doppia base (utilizzando la colla calda) e in seguito le pareti, attaccandole ai 'lati' della base (vedi disegno progettazione), tutto sempre con la colla calda. L'attacco del coperchio verrà invece fatto in un secondo momento.
### Fissaggio Arduino
Per fissare l'arduino, ma dare sempre la possibilità di attaccare o staccare la scheda, ho sfruttato delle viti con dado. Per prima cosa ho indicato sulla base i punti in cui l'arduino si andrà a fissare, in seguito ho fatto dei fori con il trapano a misura delle viti. In questo modo per togliere l'arduino sarebbe bastato svitare la vite rispettivamente il dado. Ho però incontrato il problema della lunghezza delle viti, non sufficiente a fissare l'arduino (avevo a disposizione quelle da 1 cm, considerando la base di 8mm, l'arduino e l'agio da lasciare per il dado).<br>
Per risolvere ho dunque utilizzato il trapano, con una punta a dimensione del bullone, sul fondo della base per creare un'invasatura che permettesse di inserire ed incastrare il dado nel legno. In questo modo si può avvitare e svitare la vite senza problemi in quanto il bullone è fisso in fondo, e soprattutto viene risolto il problema della lunghezza, in quanto la vita penetra più a fondo e permette effettivamente di fissare il tutto.<br>
### Chiusura
Per permettere una chiusura solida ma non troppo macchinosa ho utilizzato dei ganci per appendere quadri. Ho dunque fissato uno di questi ganci al coperchio tramite 2 chiodi e un po' di colla (facendo attenzione a fissarlo sulla parte inferiore dello stesso, altrimenti non arriverebbe al chiodo cui 'appendersi'), in seguito (valutando dove arrivava il gancio) ho inserito un chiodo su cui il gancio andrà appunto a chiudere il case.<br>
Per attaccare il coperchio invece ho semplicemente usato diverse strisce di nastro da hockey in direzioni incrociate in modo da ottenere un'attaccatura solida.
### Rivestimento
In conclusione ho coperto, in varie direzioni, tutto il case con il nastro da hockey, con particolare attenzione per gli spigoli, per i 2 punti in cui si attacca il coperchio (dunque la 'cerniera' di nastro e il gancio che chiude), e soprattutto per i 4 punti in cui i bulloni sono incastrati.

## Test

### Protocollo di test

|Test Case      | TC-001                               |
|---------------|--------------------------------------|
|**Nome**       | |
|**Riferimento**| REQ-002                               |
|**Descrizione**| Collegamento dei cavi tramite i fori |
|**Prerequisiti**| - |
|**Procedura**     |  |
|**Risultati attesi** | L'arduino si collega senza problemi ai componenti passando per i fori nel coperchio. |


### Risultati test

|Test Case      | Risultato                             |
|---------------|---------------------------------------|
| TC-001        | Passato/Non passato                   |
| TC-002        | Passato/Non passato                   |

### Mancanze/limitazioni conosciute

Descrizione con motivazione di eventuali elementi mancanti o non
completamente implementati, al di fuori dei test case. Non devono essere
riportati gli errori e i problemi riscontrati e poi risolti durante il
progetto.

## Consuntivo

Consuntivo del tempo di lavoro effettivo e considerazioni riguardo le
differenze rispetto alla pianificazione (cap 1.7) (ad esempio Gannt
consuntivo).

## Conclusioni

Quali sono le implicazioni della mia soluzione? Che impatto avrà?
Cambierà il mondo? È un successo importante? È solo un’aggiunta
marginale o è semplicemente servita per scoprire che questo percorso è
stato una perdita di tempo? I risultati ottenuti sono generali,
facilmente generalizzabili o sono specifici di un caso particolare? ecc

### Sviluppi futuri
  Migliorie o estensioni che possono essere sviluppate sul prodotto.

### Considerazioni personali
  Cosa ho imparato in questo progetto? ecc

## Bibliografia

### Bibliografia per articoli di riviste

-

### Bibliografia per libri

-

### Sitografia

-

## Allegati

Elenco degli allegati, esempio:

-   Diari di lavoro

-   Codici sorgente/documentazione macchine virtuali

-   Istruzioni di installazione del prodotto (con credenziali
    di accesso) e/o di eventuali prodotti terzi

-   Documentazione di prodotti di terzi

-   Eventuali guide utente / Manuali di utilizzo

-   Mandato e/o Qdc

-   Prodotto

-   …
