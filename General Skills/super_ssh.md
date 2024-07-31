# Nome del Problema: Super SSH

## Descrizione

Per trovare la flag ho eseguito una connessione SSH, ovvero una connessione remota criptata. Secure Shell (SSH) è il sostituto di Telnet e si forma in questo modo: `ssh user@host -p port`. Potrebbe essere richiesta una password come in questo problema. Una volta connesso, mi è stata fornita la flag.

## Passaggi

### Step 1: Connessione SSH

Ho stabilito una connessione SSH utilizzando il comando:
ssh user@host -p port

### Step 2: Autenticazione

Durante la connessione, mi è stata richiesta una password. Dopo aver inserito la password corretta, la connessione è stata stabilita.

### Step 3: Ottenimento della Flag

Una volta connesso al server remoto, mi è stata fornita la flag:
picoCTF{s3cur3_c0nn3ct10n_8306c99d}

## Risultato Finale

La flag trovata è:
picoCTF{s3cur3_c0nn3ct10n_8306c99d}

## Comandi Utilizzati

1. Connessione SSH: ssh user@host -p port

## Conclusione

Il problema è stato risolto attraverso l'uso di una connessione SSH. La comprensione di come stabilire una connessione remota sicura è stata fondamentale per trovare la flag nascosta.
