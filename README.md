# Traduzione italiana di Stellaris

Questo mod, **compatibile** con la **modalità Ironman** e gli **achievement di Steam**, sostituisce la lingua inglese con la lingua italiana.

Compatibile con versione: **Butler 2.8.***

Sono attualmente tradotti tutti i DLC fino a Lithoids Species Pack e, in particolare grazie a [Nefando](https://github.com/Nefando), abbiamo anche una prima versione corposa del DLC Federations! Grazie a [AndryRock](https://github.com/AR-9217) in particolare per la traduzione DLC Necroids Species Pack e per aver avviato la prima versione della traduzione del DLC Federations.

A causa della modalità con la quale Stellaris effettua il check dei mod all'avvio, **per poter conservare la modalità Ironman e achievement non è possibile tradurre completamente tutte le frasi presenti nel gioco** (es. nomi delle navi, nomi degli alieni, nomi delle fazioni e delle città, ecc.). Inoltre, per facilitare il confronto con il resto del mondo, **non sono tradotti volutamente i nomi degli achievement ma solo la loro descrizione**. Se avete già completato gli achievement e la modalità Ironman, o comunque non siete interessati alla cosa, usate il [mod di MM_Winther](https://steamcommunity.com/sharedfiles/filedetails/?id=2377568450) per un'esperienza di traduzione completa. 

Questo mod nasce a maggio 2019 partendo dai testi tradotti diligentemente dal team Battle of Paradox Italia ed in particolare dal buon Puxxup - grande lavoro! - non con l'obiettivo di offrire una traduzione alternativa ma con quello di mantenere la compatibilità con achievements e modalità Ironman.

## Contribuire alla traduzione

Paradox aggiorna spesso i propri prodotti, non solo aggiungendo nuovi DLC e nuovi dialoghi, ma anche correggendo dove e quando serve quelli vecchi. Questo significa che è difficile avere una traduzione sempre aggiornata al 100% all'ultima release, quindi ogni aiuto con le traduzioni è ben accetto :)

Per come è strutturato il gioco, e poiché questo mod vuole mantenere gli achievement attivi, non è possibile aggiungere una lingua al gioco: l'unica alternativa per avere l'italiano è modificare una delle lingue disponibili. Per comodità quindi questo mod sovrascrive direttamente la lingua di default, ossia l'inglese. La fonte principale di frasi da tradurre di trova all'interno della cartella [src/mod/localisation/english](src/mod/localisation/english).

### Stato della traduzione

Di seguito i file principali e lo stato della loro traduzione rispetto alla versione 2.8.1 del gioco:

| nome file | stato traduzione |
|--|--|
|achievements_l_english.yml| completa|
|ai_crisis_l_english.yml| completa|
|ancient_relics_events_l_english.yml| parziale|
|ancient_relics_l_english.yml| parziale|
|apocalypse_l_english.yml| completa|
|dip_messages_l_english.yml| completa|
|diplo_stances_l_english.yml| completa|
|distant_stars_l_english.yml| completa|
|dlc_recommendations_l_english.yml| da tradurre|
|event_chains_l_english.yml| completa|
|events_2_l_english.yml| completa|
|events_3_l_english.yml| completa|
|events_4_l_english.yml| completa|
|events_5_l_english.yml| completa|
|events_l_english.yml| completa|
|federations_anniversary_l_english.yml| da tradurre|
|federations_l_english.yml| parziale|
|federations_resolution_comments_l_english.yml| completa|
|horizonsignal_l_english.yml| completa|
|l_english.yml| parziale|
|leviathans_l_english.yml| completa|
|lithoids_l_english.yml| completa|
|mandates_l_english.yml| completa|
|marauder_l_english.yml| completa|
|megacorp_l_english.yml| completa|
|messages_l_english.yml| completa|
|modifiers_2_l_english.yml| completa|
|modifiers_3_l_english.yml| completa|
|modifiers_l_english.yml| completa|
|modifiers_utopia_l_english.yml| completa|
|musicplayer_l_english.yml| completa|
|name_lists_l_english.yml| completa|
|necroids_l_english.yml| completa|
|new_scripted_loc_l_english.yml| completa|
|observer_events_l_english.yml| completa|
|observer_l_english.yml| completa|
|pop_factions_l_english.yml| completa|
|prescripted_l_english.yml| completa|
|projects_2_l_english.yml| completa|
|projects_3_l_english.yml| completa|
|projects_4_l_english.yml| completa|
|projects_5_l_english.yml| completa|
|projects_l_english.yml| completa|
|scripted_loc_l_english.yml| completa|
|ship_sections_l_english.yml| completa|
|social_gui_l_english.yml| completa|
|standalone_l_english.yml| completa|
|synthetic_dawn_events_l_english.yml| completa|
|technology_l_english.yml| completa|
|traditions_l_english.yml| parziale|
|triggers_effects_l_english.yml| parziale|
|tutorial_l_english.yml| parziale|
|unrest_l_english.yml| completa|
|utopia_ascension_l_english.yml| completa|
|utopia_l_english.yml| completa|
|utopia_megastructures_l_english.yml| completa|

### Cosa posso modificare?

Tutto quello che trovate qui su GitHub è già traducibile senza rischi di disattivare la modalità Ironman e gli achievement, e in particolare i file che verranno sovrapposti a quelli del gioco si trovano tutti all'interno del percorso [src/mod](/src/mod).

Se dovesse servire invece aggiungere un file non ancora presente su questo repository, prima di modificarlo bisogna assicurarsi che non sia incluso nella lista di file che vengono controllati all'avvio del gioco.

Il file che indica a Stellaris la lista dei file _intoccabili_ si chiama `checksum_manifest.txt` e si trova all'interno della cartella principale di gioco. Attualmente il contenuto del file è il seguente:

```
directory 
name = common
sub_directories = yes
file_extension = .txt

directory 
name = common
sub_directories = yes
file_extension = .lua

directory
name = common
sub_directories = yes
file_extension = .csv

directory
name = events
sub_directories = yes
file_extension = .txt

directory
name = map
sub_directories = yes
file_extension = .lua

directory
name = map
sub_directories = yes
file_extension = .txt

directory
name = localisation_synced
sub_directories = yes
file_extension = .yml
```

Prendendo ad esempio la prima sezione, significa che all'avvio del gioco verranno controllati tutti i file `.txt` all'interno della cartella `common` e tutte le sue sotto cartelle. Se anche solo un file di questo tipo viene modificato, il controllo fallisce e il gioco impedisce l'attivazione della modalità Ironman e degli achievement. E lo stesso vale per tutte le altre sezioni indicate nel file di checksum.

### Chiavi e valori

Ogni file contiene delle stringhe formate da una chiave, uguale per ogni linguaggio, e dalla sua traduzione corrispondente. Es. all'interno del file [ai_crisis_l_english.yml](src/mod/localisation/english/ai_crisis_l_english.yml) si trova la linea:

```yml
crisis.2010.name:0 "Il Segnale Fantasma"
```

In questo caso `crisis.2010.name:0` è la chiave, mentre `"Il Segnale Fantasma"` è la traduzione. Da notare i doppi apici `"` che delimitano il valore vero e proprio della traduzione, in questo caso già tradotto.

### Commenti

Le linee che iniziano con il carattere speciale `#` sono dei commenti o delle frasi non più utilizzate. **Non sono da tradurre** perché non verranno mai visualizzate all'interno del gioco.

### Una riga, una traduzione

Non andate a capo durante la traduzione di un testo. Se serve andare a capo, si utilizza il doppio carattere speciale `\n\n` Lo vedrete utilizzare anche nella frase originale inglese, ma potrete usare il carattere per andare a capo in italiano dove preferite, non necessariamente nella stessa posizione della frase originale.

### Caratteri speciali

Alcune frasi contengono caratteri speciali quali `§H` oppure `§!`. **Non devono essere tradotti o rimossi**, il gioco li utilizza per dare enfasi alle frasi del gioco. Immaginate come se fossero dei delimitatori per le parole da mettere in grassetto, con `§H` che significa inizio grassetto e `§!` fine grassetto

### Variabili

Alcune frasi contengono delle variabili che possono essere racchiuse tra parentesi quadre - ad esempio `[Root.Capital.GetName]` - o dal carattere del dollaro - ad esempio `$ancrel.8010.intro$`. Queste parole **non vanno tradotte**: il gioco le sostituirà automaticamente in tempo reale con il valore corretto. **NOTA:** Alcune variabili in italiano vi creeranno problemi, in particolare tutte quelle che prevedono un articolo davanti, perché in italiano non sappiamo esattamente quale usare in anticipo. Prendete ad esempio la seguente frase:

```yml
mirror_trade_reply:0 "I was about to suggest that myself, for the benefit of all [Root.Owner.Species.GetNamePlural]!"
```

La traduzione corretta sarebbe:

```yml
mirror_trade_reply:0 "Stavo per suggerirlo io stesso, a beneficio di tutti/e i/gli/le [Root.Owner.Species.GetNamePlural]!"
```

Come potete notare, in inglese `the`, `of all`, ecc. funzionano praticamente sempre bene per tutto - _...of all Humanoids_, _...of all Reptilians_, ecc. - ma in italiano la specie potrebbe essere ad esempio "i Rettiliani", "gli Umanoidi", ecc. E questo solo per citare le specie esistenti e definite all'interno del file [name_lists_l_english.yml](src/mod/localisation/english/name_lists_l_english.yml). Ma in questo gioco anche l'utente può definire le sue specie personalizzate, quindi non lo sapremo mai con certezza a priori. Il gioco possiede variabili per il singolare e il plurale, ma non ad esempio per la differenza tra gli articoli da utilizzare.

Una possibile soluzione è quella di prenderci qualche libertà durante la traduzione e scrivere ad esempio:

```yml
mirror_trade_reply:0 "Stavo per suggerirlo io stesso, a beneficio di tutto il popolo [Root.Owner.Species.GetAdj]!"
```

In questo caso non solo ho aggiunto la parola `popolo`, ma ho usato la variabile utilizzata per definire l'aggettivo caratteristico della specie. All'interno del gioco quindi questa frase verrebbe tradotta con `popolo Rettiliano` o `popolo Umanoide`.

In generale, se vi trovate in una impasse sulla possibile traduzione, provate a vedere come è stato fatto in altri punti e seguite la stessa strada. Altrimenti aprite una segnalazione sul repo e discutiamo delle possibili traduzioni.

### Codifica dei caratteri

**La codifica dei caratteri (charset) deve essere UTF-8 con BOM**. Per sicurezza utilizzate direttamente un editor di testo che supporti più charset come ad esempio [Notepad++](https://notepad-plus-plus.org/downloads/) e il charset corretto verrà riconosciuto senza problemi.

Da notare inoltre che i file di testo possono utilizzare dei caratteri speciali all'inizio per determinare l'ordine di scrittura dei byte (il [BOM](https://it.wikipedia.org/wiki/Byte_Order_Mark)). Usando il metodo del _copia e incolla_ questo dettaglio è trascurabile, e solitamente anche se si modificano file esistenti l'editor non tocca il BOM se è presente. Se avete comunque un editor che vi permette di scegliere se applicare o meno il BOM, es. Notepad++ o Visual Studio Code, optate sempre per mantenerlo.

![Notepad++ con codifica "UTF-8-BOM"](meta/10.png)

![Visual Studio Code con codifica "UTF-8 with BOM"](meta/11.png)

### Ok, capito, ma come modifico i file?

Per contribuire alle traduzioni, potete clonare questo repository, aggiornare direttamente i file e poi procedere con una pull request per effettuare l'unione del vostro repository con quello principale.

Se non siete pratici di `git`, il mio suggerimento è di diventarlo :) E' veramente semplice da utilizzare e vi permette di lavorare in locale sul vostro PC.

Un'alternativa, è lavorare comunque sul vostro PC ma effettuare la proposta di modifica direttamente online. Una volta scaricato e tradotto il file che volete aggiornare:

1. Tornate su questo repository, assicuratevi di essere sul branch **dev**
![](meta/01.png)

1. Navigate fino al file che volete aggiornare e premete l'icona in alto a destra per la modifica, la matita che dice "Edit this file"
![](meta/02.png)

1. GitHub vi avverte che non avete permessi di scrittura sul repo, che verrà creato un repository uguale a questo sulla vostra utenza e che verrà creato un nuovo ramo con le vostre modifiche. A quel punto, potrete proporre una pull request sul repository principale. Fate una modifica puntuale o, in caso di modifiche multiple, direttamente copia e incolla di tutto il contenuto del vostro file aggiornato
![](meta/03.png)

1. premete `Preview changes` per verificare che le modifiche siano quelle che vi aspettate. Se è tutto ok, inserite un messaggio che descrive brevemente la vostra modifica e premete **Propose file change**
![](meta/04.png)

1. A questo punto avete aggiornato il vostro repository, e potete procedere con la proposta di unione. Premete il pulsante **Create pull request**, modificate il testo del commit - se per qualche motivo volete cambiare il testo rispetto a quanto avete inserito precedentemente - e poi premete nuovamente **Create pull request** per confermate
![](meta/05.png) ![](meta/06.png)

1. La vostra pull request è stata inoltrata correttamente, risulta in stato aperto (_Open_) e non dovrebbe dare errori di unione (_This branch has no conflicts with the base branch_)
![](meta/07.png)

1. Attendete che la PR sia accettata e unita

1. _Opzionale_. Una volta accetta la vostra PR sarà chiusa (_Closed_) e il vostro ramo con la modifica unito (_Merged_) a quello principale. Potete quindi decidere di cancellare il ramo che è rimasto nel vostro repository, visto che ha assolto al proprio compito di proporre la modifica che è stata accettata
![](meta/08.png) ![](meta/09.png)

## Installazione mod da release

Trovate le release già pronte del mod nell'apposita sezione [releases](https://github.com/Neurone/stellaris-italian-translation/releases). Scaricate la release che vi interessa e decomprimetela all'interno della cartella:

    <%USERPROFILE%>\Documents\Paradox Interactive\Stellaris\mod

Nel caso non fosse presente la cartella `mod` potete crearla voi normalmente.

## Creazione mod da codice sorgente

Clonare il repository:

    git clone https://github.com/Neurone/stellaris-italian-translation.git

Installare le dipendenze:

    cd stellaris-italian-translation
    npm install

### Versione release

Creare il mod:

    npx grunt

L'output sarà simile al seguente:

    ~\stellaris-italian-translation> npx grunt
    npx: installed 1 in 2.252s
    Path must be a string. Received undefined
    ~\stellaris-italian-translation\node_modules\grunt\bin\grunt
    Running "clean:folder" (clean) task
    >> 91 paths cleaned.

    Running "copy:standalone" (copy) task
    Created 1 directory, copied 86 files

    Running "compress:main" (compress) task
    >> Compressed 87 files.

    Running "copy:complete" (copy) task
    Copied 1 file

    Done.

Verrà creato il file `stellaris-italian-translation-x.x.x.zip` all'interno della cartella `build\dist`, dove `x.x.x` sarà la versione corrente del mod (es. `1.0.0`).

Per installare il mod, scompattare il file all'interno della cartella:

    <%USERPROFILE%>\Documents\Paradox Interactive\Stellaris\mod

Nel caso non fosse presente la cartella `mod` potete crearla voi normalmente. La struttura finale dei file sarà la seguente:

    <%USERPROFILE%>\Documents\Paradox Interactive\Stellaris\mod\stellaris-italian-translation.zip
    <%USERPROFILE%>\Documents\Paradox Interactive\Stellaris\mod\stellaris-italian-translation.mod

### Versione sviluppo o Steam

La versione sviluppo del mod è utile per fare modifiche, test o per effettuare il caricamento sullo Steam Workshop. La versione release **non permette** di fare il caricamento sullo Steam Workshop.

Creare il mod in versione sviluppo:

    npx grunt dev

L'output sarà simile al seguente:

    ~\stellaris-italian-translation> npx grunt dev
    npx: installed 1 in 2.625s
    Path must be a string. Received undefined
    ~\stellaris-italian-translation\node_modules\grunt\bin\grunt
    Running "clean:folder" (clean) task
    >> 0 paths cleaned.

    Running "copy:dev" (copy) task


    Done.

Verrà creata la cartella `build\dist` e all'interno troverete un file ed una cartella:

    stellaris-italian-translation\*
    stellaris-italian-translation.mod

Per installare il mod, copiate tutto **il contenuto** della cartella `build\dist` all'interno della cartella:

    <%USERPROFILE%>\Documents\Paradox Interactive\Stellaris\mod

Nel caso non fosse presente la cartella `mod` potete crearla voi normalmente. La struttura finale dei file sarà la seguente:

    <%USERPROFILE%>\Documents\Paradox Interactive\Stellaris\mod\stellaris-italian-translation\...
    <%USERPROFILE%>\Documents\Paradox Interactive\Stellaris\mod\stellaris-italian-translation.mod
