# Nome del Problema: HideToSee

## Descrizione

Per trovare la flag ho scaricato l'immagine fornita. Ho scoperto che attraverso una tecnica chiamata steganografia si possono inserire dati nascosti all'interno delle immagini. Ho utilizzato un comando da linea di comando chiamato `steghide` per estrarre i dati nascosti.

## Passaggi

### Step 1: Scaricare l'Immagine

Ho scaricato l'immagine `atbash.jpg` fornita dal problema.

### Step 2: Utilizzo della Steganografia

Sapendo che la steganografia permette di nascondere dati nelle immagini, ho cercato uno strumento adatto e ho trovato `steghide`, un tool da linea di comando.

### Step 3: Estrarre i Dati Nascosti

Ho usato il comando `steghide` per estrarre i dati nascosti nell'immagine. Il comando utilizzato è stato:

```sh
steghide extract -sf atbash.jpg
```

Fortunatamente, non è stata necessaria alcuna passkey. Questo comando ha generato un file chiamato encrypted.txt.

### Step 4: Decodifica del Testo Estratto

All'interno del file encrypted.txt, ho trovato la stringa krxlXGU{zgyzhs_xizxp_92533667}. Sapendo che si trattava di un testo cifrato con il Cifrario di Atbash, sono andato su un decodificatore online del Cifrario di Atbash e ho inserito il testo.

### Step 5: Trovare la Flag

Dopo aver decodificato il testo con il Cifrario di Atbash, ho ottenuto la flag: picoCTF{atbash_crack_92533667}.

## Risultato Finale

La flag trovata è: `picoCTF{atbash_crack_92533667}`

## Comandi Utilizzati

Il comando utilizzato per estrarre i dati nascosti è stato:

```sh
steghide extract -sf atbash.jpg
```

## Conclusione

Il problema è stato risolto utilizzando la tecnica della steganografia per estrarre dati nascosti da un'immagine. Successivamente, ho decodificato il testo cifrato con il Cifrario di Atbash per ottenere la flag. La conoscenza della steganografia e dei cifrari di sostituzione è stata fondamentale per trovare la flag nascosta.
