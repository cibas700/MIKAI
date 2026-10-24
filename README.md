# 🔐 Analisi di Sicurezza del Sistema Coges MyKey

## ⚠️ AVVISO IMPORTANTE ⚠️

Questo repository è pubblicato **esclusivamente a fini educativi, di ricerca e di sicurezza informatica**.  
Qualsiasi accesso non autorizzato, alterazione o utilizzo improprio di sistemi di pagamento cashless è **vietato dalla legge**.

Lo scopo di questa documentazione è analizzare criticamente il sistema **Coges MyKey** per favorire una maggiore consapevolezza sulle problematiche di sicurezza e promuovere l’adozione di contromisure adeguate.

**MIKAI** è progettato esclusivamente per attività di **studio, analisi e ricerca sulla sicurezza**.  
Non è uno strumento di sfruttamento e **non fornisce funzionalità automatiche per alterare sistemi di pagamento reali**.

---

## 📖 Indice

- 🇮🇹 Italiano

---

## 🇮🇹 Italiano

Questo repository contiene un’**analisi tecnica e di sicurezza** del sistema di pagamento **cashless Coges MyKey**.

---

## ⚙️ Funzionamento del programma MIKAI

MIKAI è uno strumento di analisi sviluppato per lo studio dei sistemi di pagamento cashless basati su **RFID/NFC**, con particolare riferimento alle chiavi utilizzate nei distributori automatici.

Il programma **non interagisce direttamente con infrastrutture di pagamento reali**, ma opera su **file di dump NFC** ottenuti in contesti controllati e di laboratorio.

---

## 📡 Lettore NFC utilizzato

Per l'acquisizione dei dati viene utilizzato il lettore NFC **ACR122U (ACS ACR122U USB NFC Reader)**.

L'ACR122U è un dispositivo USB per la lettura di tag e dispositivi contactless compatibili con lo standard **ISO/IEC 14443**, operante alla frequenza di **13,56 MHz**.

### 🔧 Caratteristiche principali

- **Modello:** ACS ACR122U
- **Tipologia:** lettore RFID/NFC contactless
- **Interfaccia:** USB
- **Frequenza operativa:** 13,56 MHz
- **Standard supportati:** ISO/IEC 14443 A/B
- **Tecnologia:** PC/SC, CCID
- **Compatibilità:** Windows, Linux e macOS, in funzione dei driver e delle librerie disponibili

### 🔍 Utilizzo con MIKAI

Il lettore ACR122U viene impiegato nella fase preliminare di acquisizione dei dati, esclusivamente su dispositivi di laboratorio o per i quali si dispone di autorizzazione.

Il processo di analisi prevede:

1. Collegamento del lettore NFC ACR122U al computer.
2. Rilevamento di un dispositivo RFID/NFC compatibile.
3. Acquisizione dei dati accessibili attraverso strumenti e librerie compatibili.
4. Esportazione dei dati acquisiti in un file binario o esadecimale.
5. Importazione del file nel programma **MIKAI**.
6. Analisi offline della struttura di memoria.

**Nota:** la compatibilità del lettore non garantisce automaticamente la lettura completa della memoria di ogni dispositivo. Alcune aree possono richiedere specifici meccanismi di autenticazione o non essere accessibili.

MIKAI non necessita di una connessione continua con il lettore NFC, poiché la sua funzione principale è l'analisi offline dei dump precedentemente acquisiti.

---

## 📥 Acquisizione dei dati

MIKAI lavora a partire da:

- Dump NFC / EEPROM
- File binari (`.bin`)
- File in formato esadecimale (`.hex`)

Questi file vengono caricati nel programma come **input per l'analisi offline**, evitando qualsiasi comunicazione diretta con dispositivi in uso.

---

## 🧠 Analisi della struttura di memoria

Una volta caricato un dump, MIKAI:

- Suddivide i dati in **blocchi di memoria**.
- Identifica **offset** e **dimensioni** dei singoli campi.
- Interpreta la **struttura logica della EEPROM**.
- Consente di esaminare la rappresentazione esadecimale dei dati.
- Supporta lo studio delle differenze tra acquisizioni effettuate in condizioni controllate.

L'analisi si concentra in particolare su:

- Aree di credito
- Contatori
- Campi identificativi
- Sezioni di controllo e integrità dei dati

---

## 🔒 Finalità della ricerca

Il progetto MIKAI ha come obiettivi principali:

- Comprendere l'organizzazione dei dati nei sistemi cashless RFID/NFC.
- Studiare il funzionamento logico delle memorie EEPROM.
- Analizzare i meccanismi di integrità e protezione delle informazioni.
- Individuare possibili criticità di sicurezza attraverso analisi offline.
- Promuovere lo sviluppo di sistemi di pagamento più sicuri.

**Tutte le attività devono essere svolte su dispositivi di proprietà o espressamente autorizzati, all'interno di ambienti controllati.**

---

## ⚖️ Disclaimer

Questo progetto è distribuito esclusivamente per scopi didattici e di ricerca.

Gli autori non incoraggiano né autorizzano l'utilizzo degli strumenti o delle informazioni contenute nel repository per manipolare crediti, aggirare sistemi di protezione o alterare dispositivi di pagamento reali.

L'utilizzatore è responsabile del rispetto delle normative applicabili e delle autorizzazioni necessarie.
