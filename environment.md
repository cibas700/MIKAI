## 🧩 Ambiente di esecuzione e requisiti di MIKAI

MIKAI è progettato per essere eseguito all’interno di un **ambiente Linux controllato**, configurato specificamente per l’analisi di dispositivi **RFID/NFC** a fini di studio e ricerca.

Per garantire isolamento e sicurezza, l’utilizzo avviene tipicamente tramite **sistemi virtualizzati** o ambienti Linux dedicati, evitando interferenze con il sistema operativo principale.

---

## 💻 Ambiente di test

Nei contesti di laboratorio, MIKAI viene utilizzato su:

- Sistemi Linux (es. Ubuntu / Debian)
- Ambienti virtualizzati (es. macchine virtuali)
L’uso di una macchina virtuale consente di:
- isolare i driver NFC
- evitare conflitti con il sistema host
- riprodurre scenari di test in modo controllato

---

## 🔌 Dispositivi supportati

Per le attività di analisi NFC vengono impiegati **lettori NFC compatibili con PC/SC**, comunemente utilizzati in ambito di ricerca e sviluppo.

Tali dispositivi permettono:
- la lettura dei dati NFC ( ISO14443-2 Tipo B )
- l’analisi offline delle strutture di memoria
- la sperimentazione in contesti non produttivi

## ⚙️ Configurazione del sistema

L’ambiente Linux utilizzato da MIKAI richiede:
- librerie standard per la gestione NFC 
- driver compatibili con i lettori utilizzati

---
## ▶️ Esecuzione del programma
- Aprire il terminale ed eseguire dei comandi presenti nel file comandi.md
- Collegare l'ACR122U al computer fisico
