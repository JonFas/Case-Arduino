# Case Arduino, progettazione

1. [Introduzione](#introduzione)

  - [Informazioni sul progetto](#informazioni-sul-progetto)

  - [Abstract](#abstract)

  - [Scopo](#scopo)

1. [Analisi](#analisi)

  - [Analisi del dominio](#analisi-del-dominio)

  - [Analisi e specifica dei requisiti](#analisi-e-specifica-dei-requisiti)

1. [Use case](#use-case)

  - [Pianificazione](#pianificazione)

  - [Analisi dei mezzi](#analisi-dei-mezzi)

1. [Progettazione](#progettazione)

  - [Design dell’architettura del sistema](#design-dell’architettura-del-sistema)

  - [Design dei dati e database](#design-dei-dati-e-database)



## Introduzione

### Informazioni sul progetto

  Progetto: Case per Arduino

  Allievo: Jonathan Fassora

  Docenti: Adriano Barchi, Luca Muggiasca

  Scuola Arti e Mestieri Trevano, Informatica, Modulo 306 + progetti

  Inizio: 09.09.2016

  Consegna: 21.10.2016

### Abstract

  > *Since the Arduino is a quite fragile item, it can be risky to bring it around. Considering this the request was to design and build a protective case in which the board would be protected while still being usable (connecting cables, resetting). In this document you'll find an explanation of the idea behind the creation of this case, and in the other document ('Implementazione.md') you'll find how to build it.*

### Scopo

  Lo scopo di questo progetto è principalmente didattico, si tratta di insegnare come costruire un progetto, dalla richiesta del cliente fino alla consegna allo stesso, passando per analisi, pianificazione, documentazione, metodi di lavoro,...
  L'obiettivo invece più 'fisico' di questo lavoro è creare un case che possa proteggere l'Arduino permettendone comunque l'uso (quindi non limitandosi a una semplice scatola di legno).

## Analisi

### Analisi del dominio

  Nella situazione attuale qualunqe lavoro su Arduino viene generalmente trasportato portandosi appresso la bread board e con la scheda 'penzolante', o se proprio nella scatola del kit, sperando che non si stacchi nulla o, soprattutto, che non cada. Tramite questo piccolo progetto (e il suo 'compagno', l'holder) si vuole dunque evitare questo genere di problemi, con il case in particolare si dovrebbe riuscire a trasportare la scheda dell'Arduino in modo più sicuro, essendo comunque uno strumento piuttosto fragile.

  Esistono chiaramente prodotti affini e fabbricati con precisione assoluta, fatti apposta per ogni singolo modello. Come già detto questo progetto è a scopo didattico, dunque non è necessariamente un problema creare un prodotto che non è 'all'altezza' di ciò che si trova sul mercato, e comunque il suo lavoro lo farà lo stesso.

  In conclusione quindi si dovrebbe arrivare a un oggetto creato per scopi scolastici e che possa essere sfruttato, entro i suoi limiti, nella ambito scolastico stesso.

### Analisi e specifica dei requisiti

|ID  |REQ-001                                         |
|----|------------------------------------------------|
|**Nome**    | Realizzazione case per Arduino |
|**Priorità** | 1                     |
|**Versione** | 1.0                   |
|**Note**    |-|
|**Sub-ID**            |**Sotto requisiti** |
|**001**      | Il case dev'essere di compensato, il materiale di fissaggio è a scelta |
|**002**      | Si dovrà poter accedere a USB e alimentazione con il case chiuso    |

<hr>

|ID  |REQ-002                                         |
|----|------------------------------------------------|
|**Nome**    | Fori per collegamenti ai pin |
|**Priorità** | 1                     |
|**Versione** | 1.0                   |
|**Note**    |-|
|**Sub-ID**            |**Sotto requisiti** |
|**001**      | Il case dovrà avere almeno un foro da cui possano passare i fili collegati ai vari pin quando il case è chiuso |
|**002**      | Se ci fosse la possibilità, potrà esserci un foro più ampio che permetta di collegare i suddetti fili mentre il case è chiuso |

<hr>

|ID  |REQ-003                                         |
|----|------------------------------------------------|
|**Nome**    | Chiusura |
|**Priorità** | 1                     |
|**Versione** | 1.0                   |
|**Note**    |-|
|**Sub-ID**            |**Sotto requisiti** |
|**001**      | Il case dovrà essere chiuso in modo solido, il coperchio dovrà quindi fissarsi al case al momento della chiusura. |
|**002**      | A dipendenza del tipo di chiusura, il coperchio potrà essere sempre attaccato al case o meno. |

<hr>

|ID  |REQ-004                                         |
|----|------------------------------------------------|
|**Nome**    | Fissaggio dell'Arduino |
|**Priorità** | 1                     |
|**Versione** | 1.0                   |
|**Note**    |-|
|**Sub-ID**            |**Sotto requisiti** |
|**001**      | L'Arduino dovrà posarsi nel case senza muoversi eccessivamente |
|**002**      | Dovrà di conseguenza essere fissato, in quanto una struttura ad incastro risulterebbe troppo complicata da realizzare |

<hr>

|ID  |REQ-005                                         |
|----|------------------------------------------------|
|**Nome**    | Resistenza del case |
|**Priorità** | 1                     |
|**Versione** | 1.0                   |
|**Note**    |-|
|**Sub-ID**            |**Sotto requisiti** |
|**001**      | Il case dovrà resistere dei colpi che potrebbe ricevere in un uso comune |
|**002**      | Dovrà dunque resistere piccole cadute (1 m circa) e qualche colpo (come all'interno di uno zaino) |
|**003**      | La resistenza nel tempo è relativa alla resistenza del compensato e del materiale di fissaggio scelto |

<hr>

|ID  |REQ-006                                         |
|----|------------------------------------------------|
|**Nome**    | Aerazione |
|**Priorità** | 1                     |
|**Versione** | 1.0                   |
|**Note**    |-|
|**Sub-ID**            |**Sotto requisiti** |
|**001**      | Il case dovrà avere delle uscite per il calore |


### Pianificazione

![alt text](Allegati_Immagini/gantt.png "Gantt")

### Analisi dei mezzi

  Per realizzare questo progetto abbiamo a disposizione l'Arduino (versione UNO RoboTale) e l'officina con tutti gli utensili necessari alla costruzione di lavori in legno (martelli, pinze, cacciaviti, trafori, ...).

## Progettazione

### Preparazione e prezzi

| Componente  | Quantità | Prezzo |
|:----:|:------:|----:|
| Compensato | ~ foglio A4 | ~0,50 CHF (~7 CHF/m<sup>2</sup>) |
| Nastro da hockey | 2 metri | 14,90 CHF (1 rotolo) |
| Viti 3x10 mm | 4 | 2,95 CHF (1 scatola) |
| Dadi autobloccanti | 4 | 1,95 CHF (1 scatola) |
| Gancio appendi-quadri + chiodini | 1 | 2,95 CHF (1 scatola) |

| | | |
|--|--|--|
| Lavoro | 36 h | 50 CHF/h |

### Design e progettazione
<hr>
 1. Taglio del legno;
 2. Rifinitura con carta vetrata;
 3. Assemblaggio del case tramite la colla per il legno o la colla calda (specificato più sotto);
 4. Rifinitura con carta vetrata, in particolare livellamento della parte in cui il coperchio si andrà ad appoggiare e della base doppia;
 5. Inserimento del chiodo d'aggancio;
 6. Posizionamento del gancio;
 7. Posizionamento del Coperchio;
 8. Rivestimento con il nastro da hockey e conseguente fissatura di gancio e coperchio (specificato più sotto)
  - **Attenzione**: Evitare di rivestire le parti interne e i fori per le prese, in quanto essendo fatti su misura, si rischia di impedire o rendere difficile l'inserimento dell'Arduino stesso.

<hr>
<center>***Misure in cm.***</center>
<hr>
<img src="Allegati_Immagini/Disegni/misura1.JPG" alt="Coperchio" style="width:49%;"/>
<img src="Allegati_Immagini/Disegni/misura2.JPG" alt="Base" style="width:49%;"/>
***Nota***: La base è doppia, questo perché tutta la struttura si attacca ai lati della stessa, di conseguenza è meglio avere una superficie maggiore su cui incollare.<br>
<img src="Allegati_Immagini/Disegni/misura3.JPG" alt="Retro" style="width:49%;"/>
<img src="Allegati_Immagini/Disegni/misura4.JPG" alt="Parete" style="width:49%;"/>
<img src="Allegati_Immagini/Disegni/misura5.JPG" alt="Fronte" style="width:49%;"/>
<hr>
Una volta ottenuti i pezzi, essi vanno assemblati sui lati della base.
<img src="Allegati_Immagini/Disegni/Attaccatura.png" alt="Attaccatura" style="width:49%"/>
<hr>
Sul retro del case, la chiusura avviene tramite il rivestimento con il nastro da hockey. Durante questa fase è necessario dare particolare attenzione a questa zona, facendo anche diversi giri più e più volte, per rendere la chiusura più solida. (La mobilità non ne risentirà in quanto si tratta praticamente di stoffa adesiva).

Sul fronte, invece, va inserito un chiodino che servira da aggancio per il triangolo. Il gancio stesso va attaccato in maniera analoga alla chiusura posteriore, ovvero durante la fase di rivestimento con il nastro. Anche qui fare diversi giri per assicurarsi che il gancio rimanga fermo.
<br>
<img src="Allegati_Immagini/Disegni/Chiusura_dietro.png" alt="Chiusura dietro" style="width:49%"/>
<img src="Allegati_Immagini/Disegni/Gancio.JPG" alt="Chiusura davanti" style="width:49%"/>
<hr>
