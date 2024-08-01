# Nome del Problema: transposition-trial

## Descrizione

Per trovare la flag ho dovuto scaricare il file fornito. Il problema parlava di una corruzione di dati che non ha sostituito valori, ma li ha solo messi in disordine. L'unica informazione aggiuntiva era che la prima parola era composta da 3 caratteri.

## Passaggi

### Step 1: Scaricare il File

Ho scaricato il file contenente la stringa corrotta. La stringa fornita era: `heTfl_g_as_iicpCTo{7F4NRP051N5_16_35P3X51N3_V091B0AE}2`.

### Step 2: Comprensione del Problema

Ho capito che la corruzione dei dati era una trasposizione, non una sostituzione. L'informazione chiave era che la prima parola era composta da 3 caratteri. Questo mi ha suggerito di suddividere la stringa in blocchi di 3 caratteri.

### Step 3: Suddivisione della Stringa

Ho scritto uno script Python per suddividere la stringa in blocchi di 3 caratteri:

```python
def split_into_chunks(input_string, chunk_size):
    chunks = [input_string[i:i + chunk_size] for i in range(0, len(input_string), chunk_size)]
    return chunks

split_string = "heTfl_g_as_iicpCTo{7F4NRP051N5_16_35P3X51N3_V091B0AE}2"
split_string = split_string.replace(" ", "")

chunks = split_into_chunks(split_string, 3)
```

Questo codice ha prodotto il seguente output: ['heT', 'flg', 'asi', 'icp', 'CTo', '{7F', '4NR', 'P05', '1N5', '_16', '_35', 'P3X', '51N', '3_V', '091', 'B0A', 'E}2'].

### Step 4: Riordinamento dei Blocchi

Ho osservato che la logica del riordinamento era di prendere l'ultima lettera e posizionarla prima delle altre due. Ho quindi aggiunto un altro pezzo di codice per riordinare i blocchi:

```python
def order_chunks(chunks):
    return ''.join([chunk[2] + chunk[0] + chunk[1] for chunk in chunks])

reordered_string = order_chunks(chunks)
print(reordered_string)
```

### Step 5: Trovare la Flag

Eseguendo il codice, ho ottenuto la seguente stringa riordinata: The_flag_is_picoCTF{7R4N5P051N6_15_3XP3N51V3_109AB02E}. Da questa stringa, ho estratto manualmente la flag: picoCTF{7R4N5P051N6_15_3XP3N51V3_109AB02E}.

## Risultato Finale

La flag trovata è: `picoCTF{7R4N5P051N6_15_3XP3N51V3_109AB02E}`

## Comandi Utilizzati

Non sono stati utilizzati comandi specifici, ma uno script Python per riordinare i dati trasposti.

## Conclusione

Il problema è stato risolto riconoscendo che i dati erano stati trasposti in blocchi di 3 caratteri. Utilizzando uno script Python, ho suddiviso la stringa e riordinato i blocchi per ottenere il testo corretto e la flag. La comprensione delle tecniche di trasposizione e la capacità di scrivere script Python sono state fondamentali per risolvere il problema.
Se hai altre richieste o modifiche, fammi sapere!
