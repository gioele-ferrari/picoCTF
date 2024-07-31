# Nome del Problema: Endianness

## Descrizione

Per trovare la flag ho convertito la parola fornita dal programma: `mjaar`, per prima cosa ho convertito in esadecimale la parola fornita e ho ottenuto: `6d6a616172`. Le rappresentazioni Little Endian e Big Endian sono due metodi usati per salvare i byte che compongono una parola. Little Endian significa che partiamo dal LSB per salvare la parola, al contrario Big Endian significa che partiamo dal MSB per salvare la parola. Ad esempio, la nostra parola è composta dai seguenti byte: `0x6d, 0x6a, 0x61, 0x61, 0x72` in base al tipo partiamo dal fondo o dalla testa:

## Little Endian

| Address | Data  |
|---------|-------|
| 0x00    | 0x72  |
| 0x01    | 0x61  |
| 0x02    | 0x61  |
| 0x03    | 0x6a  |
| 0x04    | 0x6d  |

## Big Endian

| Address | Data  |
|---------|-------|
| 0x00    | 0x6d  |
| 0x01    | 0x6a  |
| 0x02    | 0x61  |
| 0x03    | 0x61  |
| 0x04    | 0x72  |

## Passaggi

### Step 1: Conversione in Esadecimale

La parola `mjaar` è stata convertita in esadecimale ottenendo `6d6a616172`.

### Step 2: Rappresentazione Little Endian

La parola viene rappresentata in Little Endian come:

| Address | Data  |
|---------|-------|
| 0x00    | 0x72  |
| 0x01    | 0x61  |
| 0x02    | 0x61  |
| 0x03    | 0x6a  |
| 0x04    | 0x6d  |

### Step 3: Rappresentazione Big Endian

La parola viene rappresentata in Big Endian come:

| Address | Data  |
|---------|-------|
| 0x00    | 0x6d  |
| 0x01    | 0x6a  |
| 0x02    | 0x61  |
| 0x03    | 0x61  |
| 0x04    | 0x72  |

### Step 4: Inserimento dei Byte nel Programma

Inserendo nel programma i byte in maniera corretta otteniamo: picoCTF{3ndi4n_sw4p_su33ess_817b7cfe}

## Risultato Finale

La flag trovata è: `picoCTF{3ndi4n_sw4p_su33ess_817b7cfe}`

## Conclusione

Il problema è stato risolto attraverso la comprensione delle rappresentazioni Little Endian e Big Endian. Ogni passo è stato fondamentale per raggiungere il risultato finale e trovare la flag nascosta.
