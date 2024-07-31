# Endianness

Per trovare la flag ho convertito la parola fornita dal programma: mjaar, per prima cosa ho convertito in esadecimale
la parola fornita e ho ottenuto: 6d6a616172. Le rappresentazioni Little Endian e Big Endian sono due metodi usati per
salvare i byte che compongono una parola. Little Endian significa che partiamo dal LSB per salvare la parola, al contrario Big Endian significa che partiamo dal MSB per salvare la parola.
Ad esempio la nostra parola è composta dai seguenti byte: 0x6d, 0x6a, 0x61, 0x61, 0x72, in base al tipo partiamo dal fondo o dalla testa:

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

Inserendo nel programma i byte in maniera corretta otteniamo: `picoCTF{3ndi4n_sw4p_su33ess_817b7cfe}`.
