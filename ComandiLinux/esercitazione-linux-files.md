# Esercitazione Linux: Creare File e Cartelle e Navigare con cd

## Comandi Principali

### Comandi di Base
- `pwd` - mostra la directory corrente (Print Working Directory)
- `mkdir` - crea una nuova cartella
- `touch` - crea un file vuoto
- `cd` - cambia directory
- `ls` - elenca il contenuto di una directory
- `tree` - mostra la struttura ad albero (se disponibile)
- `cp` - copia file o cartelle
- `mv` - sposta o rinomina file e cartelle
- `rm` - rimuovi

---

## Parte 1: Preparazione dell'Ambiente

### Esercizio 1.1
Verifica in quale directory ti trovi attualmente.

### Esercizio 1.2
1. Vai nella tua home directory
2. Crea una cartella chiamata `esercitazione_linux`
3. Entra nella cartella appena creata
4. Verifica di essere nella posizione corretta

---

## Parte 2: Creare una Struttura di Cartelle

### Esercizio 2.1
Crea la seguente struttura di cartelle:
```
esercitazione_linux/
├── progetti/
│   ├── progetto_a/
│   └── progetto_b/
├── documenti/
│   ├── lavoro/
│   └── personale/
└── backup/
```

### Esercizio 2.2
Verifica che la struttura sia stata creata correttamente usando il comando `ls -R`

### Esercizio 2.3
Crea i seguenti file nelle rispettive cartelle:
- `readme.txt` e `codice.py` in `progetti/progetto_a/`
- `note.txt` in `progetti/progetto_b/`
- `report.doc` in `documenti/lavoro/`
- `lista_spesa.txt` in `documenti/personale/`
- `backup_2024.tar` in `backup/`

---

## Parte 3: Navigazione con Percorsi Relativi

I percorsi relativi partono dalla directory corrente e **non** iniziano con `/` o `~`.

### Esercizio 3.1
1. Assicurati di essere nella cartella `esercitazione_linux`
2. Entra nella cartella `progetti` usando un percorso relativo
3. Verifica la tua posizione
4. Entra nella cartella `progetto_a`
5. Verifica la tua posizione

### Esercizio 3.2
1. Dalla posizione corrente (`progetto_a`), torna indietro di un livello
2. Verifica dove ti trovi
3. Torna indietro di due livelli in un solo comando
4. Verifica dove ti trovi

### Esercizio 3.3
1. Dalla cartella `esercitazione_linux`, entra in `documenti/lavoro` usando un solo comando con percorso relativo
2. Torna alla cartella `esercitazione_linux` usando un percorso assoluto

### Esercizio 3.4 - Navigazione Avanzata
1. Dalla cartella `esercitazione_linux`, vai in `progetti/progetto_b`
2. Da `progetto_b`, vai in `documenti/personale` usando un percorso relativo (suggerimento: devi usare `../..`)
3. Torna alla directory precedente usando `cd -`

---

## Parte 4: Navigazione con Percorsi Assoluti

I percorsi assoluti partono sempre dalla radice `/` o dalla home `~` e funzionano da qualsiasi posizione.

### Esercizio 4.1
1. Vai nella cartella `progetti` usando il percorso assoluto con `~`
2. Verifica la tua posizione
3. Vai in `backup` usando il percorso assoluto
4. Vai in `documenti/lavoro` usando il percorso assoluto

### Esercizio 4.2
1. Esegui `pwd` e annota il percorso completo
2. Usa il percorso completo (quello che inizia con `/home/...`) per andare in `progetti/progetto_a`
3. Verifica la tua posizione

---

## Parte 5: Esercizi Pratici Misti

### Esercizio 5.1: Navigazione Mista
Partendo da `esercitazione_linux`, esegui questa sequenza e verifica ogni volta dove ti trovi:
1. Vai in `progetti/progetto_a` (percorso relativo)
2. Vai in `backup` usando il percorso assoluto `~/esercitazione_linux/backup`
3. Vai in `documenti/personale` (percorso relativo)
4. Torna alla home usando `cd ~`
5. Torna in `esercitazione_linux`

