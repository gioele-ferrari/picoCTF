# Interencdec

Per trovare la flag ho dovuto aprire il file che viene fornito ovvero enc_flag, viene fornita una prima stringa
ovvero: `YidkM0JxZGtwQlRYdHFhR3g2YUhsZmF6TnFlVGwzWVROclh6ZzJhMnd6TW1zeWZRPT0nCg==` a prima vista sembra una stringa
in Base64, quindi ho provato a usare un decoder online e come risultato ho ottenuto: `b'd3BqdkpBTXtqaGx6aHlfazNqeTl3YTNrXzg2a2wzMmsyfQ=='` sembra che non siamo ancora giunti a un risultato questo perchè
la flag potrebbe essere stata criptata più volte, quindi ho provato nuovamente a eseguire la conversione e ho ottenuto
un nulla di fatto ovvero: `m)5}݄ͩͭ|٭ɬ`. Ho dato una ulteriore visione alla stringa che avevo ottenuto e ho provato a prendere solamente la parte tra gli apici, in questa prova ho ottenuto: `wpjvJAM{jhlzhy_k3jy9wa3k_86kl32k2}`. Mi sono
reso conto di essere molto vicino, ma manca ancora qualcosa, sembra una cifratura di Cesare e provando la conversione sono arrivato a: `picoCTF{caesar_d3cr9pt3d_86de32d2}`.
