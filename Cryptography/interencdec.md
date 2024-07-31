# Nome del Problema: Interencdec

## Descrizione

Per trovare la flag ho dovuto aprire il file che viene fornito, ovvero `enc_flag`. Viene fornita una prima stringa: YidkM0JxZGtwQlRYdHFhR3g2YUhsZmF6TnFlVGwzWVROclh6ZzJhMnd6TW1zeWZRPT0nCg==

## Passaggi

### Step 1: Decodifica Base64

Ho provato a usare un decoder online per decodificare la stringa e come risultato ho ottenuto: b'd3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzg2a2wzMmsyfQ=='

### Step 2: Decodifica Ulteriore

Sembra che non siamo ancora giunti a un risultato, poiché la flag potrebbe essere stata criptata più volte. Ho provato nuovamente a eseguire la conversione e ho ottenuto un nulla di fatto: m)5}݄ͩͭ|٭ɬ

### Step 3: Estrarre Parte Tra Apici

Ho dato un'ulteriore visione alla stringa che avevo ottenuto e ho provato a prendere solamente la parte tra gli apici. In questa prova ho ottenuto: wpjvJAM{jhlzhy_k3jy9wa3k_86kl32k2}

### Step 4: Decrittazione Cesare

Mi sono reso conto di essere molto vicino, ma manca ancora qualcosa. Sembra una cifratura di Cesare. Provando la conversione, sono arrivato a: picoCTF{caesar_d3cr9pt3d_86de32d2}

## Risultato Finale

La flag trovata è: `picoCTF{caesar_d3cr9pt3d_86de32d2}`

## Comandi Utilizzati

1. Decodifica Base64 (prima volta):
echo "YidkM0JxZGtwQlRYdHFhR3g2YUhsZmF6TnFlVGwzWVROclh6ZzJhMnd6TW1zeWZRPT0nCg==" | base64 --decode
2. Decodifica Base64 (seconda volta):
echo "d3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzg2a2wzMmsyfQ==" | base64 --decode
3. Decrittazione Cesare:
Ho utilizzato uno strumento di decrittazione di Cesare per ottenere la flag finale.

## Conclusione

Il problema è stato risolto attraverso una serie di decodifiche e una decrittazione di Cesare. Ogni passo è stato fondamentale per raggiungere il risultato finale e trovare la flag nascosta.
