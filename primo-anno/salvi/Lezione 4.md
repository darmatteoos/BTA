
1-2 trasposoni attivi per pianta scala. se 30k i geni, e con prevedendo un po' di ridondanza, produciamo popolazione di 100k individui.

come recupero gene modificato da trasposone per inserimento, dopo aver constatato modifica di interesse in filetta? posso fare map based / positional cloning incrociando individuo in popolazioni segreganti. conoscendo il trasposone nella sua sequenza, posso recuperare regione cromosmica attigua. vi sono vari modi, tutti semplici al giorno d'oggi:
- la strategia più usata attualmente: selezione 3-4 piante con fenotipo estremo, 3-4 piante con altro fenotipo e sequenziare. sequenziare un genoma "normale" costa circa 1k, molto abbordabile (10k in totale circa). se piante derivano da stessa linea omozigote con trasposone attivo (sono isogeniche tranne per spostamento trasposone): unica differenza nel genoma dev'essere l'inserzione in gene specifico.
- sfruttare sequenza trasposonica stessa e progettare PCR. no sito inizio trascrizione, no random primer. un tempo si faceva con libraries, usando trasposoni come sonda. oligonucleotide complementare a Tr con in fondo marcatore cromoforo.
	- prendiamo genoma pianta con trasposone e tagliamo con enzimi di restrizione per produrre frammenti di 1-3k nt (lunghezza di un gene media), facilmente amplificabili (range PCR senza reagenti complicati, altrimenti fino a 40k). Si aggiunge **adattatore**, doppia elica a sequenza nota (vedi es. [qui](https://web.archive.org/web/20250310131641/https://theory.labster.com/it/adapter_ligation/)): si ha appaiamento fiancheggiante ai frammenti. possiamo usare tale porzione per progettare uno dei due primer, l'altro nel trasposone. tra i due troverò 200-1k nt del gene considerato, sufficiente a identificare gene. bisogna considerare che già conosciamo tutti i geni solitamente, pur non conoscendone la funzione. Parentesi: esistono enzimi di restrizione blunt o sticky, e anche ligasi blunt o sticky.
	- altrimenti **PCR circolare**: circolarizzo i frammenti ricavati precedentemente, trattando con ligasi, dato che abbiamo sticky ends. a questo punto si può amplificare progettando un primer sulla "sezione circolare" interna e uno esterna. ha il vantaggio di non dover passare per adattatore: i due primer sono entrambi progettati su sequenza del Tr in questo caso.

Esistono trasposoni in molte specie di interesse agrario. in alcuni casi sono stati inseriti in altre specie, e spesso continuano a funzionare in modo atteso. es. A. thaliana, con trasposoni di mais, anche soia e riso. In riso anche con trasposone nativo, anche in arabidopsis. tuttavia se non nativo si configura come ogm in europa.

# Tecnica reverse: TILLING

la più popolare in genetica agraria, tecnica di elezione. anche se adesso rivaleggia con GE. contratti tra uni e privati.

**TILLING: Targeting Induced Local Lesions In Genome**. To till vuol dire sarchiare, zappare, curare l'orto. Inventata in arabidpsis, da ricercatore ita (Luca Comai).

se conosciamo il gene, tramite TILLING possiamo rinvenire linea con mutazione in tale gene studiabile per dedurre fenotipo. si parte producendo popolazione mutagenizzata, in questo caso mutagenesi chimica, che induce **mutazioni puntiformi**, il più comune mezzo è EMS (ethylen-methan-sulfonate). produce sostituzioni, in piante e animali (è cancerogeno). Dopo aver indotto mutazioni **in semi**, allevo la popolazione da seme. cellule seme vive, che nel momento che cominciano a dividersi accumulano mutazioni nei tessuti. seme prima trattamento è detto M0 (generazione M0), poi a seguito trattamento M1. mutageno si inserisce nella doppia elica, che comporta errori durante duplicazione da parte di DNA pol. Se siamo in organismo diploide, due copie di un gene, e dato che mutazione è casuale, è assai improbabile che mutazione avvenga in entrambi. **mutazioni in eterozigosi in M1**. facendo autofecondare M1, otteniamo M2, in cui osservo che 1/4 piante saranno WT, 1/4 con mutazione in omozigosi e 1/2 eterozigoti. M2 si ottiene prendendo un seme da ciascuna pianta M1, prendo un solo seme da una siliqua/spiga, etc. E così via per generazioni successive. **sempre mantenimento stessa numerosità popolazione**. Da M2 raccolgo seme M3 e estrazione DNA da foglia corrispondente della pianta M2. Quale pianta M2 porta mutazione in gene interesse? Si tratta di sostituzione nucleotidica (non inserzione), è puntiforme. Dal momento che conosco il gene nella sequenza (reverse genetics) ma non nella funzione, è sufficiente sequenziare gene per tutta la popolazione M2. poi recupero seme da membri della pop. che presentano mutazione da sequenziamento e le coltivo. la maggior parte delle sequenze ottenute sono ==invariate?==, ma alcune presentano mutazioni nella sequenza del gene. si confronta con sequenza linea WT, verosimilmente è stata sequenziata preventivamente, o altri membri popolazione non mutati (la maggior parte). Prima che costi di seq fossero così bassi si utilizzavano altre strat molecolari.

Vi sono alcune **scorciatoie**: produrre un amplicone per tutte le 10k piante è dispendioso (piastre da 96, sarebbero ~100 piastre, ma in termini di reagenti e plastica meglio evitare). per velocizzare riconoscimento si può ricorrere al **bulking** (o **pooling**). Ossia aggregazione/miscelazione campioni diversi in un unico. tornando indietro, se 1 sola pianta su 10k fosse mutata; posso miscelare tutti gli individui di una piastra (~100). Ottengo 100 provette. Dato che DNA originali sono tutti appartenenti allo stesso genoma, posso fare PCR sul bulk di ciascuna "piastra originaria". in tutti produco unico amplicone. presenza mutazione si può verificare. A quel punto basta fare un'altra piastra con tutte le piante (~100) appartenenti al pool nel quale si è riscontrata una mutazione. riduzione da 10k a 200 pozzetti, ossia due PCR (due piastre).

## TILLING by sequencing

Sequenziamento al giorno d'oggi:
- **Sanger** (fredrick sanger, 2 nobel): 1977 esperimento pilota, basato su terminazione catena. consente di sequenziare una molecola alla volta. per ogni molecola si ottiene **elettroferogramma** (segnale di fluorescenza che identifica i singoli nucleotidi sulla base della loro fluorescenza). se abbiamo due sequenze praticamente uguali, otteniamo segnali sovrapposti; se abbiamo mutazione in eterozigosi, avremmo 1/2 picco su G per es, 1/2 su A, con colori diversi (intensità di ciascuno è metà). Picco elevato per nucleotide non mutato nel bulk da 100 piante, mentre in media solo 1/100 del segnale sarà dato da nucleotide mutato, e così si confonde con rumore. **Non adatto per TILLING**.
- **Short-read** (per estensione, **ILLUMINA**). È sequenziamento di nuova generazione, molto più economico. Azienda più importante che offre questo servizio è illumina. 99% sequenziamenti è con illumina. max 150 nt, da cui short (sanger fino a 1k, long read diverse di migliaia, anche 20-30k). sequenze sono circa 1M ==per singolo genoma? considera che 3.5miliardi per uomo, 135milioni per arabidopsis, quindi questo dato con arabidopsis quadra==, e considerando un livello di bulking 1/100, ~10k recheranno mutazione. sequenziamento di un amplicone con short read sono 100 euro. ==se ho capito bene, prima effettuiamo PCR su amplicone di gene interesse, poi sfruttiamo ILLUMINA su amplicone, cosa che non potremmo fare con sanger credo; in questo modo abbiamo molto più segnale dato da amplificazione DNA==
- Long-read

si parla di **TILLING by sequencing** nei casi visti.

---

lab salvi si occupa di tilling in orzo, clonando molti geni di interesse.

nei casi visti siamo interessati all'approccio reverse genetics, e dunque non ci focalizziamo su fenotipi interessanti che emergono incidentalmente da mutazione data dal TILLING.

**mutanti omeotici**: trasformazione di un organo in un altro (es. [antennapedia](https://en.wikipedia.org/wiki/Antennapedia) di drosophila, zampa a posto di antenna - ==in particolare in questo caso si tratta di una sottoclasse di geni omeotici noti come HOX==). in orzo antera diventa pistillo in un caso esaminato da gruppo Salvi.

geni coinvolti in sintesi amido cariosside in orzo. carente in triptofano (?) frazione proteica. amido orzo 30/70 amilosio/amilopectina, amilosio è amido resistente, ma a indice glicemico più basso. SSIIa (gene) produce amilopectina, e ne vogliamo di meno. In primis si conferma funzione in orzo (era noto in?) con approccio TILLING. Si rintraccia mutazione in quel gene. Una linea (1517) era knockout per il gene (mutazione puntiforme), quasi 50/50 la ripartizione degli amidi a seguito mutazione. La ripartizione variata non viene tuttavia compensata in una produzione totale di amido inalterata (si riduce e cariossidi sono meno gonfie). Non si sa perché vi sia tale effetto pleiotropico negativo.

Approcci simili in patata. Qui vogliamo più amilosio che amilopectina. (forse come coadiuvante tecnologico?).

In riso, a seguito di rivoluzione verde (riduzione taglia e aumento concimazioni, diminuzione allettamento, il tutto post WW2), molte varietà italiane tradizionali non hanno subito miglioramenti, soprattutto per ritrosia a seguito di preoccupazioni per destinazioni alimentari (es. risotto). Es. cultivar volano, sono noti geni (sequenziati) responsabili bassa taglia. con tilling si cerca mutazione di tale gene. Anche in vialone nano, arboreo. SIS sta lavorando in tal senso, a San lazzaro ci sono programmi di miglioramento.

Vantaggio: assenza approccio OGM.

## Riflessioni su TILLING

oltre a considerazione OGM, abbiamo il fatto che TILLING può diventare, oltre a metodo di studio funzione genica (metodo di **functional genomics**, ossia attribuire funzionalità geni con approccio biotech), anche un **metodo di miglioramento genetico**, con interesse economico/pratico (es visti prima: es. allele che abbassa taglia può essere incrociato con altre varietà - background genetici - per trovare progenie di bassa taglia)

TILLING distribuisce casualmente mutazioni, e effetto non è sotto controllo ricercatore (potremmo riscontrare mutazioni knock-out, missense, o silenti). Empiricamente, ci possiamo aspettare, in popolazione TILLING, 1-2 knockout (alleli forti che bloccano espressione), 4-5 alleli missense (cambio aminoacido) e 4-5 silenti. Senza contare mutazioni introni e su terminatore, con effetti praticamente assenti.

Si può anche produrre una **serie allelica (di mutazioni)**. Non sempre mutazione dev'essere forte (blocco con knockout proteina), per essere di interesse per miglioramento. Non vogliamo nemmeno cambiamento drammatico fisiologia (**geni letali**), incappando in geni di questo tipo non possiamo mutarli tendenzialmente. Non possiamo studiare funzione in quanto portano sempre a morte. Dunque meglio avere mutazioni blande e studiabili

# TILLING nei poliploidi

Altro grande uso. Inizialmente proposto nei diploidi. Es. frumento: se faccio amplicone ==intendevo mutazione?== su allele, essendo esaploide, omozigosi non permette di vedere fenotipo. Ma in realtà funziona ancora meglio: vedi grafici. Grafico sinistra: rappresentazione densità mutazioni accumulate in un poliploide confrontato con un diploide. Cfr. tra 3 classi di ploidia (2, 4, 6x). Dati da frumenti e brassiche, in quanto entrambi hanno rappresentanti di di, tetra e esaploidi. Cfr 2x e 6x: la densità, espressa come la distanza percorsa prima di incontrare mutazione, in media (nei grafici si usa la scala logaritmica), c'è un ordine di grandezza di divario circa, maggiormente 6x;. In orzo 1 ogni 400-500kb, in 6x circa 50kb. Dunque stessa quantità di mutazioni indotta utilizzando 10 volte meno piante. Risvolti pratici.

Dalla densità di mutazione deriva una metrica molto impiegata nei programmi di breeding: la popolazione necessaria per avere probabilità di trovare un mutante nell'80% dei geni. in orzo circa 10k piante, in frumento 1k.

si parla di mutation law ==non trovo nulla online==

ma per studiare il fenotipo in frumento esaploide? Qui abbiamo detto screening su 1k (a volte anche 400-500). Screening è su gene singolo, ma sappiamo che su 6x è triplicato. dovrei trovare un mutante anche per i due omeologhi in genomi B e C, portare in omozigosi. poi devo **piramidare** con incroci i tre alleli mutati nella medesima pianta finale. non complesso, solo limite temporale.

Riformulando: gene di interesse in due omologhi per 1A e in due omologhi per 1B (l'omeologo). Se facciamo TILLING in 4x -> avremo una mutazione casuale in 1A, dopo autofecondazione (eredità disomica) porta mutazione in omozigosi. Nello screening trovo altra pianta in stesso gene omeologo ma in 1B, porto in omozigosi anche questa con autoincrocio. Queste due linee singolarmente non vedo i fenotipi di interesse (perché gene non mutato dell'omeologo consente mantenimento fenotipo). Dunque piramidizzo (**pyramiding**, vedi [qui](https://en.wikipedia.org/wiki/Gene_pyramiding)) mutazione (si parla anche di **stacking**). Con marcatori dopo seq riusciamo a isolare le piante (poche) omozigoti per mutazioni per tutti e 4 gli alleli (omozigoti a due a due, si intende). È approccio giustificato.

Ma perché avvengono questi accumuli maggiori nelle specie poliploidi?

**mutation density si ottiene da massima quantità mutageno chimico, aumentando ancora di più la pianta risponde morendo** - è parte della procedura di taratura per massimizzare efficacia mutageno (non si può superare tale soglia, nei diploidi). negli esaploidi abbiamo ridondanza genica, e dunque piante non muoiono se accumulano più mutazioni -> mutation density senza ripercussioni più elevata.

ma perchè una densità di mutazione così piccola determina morte? 500kb di distanza media tra mutazioni, come abbiamo visto in orzo, altrimenti, come densità sarebbe troppo basta per giustificare la letalità, soprattutto se la mutazioni sono in eterozigosi. Il problema è la morte del gametofito, che è aploide, e dunque nel generare M2 muore. Se invece è tetraploide (o esa) questo non si presenta (gametofito non è aploide in senso stretto, ossia x != n).

# TILLING in silico

Non by sequencing, come quello visto ora. È una simulazione informatica. Popolazione mutagenizzata dev'essere completamente sequenziata in anticipo. mi limito a prelevare DNA fogliare da tutti individui e non faccio discrimine a monte facendo prove dopo M1, e listo mutazioni esistenti in tutti individui e tutti i geni: è sufficiente interrogare db. Aumenta costi a monte ==NB: penso che differenza determinante sia il fatto che in TILLING anche da sequencing si sequenziano delle short-reads per il gene di interesse, mentre qui bisogna fare WGS su tutta la popolazione; ma altrimenti il metodo di procedere è esattamente lo stesso?== ma li diminuisce a valle. Solo 2-3 specie (orzo, frumento, arabidopsis). Frumento scelto per densità mutazione elevata, nonostante grande genoma, dunque sequenziamento di minor numero piante. Inoltre altre strategie per ridurre ulteriormente seq: ci si limita a sequenziare porzione codificante (**2-3%** genoma eucariote in media costituito da esoni, riduzione considerevole costi), che reca 90% funzioni (così perdo per es. RNA non codificanti). UC davis [ha prodotto](https://www.wheat-training.com/tilling-mutant-resources/) popolazione frumento TILLING completamente seq nella sua componente esonica (**exome sequencing**).

ti mandano linea già piramidata.

cattura dell'esoma.

popolazioni non silico si perdono negli anni perché hanno accumulato mutazioni (10k si sono ridotti a 3500 nel caso della popolazione di orzo del prof). costo conversione in silico (1000euro * 3500)

in fagiolo, con genoma 10x più piccolo, 100 euro per sequenziamento. 300k è un normale finanziamento per la ricerca.

alcune start-up si configurano come spin-off universitari, università che offrono pacchetti in cui creano, previo pagamento, popolazioni ad hoc per effettuare tilling su alcuni determinati geni (2,3 es.), si dà il tutto all'azienda e poi si "straccia" la popolazione.

# T-tagging

mutagenesi per inserzione trasposone, si può aggirare la difficoltà nell'inserimento. Si usa T-DNA, tratto inserito da A. tumefaciens in cellula infettata. le 10k piante le produco non per spostamento trasposone, ma infettando e trasformando tali piante con A. tumefaciens. Si parla di **T-tagging**. High throughput transformation. In Arabidopsis esistono protocolli, vedi **floral dip**: pianta fiorita si immerge in una soluzione agrobacterium. Perde infiorescenza e si trasformano sporociti, che poi formano gameti mutati. Se inserisco resistenza a erbicida/antibiotico in T-DNA, posso allevare in terreno selettivo per selezione negativa su piante non-mutagenizzate. In un mese si produce in arabidopsis una tale popolazione. Poi si può approcciare con forward o reverse. 125Mb è dimensione genoma arabidopsis (5miliardi in orzo, 40x). 1000/40 euri (cfr. costo di prima) costo seq: irrisorio.

Più facile trovare mutazioni in questo caso, perché? Non ho sentito (senti fine lezione) ==Immagino perché possiamo sia screenare, sia usare==

## Transposon tagging

si può inserire anche - **transposon tagging** - trasposone in TDNA (ad es. sistema Ac/Ds del mais, elemento autonomo + non, con due transfezioni successive, poi si rimuove l'autonomo per fissare mutazione) ==ma qual è beneficio a semplice inserimento T-DNA? In entrambi i casi si inserisce casualmente, ma nel caso del trasposone dobbiamo anche eseguire un altro passo per fissare mutazione==

## Activation tagging

mutazioni a carico di esoni quelle impiegate in tilling (silenti, miss sense o non sense). i geni possono essere alterati o non funzionando più o alterando funzionalità. facendo tagging o TILLING normale, l'effetto è più o meno lo stesso. in entrambi i casi si tratta di mutazioni/alleli recessive. Per studiarli devo produrre omozigosi e poi confrontarli a WT. Ma è approccio riduttivo: dover disattivare funzione (piante più deboli) per ottenere indizi su funzionamento del gene. Questa è la premessa per un altro approccio:

**activation tagging**: mutagenesi volta a aumentare funzione gene. inducendo mutazioni **dominanti**. Spesso con GE, più complicato con TILLING, possibile con T-tagging. ma seq T-DNA contiene **superpromotore** ==ma nessun gene?==. Se finisce vicino a un gene, produrrà sovra espressione gene. mutazione è visibile anche in eterozigosi: vantaggio. Infatti una copia molto espressa risulta visibile rispetto a diminuzione espressione di una dei due alleli. popolare in arabidopsis e riso. frontiera in pomodoro e anche nei cereali. come superpromotore si usano promotori superefficienti, **CaMV35S**, di gene virale virus brassicaceae (risponde a RNA pol piante, richiede efficacia elevata). Viene ripetuto **4-5x** per essere sicuro che attivi trascrizione gene. ==Attivazione stando a immagine su slide può avvenire a valle ma anche a monte di sito inserzione, forse fungendo da enhancer?== 