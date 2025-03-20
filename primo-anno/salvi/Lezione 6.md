12-3-25

tramite chip è possibile rinvenire fino a 100k posizioni per SNP in un genoma. Se 10 cromosomi, 10k per cromosoma. 100 euro per individuo. si usa dischetto fogli

# Distanze tra loci

basata su frequenza di ricombinazione, in cM (centiMorgan).

Si parte da FR (frequenza di ricombinazione) = proporzione gameti ricombinanti su totale gameti analizzati.

FR per questo motivo non può superare 0.5:

![](attachments/Pasted%20image%2020250314105149.png)

I 4 gameti in basso a sx, se ricombinazione è completamente casuale, sono ugualmente probabili, e dunque FR = 0.5. Ma non può essere più di 0.5 (in media, ovviamente, perché un campione potrebbe benisismo avere FR > 0.5), altrimenti i reincroci sarebbero "deterministici"? Nulla ci fa supporre che i crossing over non siano casuali, stando alle conoscenze attuali.

Come osserviamo la composizione del genotipo? Possiamo osservare al microscopio, o utilizzare marcatori sul singolo gamete, ma difficile. Altrimenti si fa un reincrocio con un genitore omozigote, che produce un solo tipo di gamete

![](attachments/Pasted%20image%2020250314105738.png)

Applico a BC1 una analisi a marcatori, contando i ricombinanti nella BC1 è come se contassi i gameti che hanno portato alla formazione della popolazione di reincrocio. Lo faccio con tutte le coppie di tutti i marcatori, e in tal modo costruisco una mappa.

se sono vicini bassa FR (rara riconbimanzione) e dunque distanza piccola. Se sono molto distanti avranno FR quasi a 0.5, e dunque si comportano quasi ricombinando casualmente, come per i loci tra due cromosomi diversi, che assortiscono indipendentemente per la terza legge di mendel.

Tuttavia il cromosoma è più "lungo" di 0.5, la massima distanza FR. Cioè hanno lunghezze diverse. Come si risolve questa contraddizione. Es. cromosoma può essere lungo 200cM ma ricombinazione tra loci agli estremi è 0.5. Questo è dovuto al fatto che distanze con FR non sono additive, perché si basano su osservazioni dei ricombinanti, ma è un modo grossolano di calcolo distanza. Meno approssimativo sarebbe il computo del **numero dei crossing-over**.

![](attachments/Pasted%20image%2020250314110503.png)

Se ci limitiamo a considerare A e B, ci sfugge la casistica sopraccitata, ottenuta inserendo un marcatore di mezzo tra A e B. Classificheremmo i cromosomi di dx come parentali, esaminando solo A e B, tuttavia si tratta in realtà di doppi ricombinanti. Essi divengono sempre più probabili man mano che separiamo i due loci sul cromosoma, ossia distanza in senso tradizionale sempre più imprecisa (distanza sottostimata, sempre in generale). Come passiamo al conteggio diretto dei crossing over?

Si impiega un modello matematico che stima il numero di crossing over che non emergono alla disamina diretta, ipotizziamo distribuzione casuale di crossing over, con distribuzione di poisson. Funzioni di mappa di Haldane e Kosambi. Dunque è una trasformazione da FR a distanza effettiva data su numero crossing over. Otteniamo valori in cM. **cM misura frequenza di crossing over, FR in termini di ricombinazione di loci**. Questa distanza non ha un massimo. **1 cM corrisponde a 1 evento di crossing over su 100 individui, tra i due marcatori considerati**. (NB: posso avere anche 200 crossing over tra i due loci, nei 100 individui)

![](attachments/Pasted%20image%2020250314111029.png)

Si tratta di una correzione. Tuttavia più i loci sono distanti, più correzione non è fine. Per migliorare precisione, **posso usare più marcatori**, che ci consente di spottare i doppi crossing over, senza necessariamente doverli stimare e basta sulla base di una distribuzione degli stessi ipotetica. Entrambi assieme ideale (?).

Tanto più due loci sono lontani, tanto più è facile che avvenga crossing over, perché avvengono casualmente. ci sono in media 2-3 eventi di crossing over per coppia di cromosomi omologhi. Perché così pochi? Non sono nemmeno mai 0, ma nemmeno mai con 20-30 crossing over. Un mistero della biologia. Anche i parentali fanno crossing over, ma non ci interessano perché gli alleli ai loci rimangono invariati.

# Mappaggio di QTL con linkage

Caliamo discorso forward genetics a caratteri non mendeliani. Si parla di **mappaggio tramite linkage**, sempre tramite marcatori. Esiste poi seconda grande categoria, con mappaggio per associazioni (GWAS).

Due approcci:
## Mappaggio a singolo marcatore

1. popolazione sperimentale prodotta ad hoc
2. estrazione dati fenotipici (come nella F2 vista prima), sulla base dei nostri interessi.
3. genotipizzazione con sistema dei marcatori
4. elaborazione statistica da cui emerge localizzazione

### RIL

