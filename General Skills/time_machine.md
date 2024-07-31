# Nome del Problema: Time Machine

## Descrizione

Per trovare la flag ho aperto il file `message.txt` che suggeriva di guardare i commit fatti. Ho quindi esplorato la cartella `.git` dove risiedono queste informazioni.

## Passaggi

### Step 1: Apertura del File `message.txt`

Ho aperto il file `message.txt` che conteneva il suggerimento di guardare i commit fatti.

### Step 2: Esplorazione della Cartella `.git`

Ho aperto la cartella `.git` che contiene tutte le informazioni relative ai commit.

### Step 3: Apertura del File `COMMIT_EDITMSG`

All'interno della cartella `.git`, ho trovato e aperto il file `COMMIT_EDITMSG` che conteneva la flag.

### Step 4: Ottenimento della Flag

All'interno del file `COMMIT_EDITMSG`, ho trovato la flag:
picoCTF{t1m3m@ch1n3_e8c98b3a}

## Risultato Finale

La flag trovata è:
picoCTF{t1m3m@ch1n3_e8c98b3a}

## Comandi Utilizzati

Non sono stati utilizzati comandi specifici per risolvere questo problema. La soluzione è stata ottenuta esplorando manualmente i file all'interno della cartella `.git`.

## Conclusione

Il problema è stato risolto esplorando la struttura della cartella `.git` e trovando la flag nel file `COMMIT_EDITMSG`. La comprensione del funzionamento dei repository Git è stata fondamentale per trovare la flag nascosta.
