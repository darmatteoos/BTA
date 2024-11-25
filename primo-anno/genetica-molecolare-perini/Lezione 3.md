
Tre tipologie di vettori:
- Vettori di propagazione: i più semplici
- di espressione:
- reporter

Tutti i plasmidi con costrutti vengono amplificati nei batteri

la scorsa volta avevamo affrontato pUC18/19.

Tutti i vettori necessitano di:
- origine di replicazione (per replicazione nel batterio E. coli)
- gene di selezione (nel caso di pUC18/19 bla): pennicillina o ampicillina (più stabile e necessaria in minor quantità)
- sito di clonaggio: MCS. Disegnata per essere tagliata selettivamente da un enzima di restrizione del plasmide, con sequenza unicamente presente nel sito di interesse. Esempi di enzimi di restrizione: EcoR1 (di E. coli) -> è meccanismo di difesa da DNA esogeno. Non taglia il proprio. Sistemi di modificazione e restrizione. Sequenza: GAATTC, è metilata sull'adenina iniziale nel DNA di coli (e nell'adenina palindroma). Un DNA esogeno non ha metilazioni. Ma non possiamo, anche inserendo EcoRI in MCS e poi inserendo in E. coli, avere funzionamento corretto. Perché verrebbe, il plasmide, identificato come esogeno e ristretto. Bisogna creare E. coli con mutazione sul proprio EcoRI (es. DH5alfa, in cui vi è una delezione), in modo che non sia attivo. Questo è necessario solo se gli enzimi di restrizione impiegati sono quelli presenti in E. coli, altrimenti non servono delezioni nel ceppo prima della "transfezione".

Sequenza GAATTC, palindroma, viene tagliata con estremità appiccicose (5' protruding): il plasmide da circolare diviene lineare. Appiccicose perchè permettendo alle sequenze di riapprocciarsi, si legano allo stesso modo (con legami idrogeno tra basi) presente in origine. La DNA ligasi, impiegando  rottura ATP (AMP liberata da idrolisi  ATP -> AMP + PPi , legata all'enzima, si lega al PO al 5', aumentando la sua carica parziale positiva, e attacco nucleofilo di O al 3' al fosfato, si rompe legame di P con OAMP, perchè se ne crea un'altro tra O al 3' e P, si rilascia AMP complessata a ligasi, altre, meno efficienti, sono NAD+ dipendenti) ligasi che ha legato AMP è cataliticamente attiva e la reazione può essere ripetuta più volte (ma è reversibile), ricuce i legami fosfodiesterici. Nella pratica introduciamo altri plasmidi

A seguito di DNA ligasi, sfruttiamo il principio di trasformazione (scoperto da griffin nel 1988? Rivedi anche la sezione sulla permeabilizzazione della membrana con calcio cloruro; replicazione a freddo, poi si attende una mezzoretta, poi si piastra su petri con agar in cui avviene duplicazione) della cellula batterica, in cui la cellula è in grado di inglobare DNA esterno all'interno del proprio citoplasma.

in altri casi la DNA ligasi può anche legare estremità piatte (blunt, non sfalsati i tagli): ma è poco efficiente, perchè deve avvenire una collisione, dunque qui la reazione avviene a 4 °C e si mantengono quelle condizioni per molte ore (credo di aver sentito). Esempio enzima SmaI. Ligazione avviene a temperature più basse anche nel caso delle sticky: se la temperatura fossero più alte, vi sarebbero continui "saltelli" degli strand non legati, e la legasi ha bisogno di stabilità. Ligasi però ha optimum a 37 gradi. Compromesso a 15-20 °C, e si aggiunge molta più ligasi. 

la reazione si fa in vitro dopo aver purificato la ligasi.

Normalmente basi sono 4 o 6. In rari casi sono 8, ma hanno alta percentuale CG. Se voglio clonare uso enzimi ad alta frequenza di taglio (come uno a 4 basi: 1/4^4 = 1/256 -> in media si trova ogni 256 basi nel genoma). Sopra i 10k basi comunque emergono problemi di integrazione nel plasmide: ci sono altre strategie, come la creazione di cromosomi artificiali.