Popolazione sperimentale ottenuta da P1 x P2, da F1 sviluppiamo la popolazione. P1 e P2 devono essere particolarmente diversi per carattere di interesse (es. quantità biomassa, altezza, etc., chiaramente carattere che ci aspettiamo sia QTL). Sarebbe meglio linee pure. Da autofecondazione F1 otteniamo generazione segregante F2, idealmente continuiamo ad autofecondarle, F3. Si prosegue tipicamente fino a F8 (tutte autofecondazioni). Ad ogni ciclo numero eterozigoti si dimezza (probabilità che locus sia eterozigote si dimezza). A F8 abbiamo quasi una linea pura. Si fissano i crossing over. Abbiamo popolazione di omozigoti ma con genotipo assortito. Si parla di popolazione **RIL** (**recombinant inbred lines** - linee inincrociate ricombinanti). Non si usa quasi mai la F2. Come mai? Perché le generazioni omozigoti possono dare semi da cui possiamo ottenere repliche spaziali/temporali, lo stesso non si può dire su generazioni precedenti. 

Repliche importantissime per QTL, che sono intrinsecamente influenzabili da ambiente, e ipotizziamo che effetti ambientali siano distribuiti casualmente (es. per altezza una zolla potrebbe essere ricca di azoto, se avessi n = 1 metterei a repentaglio riproducibilità).

Se biologia specie consente propagazione vegetativa, ci consente di fermarci a F2 e propagare vegetativamente. Es. nelle arboree molto frequente, ma anche orticole come cucurbitaceae (possono essere innestati?), anche la fragola. monocotiledoni faticoso, aglio e cipolla è facile.

Altro metodo è usare aploidi raddoppiati (riduco a 1 anno - 1 generazione - il lavoro di 8 anni). Il punto di arrivo è il medesimo, in quanto il gamete che viene raddoppiato può essere ricombinante, prima di diventare omozigote a tutti i loci.

C'è tuttavia una piccola differenza: nei DH c'è un unico evento di crossing over per ricombinare, le RIL invece sono frutto di svariate meiosi, con loci che poi comunque vengono portati in omozigosi. I genomi parentali dei RIL sono molto più "frammentati". Dunque la risoluzione dei marcatori nei RIL è più elevata.

In entrambi i casi comunque supponiamo che non rimangano eterozigoti, dunque non dobbiamo considerare l'effetto di dominanza visto nella lezione 5 proprio dei QTL. Otteniamo un valore medio dalle varie repliche nelle diverse parti del pianeta, in modo che fenotipi siano robusti. Poi ho raccolto genotipi ai marcatori per ogni individuo.

M1 marcatore, supponiamo di aver genotipizzato per quel marcatore tutti gli individui. Possiamo correlare il genotipo omozigote a questi marcatori con i parentali da cui siamo partiti.

![](attachments/Pasted%20image%2020250314115638.png)

Facciamo medie dei fenotipi delle piante omozigoti per i diversi alleli parentali dei marker. Se non notiamo discordanza per un marcatore, lo ignoriamo. L'allele al locus M4, invece, è predittivo, in media, per il fenotipo che stiamo considerando. Il marcatore M4 si troverà a un QTL. 

Il parentale P1 (per convenzione quello con gli alleli maiuscoli) porta M4 sullo stesso cromosoma dove, in linkage, si trova un allele a un QTL che controlla, incrementandolo, il carattere considerato. Dal momento che vi è linkage, la maggior parte di questi cromosomi, appartenenti a questo parentale, hanno tale allele/alleli.

M1 e QTL, invece, sono sufficientemente distanti nel cromosoma in modo da ricombinare frequentemente. Dunque gli individui con M1 hanno un'uguale probabilità di avere Q e q.

==Dunque entrambi i marker sono sullo stesso cromosoma?==

Conclusione analisi: Q vicino a M4 ma abbastanza distante da M1.

Prima verifichiamo genotipo a marcatori, poi esaminiamo se hanno media diversa per fenotipo, e sulla base di ciò concludiamo che sono in linkage.

la distanza tra le medie non è altro che quella vista nella lezione precedente (==distanza di mader?? modello di mader==) tra media di QQ e  media di qq. dunque a è la metà della distanza. c'è approssimazione perché non so veramente dove sia Q/QTL, ma stimo mediante marcatore. Dunque posso anche stimare l'effetto del QTL, tramite a. 

Faccio questa considerazione su tutto il genoma, su vari marcatori. Se trovo oltre a M4 altri marker nelle vicinanze che mostrano un simile spostamento in termini di a, forse non ci troviamo di fronte a più QTL ma allo stesso (rasoio di occam). a ha un segno (direzione).

---

Ultimi minuti lezione poco chiari, serve grafico.

significatività della differenza: perché ignoriamo/scartiamo una delle due medie mentre reputiamo significativa l'altra (quella di M4)? Applichiamo un test statistico, nella fattispecie il t-test o t di student (confronto tra due medie, altrimenti con più di due ANOVA). Ciascuna osservazione si discosta di un det. valore dalla media. Prendiamo tutti gli scostamenti, pochi individui avranno scostamento ampio. Possiamo calcolare prob. che da un campione di quegli individui possa ottenere una media m1 o m2. 5% soglia di significatività. 

---

Identificare posizione QTL non sempre essenziale: se voglio clonarlo chiaramente sì, se voglio migliorare geneticamente mi è sufficiente impiegare dei buoni marker.

Il solo sequenziamento, successivamente al rinvenimento del marker, non è sufficiente per restringere il campo in specie altamente polimorfiche, che differiranno anche ma non solo sui QTL.

numero medio geni 30k, numero medio cromosomi 10, dunque 3k per cromosoma.
## Mappaggio per intervalli