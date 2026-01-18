## ⚙️ Comandi da eseguire nel terminale della macchina Linux

```bash
sudo apt-get install flex libpcsclite-dev libusb-dev checkinstall
sudo apt-get install libnfc6
sudo apt-get install libnfc-bin libnfc-dev
sudo apt-get install libacsccid1
sudo apt-get install gedit
sudo gedit /etc/modprobe.d/blacklist-libnfc.conf
```

Aggiungere queste 3 voci
- blacklist nfc
- blacklist pn533
- blacklist pn533_usb

```bash
sudo reboot
```

---

##⚙️Comandi da eseguire dopo aver effettuato il riavvio:
Aprire il terminale e spostarsi con il terminale nella cartella dove è stato estratto MIKAI ed eseguire:

```bash
chmod +x mikai.appimage
```

Per eseguire il programma:

```bash
./mikai.appimage
```
