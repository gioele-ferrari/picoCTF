# Nome del Problema: basic-mod1

## Descrizione

Per trovare la flag ho dovuto scaricare il file fornito dal problema, il quale conteneva una sequenza di numeri. La sequenza era la seguente:

350 63 353 198 114 369 346 184 202 322 94 235 114 110 185 188 225 212 366 374 261 213

Il problema richiedeva di eseguire il modulo 37 su ogni valore della sequenza e di assegnare un carattere alfabetico o numerico in base al risultato del modulo. La mappatura era la seguente:

- Da 0 a 25: Lettere dalla A alla Z
- Da 26 a 35: Numeri da 0 a 9
- 36: Carattere "_"

## Passaggi

### Step 1: Scaricare il File

Ho scaricato il file contenente la sequenza di numeri.

### Step 2: Analisi del Problema

Ho capito che dovevo eseguire il modulo 37 su ogni valore della sequenza e mappare i risultati a caratteri specifici in base alla seguente logica:

- 0-25: A-Z
- 26-35: 0-9
- 36: _

### Step 3: Scrivere lo Script di Decodifica

Ho scritto uno script Python per eseguire il modulo 37 su ogni numero e mappare i risultati ai caratteri appropriati. Il codice dello script è il seguente:

```python
def decode(number):
    return number % 37

def create_flag():
    file = open("message.txt", "r").read()
    content = [decode(int(value)) for value in file.split()]

    mapping = {i: chr(65 + i) for i in range(26)}  # A-Z
    mapping.update({i + 26: str(i) for i in range(10)})  # 0-9
    mapping[36] = "_"  # _

    flag = "".join(mapping[value] for value in content)
    return flag

print("picoCTF{" + create_flag() + "}")
```

### Step 4: Eseguire lo Script

Ho eseguito lo script, che ha prodotto la seguente flag: picoCTF{R0UND_N_R0UND_ADD17EC2}.

## Risultato Finale

La flag trovata è: `picoCTF{R0UND_N_R0UND_ADD17EC2}`

## Comandi Utilizzati

Non sono stati utilizzati comandi specifici, ma uno script Python per decodificare la sequenza di numeri.

## Conclusione

Il problema è stato risolto eseguendo il modulo 37 su ogni valore della sequenza numerica fornita e mappando i risultati ai caratteri appropriati. Utilizzando uno script Python, ho ottenuto la flag corretta. La comprensione dei concetti di modulo e mappatura dei caratteri è stata fondamentale per risolvere il problema.
