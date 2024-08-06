# Nome del Problema: substitution0

## Descrizione

Per trovare la flag ho dovuto scaricare il file fornito dal problema che conteneva un testo cifrato. Ho notato che alla fine del testo era chiaramente presente la flag. Questo mi ha portato a considerare che il testo fosse cifrato con un metodo di sostituzione.

## Passaggi

### Step 1: Scaricare il File

Ho scaricato il file che conteneva il seguente testo cifrato:

```text
DECKFMYIQJRWTZPXGNABUSOLVH

Ifnfuxpz Wfyndzk dnpaf, oqbi d yndsf dzk abdbfwv dqn, dzk enpuyib tf bif effbwf
mnpt d ywdaa cdaf qz oiqci qb oda fzcwpafk. Qb oda d efdubqmuw acdndedfua, dzk, db
bidb bqtf, uzrzpoz bp zdbundwqaba—pm cpunaf d ynfdb xnqhf qz d acqfzbqmqc xpqzb
pm sqfo. Bifnf ofnf bop npuzk ewdcr axpba zfdn pzf flbnftqbv pm bif edcr, dzk d
wpzy pzf zfdn bif pbifn. Bif acdwfa ofnf flcffkqzywv idnk dzk ywpaav, oqbi dww bif
dxxfdndzcf pm eunzqaifk ypwk. Bif ofqyib pm bif qzafcb oda sfnv nftdnrdewf, dzk,
bdrqzy dww biqzya qzbp cpzaqkfndbqpz, Q cpuwk idnkwv ewdtf Juxqbfn mpn iqa pxqzqpz
nfaxfcbqzy qb.

Bif mwdy qa: xqcpCBM{5UE5717U710Z_3S0WU710Z_59533D2F}
```

### Step 2: Identificazione del Metodo di Cifratura

Ho notato che la prima riga del file conteneva una stringa con esattamente 26 caratteri: `DECKFMYIQJRWTZPXGNABUSOLVH`. Questo mi ha suggerito l'uso di una cifratura a sostituzione, dove ogni lettera dell'alfabeto è sostituita da un'altra lettera secondo una chiave specifica.

### Step 3: Utilizzo di un Decoder Online

Ho utilizzato un decoder online per decifrare il testo, usando la stringa della prima riga come chiave di sostituzione. Il testo decifrato è risultato essere:

```text
HEREUPON LEGRAND AROSE, WITH A GRAVE AND STATELY AIR, AND BROUGHT ME THE BEETLE FROM A GLASS CASE IN WHICH IT WAS ENCLOSED. IT WAS A BEAUTIFUL SCARABAEUS, AND, AT THAT TIME, UNKNOWN TO NATURALISTS--OF COURSE A GREAT PRIJE IN A SCIENTIFIC POINT OF VIEW. THERE WERE TWO ROUND BLACK SPOTS NEAR ONE EXTREMITY OF THE BACK, AND A LONG ONE NEAR THE OTHER. THE SCALES WERE EXCEEDINGLY HARD AND GLOSSY, WITH ALL THE APPEARANCE OF BURNISHED GOLD. THE WEIGHT OF THE INSECT WAS VERY REMARKABLE, AND, TAKING ALL THINGS INTO CONSIDERATION, I COULD HARDLY BLAME QUPITER FOR HIS OPINION RESPECTING IT. THE FLAG IS: PICOCTF{5UB5717U710N_3V0LU710N_59533A2E}
```

### Step 4: Estrarre la Flag

Dopo aver decifrato il testo, ho individuato la flag alla fine del testo: `PICOCTF{5UB5717U710N_3V0LU710N_59533A2E}`.

## Risultato Finale

La flag trovata è: `PICOCTF{5UB5717U710N_3V0LU710N_59533A2E}`

## Comandi Utilizzati

Non sono stati utilizzati comandi specifici, ma un decoder online per cifrature a sostituzione.

## Conclusione

Il problema è stato risolto riconoscendo l'uso di una cifratura a sostituzione. Utilizzando la stringa chiave fornita nel file, ho decifrato il testo con un decoder online e ho individuato la flag nascosta alla fine del testo. La comprensione delle cifrature a sostituzione è stata fondamentale per risolvere il problema.
