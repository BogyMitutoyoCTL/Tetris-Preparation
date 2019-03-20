# Tetris-Preparation
Vorbereitung auf die Implementierung des Riesen-Tetris mit Raspberry und Python.

Dieses Projekt entsteht als Teil der Berufsorientierung für Gymnasiasten (BOGY) für das [Leibnitz-Gymnasium in Rottweil](https://lg.rw.schule-bw.de/home/?page_id=11268) im Schuljahr 2018/19. Als Firmenpartner steht [Mitutoyo CTL in Oberndorf](http://www.mitutoyo-ctl.de/de/karriere/ausbildungundstudium) als Ansprechpartner mit Hardware, Räumlichkeiten und Ansprechpartnern zur Verfügung.

Inspiration für das Thema "Riesen-Tetris" waren

* [Arduino LED Coffee Table (Artikel auf Instructables)](https://www.instructables.com/id/Arduino-LED-Coffee-Table/)
* [Interaktiver LED Tisch mit Raspberry Pi (Artikel auf Heise Make)](https://www.heise.de/make/meldung/Fleissarbeit-Interaktiver-LED-Tisch-mit-Raspberry-Pi-3619636.html)
* [Raspberry Pi Retro Gaming LED Display (Artikel auf Hackaday)](https://hackaday.io/project/11064-raspberry-pi-retro-gaming-led-display)

## Hardware

Das Praktikum befasst sich hauptsächlich mit der (teils hardwarenahen) Software-Seite. Die Hardware wurde im Wesentlichen von Mitutoyo CTL vorbereitet. Für eine komplette Vorbereitung im Rahmen des BOGY wäre nicht genügend Zeit. Damit dieses Projekt auch von anderen Interessenten umgesetzt werden können, beschreiben wir natürlich auch die [Hardware](Hardware.md).

## Erster Nachmittag, 20.2.2019

Nach der Begrüßung und Führung durch das Gebäude haben wir mit Hilfe der [Firmenpräsentation](Präsentationen/Firmenpräsentation_16_9.pptx) die Firma Mitutoyo, ihre Software und das angebotene Studium der Informatik (Informationstechnik) kennengelernt.

Im Anschluss haben wir kurz die Idee vorgestellt: es soll eine Hardware-Software-Kombination entstehen, mit der man zumindest Tetris spielen kann. Das [Brainstorming](Brainstorming.md) ergab noch einige weitere Ideen und Anregungen, die wir optional umsetzen können, sofern gegen Ende des BOGY noch Zeit bleibt.

Für einen ersten Überblick gab es die [Raspberry Pi Einführung](Präsentationen/Raspberry%20Hardware.pptx). Den haben wir dann auch zusammengebaut, eingeschaltet und die Software aktualisiert (`sudo apt-get update` und `sudo apt-get upgrade`). Außerdem haben wir uns einen Überblick über die verwendete [Hardware](Hardware.md) des Spielbretts verschafft sowie die dazu nötigen [Ein- und Ausgabemöglichkeiten des Raspberrys](Präsentationen/Hardware%20Einführung.pptx).

Alle Teilnehmer haben bereits einen [Github Account](https://github.com/join) angelegt und wurden zu diesem Projekt hinzugefügt.

Weil noch Zeit übrig war, haben wir gleich die [USB Soundkarte](Präsentationen/USB%20Soundkarte.pptx) konfiguriert.

Hausaufgaben:

* Fotofreigabedokument von den Eltern unterschreiben lassen

## Zweiter Nachmittag, 27.2.2019

Heute sind wir tiefer eingestiegen in die Welt des Raspberry. Wir haben die [Grundlagen von Linux](Prsäentationen/Linux.pptx) besprochen, darunter im Wesentlichen den Systemaufbau, Benutzerrechte, Dateien und die Verzeichnisstruktur.

Ein Linuxsystem wie der Raspberry (genauer: Raspbian als Betriebssystem des Raspberry) lässt sich kaum ohne die Konsole einrichten. Daher sind wir auch auf die Befehle des Terminals [Bash](Präsentationen/Bash.pptx) eingegangen und haben Dateien bearbeitet, Rechte geändert.

Hausaufgaben:

* [Virtuellen Raspberry Pi einrichten](virtual_raspberry.md)

## Dritter Nachmittag, 13.3.2019

Beim Daily Standup haben wir gefragt, wer sich zuhause einen virtuellen PC mit Raspbian eingerichtet hat.
Mit den Folien der [Bash](Präsentationen/Bash.pptx) waren wir noch nicht ganz durch, daher haben wir diesen Teil noch nachgeholt. Danach haben wir [PyCharm](Präsentationen/Pycharm.pptx) kennengelernt und installiert. Damit waren wir vorbereitet für die Übungen aus der [Python Einführung](Präsentationen/Python%20Einführung.pptx).

Hausaufgaben:

* PyCharm Community Edition für Windows zuhause installieren
* Eine oder zwei Aufgaben von [Project Euler](https://projecteuler.net/archives) in Python lösen

## Vierter Nachmittag, 20.3.2019

Im Daily Standup haben wir uns natürlich erkundigt, wer sich mit den Python Hausaufgaben beschäftigt hat. Danach haben wir die [Python Einführung](Präsentationen/Python%20Einführung.pptx) beim Thema Listen fortgesetzt und sind danach in die objektorientierte Programmierung mit der Präsentation [Python Erweitert](Python%20Erweitert.pptx) eingestiegen.

Für dieses Projekt nützliche Bibliotheken können sein:

* [Luma](https://pypi.org/project/luma.core/) zur Ansteuerung von LEDs
* [Pygame](https://www.pygame.org/docs/) zum Abspielen von Musik
* [Aiohttp](https://aiohttp.readthedocs.io/en/stable/) für den Webserver, der das Spiel aufs Handy liefert
* [PyBluez](https://github.com/pybluez), falls wir Zeit haben, Bluetooth-Unterstützung einzubauen

Hausaufgaben:

* aus der Präsentation, Folie 20: 
 * a) füge eine Methode zur Klasse hinzu, die den Quader in einer Richtung dreht.
 * b) füge eine Funktion zur Klasse hinzu, die das Volumen des Quaders ausrechnet.