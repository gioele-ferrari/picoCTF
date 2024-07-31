# Nome del Problema: ReadMyCert

## Descrizione

Per trovare la flag ho dovuto capire cosa fosse un file CSR. Un CSR (Certificate Signing Request) è un file generato dalla propria chiave privata per richiedere un certificato da una CA (Certificate Authority). Contiene le informazioni principali dell'ente che ha generato il file.

## Passaggi

### Step 1: Comprensione del CSR

Ho iniziato documentandomi sui file CSR. Ho appreso che un CSR è utilizzato per richiedere un certificato SSL ed è generato a partire da una chiave privata. Questo file contiene informazioni come il nome del dominio, l'organizzazione e la località.

### Step 2: Decifrazione del CSR

Successivamente, ho cercato un decifratore di CSR online. Ho trovato uno strumento che permette di decifrare il contenuto di un file CSR e ho caricato il file fornito nel problema.

### Step 3: Trovare la Flag

Dopo aver inserito il CSR nel decifratore, ho analizzato il summary del file decifrato. Ho trovato la flag `picoCTF{read_mycert_5aeb0d4f}` all'interno del summary.

## Risultato Finale

La flag trovata è: `picoCTF{read_mycert_5aeb0d4f}`

## Comandi Utilizzati

Non sono stati utilizzati comandi specifici per risolvere questo problema. La soluzione è stata ottenuta utilizzando un decifratore di CSR online.

## Conclusione

Il problema è stato risolto comprendendo il significato di un file CSR e utilizzando uno strumento online per decifrare il suo contenuto. La flag è stata trovata all'interno del summary del file decifrato. La conoscenza dei file CSR e l'uso degli strumenti di decifrazione sono stati fondamentali per trovare la flag nascosta.
