# Anleitung um DietPi für den Betrieb von CryptoHID vorzubereiten. 

Prinzipiell kann man auch andere Distributionen nutzen die auf dem Raspberry Pi laufen. Wir haben uns für eine schnelle und schlanke Distribution entschieden und gehen hier näher auf DietPi ein. 

## Basissystem installieren 

### 1.) Download DietPi
https://dietpi.com/#download

### 2.) 7z Entpacken

### 3.) Etcher starten und DietPi.img auf die SDKarte schreiben.

### 4.) Wifi (optional)
Beim ersten Start schon aktivieren und konfigurieren.Dazu die Datei
 **dietpi-wifi.txt** bearbeiten und die Werte
 ```
  aWIFI_SSID[0]='MySSID' 
  aWIFI_KEY[0]='MyWifiKey'
 ``` 
  anpassen.
## 5.) Tastatur und weitere anpassen
**dietpi.txt** bearbeiten und die Werte
``` 
AUTO_SETUP_KEYBOARD_LAYOUT=de
AUTO_SETUP_NET_WIFI_ENABLED=1
AUTO_SETUP_NET_HOSTNAME=MyServer
AUTO_SETUP_TIMEZONE=Europe/Berlin
``` 
anpassen. 


## 5.) Erststart 
SD Karte stecken und Raspi booten (SSH ist schon per default aktiv)

## 6.) Terminalverbindung öffnen
ssh root@IP ( Passwort = **dietpi** )

## 7.) Basiseinstellungen mit dem Assistenten durchführen
Alle wichtige Einstellungen tätigen. Kennwörter anpassen und Serial **aktivieren**


# Zusätzliche Befehle zur Wartung und Pflege des Systems.
## DietPi-Distribution aktualisieren:
dietpi-update

apt upgrade

apt autoremove

## Raspi Neustarten:

shutdown -r now

## Computer herunterfahren:

shutdown now


**dietpi-banner** – damit lässt sich sich der Bildschirm nach dem Anmelden anpassen.

**dietpi-software** – hiermit können Softwarepakete installiert werden, die 

**dietpi-config** – hier lassen sich Grundeinstellungen vornehmen, wie z.B. Wifi oder Bluetooth konfigurieren.



Gute Anleitung:
https://onkeljordi.de/2019/01/dietpi-klein-schlank-und-schnell-2019/