Optimum tra quantità inserto e quantità vettore (plasmide): vedi tabella. Vogliamo che la reazione vada nella direzione dell'addizione dell'inserto e non la rilegazione (reversione a condizione iniziale del plasmide). Si esprime in termini di rapporto molare Insert/vector. **Optimum è a circa 3 molecole di inserto per una di vettore**: aumentando oltre, inserto si lega a sua volta all'inserto. Si ha la cosiddetta oligomerizzazione. Si valutano facendo screen visivi

come distinguiamo plasmide che si è richiuso da quello con inserimento? Colonie sono ampicillina resistenti portano il gene per resistenza. In più sono colorate diversamente (**in un colpo solo selezione e screen**, selezione è vita o morte, screening è eliminazione discrezionale di oggetti che non ci interessano). Perché quella ocn inserimento è blu? Inseriamo xgal (non è di per sè, ma vi è gruppo indolico) nei plasmidi, e in presenza di galattosidasi, vi è separazione di galattosio e la componente. Il MCS con modifiche interrompe, per costruzione, la continuità, (la trascrizione inizia, ma non verrà nella maggior parte dei casi, portata a termine la trascrizione - in più potrebbero esserci codoni di stop lungo la sequenza inserto): si inserisce all'interno della regione codificante della beta galattosidasi, nel suo sito di inizio. Dunque la beta galattosidasi si esprime solamente nei plasmidi senza inserimento (MCS è comunque inserita, ma rimane in registro (cioè venogno inseriti codoni interi - con basi in multiplo di tre) -> nel momento in cui introduciamo il costrutto, non in multiplo di 3, oppure potremmo avere delle codoni di stop, se la sequenza inserita è di un gene, avremo dei codoni otteniamo una frameshift che invalida tutta la struttura a valle). Si ripristina il registro ogni tanto (ma magari non funziona in maniera ottimale: vedi puntini sia bianchi che blu). Xgar è termolabile: va aggiunto a piastra già agarizzata: va spansa (vi saranno spot di disomogeneità). Per questo motivo si inserisce l'MCS a inizio enzima.

inserto è conseguente a clonaggio con per es. EcoR1. Poi estraggo DNA plasmidico e verifico che vi sia inserto: inseriamo plasmidi e EcoR1 e attendiamo digestione: otterremo su elettroforesi due bande per e nell'altro caso una banda con peso di vettore.

se DNA è circolare migra come superavvolto

a volte avviene mutazione nella regione della beta galattosidasi anche in assenza di inserzione e quindi lo screening lo mostra bianco, e selezione con ampicillina rimane all'esterno della MCS.

Questo avviene se non conosco sequenza

alcuni plasmidi avranon. Questo è clonaggio per amplificazione, se vogliamo un vettore di espressione ci interessa che siano tutti inseriti in un unico senso e possiamo ottenere ciò usando due sequenze di restrizione distinte a monte e valle.

---- 

# vettori di espressione (conosco sequenza?)


Si usa specialmente per esprimere proteine (per es. di Arabidopsis) in E. coli, perchè magari non ne produce abbastanza, oppure per analizzare una mutazione effettuata all'organismo di partenza

avremo sempre il passaggio in coli per amplificazione (abbiamo necessità di microgrammi di plasmide), un plasmide è 10k kbp (6.6 x 10^2 Da una bp) 1 mol di plasmide corrisponde a una massa di 6.6 tonnellate. 1 ug. 

abbiamo sempre ori e resistenza, oltre a sequenza artificiale, GST (glutatione S transferasi, trovata in un nematode). vi sono problemi di folding in E coli per proteine esogene. GST esprime proteine di fusione (porzione ammino terminale, con ORF continua nella porzione che vogliamo trascrivere)

