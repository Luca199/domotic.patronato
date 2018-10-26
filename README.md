# Domotic Patronato

## Intro
Domotic Patronato è un progetto domotico per uso domestico che permette l'accensione e o spegnimento delle luci da remoto.  
Il progetto utilizza un **Raspberry PI 3B+** e una scheda rele.  
Il software è basato **Openhabian** e **MQTT** (tramite Mosquito).  
L'attuazione dell'impianto avviene tramite il servizio cloud di Openhab, su unapagina web, oppure tramite app di Openhab.  

![openhab screenshot](https://image.ibb.co/eoFCVq/openhab-screen.png)  

## Stato del progetto  
Il primo prototipo funziona, lo stato è concluso, il progetto è stato di carattere didattico e il corso è terminato. Il repository quindi non è più mantenuto.

## Hardware  
BOM (Bill of material):  
* Raspberry Pi3B+  
* Modulo relè optoisolato, con il numero di canali necessari  
* Jumper dupont  
* Un pulsante 6x6mm

## Software  
Istruzioni per l'installazione:  

1. Installare openhabian seguendo la [guida ufficiale](https://www.openhab.org/docs/installation/openhabian.html)  
1. Prima del primo avvio, creare il file `ssh` nella root della SD, facendo attenzione che non abbia estensione  
1. Trovare l'ip del raspberry connesso in rete ed utilizzare un client SSH (_ad esempio PuTTY_) per connettersi. Di default sono user: `openhabian` e pw `openhabian`.    
1. Aggiornare il sistema con: 
    ```
    sudo apt update
    sudo apt upgrade
    ```  
1. Entrare nella cartella `etc/openhab2`
