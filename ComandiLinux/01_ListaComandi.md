# Lista Comandi Github

## cd - Change Directory
Da utilizzare con percorsi assoluti o relativi
- ~ rappresenta la mia home directory
- / root directory
Tutte le volte che uso questi due simboli sto navigando con un percorso assoluto.

Spiegazione dei simboli o opzioni per i comandi:
- `.` directory corrente
- `..` directory genitore
- `~` home directory 
- `/` root directory
- `-` directory precedente

## Tipi di File 
Quando lancio il comando `ls -l` ottengo vari risultati
- drwxrwxrwx 1 root ....

Primo Carattere
- `d` = directory
- `-` = file generici
- `l` = link, puntano ad un altro file
- `s` = socket 
- `p` = pipe
- `b` = block file
- `c` = character file

Permessi `rwxrwxrwx`. Si dividono in 3 parti da 3 caratteri
- i primi 3 per lo user
- i secondi 3 per il gruppo
- i terzi per gli special 

Nomenclature
- `r` readable
- `w` writable
- `x` executable

Quando incontro un `-` vuol dire che quel particolare permesso non è disponibile per quella categoria.

Esempio: `rwxrw-r--` --> l'utente può fare tutto, il gruppo solo leggere/scrivere e non eseguire, gli special solo leggere
