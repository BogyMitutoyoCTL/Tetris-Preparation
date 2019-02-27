# Raspbian mit VirtualBox…
## Download VirtualBox und Installation
VirtualBox könnt ihr Euch hier: 
https://www.virtualbox.org/wiki/Downloads
herunterladen. (Für Windows ist die EXE-Datei ca. 215 MB groß)
Ist die Datei heruntergeladen, installiert ihr VirtualBox auf Eurem Rechner.

## Download Raspbian
Um das Raspbian-ISO-Image herunterzuladen folgt ihr diesem Link:
https://www.raspberrypi.org/downloads/raspberry-pi-desktop/
(Das aktuelle Raspbian Stretch hat ca. 2,5 GB)
## VirtualBox starten und Raspbian einrichten
Nun startet Ihr VirtualBox. Es sollte ungefähr so aussehen:

![image](https://user-images.githubusercontent.com/3775529/53506468-5077d400-3ab6-11e9-9d3f-13b6162d5dab.png)

Über die Schaltfläche „Neu“ legt ihr ein neues Virtuelles System an:

![image](https://user-images.githubusercontent.com/3775529/53506621-a51b4f00-3ab6-11e9-855e-80ffa72834a7.png)

Die Einstellungen zum Hauptspeicher könnt ihr so lassen:

![image](https://user-images.githubusercontent.com/3775529/53507514-579fe180-3ab8-11e9-8877-ddcc704c1310.png)

Ebenso die Einstellungen für die Festplattengröße:

![image](https://user-images.githubusercontent.com/3775529/53507616-80c07200-3ab8-11e9-952e-729db1121c35.png)

Sowie den Festplattentyp:

![image](https://user-images.githubusercontent.com/3775529/53507673-99308c80-3ab8-11e9-9b9f-983a1e948b24.png)

Und die Art der Speicherung:

![image](https://user-images.githubusercontent.com/3775529/53507721-aea5b680-3ab8-11e9-83b0-c8705f889d23.png)

Zum Schluß vergebit ihr der virtuellen Festplatte noch einen Namen:

![image](https://user-images.githubusercontent.com/3775529/53507829-e3b20900-3ab8-11e9-964d-482fda671c77.png)

Und klickt zum Abschluss auf "Erzeugen"...

## Boot-Medium hinzufügen...

Jetzt müsst ihr dem virtuellen System noch sagen von welchem Medium es booten soll. Wie ihr es vielleicht schon von anderen Betriebssystemen kennt, kommen diese oft also ISO-Dateien, die dann auf eine CD gebrannt werden, oder auf einen bootfähigen USB-Stick geschrieben werden.

Bei der VirtualBox läuft das ähnlich, aber hier sagen wir nur: Tue so als ob am System ein CD-Laufwerk angeschlossen ist, mit dem Inhalt der ISO-Datei.

Dazu klicken wir in unserem virtuellen System auf "Ändern"

![image](https://user-images.githubusercontent.com/3775529/53508260-b44fcc00-3ab9-11e9-84ee-60a3cd598d0f.png)

Und gehen wählen dann über "Massenspeicher", "leer" und "Optisches Laufwerk" die ISO-Datei aus, die wir zuvor heruntergeladen haben:

![image](https://user-images.githubusercontent.com/3775529/53509268-c16dba80-3abb-11e9-89a0-80f502e84970.png)

Wenn ihr auf "Datei für optisches Medium auswählen" klickt, könnt ihr die Datei suchen:

![image](https://user-images.githubusercontent.com/3775529/53509483-25907e80-3abc-11e9-86ef-d634ab0fe584.png)

Bestätigt nach der Auswahl mit "OK".

## Start des virtuellen Systems

Jetzt haben wir alle Vorbereitungen getroffen und können das virtuelle System starten...
In der Übersicht sehen wir auch unter "Massenspeicher" welches ISO-Image wir gewählt haben.

![image](https://user-images.githubusercontent.com/3775529/53509653-7c965380-3abc-11e9-8498-60e8483a967f.png)

Jetzt sollte Euer virtuelles System starten...

## Installation von Raspbian auf dem virtuellen System

Wenn alles geklappt hat, dann solltet ihr dies sehen:

![image](https://user-images.githubusercontent.com/3775529/53510592-a81a3d80-3abe-11e9-8c98-c9b98487ab59.png)

Über "Install" installiert ihr das System auf die virtuelle Festplatte.

Jetzt solltet ihr duchrt die Installation hindurchgeführt werden:

![image](https://user-images.githubusercontent.com/3775529/53510863-40b0bd80-3abf-11e9-8058-b93a308c8a72.png)

## Probleme

### Hyper-V Installation
Wenn auf dem Host-Rechner noch eine Hyper-V Installation läuft, muss diese evtl. abgeschaltet werden.
Das kann mit folgendem Befehl mit CMD.exe (als Admin ausgeführt) gemacht werden:

```
C:\WINDOWS\system32>dism.exe /Online /Disable-Feature:Microsoft-Hyper-V
```
wieder einschalten:

```
C:\WINDOWS\system32>dism.exe /Online /Enable-Feature:Microsoft-Hyper-V
```



