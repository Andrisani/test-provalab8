# Test-provalab8

## Semafori p.1

Spett. Ditta, 
In seguito all’incontro tenuto presso la nostra sede vi trasmettiamo le informazioni richieste dal 
vostro analista. 

Il  sistema  di  controllo  del  traffico  veicolare  sulle  **tratte**  stradali  interessate  a  lavori  di 
manutenzione  straordinaria,  per  i  quali  non  è  possibile  provvedere  in  anticipo 
all’incanalamento  standard,  deve  essere  in  grado  di  operare  in  due  modalità:  connessa  e 
autonoma. 

In entrambe le modalità la coppia di **semafori** a due luci (l’uso della luce gialla è 
sostituito dalla temporizzazione a doppia luce rossa) provvede a bloccare il traffico da uno dei 
due  lati  (convenzionalmente  chiamati  blu  e  bianco)  e  a  consentire  il  deflusso  dei  **veicoli** 
accodati dall’altro. In pratica, i **veicoli blu** (accodati dal lato del rispettivo colore) attendono 
l’accensione della luce verde e, ottenuto il consenso, procedono all’attraversamento del tratto 
stradale interessato. 

Dopo un periodo di tempo, configurabile dall’operatore al momento della 
predisposizione  del  sistema  sul  campo,  il  **semaforo  del  lato  blu**  spegne  la  luce  verde  e 
accende  quella  rossa  per  consentire  lo  sgombero  del  tratto  stradale.  La  durata  del  periodo  a doppia luce rossa è calcolata dal sistema in base alla lunghezza del tratto stradale e alla velocità media  di  percorrenza  (dati  configurabili  dall’operatore).  

Al  termine  di  questo  periodo,  il **semaforo del lato bianco** spegne la luce rossa e accende quella verde, iniziando per i **veicoli bianchi** un ciclo analogo a quello precedente. Per motivi di sicurezza, il sistema è dotato di un meccanismo  di  blocco/sblocco  che  interrompe  il  ciclo  di  luce  verde  e  attiva  la  condizione  di doppia  luce  rossa.  

Lo  stato  bloccato  è  esplicitamente  liberato  dall’operatore  mediante  il meccanismo di blocco/sblocco. 

Restiamo in attesa di un vostro riscontro per procedere alla fase successiva del progetto. 
Cordiali saluti, 

Ing. Franco Strada 

****

**Domanda**. Dare  un  diagramma  delle  classi,  relativo  ai  concetti evidenziati in neretto nell’enunciato. 

****

## Semafori p.2

Spett. Ditta,

In seguito alla sperimentazione sul campo del sistema di controllo del traffico veicolare sono 
emerse alcune situazioni che richiedono un’evoluzione del sistema.

In particolare, si è osservato che quando la lunghezza della tratta stradale controllata è maggiore di 500 metri spesso i tempi di attesa sono eccessivi e, di conseguenza, rallentano il traffico. 

Per mitigare questo fenomeno, i nostri tecnici hanno proposto l’uso di quattro **sensori** di passaggio direzionale dei veicoli, per consentire al sistema di rilevare l’assenza di veicoli in transito su entrambi i lati della tratta. 

Un **sensore in** sarà posizionato prima del semaforo blu (la distanza di posizionamento dipende 
dalle caratteristiche della tratta) per rilevare il passaggio dei veicoli che arrivano dal lato blu.

Un **sensore out** sarà posizionato all’altezza del semaforo bianco, per rilevare il passaggio dei 
veicoli  arrivati  dal  lato  blu  che  hanno  completato  l’attraversamento  della  tratta.  

Altri  due sensori  sono  posizionati  simmetricamente,  per  rilevare  il  passaggio  dei  veicoli  bianchi.

Il comportamento del sistema deve essere modificato in modo da interrompereanticipatamente il ciclo verde in assenza di veicoli in transito. 

Per evitare fenomeni di oscillazione, il ciclo verde deve  avere  una  durata  minima  *tempoMin*,  configurabile  dall’operatore  al  momento  della predisposizione del sistema sul campo.


Restiamo in attesa di un vostro riscontro.

Cordiali saluti, 
Ing. Franco Strada  

****

**Domanda n.1.**  Dare un diagramma di classi, relativo ai concetti evidenziati in neretto negli enunciati Semaforo1 e Semaforo2.

**Domanda n.2.** Disegnare il relativo diagramma dei casi d'uso(Semaforo1 e Semaforo2).