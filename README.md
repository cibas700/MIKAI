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

## 📥 Acquisizione dei dati

MIKAI lavora a partire da:

- dump NFC / EEPROM  
- file binari  
- file in formato esadecimale  

Questi file vengono caricati nel programma come **input per l’analisi offline**, evitando qualsiasi comunicazione diretta con dispositivi in uso.

---

## 🧠 Analisi della struttura di memoria

Una volta caricato un dump, MIKAI:

- suddivide i dati in **blocchi di memoria**
- identifica **offset** e **dimensioni** dei singoli campi
- interpreta la **struttura logica della EEPROM**

L’analisi si concentra in particolare su:

- aree di credito  
- contatori  
- campi identificativi  
- sezioni di controllo e integrità dei dati  
