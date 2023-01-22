# Zusammenbau

## Tag 1

```
Heute haben wir uns mit der Anleitung vertraut gemacht und mit dem Bau der Drohne begonnen.
```

Eingebaute Teile:

- Carbon Frame
- Motors
- Speed Controller ( ESC )
- Power Distribution Board ( PDB )
- Flight Controller ( <a href=https://clover.coex.tech/en/coex_pix.html>COEX Pix Pinout</a> )

Zusatzinformationen:<br>
Die Motoren wurden mit den ESCs verbunden.<br>
Die ESCs wurden mit dem PDB verbunden und befestigt.

### Bilder

<img src="images/1_Drohne_Tag_1.jpg" width="350"> <img src="images/3_Drohnenbau_Tag_1_2.jpg" width="350">

## Tag 2-3

```
Bau der Drohne wurde fortgesetzt.
Das Raspberry Pi Image wurde auf die SD-Karte geflasht und in den Pi eingesetzt.
Softwareupdate (apt update/upgrade) wurde durchgeführt.
Der Flight-controller wurde zudem auch geflasht, jedoch muss noch die richtige config manuell eingestellt werden, welche die richtigern Parameter beinhaltet. Diese ist auf der COEX Website zu finden.
```

Eingebaute Teile:

- Flight Controller
- Raspberry Pi
- Radio Reciever

Zusatzinformationen:
Der Flight-controller wurde an den Strom angeschlossen und kurz angeschaltet.<br>
Der Recieve wurde an das "Mounting Deck" geklebt.

## Tag 4

```
Wir haben versucht die Drohne zur Fernbedienung zu verbinden aber ohne Erfolg.
Motortest nicht möglich, da "Command nicht in Software vorhanden". Die Firmware ist oft nicht richtig geflasht worden.
```

Eingebaute Teile:

- GPS Modul

Zusatzinformationen:
GPS Modul noch nicht fest eingebaut. Da keine vorgegebene stelle an der Drohne vorhanden ist.

## Tag 5

```
Gegen Ende der Stunde haben wir es geschafft endlich die Motoren drehen zu lassen, dabei durften wir zusehen wie Justin die Motoren seiner Gruppe gegrillt hat, da er statt 5mm Schrauben, 8mm Schrauben verwendet hatte welche die Spulen des Motors berührten. Wir haben die SD-Karte des Flight Controllers neu formatiert und dann die original [ PX4 Firmware v1.13.2 ] draufgeflasht. Die SD-Karte des Flightcontrollers ist nicht Relevant, da darauf nur Logs Und Missionsdaten gespeichert werden.
```

Eingebaute Teile: -

Zusatzinformationen:
Motoren drehen sich, da die Firmware neu geflasht wurde und einige parameter verändert wurden.

## Tag 6

```
Wir bauen das GPS Modul ohne Anleitung drauf. Wir positionieren es oben über dem Flight Controller.

[ ACHTUNG ] Es ist wenig platz zwischen dem GPS-Modul und der Batterie.

```

<img src="images/Pasted_image_20221207081422.png" width="600">

## Tag 7-8

```
Propeller wurden draufgebaut und festgezogen.

[ ACHTUNG ]
- Die Propeller richtig herum draufschrauben (Erspart viele Kopfschmerzen).
- Bei jedem Test ohne flugversuch die Propeller abnehmen(erspart zwei BG Rechnungen).

[ TIPP ] Die Drohne nochmal neu kalibrieren wenn diese komisch fliegt.
```

Eingebaute Teile:

- Propeller

Zusatzinformationen: -

## Tag X der tag der Verdammnis

```
Die Batterie der Drohne ist volkommen unverständlich, die Zellen könnten Tiefentladen sein und daher nichtmehr von dem Ladegerät erkannt werden. Das ladegert lädt bei den Defekten Batterien nurnoch auf 12,6 Volt. Sicher sind wir uns nicht. 3 Batterien sind Scheinbar Kaputt. Die Zelle 4 hat 0 Volt und keinen Wiederstand (Kurzschluss). Wir haben eine Batterie aufgeschnitten und die defekte Zelle abgelötet. Nach dem anlöten der Neuen Zelle und der erneuten Kalibrierung der Drohne Funktioniert die modifizierte Batterie normal.
```

## Zwischenarbeit 1

```
Experimentieren mit GPS und Verbindungsmöglichkeiten der Drohne. Die Drohne hebt nicht ab wenn eine Mission gestartet wird, da die Posotion der Drohne nicht genau genug ist. Außerdem "Driftet" das GPS stark. Warum das GPS-Modul einen USB-micro-Port hat ist uns nicht klar. Wir haben es mit dem USB-Port des Raspis Verbunden. Und mit I2C mit dem Flightcontroller.

[ TIPP ] GPS braucht ein paar Minuten um die Satelliten zu finden und eine Verbindung aufzubauen.
Das GPS funktioniert nur draußen, am besten mit freier Sicht auf den Himmel.
```

Eingebaute Teile: -

Zusatzinformationen: -

## Hilfe und Probleme bei anderen Gruppen

```
Bei Justins Gruppe wurden in der qGroundControl app die Channel der RC nicht angezeigt. Wir haben ihnen geholfen die RC neu zu "Binden" da dies nicht von Werk aus gemacht wurde.
Dazu muss man beim Start des Recievers den Bind Knopf drücken und dann die RC einschalten. Danach sollte die RC mit der Drohne verbunden sein.

Sebis Gruppe hatte eine verbundene RC, jedoch wurden die Channel trotzdem nicht angezeigt. Dagegen muss man den Knopf am Reciever für 2 Sekunden Drücken. Danach sollten die Channel in der Software angezeigt werden.
```

# WICHTIGE INFORMATIONEN

- Batterien nicht zu sehr entladen, da diese sonst unbrauchbar werden.
- Den Motortest nur ohne Propeller durchführen da verletzungen und Schäden an der Drohne und anderen Gegenständen entstehen können.

---

# References

Links:

- <a href=https://clover.coex.tech/en/assemble_4_2.html>Anleitung</a>
- <a href=https://github.com/CopterExpress/clover>Clover Github</a>
- <a href=https://github.com/CopterExpress/Firmware/releases/download/v1.8.2-clover.13/px4fmu-v4_default.px4>Flight Controller Firmware</a>
- Drone WI-FI: cloverwifi
- Wi-Fi Gateway / PI-IP: <a href=http://192.168.11.1>192.168.11.1<a>
- LAN: <a href=http://192.168.137.177>192.168.137.177<a>