### Esercizio 5.2: Crea e Naviga
1. Torna in `esercitazione_linux`
2. Crea una struttura `nuova_cartella/sottocartella1/sottocartella2` con un solo comando (usa `mkdir -p`)
3. Crea il file `file1.txt` in `nuova_cartella`
4. Crea il file `file2.txt` in `nuova_cartella/sottocartella1`
5. Naviga fino a `sottocartella2` usando percorsi relativi
6. Torna in `esercitazione_linux` usando `cd` e `..` (quante volte devi usare `..`?)
7. Vai direttamente in `sottocartella2` usando un percorso assoluto

### Esercizio 5.3: Sfida Finale
Partendo da `~/esercitazione_linux/progetti/progetto_a`, completa questa sequenza:
1. Vai in `documenti/personale` usando **solo** un percorso relativo
2. Crea un file chiamato `note_personali.txt`
3. Vai in `backup` usando un percorso assoluto
4. Torna alla directory precedente usando `cd -`
5. Ritorna in `esercitazione_linux` (trova tu il metodo migliore!)

---

## Parte 6: Domande di Verifica

Rispondi a queste domande (non per iscritto) per verificare la tua comprensione:

1. Qual è la differenza tra `cd progetti` e `cd ~/progetti`?
2. Cosa fa il comando `cd ..`?
3. Come torni alla tua home directory con il comando più breve?
4. Se sei in `/home/user/esercitazione_linux/progetti/progetto_a` e vuoi andare in `/home/user/esercitazione_linux/documenti/lavoro`, come fai usando un percorso relativo?
5. Cosa fa il comando `cd -`?
6. Come crei una cartella con più sottocartelle in un solo comando?
7. Qual è la differenza principale tra percorso assoluto e percorso relativo?
8. Qual è la differenza tra `cp` e `mv`?
9. Come fai a copiare un'intera cartella con tutti i suoi contenuti?
10. È possibile rinominare un file con il comando `mv`? Come?

---

## Parte 7: Esercizio Creativo

Crea la seguente struttura di cartelle e file rappresentante un progetto web:

```
sito_web/
├── frontend/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── index.html
├── backend/
│   ├── api/
│   │   └── server.py
│   └── database/
│       └── config.db
└── docs/
    └── README.md
```

Dopo aver creato la struttura:
1. Naviga in `frontend/css` usando percorsi relativi
2. Torna in `sito_web`
3. Vai in `backend/database` usando un percorso assoluto
4. Vai in `frontend/js` usando un percorso relativo
5. Torna in `sito_web` usando il metodo che preferisci

---

## Parte 8: Copiare File e Cartelle (comando cp)

Il comando `cp` serve per copiare file e cartelle.

**Sintassi base:**
- `cp file_origine file_destinazione` - copia un file
- `cp -r cartella_origine cartella_destinazione` - copia una cartella (ricorsivamente)

### Esercizio 8.1: Copiare File
Dalla cartella `esercitazione_linux`:
1. Copia il file `progetti/progetto_a/readme.txt` nella cartella `backup`
2. Copia il file `documenti/lavoro/report.doc` in `documenti/personale` rinominandolo in `report_personale.doc`
3. Verifica che le copie siano state create correttamente

### Esercizio 8.2: Copiare con Percorsi Assoluti
1. Vai in `progetti/progetto_b`
2. Da questa posizione, copia il file `lista_spesa.txt` da `documenti/personale` nella directory corrente usando un percorso assoluto
3. Verifica che il file sia stato copiato

### Esercizio 8.3: Copiare Cartelle
1. Torna in `esercitazione_linux`
2. Copia l'intera cartella `progetti/progetto_a` chiamandola `progetti/progetto_a_backup`
3. Verifica che la cartella e tutti i suoi file siano stati copiati
4. Copia l'intera cartella `documenti` in `backup/documenti_backup`

### Esercizio 8.4: Copiare Multipli File
1. Vai in `progetti/progetto_a`
2. Copia sia `readme.txt` che `codice.py` nella cartella `backup` con un unico comando (suggerimento: `cp file1 file2 destinazione/`)
3. Verifica che entrambi i file siano stati copiati

---

## Parte 9: Spostare e Rinominare (comando mv)

Il comando `mv` serve sia per spostare che per rinominare file e cartelle.

**Sintassi base:**
- `mv file_origine file_destinazione` - sposta o rinomina un file
- `mv cartella_origine cartella_destinazione` - sposta o rinomina una cartella