GST non ha codone di stop (lo rimuoviamo, ma comincia con secondo codone dell'inserto: si crea proteina di fusione. inserto è scelto appositamente.

avremo promotore, esoni, introni, etc.; DNA Pol II. Nel trascritto vi è troncamento e aggiunta di Poly-A, mentre in cima viene aggiunto cappuccio (GPPP).

trascritto maturo (mRNA) ha la 5' UTR e 3' UTR dopo AUG e prima di UGA (o altro codone di stop). Sono due regioni non codificanti. La loro indispensabilità verrà

peso medio di un amminoacido: 110Da

nucleotide: 330Da

6000 nucleotidi di cui 750 nucleotidi codificanti nell'esempio fatto (mettiamo 2000 5' UTR e 3250 3' UTR): servono per il controllo della trascrizione.

Nel caso di una proteina di fusione GST-RbcL: inseriamo la ORF - AUG iniziale per la RbcL, dunque eliminiamo il primo codone (partiamo dal secondo amminoacido, non il primo che è sempre metionina, e normalmente viene rimossa, nei batteri è una formil-metionina).

ORF: open reading frame. registro di lettura aperto. sequenza interna a AUG -> UGA, in questo caso di 750 codoni. si tratta della sequenza codificante di un trascritto. ve n'è una sola (non sono sovrapposte, a parte ?). 

esistono 3 registri di lettura: modulo 3 (ampiezza codone). Però il registro parte solo se trova un AUG. Dunque per ciascun registro è associato un corrispondente AUG. Il corretto è quello che contiene il maggior numero di codoni associati ad amminoacidi (ossia otteniamo un stop codon non prematuro): si tratta dell'ORF più grande.

Tutti i trascritti hanno i 3 registri ma solo uno è produttivo.

con porzione di GST si ha mantenimento di struttura secondaria e terziaria, sia propria sia di ciò che segue

confronto estratti proteici estratti da ceppi di E.coli con plasmidi con espressione GST fusa a proteina. Questo consente la selezione? Perché all'espressione di proteine in coli solitamente segue la purificazione. Nell'elettroforesi vi sono centinaia di proteine visibili (le più abbondanti). La GST ci viene in soccorso: glutatione S transferasi trasferisce il glutatione (GSH) ridotto. Su una matrice (prodotta in lab, con legato GSH) GSH si lega alla GST, con altissima affinità. Dunque possiamo far sì che la proteina fusa si leghi alla membrana, previa incubazione. Questo può avvenire in una colonna, in cui poi si lava con soluzione fisiologica: si parla  di cromatografia per affinità. Per slegarla: C (resina) + Glu -> A + B (), 

inserendo glutatione ridotto libero, sposto l'equilibrio verso sx (GSH si lega a GST con alta affinità e essa si stacca da quello presente sulla resina)

proteina infilata in sacchetto con buchi, e tramite dialisi; glutatione riesce a transitare, ma proteina troppo ingmbrante. Glutatione è legato ma non covalentemente. GST è inerte (non interferisce con funzione proteica).

non devo aggiungere codone di stop.

promotore GST è un promotore inducibile (indotto da un determinato substrato)

Lac operone: operone lattosio: si attiva in presenza di lattosio (galattosio + glucosio si scindono). Si tratta di un insieme di enzimi che convertono e metabolizzano tale zucchero. Composto da 3 geni (tra cui beta-galattosidasi). Finché E coli usa come substrato energetico il saccarosio (credo), l'operone è inattivo. Il promotore è legato da un repressore (lacI) finchè non vi è lattosio. un isomero del lattosio entra nella cellula, intercetta repressore e lo rimuove dal promotore - perché cambia conformazione (su cui dovrebbero legar). qui operatore e non promotore, ma stesso concetto.

il vettore ha anche sequenza per il repressore lacI. il promotore di GST è regolato da una RNA polimerasi fagica che riconosce una specifica sequenza. all'attivazione repressore, repressore si lega anche a RNA polimerasi. 

IPTG (isopropiltiogalattoside)

T7 RNA polimerasi

tac promoter

lacI reprime anche la T7 RNA polimerasi lac

RNA batterica richiede 4 subunità, le fagiche hanno solo 1 polipeptide (più facili da esprimere) ma hanno legame specifico. promotore T7 contiene operatore lac a sua volta.

il tac promoter va sostituito nel caso in cui vogliamo introdurre il gene in una pianta (il tac è specifico per E. coli)

---

vettore reporter: esprime proteine che servono **per studiare sequenze regolatorie** (es. promoter) di un gene. TF tessuto-specifici li regolano.

I geni reporter sono associati alle sequenze regolatorie che vogliamo

uno è beta-galattosidasi (simil-reporter), oppure la GFP (green flourescent protein - se esposta a UV).

vediamo da screening le regioni in cui viene espresso il gene reporter. costrutto in cui la ORF di GFP è presente al suo interno.

supponiamo di studiare gene che non conosciamo ma che presumiamo espresso nella foglia e non in altri organi vegetali. otteniamo un callo di protoplasti, dopo aver plasmolizzato le cellule, su cui poi rigeneriamo con ormoni le pareti.

La tecnica più comune per transfezione è la gene-gun (con particelle di tungsteno)

esponendo pianta a UV, la foglia diventerà fluorescente selettivamente se promotore è tessuto-specifico. In tutte le altre regioni gene per GFP esiste ma non è espresso.

esistono vari colori per GFP. (EFP in generale? o IFP). GFP estratta da medusa

**finestra fenocritica**: momento esatto in cui un determinato gene viene acceso e spento per scatenare un effetto domino, e poi hanno espressione infinitesima; gli altri sono geni ad espressione costitutiva. Per questi geni con finestra fenocritica utilizziamo i reporter (es. primissima fase di formazione cotiledoni).

che cosa media la differenza di espressione nelle varie cellule? 

# Controllo dell'espressione genetica

Tre livelli:
- Interazione DNA-proteina
- regolazione trascrizionale (per es. splicing alternativo: varie combinazioni di esoni)
- regolazione post-trascrizionale 

Piante hanno 5 RNA pol (animali 3)

drosophila mangia lieviti e li deposita altrove, depone nella frutta

DSCAM: drosophila  cell avision molecule. proteina di membrana che è effettua alternative splicing: si generano mediamente 5 isoforme da un gene nell'uomo; in questo caso sono 38975, non tutte le isoforme sono espresse sulla membrana di un neurone, ma in realtà un solo isoforma per neurone. invalida un gene un trascritto; poi scoperto gene trascritto complesso (peptide). trascritto primario è lo stesso in tutte le cellule, la selezione dell'isoforma è ancora un mistero. Drosophila ha 14k geni, ciascuno ha almeno con supponiamo 2 isoforme: 2^14000 combinazioni. Ovviamente non tutte verranno sfruttate, ma le possibilità sono sconfinate. 

In una colonia di coli abbiamo circa 10^6 cellule. Ma ci sono strati con funzioni diverse (biofilm)

primo prodotto genico è trascritto, secondo è proteina. ma tra i due vi sono molte sottigliezze (splicing, quantità di trascritto, trasporto)

controllo trascrizionale processamente RNA trasporto nel citosol, degradazione (meccanismi per ), controllo traduzione, controllo della proteina. ci sono 176 circa modifiche post-tradizionale (es. acetilazione, metilazione), collocazione in un distretto cellulare.

Splicing e trascrizione sono concomitanti/contestualmente. poi cappiing, 3'poly A. esoni sono 100-200bp circa. mentre gli introni potrebbero anche essere lunghi 10kbp. 28k AA la più grande proteina.

Perchè questa differenza tra esoni e introni. Un introne enorme fa passare un sacco di tempo tra la trascrizione e splicing contestuale di due esoni che sono separati da tale enorme introne; se poi successivamente vi è un esone a breve distanza, possiam oavere splicing alternativo, se poi successivamente ci sono due altri grandi introni, non c'è possibilità di scelta (scelta obbligata perchè intercorre molto tempo nel frattempo)

16h può essere il tempo per trascrizione di trascritto primario di 3MBbp (distrofina). Nel caso di drosofila ci sono tantissimi esoni ravvicinati e intervallati da piccolissimi introni.


