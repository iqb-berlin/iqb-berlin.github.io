# 1.TBA Einführung

Nach zahlreichen Vorarbeiten arbeitet das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de)
seit 2018 gezielt im Auftrag der Ländern an der Umstellung der papierbasierten Kompetenzerhebung auf eine technologiebasierte Durchführung. 
Details zu den Projekten bzw. zu weiteren Planungen entnehmen Sie bitte hier:

* [TBA-Projekt 2018-2020](https://www.iqb.hu-berlin.de/research/dm/tba/)
* [TBA-Projekt 2021-2023](https://www.iqb.hu-berlin.de/research/dm/tba21/)
* [VERA online](https://www.iqb.hu-berlin.de/vera/online/)

Dieses Kapitel soll eine Einführung in die IQB Instrumentarien geben, die zur Umsetzung der technologiebasierten Kompetenzerhebung
seitens des IQB zum Einsatz kommen.
 
<!--++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-TBA-Module-Aufbau">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 1.1 TBA Module Aufbau

Nachfolgend wird ein Überblick über die wesentlichen softwarebasierten Bestandteile des Computerbasierten Testens gegeben.
Detaillierte Informationen zu den Software Modulen entnehmen Sie bitte den gleichnamigen Kapiteln.
Die meisten Anwender\*innen werden im Rahmen einer Testgestaltung und Testdurchführung vorwiegend mit den Modulen 
**Teststudio** und **Testcenter** in Berührung kommen.
 
![iqb online assessment applications with relations: testcenter, Teststudio, conding, data analysis, archive, taskpool](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/EF_Ablauf_TBA_final.png)

### IQB-Teststudio

Das **Teststudio** besteht vereinfacht ausgedrückt aus einer Datenbank und einer Benutzeroberfläche.
Letztere kann mittels einer Adresse in einem Internetbrowser geöffnet werden. Anschließend erfolgt eine Anmeldung mit den entsprechenden 
Zugangsdaten. In die Benutzersoberfläche ist ein Editor eingebettet mit dessen Hilfe die interaktiven Einheiten eines Kompetenztests 
(Units) bearbeitet und erstellt werden können. Nähere Informationen zur Bearbeitung und Erstellung von Aufgaben entnehmen Sie bitte dem Kapitel:
**Teststudio**. Nach finaler Editierung der Aufgaben, generiert das **Teststudio** die Einheiten eines Kompetenztests 
(Units und weitere für den Test erforderliche Dateien) in einem komprimierten Dateiformat (Zip-Datei). Die Einheiten können bei Bedarf 
nachträglich bearbeitet und an die entsprechende Testumgebung angepasst werden. Anschließend können die Testdateien dann im **Testcenter** 
geladen und wiedergegeben werden.
> Das **Teststudio** für die Technologie basierten Aufgaben befindet sich noch in einer Entwicklungsphase und wird im Projektzeitraum 2021-2023 grundlegend überarbeitet. 
> Die derzeitige Version nennt sich **Teststudio Lite**. Die überarbeitete Version wird dann den Namen **Teststudio Pro** tragen.

### IQB-Testcenter

Mit dieser Anwendung werden Kompetenztests durchgeführt und von den Testorganisator\*innen in den Abläufen getestet. Das **Testcenter**
besteht wieder vereinfacht ausgedrückt aus einer Datenbank und einer Benutzeroberfläche. Letztere wird mittels Adresseingabe in einem 
Internetbrowser geöffnet. Nach Anmeldung mit den entsprechenden Zugangsdaten, können die zuvor im **Teststudio** generierten Einheiten 
eines Tests geladen, gelöscht oder bestehende Dateien heruntergeladen werden. Die Einheiten, Metadaten und Konfigurationen des Tests werden 
dabei in der Datenbank gespeichert und verwaltet. Reihenfolgen, Bezeichnungen, Strukturen und Abläufe des Kompetenztests, können mittels 
Bearbeitung bestimmter Testeinheiten (Testdateien) beinflusst werden. Die Änderungen können dann von den Testorganisator\*innen in 
Probedurchläufen im **Testcenter** begutachtet werden. Dies trägt zu einem gesicherten Ablauf des finalen Tests bei.
Mehr zum Thema **Testcenter** erfahren Sie im gleichnamigen Kapitel.
  

### IQB-Dateneditor

Die Antworten müssen geprüft und aufbereitet werden. Hierzu stehen für die Beteiligten entsprechen ihrer Rolle Funktionen wie Kodieren, 
Verifizieren, beschreibende Statistik abrufen oder Export als Excel-Datei zur Verfügung. Aus den aufbereiteten Daten werden schließlich 
die gewünschten Ergebnisse der Unternehmung erzeugt: Berichte, Publikationen, Rückmeldungen an Schulen.

### IQB-Testarchiv

Eine Testung, Befragung oder allgemein "Studie" sollte gut dokumentiert werden. Hierzu zählen die verwendeten Units, Testhefte, Roh-/Primärdaten, 
Analysedaten, Berichte aber auch Protokolle der Testdurchführung, eine Kritik der Analyseverfahren, Verweise auf Bildungsstandards etc.. 
Diese dann zu archivierende Dokumentation kann auch als Basis für eine Veröffentlichung der Daten für Sekundäranalysen in einem 
Forschungsdatenzentrum dienen. Im Testarchiv wird besonderer Wert auf eine Langzeitarchivierung gelegt (besondere Speicherverfahren, 
besondere Formate für die Dateien usw.).

### IQB-Testdepot

Wenn Aufgaben bzw. Fragebögen verwendet wurden, haben sie ihre Eignung für bestimmte Fragestellungen unter Beweis gestellt. 
Man weiß, unter welchen Bedingungen sie bei welchen Testpersonen mit welcher Genauigkeit Erkenntnisse liefern. 
Diese wertvollen Informationen werden als Metadaten mit den Units und Testheften in einer Datenbank gespeichert. 
Über Suchformulare oder auch über Algorithmen können sie für andere Studien ausgewählt werden. Diese Studien mögen als 
Großprojekte in einem Jahrgang der Schulen eines Landes angelegt sein, es kann sich aber auch um einzelne Lehrkräfte handeln, 
die für einen kurzen Test in ihrem Kurs Aufgaben zusammenstellen.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2-Ablauf-Entwurf-und-Durchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.-TBA-Einf%C3%BChrung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 1.2 Ablauf Entwurf und Durchführung

Nachfolgend wird der grundsätzliche Ablauf vom Entwurf bis zur Auswertung grob aufgezeigt:

![iqb online assessment applications with relations: Einführung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/EF_Datenaust_TS_TC_final.png)

### Entwurf

In der Entwurfsphase wird mittels Editor im **Teststudio** die Aufgabe entworfen und final ausgearbeitet.
Mehr zu diesem Thema entnehmen Sie bitte dem Kapitel: **Teststudio**. Anschließend werden die interaktiven Testeinheiten in einem Zip-Format ausgegeben. 
Diese können dann vor der Eingabe in das **Testcenter** bearbeitet und an die entsprechende Testumgebung angepasst werden.

### Bearbeitung der Testdateien

Die Dateien (Einheiten) eines Tests können bzgl. spezifischer Testumgebung angepasst werden. 
Es müssen Anmeldedaten für die Testdurchführenden angelegt werden, damit abschließend jeder Test auch einem Probanden zugeordnet werden kann.
Eventuell müssen Unitbezeichnungen oder auch Bookletbezeichnungen geändert werden. Auch die Reihenfolge der Units ist anpassbar.
Jede Datei eine Tests verfügt über die entsprechenden Parameter und Strukturen um diese Änderungen durchzuführen.
Welche Parameter das sind entnehmen Sie bitte dem Kapitel: [TBA Einführung / Bestandteile eines Tests](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.3-Bestandteile-eines-Tests)
Mehr zum Thema Bearbeitung finden Sie auch im Kapitel: **Testcenter**.

### Durchführung

Sind die Dateien entsprechend der spezifischen Testumgebung angepasst wurden, können sie im **Testcenter** abgespielt werden. 
Dabei ist es den Testorganisator\*innen möglich mittels Konfiguration einer betimmten Datei (*Testtakers.xml*) den Ablauf eines Tests
(Probedurchlauf, finaler Durchlauf und andere Optionen) festzulegen. Testorganisator\*innen können somit die Testdateien bzgl. bestimmter
Parameter bearbeiten und die Ergenisse ihrer Änderungen immer wieder im **Testcenter** begutachten. Haben die Organisator\*innen die Bearbeitung
des Test abgeschlossen, kann der finale Test gestartet werden. Testdurchführende erhalten dazu, die in der entsprechenden Datei (*Testtakers.xml*)
von Orgnanisator\*innen festgelegten Zugangsdaten. Nach erfolgreicher Anmeldung startet der finale Test.

### Auswertung

Nach einer finalen Testdurchführung sind weitere Nachbearbeitungsschritte notwendig um zu einer aussagekräftigen Auswertung zu gelangen.
Genannt sei hierbei die Kodierung, die für die statistische Auswertung eine wichtige Rolle spielt. Es gibt auch weitere nachbearbeitende
Schritte auf die hier nicht näher eingegangen wird.

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.3-Bestandteile-eines-Tests">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++backward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-TBA-Module-Aufbau">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 1.3 Bestandteile eines Tests

Das **Teststudio** erzeugt nach dem finalen Entwurf die folgenden Bestandteile eines Kompetenztests:

![iqb online assessment applications with relations: Einführung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/EF_TS_Output_final.png)

---

### Funktion der Dateien

**Testtakers.xml**
* Aufruf gewünschtes Booklet mittels eindeutiger Booklet ID (ID muss entsprechend im Booklet vorhanden sein)
* Definition User\*in und Testmodus
* Definition Testgruppe


**Booklet.xml**
* Layout des Booklets
* Namen des Testheftes
* Aufruf der gewünschten Units mittels eindeutiger Unit-ID (ID muss entsprechend in der Unit vorhanden sein)
* Name der Unit
* Beschränkungen mittels Codewörtern

**Unit.xml**
* Definition des zu verwendenden Players
* Definition der zu verwendenden Ressourcen Datei

**Unit.voud oder Unit.htm**
* Aufgabeninhalte und Aussehen
  
**Ressourcen.html**
* Ressourcen für Player und anderes

---

### Parameter der Dateien

Welche Werte in diesen Dateien beeinflusst werden können, ist nachfolgend aufgelistet.
Mehr zu diesem Thema finden Sie auch im Kapitel: [Testcenter / Bearbeiten eines Tests](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Bearbeiten-eines-Tests)

**Testtakers.xml**
* Anmeldedaten
* Art und Weise der Testdurchführung (Testmodi)
  
**Booklet.xml**  
* Namensgebung Booklet
* Unit Reihenfolge/ Unit Aufruf
* Booklet Konfiguration
  
**Unit.xml**
* Einbindung Ressourcendateien (Player, zugehörige .voud-Datei mit den Testinhalten)

**Unit.voud**
* Enthält die Aufgabeninhalte die im Teststudio mittels Editor entwurfen wurde.<br>
Hier sind von Hand keine Änderungen möglich.

**Player.html**
* Enthält Player spezifische Parameter und sollte nicht verändert werden.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.4-Aktueller-Entwicklungsstand">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2-Ablauf-Entwurf-und-Durchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 1.4 Aktueller Entwicklungsstand

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 17.03.2021
todo:
  - IQB-Dateneditor: Änderung des Links, wenn es zu diesem Thema eine eigene Wikiseite gibt!
  - Mit Martin über dieses Kapitel sprechen. Gehört es hier hin, ist es final etc?
```
---

(Februar 2021)
### IQB-Testcenter
Diese Web-Anwendung hat einige Einsätze absolviert und wird seitens des IQB als stabil und produktiv einsetzbar angesehen. Nächste Entwicklungsschritte:
* Massiver Ausbau der Dokumentation/ Wissensbasis, z. B. Entwicklung typischer Einsatzszenarien mit ausführlicher Verfahrensbeschreibung einschl. Datensicherheitskonzept
* Einsatz eingebettet in eine fremde Anwendungsumgebung: Das Einspielen von Testinhalten und das Auslesen von Testantworten erfolgt nicht über das Verwaltungsportal des IQB-Testcenters, sondern durch Drittanwendungen über das API des IQB-Testcenters.
* Optimierung des Installationspaketes hinsichtlich Lastverhalten während des Tests

### IQB-Teststudio
Diese Anwendung liegt derzeit als Prototyp vor. Kleine eingearbeitete Teams können hinreichend schnell Aufgaben gestalten. Diese einfache Version des IQB-Teststudios wird als IQB-Teststudio-Lite weitergeführt. Nächste Entwicklungsschritte:
* Verbesserung der Import/Export-Funktionen
* Konzeption eines IQB-Teststudios mit komplexen Arbeitsabläufen, differenzierten Rollen, Projektmanagement und Definition der Antwortverarbeitung

### IQB-Dateneditor

Diese Anwendung wird derzeit konzipiert. Die Ergebnisverarbeitung unterstützt aktuell eine Windows-Desktop-Anwendung [ict-Toolbox](https://github.com/iqb-berlin/itc-toolbox/blob/master/README.md).

### IQB-Testarchiv IQB-Testdepot
Diese Anwendungen werden derzeit konzipiert. 

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.5-Studiendurchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward+++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.3-Bestandteile-eines-Tests">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 1.5 Studiendurchführung

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 17.03.2021
todo:
  - Mit Martin über dieses Kapitel sprechen. Gehört es hier hin, ist es final etc?
```

### Planung
Die Beteiligten brauchen rechtzeitig klare Anweisungen, wie die Studie vorbereitet, durchgeführt und ausgewertet wird. Hierzu sind zunächst eine Reihe von Fragen zu beantworten und ggf. bestimmte Schritte vorzuziehen. Mitunter müssen die Festlegungen in Dokumenten festgehalten und verschickt werden: allg. Handreichungen, Manual für die Testleitung, Anschreiben für System-Check, Anträge beim Datenschutz, Elternanschreiben, usw.

* Soll ein System-Check durchgeführt werden?
* Wie genau erfolgt die Anmeldung der Testperson (durch die Testaufsicht, oder nur teilweise, oder nur durch Link usw., siehe [hier](https://github.com/iqb-berlin/testcenter-frontend/wiki/Varianten-der-Anmeldung-einer-Testperson))?
* Soll der Testablauf einer Testgruppe beobachtet oder gesteuert werden (Testleitungskonsole)?
* Erhalten die Schulen eine Rückmeldung? Wie sieht die aus?
* Welche Zusatzmaterialien werden vor Ort benötigt: Taschenrechner, Lineal, Notizpapier, Kopfhörer?
* Stehen für die Durchführung Testleiterinnen oder Testleiter oder zumindest Coaches zur Verfügung?
* Soll es eine Hotline geben? Für welchen Zeitraum?
* Wie hoch ist das Risiko für technische Probleme? Soll jemand aus der Systemadministration oder Programmierung ständig greifbar sein?
* Wie lautet die genaue Internet-Adresse für die Testung bzw. Befragung?

### Units gestalten mit IQB-Teststudio

#### Vorbereitung

* Zugangsdaten erhalten
* Neuen Arbeitsbereich (Workspace) anlegen lassen
* Testablauf planen: Welche Units, welche Zwischenseiten?
* Entscheidungen treffen: Welcher Player, welcher Editor?, ggf. in das IQB-Teststudio hochladen lassen
* ggf. Audios aufbereiten: Größe reduzieren, Exif-Metadaten eintragen
* ggf. Grafikdateien aufbereiten (Farben prüfen, Auflösung bei Zoom)
* Konventionen festlegen (Einrückung, Schriftart/-größe, Zeilenabstand, Formulierung bei Instruktionen, Benennung der Units usw.)

#### Übertragung organisieren

* Trello, CryptPad Kanban o. ä. einrichten, um für jede Unit den aktuellen Status zu dokumentieren
* Workflow definieren: Wer macht ersten Entwurf, wer schaut drüber, wer prüft psychometrisch, wer prüft fachdidaktisch usw.
* Schulungen und Austausch der Autorinnen und Autoren untereinander planen

#### Gestaltung

* Gute Kurznamen für Units wählen, sprechende Titel
* Voransicht nutzen, um Layout und Verhalten zu prüfen
* Erzeugte IDs der Interaktionselemente notieren (canvasElement214...; z. B. über Excel- oder CryptPad-Tabelle)
* Beteiligte sollten sich regelmäßig ihre Units zeigen und Erfahrungen austauschen
* frühzeitig einige Units in das IQB-Testcenter übertragen, um deren Verhalten zu überprüfen
* Units regelmäßig als Dateien exportieren als Backup

#### Export

* Units exportieren mit Xml und Voud
* (Stand Februar 2021) Xml nachbearbeiten (s. [hier](https://github.com/iqb-berlin/teststudio-lite-frontend/wiki/Workaround-%22Fehlerhafte-Unit-Xml%22))

### Teststudio einrichten

#### Vorbereitung

* Zugangsdaten erhalten
* Neuen Arbeitsbereich (Workspace) anlegen lassen
* System-Check ggf. einrichten und freigeben

#### Units hochladen

* (Stand Februar 2021) Xml nachbearbeiten (s. [hier](https://github.com/iqb-berlin/teststudio-lite-frontend/wiki/Workaround-%22Fehlerhafte-Unit-Xml%22))
* Erst die voud-Dateien, dann die Xml-Dateien hochladen. Es könnte sonst passieren, dass eine Xml abgewiesen wird, wenn sie auf eine nicht vorhandene Voud-Datei verweist.

#### Testhefte hochladen

* Eine [xlsx-Datei für die ict-Toolbox](https://github.com/iqb-berlin/itc-toolbox/blob/master/docs/manual-booklet.md) kann helfen, das Testdesign transparent zu planen: Units, Blöcke, Testhefte sind hier einzutragen und dann die daraus erzeugten Xml-Dateien hochzuladen.
* Sollten Units im Testheft mehrfach auftauchen (z. B. Fragen zur Motivation) bitte darauf achten, dass die Units unterschiedliche Aliase bekommen!

### Review und Probelauf

* Allgemein bitte [diese Hinweise](https://github.com/iqb-berlin/itc-toolbox/blob/master/docs/manual-logins.md) zu Logins beachten.
* Die Xml zu Testteilnehmern (sog. Testtaker) ersteinmal nur für [Review-Modus](https://github.com/iqb-berlin/testcenter-frontend/wiki/Modi-der-Testdurchf%C3%BChrung) anlegen für alle Verantwortlichen der Studie hochladen.
* Nach jeder Review-Schleife die Kommentare aus dem Testcenter-Admin-Portal herunterladen und auswerten, Änderungen an den Units vornehmen, neu exportieren und NUR DIE neuen VOUD-Dateien ins Testcenter hochladen (sonst überschreibt man die Xml-Änderungen).
* Auch Logins im hot-restart-Modus anlegen, Real-Time-Tests durchführen und sorgfältig auswerten

### Studie durchführen

* Logins für Durchführung hochladen, ggf. Zeitfenster gut dokumentieren
* täglich Antworten und Logs ziehen und speichern
* Probeauswertungen vornehmen: Nur so erkennt man früh, wenn bestimmmte Variablen nicht ankommen
* Hotline auswerten, auch erste Testprotokolle analysieren

### Auswertung, Evaluation

* Daten wie vorgesehen auswerten, Berichte schreiben, Rückmeldung an Schulen geben
* Evaluieren: Dabei hilft die Vorstellung, dass man die gleiche Studie nächste Woche nochmal durchführen soll
* Feiern...

---

<!--+++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.6-Verfügbarkeit-IQB-Programmierung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.4-Aktueller-Entwicklungsstand">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 17.03.2021
todo:
  - Mit Martin über dieses Kapitel sprechen. Gehört es hier hin, ist es final etc?
```

## 1.6 Verfügbarkeit IQB Programmierung

### Der Auftrag

Das IQB ist länderfinanziert und erhält daher Aufträge stets mit Blick auf den Nutzen für die Länder der Bundesrepublik Deutschland. Dies ist insbesondere beim computerbasierten Testen im Bildungswesen der Fall. Denn wenn bisher die Aufgaben als Druckvorlagen an die Länder geliefert wurden, die jede Druckerei vervielfältigen kann, sind Testaufgaben im Online-Format nur durch spezielle Testsysteme nutzbar. Das Speicherformat muss kompatibel sein.

Viele der Kompetenztestungen finden durch die Länder selbst statt ohne Beteiligung des IQB. Daher sind alle Programmierarbeiten am IQB mit der Auflage verbunden, die Nutzbarkeit der Aufgaben durch die Länder sicherzustellen.

### Software ist frei nutzbar

Der erste Schritt hierzu ist die Veröffentlichung des Codes und der Dokumentationen sowie der Installationspakete aller IQB-Anwendungen hier auf GitHub. Alle Interessierten können die Software installieren und ohne Kenntnis des IQB einsetzen. Gemäß des o. g. Auftrages sind wir sehr daran interessiert, die Nutzung durch Dritte zu unterstützen, insbesondere durch die Länder.

### Aufgabenaustausch

Wie sieht es aber mit Einrichtungen aus, die eigene Anwendungen (weiter-)nutzen? Wie können hier die Aufgaben eingesetzt werden? Eine länderübergreifende Fachgruppe evaluierte die Optionen. Zunächst wurde die Nutzung eines vorhandenen Speicherstandards verworfen. Entweder erfüllt ein Standard nicht alle Anforderungen (nicht alle Interaktionsformate können abgebildet werden), oder zu dessen Verwendung ist Software nötig, die zu teuer oder nur über spezialisierte Dienstleister nutzbar ist. Einen neuen Standard für ein Speicherformat zu entwickeln, wurde ebenfalls verworfen.

Die Lösung liegt darin, viele Speicherformate zuzulassen und jeweils Programmcode mitzuliefern, der zwischen Testsystem und der Aufgabe vermittelt. Für spezielle Anforderungen können also jederzeit neue Speicherformate entwickelt werden, solange der erforderliche Programmcode mitgeliefert wird. Ein vorhandenes Testsystem muss nur einmalig die Schnittstelle zu derartigem Programmcode implementieren.

Dieses modulare System analog eines Plug-In gewährleistet eine enorme Flexibilität der Aufgabenformate, ohne dass jeweils ein ganzes Testsystem angepasst werden muss. Dieser Mechanismus ist [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.5-Verona) beschrieben.

### Lizenzen

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/) für Spezifikationen, Dokumentationen, Videos, Metadatenkataloge und ähnliche Inhalte.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT) für Programmcode.

Diese Lizenzen sollen die Verwendung so wenig wie möglich einschränken. Auch eine Nutzung in kommerziellem Zusammenhang ist möglich, solange Urheber genannt werden und die abgeleiteten Produkte ebenfalls frei zugänglich sind.

---

<!--+++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.7-Was-macht-VERA-so-speziell%3F?">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.5-Studiendurchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 1.7 Was macht VERA so speziell?

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 17.03.2021
todo:
  - Mit Martin über dieses Kapitel sprechen. Gehört es hier hin, ist es final etc?
```

Der Name VERA steht für "Vergleichsarbeiten". Diese groß angelegten Kompetenztests dienen der Qualitätssicherung auf Ebene der
Schulen. Weitere Informationen finden Sie beim [IQB](https://www.iqb.hu-berlin.de/vera/) und bei der [Kultusministerkonferenz](https://www.kmk.org/fileadmin/Dateien/veroeffentlichungen_beschluesse/2015/2015_06_11-Gesamtstrategie-Bildungsmonitoring.pdf). 

Die Testaufgaben und auch die Zusammenstellungen der Aufgaben (Module, Testhefte) werden vom IQB geliefert. Die Durchführung selbst liegt in der Hand der Länder, d. h. es gibt hier keine gemeinsame Infrastruktur. Beim bisherigen papierbasierten Verfahren übergibt das IQB Druckvorlagen (pdf), die in Länderregie gedruckt und verteilt werden. Hier kommen mitunter Online-Portalsysteme zum Einsatz, um die Logistik zu bewältigen, aber auch um die Antworten der Schülerinnen und Schüler einzugeben und zu bewerten. Die Lehrkräfte erhalten außerdem über diese Portale die Ergebnisse der Datenanalysen, aus denen sie für den Unterricht Verbesserungen ableiten können (sog. Rückmeldungen).

Die ersten Ansätze der Online-Durchführung sehen eine manuelle Übertragung der Papierversion der Aufgaben in ein Online-Format vor. Das jeweilige vorhandene Portalsystem wird um einen Onlinetest erweitert. Diese Übertragung der Aufgaben erfolgt für jedes Portalsystem für jedes Jahr. Auf diese Art können viele Länder seit einigen Jahren den Schulen parallel eine Online-Durchführung von VERA anbieten.

Der nächste Schritt ist die Lieferung der Aufgaben durch das IQB im Online-Format. Angesichts der Vielfalt der vorhandenen technischen Lösungen ist dies  ein anspruchsvolles [Vorhaben](https://www.iqb.hu-berlin.de/research/dm/tba21/) und wird viele Jahre in Anspruch nehmen.

![Schema Online-Durchführung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Running-VERA.png)

<!--+++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.6-Verfügbarkeit-IQB-Programmierung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---