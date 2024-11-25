# Non complementazione del 2° tipo e rescue of phenotype

eccezione al test di complementazione.

Non complementazione del secondo tipo (complementazione solo con alleli recessivi)

mutazioni stanno su cromosomi diversi e non complementano (sembra paradossale, perchè se messi entrambi i geni mutati in eterozigosi avremmo almeno un allele wild type per gene)

si spiega come per la dominanza negativa, con un prodotto funzionale costituito dalla somma dei due geni. La differenza sta nel fatto che i geni mutati daranno prodotti che non complementano (fenotipo selvatico si osserva se viene prodotto almeno il 50% dell'omozigote wild type). solo il 25% delle combinazioni è in grado di dare un prodotto funzionale (<50% di prodotto per considerarsi wild-type):

![](https://phepatus.xyz/data/md-attachments-prova/2nd_type_non_complementation.svg)

ciò è molto riscontrato nei TF, che sono spesso dimeri e, tra essi, molti sono eterodimeri (costituiti da monomeri diversi). È una questione di quantità di prodotto funzionale circolante, non di competizione.

suggerisce la ricerca di un dimero

come bypassiamo il problema? freccia descrive TSS (transcription start site). RNA pol II ha bisogno per funzionare bene dei TF. TF è costituito supponiamo da due parti codificate da geni diversi, se le parti sono legati la pol II funziona, altrimenti no. Si tratta comunque di un equilibrio ($\ce{FT + DNA <=> FT-DNA}$). Dunque aumentando la quantità, aumentiamo formazione DNA-proteina che produrrà a sua volta più trascritto.

Cambiando promotore dei due geni che producono monomeri TF (intervengo solo sugli alleli selvatici di tale gene, vedi dopo per dettagli), ne possiamo far produrre molto di più, pur in un contesto di eterozigosità con non complementazione di secondo tipo -> recuperiamo dunque il fenotipo (**rescue of** (wt) **phenotype**)

Ingegneristicamente inserisco in cellule sdifferenziate plasmidi recanti plasmidi con gene A e B (quindi non inserimento nel genoma nucleare). Il recupero determina la **soppressione** del fenotipo originale (soppressione per over espressione). Strutture **episomali** (sono sufficientemente stabili pur non introducendosi nel genoma).

Tuttavia se la mutazione originale (del prodotto non funzionale) fosse uno SNP (single nucleotide polymorphism), potremmo anche intervenire con CRISPR/CAS9.

Regione regolativa è dove si inseriscono TF.

il promotore del costrutto a cDNA è solitamente forte (in natura produce molto trascritto, come quello di un gene costitutivoa)

esistono **plasmidi a basso e alto numero di copie**. I primi sono quelli che rifletto la biologia cellulare della duplicazione:

nella fase S avviene la duplicazione, formando i cromatidi fratelli (sister cromatids) e gli omologhi (uno per genitore). mitosi successiva fa sì che per ciascuna coppia di fratelli, una confluisca in una cellula, l'altra nell'altra.

i centromeri garantiscono l'assenza di aneuploidie (anomalie nel numero di copie di uno o più cromosomi - non di tutto il genoma), e meccanismi di ultra replicazione (es. se plasmide ha centromero, quel determinato centromero garantisce che esistano al più due copie, in quanto verrà riconosciuto dall'apparato mitotico delle fibre del fuso, per la segregazione). dunque un plasmide che si integra nel cromosoma deve essere a basso numero di copie, in quanto dobbiamo far sì che segua il meccanismo di duplicazione

cellula reagisce a centromero facendo duplicare il genoma a cui fa capo così come il genoma nucleare.

Viceversa, la segregazione delle numerose copie nel caso di plasmide a alto numero di copie sarà casuale, con cellule recanti decine di copie, altra cellula con 1-2 copie. Otteniamo un plasmide ad alto numero di copie facendo sì che non vi siano regioni centromeriche. Effettuando screening per cellule con strutture episomali in molte copie, otteniamo un'espressione forte.

Una strategia alternativa è avere un plasmide a poche copie ma con promotore forte.

esistono sequenze centromeriche che si possono inserire. ma questo avviene prevalentemente in lieviti (100aio di coppie di basi), le piante hanno sequenze centromeriche molto lunghe e difficilmente ingegnerizzabili.

# Soppressione

[immagine con nervature piante]

Col-0, saul1-1 mutazione, combinata con susa3-1 ristabilisce parzialmente fenotipo. due mutazioni che si comportano come il selvatico. qui abbiamo fenomeno di **soppressione**. NB: susa2, susa3, saul1 sono tutte mutazioni ma **in geni diversi**, non varianti alleliche!

immaginiamo sempre due geni su due cromosomi separati (in omozigosi: quindi senza non complementazione del secondo sito, che si manifesta con l'eterozigosi) formanti due prodotti che a loro volta formano dimero

però supponiamo che i due mutanti possano tra loro formare un prodotto funzionale, ma non gene1 wt e gene 2 mutato, o gene 1 mutato e gene 2 wildtype (tutti omozigoti). i mutanti "complementano" (prodotto di complementazione è diverso ma alternativo al wild-type), sopprime il fenotipo della prima

irradio un organismo con una mutazione (deleteria), sperando che si formi una seconda mutazione, che generi, dopo coltura in piastra, un fenotipo simile a wild type -> siamo andati alla ricerca di una mutazione di soppressione (soppianta?). Potrebbe anche presentarsi fenomeno di reversione: se mutazione casca su stesso gene (non è quello che cerchiamo, ma darebbe effetto simile). Si spiega microscopicamente con superficie complementare tra i due prodotti, seppur diversi dai wild-type.

[inserisci immagine]

qui mutazioni sono, ricordiamo, entrambe in omozigosi.

i singoli cromosomi sono parzialmente isolati (compartimentalizzate) e rispetto al tipo cellulare, grazie a struttura gelatinosa e interazioni tra cromosomi (intercromosomali), sono molto diversi nella loro disposizione, in quanto danno vita a relazioni funzionali. Si parla di separazione di fase (in termini fisici, sulla base della diffusione di un determinata regione, tale che la differente diffusione comporta induzione o repressione della trascrizione)

# Enhancement (o letalità) genetica

Interazione tra i prodotti dei geni, non tra i geni stessi.

Lievito riferimento. due ceppi. Organismo aploide (in questo caso). Ceppo selvatico gemmante (non scissione binaria). Mutazione nel gene A o gene B prese singolarmente non dà esiti, mentre insieme generano letalità. Unica spiegazione:

syp22-1 non genera stelo (o infiorescenza?). vamp727 x sym22-1 genera quasi letalità. Esattamente l'opposto del fenomeno di soppressione (fenotipo).

Mutanti termosensibili (ts). Es. a 30 °C pianta è malforme. DUe mutanti, ts1 e ts2, che a 30 °C sono malformi. A 25°C (temperatura permissiva) nessuna delle due è degenere.

Pianta contenente ts1 e ts2 assieme, a 25°C muore.

Anche in questo caso si genera un complesso, dall'interazione tra i due prodotti

nel punto di giunzione tra i due, mutazione su amminoacido che ad alta T destabilizza proteina e complesso non può formarsi, su uno dei due prodotti. ts2 fa la stessa cosa ma sull'altro monomero proteico. Gli amminoacidi modificati sono interagenti, così che non possano interagire se entrambe le mutazioni non sono presenti (perché magari una parte mancante reca una carica positiva, l'altra negativa).

Letalità sintetica: fenotipo esacerbato a temperatura permissiva, laddove prima avveniva una letalità inferiore, ma a temperatura elevata.

# Genetica classica vs inversa

Genetica molecolare: conoscenza funzione gene prima del 

gene clonato con funzione ignota (di gene conservato, che devono possedere un ruolo cruciale) -> generiamo dei mutanti -> osserviamo fenotipo (es. assenza fiore) -> cerchiamo di dedurre il meccanismo biologico sotteso (tutti i geni coinvolti nella creazione del fiore)

Classica: processo biologia

RNA: ribosio (due OH in posizione 2' e 3'), uracile al posto a timina
DNA: deossiribosio (un OH in posizione 3), timina

DNA in plastoma, DNA mitocondriale e DNA nucleare

duplex RNA RNA è molto più stabile di duplex DNA RNA e a sua volta di DNA DNA.

DNA è più stabile per garantire stabilità nelle varie cellule, e soprattutto nelle cellule della linea somatica, che devono presentare assolutamente le medesime caratteristiche al momento del passaggio nella linea germinale.

RNA dev'essere instabile, in quanto la funzione di trascrizione è differenziata sulla base diversi tessuti (salvo espressione costitutiva), e a un certo punto deve degradarsi per far fronte a cambiamenti nell'ambiente cellulare e nella segnalazione. Ormone per antesi sottostanno a geni con espressione. Oppure addirittura in una fase differente, nella stessa cellula, un gene prima è attivo poi no, poi di nuovo attivo.

A rendere l'RNA instabile è la posizione del secondo OH (in posiz 2), che può effettuare un attacco elettrofilo (O attacca P del legame fosfodiesterico che ha quattro legami con O, e quindi è parzialmente carico positivamente). Questo avviene spontaneamente, ma anche mediato da enzimi, Si forma un ciclo con il P, che porta a idrolisi del legame con il successivo nucleotide. Idrolisi impossibile su DNA perché non esiste OH. Esistono ribonucleasi. oppure in ambiente basico OH si deprotona e O con carica negativa attacca ancora più facilmente.

DNA molecola estremamente inerte.

Inoltre importanza uracile per ribonucleasi, per il riconoscimento, importante per discriminazione soprattutto considerando che nei batteri RNA e DNA condividono ambiente in soluzione.

Citosina spontaneamente va incontro a reazione al C4: il gruppo amminico diventa gruppo chetonico (deamminazione), che è uracile. Il più importante sistema di riparazione del DNA è quello del DNA uracil glicosidasi. Rompe legame con lo zucchero prontamente (è prodotta massicciamente per discriminare DNA da RNA)

reazioni avvengono a pH neutro. vi è equilibrio tra gruppo amminico e imminico in tutte le basi, e equilibrio spostato a secondo di . Nella timina è rovesciato.

Denaturazione avviene a pH basico, oppure con T (ma non in vivo) -> importante se vogliamo preservare enzimi

slide appaiamenti watson-crick (11.1 AG e  AT 10.8 A -> fornisce struttura parallela ed elicoidale). Importante pH neutro.

Elica destrorsa: dall'alto in senso orario.

esistono dna sinistrorsi, ma sono problematici

vedi struttura B vs struttura Z (sinistrorsa). forma A è artificiale (alta concentrazinoe salina)

struttura Z ha concentrazinoe salina e combinazione basi diversa, alta concentrazione CG (una via di mezzo, è rara ma non sintetica come forma A)

esistono anche struttura a tripla elica (ma in maniera localizzata). 

solco maggiore vs minore: zone di esposizione delle basi sono alternate. La differenza tra i solchi è più modesta nel (ma artificiale con soluzione salina 1M di NaCl)

DNA polimerasi richiede l'esposizione di un 3' OH per avviare replicazione (per posizionare il 5' e poi procedere in 5'->3'). È dato da un primer.

Arturo Palaschi

RNA polimerasi ha sempre direzionalità, si fissa su stampo, ma necessita di TF che si legano alle sequenze promotrici e poi a RNA polimerasi (sono specifici, anche tessuto specifici: un TF non lega tutti i promotori)

istoni nucleosoma. core istonici ogni 250-300 bp. con superavvolgimenti si genera cromosoma condensato pre-mitotico. Primo livello di oranizzazione però non è quello, vedi batteri (hanno istoni, e nucleosomi).

proteine (cariche positive) hanno affinità elevatissima ma specificità (in quanto devono garantire intervallazione costante su tutto il genoma, con bp e sequenze diverse) bassissima per fosfati del dna.

Un TF viceversa (elevata specificità e moderata affinità), riconosce delle sequenze specifiche (1/2^6 per una sequenza da 6bp). Solchi permettono lettura e penetrazione. alfa elica, struttura secondaria proteine, solco maggiore è perfettamente incastonabile. Dominio ad alfa elica permette interezione (trasversalmente nei viventi) con DNA. Alfa-eliche con composizione amminoacidica che permettono il legame con determinate sequenze di basi.

polimerasi si colloca pressapoco allo stesso modo sui geni, ma è l'interazione con i TF a modificare le caratteristiche cinetiche dell'RNA polimerasi.

il numero di basi riconoscibile non dirimente nel caso di solchi più piccoli (forme A e Z), es. 2-3 basi non sufficiente, se solco è tale. alcuni TF riconoscono fino a 13 basi.

non sempre interazione tramite alfa elica ma stragrande maggioranza di casi

# Contenuto in ATGC

Può essere sfruttato per caratterizzare una specie

centrifugazione zonale/isotipica: separazione per diversa densità locale del DNA. Appaiamento GC la rende più compatta (10.8A vs 11.1A) -> aumentano la densità della sequenza (più compatto).

Possiamo separare su un gradiente di CeCl, in ultracentrifuga (rivedi concentrazione). Rotore a bracci ortogonali a asse di rotazione (fino a 100k rpm). Atomi Ce pesanti, si muovono con la forza centrifuga: verso l'esterno saranno più presenti rispett oa vicino ad asse (si genera gradiente). Se inserisco molecola che ha densità intermedia, creerò bande.
raggiungerà al massimo la corsa del cesio. Si creano stratificazioni in base a contenuto AT e GC. La densità media del DNA genomico aumenta linearmente all'aumentare del contenuto in GC (in %). At è . I termofili hanno contenuto GC elevato (anche gli alofili). Ricorda T di melting, che aumenta a CG. Ha a che fare con il triplo legame idrogeno (più energia richiesta per spezzarli).

# Hyperchromic shift

coefficiente estinzione molare: capacità di assoebimento di una lunghezza d'onda e quanto assorbe. 360nm max assorbimento del DNA -> si traduce in 1 OD (unità ottica di densità) che corrisponde arbitrariamente a 50 ug/ml. Per l'RNA sono 40 ug/ml.

cuvetta di quarzo (assai trasparente e non deflette radiazione luminosa)

Hyperchromic shift: caratteristica DNA

picco di assorbanza a 260nm (doppio filamente), se invece si ricalcola coeeficinete estinzione e lunghezza d'onda 

basi libere fa sì che si possano assorbire maggiori energie, altrimenti se ci sono legami in essere, assorbimento comporta modificazione temporanea legame.

assorbanza = trasmittanza .. ?

curva di assorbimento in fne di T. Osserviamo a 260nm il double strand. a 50 °C tutto doppio filamento e reference value per assorbanza (consideriamo assorbanza relativa), e assorbimento max a circa 90°C.  Tm corrisponde a valore in cui abbiamo 50% assorbanza relativa (50% delle basi sono denaturate). Tm è valore caratteristico di una determinata molecola di DNA.

in laboratorio bisogna anche tener conto di forza ionica (salinità)

temperatura di annealing: sottraiamo a Tm 5 gradi (a tale temperatura è facilitato nel reannealing)

DNA nudo di batteri termofili si comportano allo stesso modo (vi sono altre compensazioni endogene)

cinetica di de/rinaturazione, vedi slide dedicata.

istruiamo il termociclatore di scendere di 1°C per min. Le molecole single strand denaturate, appena trovano un punto di ibridazione, avviene la rinaturazione (evento di nucleazione e zipping: esso non prosegue e non viene portato a conclusione). È importante rispettare un decremento non repentino degli eventi di collisione.

1000-10000 primer iniziali massa critica per avviare PCR.

Riproposta la formula che abbiamo visto in laboratorio per la determinazione della T di melting.

# Vettori per manipolazione

Il più semplice (sia in ambito vegetale, batterico o animale): vettori circolari, d'espressione e reporter.

pUc1918. _ SI REPLICA bene in E.coli. può essere sostituito da PCR se conoscessimo regione di amplificazione.

Caratteristica di ogni: replicazione autonoma all'interno del sistema biologico (in uesto caso coli, ogni 20, dopo 24h ho 1miliardo di plasmide)
- selezione (discriminare vettore con inserto e non). tecnica di transfezione (o trasformazione artificiale: sensibilizzazione cellule a ricevere DNA esogeno, es. permeabilizzazione membrana con trattamento CaCl: crea dei fori sito di ingresso DNA, poi facciamo avvenire riparazione membrana, certe cellule riceveranno e piastrate su terreno selettivo a determinato antibiotico inserito - cassetta con gene di resistenza - permettono discriminazione). se vogliamo plasmide ricombinante (con inserto dna esogeno, pUC1918 + inserto) altrimenti pUC1918 viene introdotto così com'è. 
- esiste in un punto del plasmide primario l'MCS (multi cloning site, sintetizzata artificialmente), per permettere il riconoscimento selettivo da parte di alcuni domini di restrizini (interagiscono tramite dominio ) CAATTG per es. in questo caso (la maggioranza sono sequenze palindromiche), ed è unica su tutto il plasmide. Dopo restrizione diventa lineare il plasmide. Estremità hanno sequenza specifica (enzima taglia tra GA di un filamento e GA dell'altro filamento complementare), rimangono code (sticky ends). Riportandole assieme ricostituiamo la sequenza. riappaiandosi e introducendo enzima ligasi (rigenera legame fosfodiesterico). Se usiamo HindIII per tagliare plasmide ma mettiamo nella stessa soluzione un inserto dotato di tali estremità (o meglio le loro complementali), abbiamo formazione di plasmide ibrido. In questo modo creiamo una libreria, se prima sezioniamo un genoma con tale enzima di restrizione e poi introduciamo ogni frammento ricavato in plasmidi diversi.
- plasmide rimane come elemento episomale (cromosoma ; perché non ha origine di replicazione nel batterio)

Bisogna saper manipolare E. coli per le prime operazioni di taglia&cuci

blu vettore a se stante, gialle hanno anche dna esogeno (selezione con ampicillina porta a screening visivo)