### Esercizio 9.1: Rinominare File
Dalla cartella `esercitazione_linux`:
1. Rinomina il file `progetti/progetto_b/note.txt` in `appunti.txt`
2. Verifica che il file sia stato rinominato correttamente
3. Rinomina il file `backup/backup_2024.tar` in `backup_completo.tar`

### Esercizio 9.2: Spostare File
1. Sposta il file `documenti/personale/lista_spesa.txt` nella cartella `backup`
2. Verifica che il file non sia più in `documenti/personale` e che sia in `backup`
3. Sposta il file `progetti/progetto_a/codice.py` in `progetti/progetto_b`

### Esercizio 9.3: Rinominare Cartelle
1. Rinomina la cartella `nuova_cartella` in `test_cartella`
2. Verifica il cambiamento
3. Rinomina la cartella `progetti/progetto_b` in `progetti/progetto_beta`

### Esercizio 9.4: Spostare Cartelle
1. Sposta la cartella `test_cartella` dentro la cartella `backup`
2. Verifica che la cartella sia stata spostata
3. Sposta la cartella `documenti/personale` dentro `progetti`

### Esercizio 9.5: Spostare e Rinominare Contemporaneamente
1. Sposta il file `progetti/progetto_a/readme.txt` nella cartella `docs` (che dovrai creare) rinominandolo in `documentazione.txt`
2. Verifica che il file sia nella nuova posizione con il nuovo nome

---

## Parte 10: Esercizi Combinati

### Esercizio 10.1: Backup Completo
Crea uno scenario di backup:
1. Crea una cartella chiamata `backup_finale` in `esercitazione_linux`
2. Copia tutta la cartella `progetti` in `backup_finale`
3. Copia tutti i file dalla cartella `documenti/lavoro` in `backup_finale`
4. Rinomina la cartella copiata `backup_finale/progetti` in `backup_finale/progetti_salvati`

### Esercizio 10.2: Riorganizzazione
1. Crea una cartella chiamata `archivio` in `esercitazione_linux`
2. Sposta tutti i file che contengono "backup" nel nome dentro `archivio`
3. Crea una sottocartella `archivio/vecchi_progetti`
4. Copia la cartella `progetti/progetto_a_backup` in `archivio/vecchi_progetti`
5. Rinomina `archivio/vecchi_progetti/progetto_a_backup` in `archivio/vecchi_progetti/progetto_2024`

### Esercizio 10.3: Gestione File di Progetto
Nel tuo `sito_web`:
1. Crea un file `template.html` in `frontend`
2. Copia `template.html` in tutte le sottocartelle di `frontend` (css, js)
3. Rinomina il `template.html` in `frontend/css` come `test.html`
4. Sposta il file `frontend/index.html` in una nuova cartella `frontend/pages`
5. Copia `backend/api/server.py` creando un backup chiamato `server_backup.py` nella stessa cartella

### Esercizio 10.4: Sfida Finale con cp e mv
Parti da `esercitazione_linux` e completa questa sequenza complessa:
1. Crea una struttura `progetto_finale/src/main` e `progetto_finale/src/test`
2. Copia tutti i file `.py` da qualsiasi posizione in `progetto_finale/src/main`
3. Copia tutti i file `.txt` in `progetto_finale/src/test`
4. Rinomina la cartella `progetto_finale` in `progetto_2025`
5. Sposta l'intera cartella `progetto_2025` dentro `backup_finale`
6. Crea una copia di `backup_finale` chiamata `backup_finale_v2`

---o.

### Comandi Utili
- `ls -R` - elenca tutto ricorsivamente
- `tree` - mostra la struttura ad albero (se disponibile)
- `mkdir -p` - crea cartelle annidate in un comando
- `pwd` - ricordati sempre dove sei!
- `cp -v` - copia con output verboso (mostra cosa sta copiando)
- `mv -v` - sposta con output verboso
- `cp -i` - chiede conferma prima di sovrascrivere
- `mv -i` - chiede conferma prima di sovrascrivere

## Riepilogo: Percorsi Assoluti vs Relativi

### Percorsi Assoluti
- Iniziano con `/` (radice) o `~` (home)
- Funzionano da qualsiasi posizione
- Esempio: `cd /home/user/documenti`
- Esempio: `cd ~/esercitazione_linux/progetti`

### Percorsi Relativi
- Non iniziano con `/` o `~`
- Dipendono dalla directory corrente
- Esempio: `cd progetti/progetto_a`
- Esempio: `cd ../documenti`
