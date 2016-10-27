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

<i>Nota: </i>l'arduino è stato fissato solo tramite i 2 fori 'posteriori', questo perché la larghezza dei fori davanti non è sufficiente per inserire la testa delle viti usate. È comunque più che abbastanza utilizzarne 2 per questo scopo.
### Chiusura
Per permettere una chiusura solida ma non troppo macchinosa ho utilizzato dei ganci per appendere quadri. Ho dunque fissato uno di questi ganci al coperchio tramite 2 chiodi e un po' di colla (facendo attenzione a fissarlo sulla parte inferiore dello stesso, altrimenti non arriverebbe al chiodo cui 'appendersi'), in seguito (valutando dove arrivava il gancio) ho inserito un chiodo su cui il gancio andrà appunto a chiudere il case.<br>
Per attaccare il coperchio invece ho semplicemente usato diverse strisce di nastro da hockey in direzioni incrociate in modo da ottenere un'attaccatura solida.
### Rivestimento
In conclusione ho coperto, in varie direzioni, tutto il case con il nastro da hockey, con particolare attenzione per gli spigoli, per i 2 punti in cui si attacca il coperchio (dunque la 'cerniera' di nastro e il gancio che chiude), e soprattutto per i 4 punti in cui i bulloni sono incastrati.

## Test

### Protocollo di test

|Test Case      | TC-001                               |
|---------------|--------------------------------------|
|**Nome**       | Collegamenti |
|**Riferimento**| REQ-002                               |
|**Descrizione**| Verificare che i cavi stiano collegati tramite i fori. |
|**Prerequisiti**| - |
|**Procedura**     | Con l'Arduino fuori dal case, collegare alcuni cavi di test. Fatto questo inserire la scheda nel case e fissarla tramite le apposite viti. Chiudere il coperchio. |
|**Risultati attesi** | L'arduino si collega senza problemi all'esterno passando per i fori nel coperchio. |
<hr>

|Test Case      | TC-002                               |
|---------------|--------------------------------------|
|**Nome**       | CHiusura |
|**Riferimento**| REQ-003                               |
|**Descrizione**| Verificare la solidità della chiusura. |
|**Prerequisiti**| - |
|**Procedura**     | Chiudere il coperchio e abbassare il gancio per quadri sul chiodo. Fatto questo provare a rivoltare al contrario il case e verificare che non si apra. |
|**Risultati attesi** | Il case rimane chiuso. |
<hr>

|Test Case      | TC-003                               |
|---------------|--------------------------------------|
|**Nome**       | Fissaggio Arduino |
|**Riferimento**| REQ-004                               |
|**Descrizione**| Verificare che l'Arduino sia sufficientemente fisso. |
|**Prerequisiti**| - |
|**Procedura**     | Inserire l'Arduino nel case facendo in modo che la porta che si collega all'USB vada ad incastrarsi esattamente nel buco apposito. Fatto questo raddrizzare leggermente se necessario la scheda per far coincidere i buchi con quelli sulla base del case. Dopo di che inserire le viti (3x10) nei 2 buchi posteriori, facendo attenzione ad avvitare troppo e spaccare il legno, in quanto è sufficiente che abbiano solo un po' di presa sul dado sul fondo della base. Provare a girare il case e verificare che stia attaccato. |
|**Risultati attesi** | L'Arduino rimane fissato al case. |
<hr>

|Test Case      | TC-004                               |
|---------------|--------------------------------------|
|**Nome**       | Resistenza agli urti |
|**Riferimento**| REQ-005                               |
|**Descrizione**| Verificare che il case resista a una caduta di un 1 metro. |
|**Prerequisiti**| - |
|**Procedura**     | Prendere il case e lasciarlo cadere da un 1 metro di altezza in vari angoli. Verificare che sia ancora intatto. |
|**Risultati attesi** | Il case non riporta gravi danni. |
<hr>

|Test Case      | TC-005                               |
|---------------|--------------------------------------|
|**Nome**       | Aerazione |
|**Riferimento**| REQ-006                               |
|**Descrizione**| Verificare l'esistenza di una ventilazione. |
|**Prerequisiti**| - |
|**Procedura**     | Verificare che i fori per i cavi abbiano un sufficiente spazio per ventilare l'interno. |
|**Risultati attesi** | L'Arduino è ventilato anche quando il case è chiuso. |
<hr>

### Risultati test

|Test Case      | Risultato                             |
|---------------|---------------------------------------|
| TC-001        | <span style="color:green">Passato</span>                   |
| TC-002        | <span style="color:green">Passato</span>                   |
| TC-003        | <span style="color:green">Passato</span>                   |
| TC-004        | <span style="color:green">Passato</span>                   |
| TC-005        | <span style="color:green">Passato</span>                   |

### Mancanze/limitazioni conosciute

Niente da segnalare.

## Consuntivo

![alt text](Allegati+Immagini/ganttConsuntivo.png "Gantt")

Il tempo complessivo utilizzato è stato il medesimo della pianificazione (anche perché si trattava di un progetto guidato). Alcune attività sono state effettuate a cavallo di 2 lezioni (mi risultava difficile rappresentarlo sul gantt), ma l'effettivo è comunque molto molto simile a quanto pianificato.
Il costo totale finale è di circa 20 CHF di materiali (in realtà utilizzati molto meno, si parla di 20 CHF a causa delle quantità in cui vengono venduti determinati pezzi), e 1800 CHF di lavoro sulle 36 ore usate.

## Conclusioni

La conclusione di questo progetto è molto fine a quel che se ne farà il committente, di per sé è efficace per quel che deve fare, sicuramente non sarà un grande cambiamento, e credo a dire il vero che sia più comodo rischiare di rompere l'Arduino invece che dover ogni volta utilizzare questo case, alla fine basta prendersi un po' di cura per le cose e questi prodotti non dovrebbero essere neanche necessari.

### Sviluppi futuri
Nel futuro (neanche troppo futuro) lavori del genere potranno molto probabilmente essere realizzati tramite una stampante 3D.

### Considerazioni personali
  Questo progetto è stato sicuramente utile proprio perché, essendo il primo, è stato utilizzato per guidarci nello sviluppo di lavori del genere. Ho trovato una buona idea quella di farci uscire dal nostro campo con un lavoro più 'artigianale', che può probabilmente far comprendere meglio la fase di progettazione (più concreta), seppure a discapito di altri punti che possono apparire quasi surreali (test case, use case).

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
