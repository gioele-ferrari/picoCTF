# Nome del Problema: Rotation

## Descrizione

Per trovare la flag ho dovuto aprire il file fornito `encrypted.txt` e ho trovato al suo interno una stringa cifrata:
xqkwKBN{z0bib1wv_l3kzgxb3l_4k71n5j0}

Ho subito capito che si trattava di una stringa cifrata con il metodo di Cesare, ovvero con un numero di shift sull'intera stringa di caratteri.

## Passaggi

### Step 1: Apertura del File `encrypted.txt`

Ho aperto il file `encrypted.txt` e ho trovato la stringa cifrata al suo interno.

### Step 2: Identificazione del Metodo di Cifratura

Ho riconosciuto che la stringa era cifrata utilizzando il metodo di Cesare, che prevede uno shift dei caratteri.

### Step 3: Decodifica della Stringa

Ho utilizzato un cifratore online per decifrare la stringa. Inserendo la stringa cifrata e provando diversi valori di shift, ho trovato la flag:
picoCTF{r0tat1on_d3crypt3d_4c71f5b0}

## Risultato Finale

La flag trovata è: `picoCTF{r0tat1on_d3crypt3d_4c71f5b0}`

## Comandi Utilizzati

Non sono stati utilizzati comandi specifici per risolvere questo problema. La soluzione è stata ottenuta utilizzando un cifratore online per il metodo di Cesare.

## Conclusione

Il problema è stato risolto riconoscendo la cifratura di Cesare nella stringa trovata nel file `encrypted.txt` e decodificando la stringa con uno strumento online. La comprensione del metodo di cifratura di Cesare è stata fondamentale per trovare la flag nascosta.
