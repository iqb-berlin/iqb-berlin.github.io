# 1. Einführung

### Zum Begriff TBA
TBA steht für Technology Based Assessment, also technologie- oder technikbasiertes Testen. Damit ist nicht nur der Computer als Testinstrument gemeint, sondern auch andere digitale Hilfsmittel wie z. B. Stifte, die beim Schreiben scannen. Am IQB wird zur Zeit nur der Computer (Desktop, Tablet, Notebook) als Medium eingesetzt. Daher kann man CBA - Computer Based Assessement - hier als Synonym betrachten für TBA. Andere Begriffe wie Digital Assessment sind ebenfalls zutreffend.

## Projektbezug
Nach zahlreichen Vorarbeiten arbeitet das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de)
seit 2018 gezielt im Auftrag der Ländern an der Umstellung der papierbasierten Kompetenzerhebung auf eine technologiebasierte Durchführung. 
Details zu den Projekten bzw. zu weiteren Planungen entnehmen Sie bitte [den TBA-Projektseiten des IQB](https://www.iqb.hu-berlin.de/tba/)!

Dieses Kapitel soll eine Einführung in die IQB Instrumentarien geben, die zur Umsetzung der technologiebasierten Kompetenzerhebung
seitens des IQB zum Einsatz kommen.
 
<!--++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-Überblick">
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

# 1.1 Überblick

## Ablauf des computerbasierten Testens

![online assessment components: tasks, testees, booklets, authoring, testing, reporting](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/einfuehrung_1.png)

* Testaufgaben: Die Aufgaben und alle Seiten, die bei einem Test angezeigt werden, müssen angelegt werden.
* Testablauf: Es muss der Testablauf definiert werden, d. h. die Position aller Testaufgaben und ergänzenden Seiten im Test sowie ggf. Zeitbeschränkungen.
* Testpersonen: Jede Person, die den Test absolvieren soll, muss Zugangsdaten erhalten und es muss definiert werden, welcher Testablauf zugewiesen werden soll, d. h. welche Aufgabenfolge diese Person präsentiert bekommen soll.

## IQB-Anwendungen 

Einen groben Überblick der Testsysteme und deren Zusammenwirken verschafft auch diese [Video](https://box.hu-berlin.de/f/2530ebf557404b1bac8b/)

![iqb applications: testcenter, teststudio, codingbox](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/einfuehrung_2.png)

#### IQB-Teststudio

Das **Teststudio** besteht vereinfacht ausgedrückt aus einer Datenbank und einer Benutzeroberfläche.
Letztere kann mittels einer Adresse in einem Internetbrowser geöffnet werden. Anschließend erfolgt eine Anmeldung mit den entsprechenden 
Zugangsdaten. In die Benutzersoberfläche ist ein Editor eingebettet, mit dessen Hilfe die interaktiven Einheiten eines Kompetenztests 
(Units) bearbeitet und erstellt werden können. Nähere Informationen zur Bearbeitung und Erstellung von Aufgaben entnehmen Sie bitte dem Kapitel:
**Teststudio**. Nach finaler Editierung der Aufgaben generiert das **Teststudio** die Einheiten eines Kompetenztests 
(Units und weitere für den Test erforderliche Dateien) in einem komprimierten Dateiformat (Zip-Datei). Die Einheiten können bei Bedarf 
nachträglich bearbeitet und an die entsprechende Testumgebung angepasst werden. Anschließend können die Testdateien dann im **Testcenter** 
geladen und wiedergegeben werden.
> **Das Teststudio für die Aufgaben befindet sich noch in einer Entwicklungsphase und wird im Projektzeitraum 2021-2023 grundlegend überarbeitet. 
> Die derzeitige Version nennt sich Teststudio Lite.**

#### IQB-Testcenter

Mit dieser Anwendung werden Kompetenztests durchgeführt und von den Testorganisator\*innen in den Abläufen getestet. Das **Testcenter**
besteht wieder vereinfacht ausgedrückt aus einer Datenbank und einer Benutzeroberfläche. Letztere wird mittels Adresseingabe in einem 
Internetbrowser geöffnet. Nach Anmeldung mit den entsprechenden Zugangsdaten, können die zuvor im **Teststudio** generierten Einheiten 
eines Tests geladen, gelöscht oder bestehende Dateien heruntergeladen werden. Die Einheiten, Metadaten und Konfigurationen des Tests werden 
dabei in der Datenbank gespeichert und verwaltet. Reihenfolgen, Bezeichnungen, Strukturen und Abläufe des Kompetenztests, können mittels 
Bearbeitung bestimmter Testeinheiten (Testdateien) beinflusst werden. Die Änderungen können dann von den Testorganisator\*innen in 
Probedurchläufen im **Testcenter** begutachtet werden. Dies trägt zu einem gesicherten Ablauf des finalen Tests bei.
Mehr zum Thema **Testcenter** erfahren Sie im gleichnamigen Kapitel.

#### IQB-Kodierbox

Die Antworten müssen geprüft und aufbereitet werden. Hierzu stehen für die Beteiligten entsprechen ihrer Rolle Funktionen wie Kodieren, 
Verifizieren, beschreibende Statistik abrufen oder Export als Excel-Datei zur Verfügung. Aus den aufbereiteten Daten werden schließlich 
die gewünschten Ergebnisse der Unternehmung erzeugt: Berichte, Publikationen, Rückmeldungen an Schulen.

> **Diese Web-Anwendung ist noch im Entwurfsstadium. Die Aufbereitung der Ergebnisse wird derzeit durch die Windows-Anwendung `itc-Toolbox` unterstützt.**

#### Archivierung und Veröffentlichung

Eine Testung, Befragung oder allgemein "Studie" sollte gut dokumentiert werden. Hierzu zählen die verwendeten Units, Testhefte, Roh-/Primärdaten, 
Analysedaten, Berichte aber auch Protokolle der Testdurchführung, eine Kritik der Analyseverfahren, Verweise auf Bildungsstandards etc.. 
Diese dann zu archivierende Dokumentation kann auch als Basis für eine Veröffentlichung der Daten für Sekundäranalysen in einem 
Forschungsdatenzentrum dienen. In einem Archiv wird besonderer Wert auf eine Langzeitarchivierung gelegt (besondere Speicherverfahren, 
besondere Formate für die Dateien usw.).

Wenn Aufgaben bzw. Fragebögen verwendet wurden, haben sie ihre Eignung für bestimmte Fragestellungen unter Beweis gestellt. 
Man weiß, unter welchen Bedingungen sie bei welchen Testpersonen mit welcher Genauigkeit Erkenntnisse liefern. 
Diese wertvollen Informationen können als Metadaten mit den Units und Testheften in einer Datenbank veröffentlicht werden. 
Über Suchformulare oder auch über Algorithmen können sie für andere Studien ausgewählt werden. Diese Studien mögen als 
Großprojekte in einem Jahrgang der Schulen eines Landes angelegt sein, es kann sich aber auch um einzelne Lehrkräfte handeln, 
die für einen kurzen Test in ihrem Kurs Aufgaben zusammenstellen.

> **Für Archivierung und Veröffentlichung gibt es derzeit keine spezialisierten Anwendungen.**

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2-Stand-der-Entwicklung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1-Einf%C3%BChrung">
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

# 1.2 Stand der Entwicklung

In einer [ersten Projektphase](https://www.iqb.hu-berlin.de/research/dm/tba/) hat das IQB die wichtigsten Web-Anwendungen prototypisch angelegt. Die [Projektphase 2021-2023](https://www.iqb.hu-berlin.de/research/dm/tba21/) dient dem Ausbau und der umfassenden Nutzbarmachung für die IQB-Aufgaben Bildungstrend und VERA. Diese Seite beschreibt den Entwicklungsstand jeweils zum Datum im Seitenkopf. Sie können über [eine E-Mail an unseren Mailing-Server](mailto:sympa@lists.hu-berlin.de?subject=subscribe%20iqb-tbadev-news) einen Newsletter abonnieren.

## IQB-Testcenter

Diese Web-Anwendung hat einige Einsätze absolviert und wird seitens des IQB als stabil und produktiv einsetzbar angesehen. Nächste Entwicklungsschritte:
* Massiver Ausbau der Dokumentation/ Wissensbasis, z. B. Entwicklung typischer Einsatzszenarien mit ausführlicher Verfahrensbeschreibung einschl. Datensicherheitskonzept
* Einsatz eingebettet in eine fremde Anwendungsumgebung: Das Einspielen von Testinhalten und das Auslesen von Testantworten erfolgt nicht über das Verwaltungsportal des IQB-Testcenters, sondern durch Drittanwendungen über das API des IQB-Testcenters.
* Optimierung des Installationspaketes hinsichtlich Lastverhalten während des Tests

## IQB-Teststudio

Diese Anwendung liegt derzeit als Prototyp vor. Kleine eingearbeitete Teams können hinreichend schnell Aufgaben gestalten. Diese einfache Version des IQB-Teststudios wird als IQB-Teststudio-Lite weitergeführt. Nächste Entwicklungsschritte:
* Verbesserung der Import/Export-Funktionen
* Konzeption eines IQB-Teststudios mit komplexen Arbeitsabläufen, differenzierten Rollen, Projektmanagement und Definition der Antwortverarbeitung

## IQB-Kodierbox

Diese Anwendung wird derzeit konzipiert. Die Ergebnisverarbeitung unterstützt aktuell eine Windows-Desktop-Anwendung mit dem Namen: **itc-Toolbox**.

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.3-Glossar">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward+++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-Überblick">
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

# 1.3 Glossar

<table>
  <tr>
    <td><a href="#Unit">Unit</a></td>
    <td><a href="#Testheft">Testheft/ Booklet</a></td>
    <td><a href="#Testperson">Testperson/ Testtaker</a></td>
  </tr>
</table>

---

```yaml
Dokumentstatus: Entwurf (TH 8.4.2021)
Stand: 1.4.2021
todo: - weitere wichtige Schlüsselthemen einbringen
```

## <a name="Unit"></a>Unit / Aufgabe / Seite

Eine Frage an die Testperson ist stets auf einer Seite platziert. Es ist nun meist nicht ökonomisch, nur eine Frage pro Seite vorzusehen, d. h. man gruppiert mehrere Fragen zusammen auf eine Seite. Es gibt noch weitere Seitenelemente, z. B. Fotos oder Sachtexte, die gleichzeitig zu den Fragen präsentiert werden sollen. In den IQB-Anwendungen nennen wir eine solche Gruppe von Elementen, die stets zusammen der Testperson präsentiert werden sollen, eine *Unit*. Diese Unit wird als Ganzes entwickelt, also in den Anwendungen als ein Paket editiert, importiert, exportiert usw. 

Es kann sich bei der Unit um eine einzelne *Seite nur mit Text* handeln - dann dient die Unit z. B. als Begrüßungsseite am Beginn des Tests oder als Ankündigung von Hörverstehensaufgaben mit der Aufforderung, die Kopfhörer aufzusetzen. Es können auch Frage-Elemente enthalten sein, deren Antworten für Kompetenztests ausgewertet werden - dann kann man die Unit eine *Aufgabe* nennen. Sollte es sich nicht um einen Kompetenztest, sondern um eine Befragung handeln, dann wird die Unit vielleicht *Abschnitt* genannt, denn es sind hier keine Aufgaben zu lösen.

Innerhalb einer Unit kann es sinnvoll sein, die Frage-Elemente auf mehrere Seiten zu verteilen. Z. B. soll ein Lesetext links ständig zu sehen sein, und rechts sollen nach und nach Seiten mit Fragen dazu präsentiert werden. Im Schulkontext ist dies weit verbreitet. In diesem Fall gibt es für den Gesamttest eine Navigation zwischen den Units, und innerhalb einer Unit außerdem eine Navigation zwischen den Seiten einer Unit.

## <a name="Testheft"></a>Testheft / Booklet / Testablauf / Aufgabenfolge

Für die Testdurchführung ist es notwendig, die Abfolge der Aufgaben/Seiten/Units festzulegen. Es können außerdem Festlegungen getroffen wie
* Zeitbeschränkung: Die Testperson hat nur eine bestimmte Zeit für die Beantwortung
* Freigabewort: Die Navigation wird erst erlaubt, wenn ein (von der Testleitung angesagtes) Codewort eingegeben wird. Darüber kann der Testablauf innerhalb einer Testgruppe (Klasse) zeitlich synchronisiert werden.
* Bedingte Fortsetzung/Filterführung: Nur bei bestimmten Antworten ist die Navigation insgesamt oder zu bestimmten Testblöcken erlaubt.

## <a name="Testperson"></a>Testperson / Testtaker / Testee / Befragte*r

Mit diesen Begriffen wird die Person bezeichnet, die als Endzweck der Studie befragt bzw. getestet wird. Die Antworten dieser Person bilden den Rohdatensatz der Studie. Um einen Testablauf zu erproben oder zu evaluieren, kann natürlich auch jemand aus dem Autorenteam diese Rolle einnehmen. Dann könnte die Durchführung modifiziert werden, damit z. B. nicht alle Hörtexte jedesmal gehört werden müssen oder die Navigation ist unbeschränkt. 

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.4-Studie-durchführen-Schritt-für-Schritt">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward+++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2-Stand-der-Entwicklung">
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

# 1.4 Studie durchführen Schritt für Schritt

Dieser Text fasst alle Schritte zusammen, die für eine kleinere Studie nötig sind. Es werden dabei nicht nur technische Aspekte angesprochen, sondern es fließen auch Erfahrungen im allgemeinen Testmanagement ein. Voraussetzung für diese Schritte sind die erfolgreichen Installationen der IQB-Anwendungen IQB-Teststudio und IQB-Testcenter. Nachfolgend finden Sie eine grobe Übersicht wie die IQB Instrumentarien zusammen arbeiten:

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/EF_Datenaust_TS_TC_final.png)

## Planung

Die Beteiligten brauchen rechtzeitig klare Anweisungen, wie die Studie vorbereitet, durchgeführt und ausgewertet wird. Hierzu sind zunächst eine Reihe von Fragen zu beantworten und ggf. bestimmte Schritte vorzuziehen. Mitunter müssen die Festlegungen in Dokumenten festgehalten und verschickt werden: allg. Handreichungen, Manual für die Testleitung, Anschreiben für System-Check, Anträge beim Datenschutz, Elternanschreiben, usw.

* Soll ein System-Check durchgeführt werden?
* Wie genau erfolgt die Anmeldung der Testperson (durch die Testaufsicht, oder nur teilweise, oder nur durch Link usw.?
* Soll der Testablauf einer Testgruppe beobachtet oder gesteuert werden (Testleitungskonsole)?
* Erhalten die Schulen eine Rückmeldung? Wie sieht die aus?
* Welche Zusatzmaterialien werden vor Ort benötigt: Taschenrechner, Lineal, Notizpapier, Kopfhörer?
* Stehen für die Durchführung Testleiterinnen oder Testleiter oder zumindest Coaches zur Verfügung?
* Soll es eine Hotline geben? Für welchen Zeitraum?
* Wie hoch ist das Risiko für technische Probleme? Soll jemand aus der Systemadministration oder Programmierung ständig greifbar sein?
* Wie lautet die genaue Internet-Adresse für die Testung bzw. Befragung?

## Units gestalten mit IQB-Teststudio

### Vorbereitung

* Zugangsdaten erhalten
* Neuen Arbeitsbereich (Workspace) anlegen lassen
* Testablauf planen: Welche Units, welche Zwischenseiten?
* Entscheidungen treffen: Welcher Player, welcher Editor?, ggf. in das IQB-Teststudio hochladen lassen
* ggf. Audios aufbereiten: Größe reduzieren, Exif-Metadaten eintragen
* ggf. Grafikdateien aufbereiten (Farben prüfen, Auflösung bei Zoom)
* Konventionen festlegen (Einrückung, Schriftart/-größe, Zeilenabstand, Formulierung bei Instruktionen, Benennung der Units usw.). Mehr dazu finden Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/IQB-Konventionen-Aufgabengestaltung)

### Übertragung organisieren

* Trello, CryptPad Kanban o. ä. einrichten, um für jede Unit den aktuellen Status zu dokumentieren
* Workflow definieren: Wer macht ersten Entwurf, wer schaut drüber, wer prüft psychometrisch, wer prüft fachdidaktisch usw.
* Schulungen und Austausch der Autorinnen und Autoren untereinander planen

### Gestaltung

* Gute Kurznamen für Units wählen, sprechende Titel
* Voransicht nutzen, um Layout und Verhalten zu prüfen
* Erzeugte IDs der Interaktionselemente notieren (canvasElement214...; z. B. über Excel- oder CryptPad-Tabelle)
* Beteiligte sollten sich regelmäßig ihre Units zeigen und Erfahrungen austauschen
* frühzeitig einige Units in das IQB-Testcenter übertragen, um deren Verhalten zu überprüfen
* Units regelmäßig als Dateien exportieren als Backup

### Export

* Units exportieren mit Xml und Voud
* Der Export im Teststudio erlaubt es, eine Booklet-Xml und eine Testtaker-Xml zu erzeugen, die zu den exportierten Units passt. Diese Dateien sind allerdings nur ein Vorschlag und sollten bearbeitet werden.

## Testcenter konfigurieren

### Vorbereitung

* Zugangsdaten erhalten
* Neuen Arbeitsbereich (Workspace) anlegen lassen
* System-Check ggf. einrichten und freigeben

### Units hochladen

* (Stand Februar 2021) Xml nachbearbeiten (s. [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Workaround-Unit%E2%80%90Xml))
* Erst die voud-Dateien, dann die Xml-Dateien hochladen. Es könnte sonst passieren, dass eine Xml abgewiesen wird, wenn sie auf eine nicht vorhandene Voud-Datei verweist.

### Testhefte hochladen

* Eine xlsx-Datei für die **ict-Toolbox** kann helfen, das Testdesign transparent zu 
  planen: Units, Blöcke, Testhefte sind hier einzutragen und dann die daraus erzeugten Xml-Dateien hochzuladen.
* Sollten Units im Testheft mehrfach auftauchen (z. B. Fragen zur Motivation) bitte darauf achten, dass die Units unterschiedliche Aliase bekommen!

### Review und Probelauf

* Allgemein bitte [diese Hinweise](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren) zu Logins beachten.
* Die Xml zu Testteilnehmern (sog. Testtaker) ersteinmal nur für [Review-Modus](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung) anlegen für alle Verantwortlichen der Studie hochladen.
* Nach jeder Review-Schleife die Kommentare aus dem Testcenter-Admin-Portal herunterladen und auswerten, Änderungen an den Units vornehmen, neu exportieren und NUR DIE 
  neuen VOUD-Dateien ins Testcenter hochladen (sonst überschreibt man die Xml-Änderungen).
* Auch Logins im hot-restart-Modus anlegen, Real-Time-Tests durchführen und sorgfältig auswerten

## Studie durchführen

* Logins für Durchführung hochladen, ggf. Zeitfenster gut dokumentieren
* täglich Antworten und Logs ziehen und speichern
* Probeauswertungen vornehmen: Nur so erkennt man früh, wenn bestimmmte Variablen nicht ankommen
* Hotline auswerten, auch erste Testprotokolle analysieren

## Auswertung, Evaluation

* Daten wie vorgesehen auswerten, Berichte schreiben, Rückmeldung an Schulen geben
* Evaluieren: Dabei hilft die Vorstellung, dass man die gleiche Studie nächste Woche nochmal durchführen soll

---

<!--+++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.5-Copyright,-Lizenz">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.3-Glossar">
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

# 1.5 Copyright, Lizenz

```yaml
Dokumentstatus: Review
Stand: 1.4.2021
todo: - Aufgabenaustausch > Wo soll dortiger Link hin verweisen?
```

Das IQB ist länderfinanziert und erhält daher Aufträge stets mit Blick auf den Nutzen für die Länder der Bundesrepublik Deutschland. Dies ist insbesondere beim computerbasierten Testen im Bildungswesen der Fall. Denn wenn bisher die Aufgaben als Druckvorlagen an die Länder geliefert wurden, die jede Druckerei vervielfältigen kann, sind Testaufgaben im Online-Format nur durch spezielle Testsysteme nutzbar. Das Speicherformat muss kompatibel sein.

Viele der Kompetenztestungen finden durch die Länder selbst statt ohne Beteiligung des IQB. Daher sind alle Programmierarbeiten am IQB mit der *Auflage verbunden, die Nutzbarkeit der Aufgaben durch die Länder sicherzustellen*.

## Software ist frei nutzbar

Der erste Schritt hierzu ist die Veröffentlichung des Codes und der Dokumentationen sowie der Installationspakete aller IQB-Anwendungen hier auf GitHub. Alle Interessierten können die Software installieren und ohne Kenntnis des IQB einsetzen. Gemäß des o. g. Auftrages sind wir sehr daran interessiert, die Nutzung durch Dritte zu unterstützen, insbesondere durch die Länder.

## Aufgabenaustausch

Wie sieht es aber mit Einrichtungen aus, die eigene Anwendungen (weiter-)nutzen? Wie können hier die Aufgaben eingesetzt werden? Eine länderübergreifende Fachgruppe evaluierte die Optionen. Zunächst wurde die Nutzung eines vorhandenen Speicherstandards verworfen. Entweder erfüllt ein Standard nicht alle Anforderungen (nicht alle Interaktionsformate können abgebildet werden), oder zu dessen Verwendung ist Software nötig, die zu teuer oder nur über spezialisierte Dienstleister nutzbar ist. Einen neuen Standard für ein Speicherformat zu entwickeln, wurde ebenfalls verworfen.

Die Lösung liegt darin, viele Speicherformate zuzulassen und jeweils Programmcode mitzuliefern, der zwischen Testsystem und der Aufgabe vermittelt. Für spezielle Anforderungen können also jederzeit neue Speicherformate entwickelt werden, solange der erforderliche Programmcode mitgeliefert wird. Ein vorhandenes Testsystem muss nur einmalig die Schnittstelle zu derartigem Programmcode implementieren.

Mehr zu diesem Thema entnehmen Sie bitte diesem [Kapitel](1.7-Technische-Details).

### Lizenzen

[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/) für Spezifikationen, Dokumentationen, Videos, Metadatenkataloge und ähnliche Inhalte.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT) für Programmcode.

Diese Lizenzen sollen die Verwendung so wenig wie möglich einschränken. Auch eine Nutzung in kommerziellem Zusammenhang ist möglich, solange Urheber genannt werden und die abgeleiteten Produkte ebenfalls frei zugänglich sind.

---

<!--+++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.6-Herausforderung-VERA">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.4-Studie-durchführen-Schritt-für-Schritt">
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

# 1.6 Herausforderung VERA

Der Name VERA steht für "Vergleichsarbeiten". Diese groß angelegten Kompetenztests dienen der Qualitätssicherung auf Ebene der
Schulen. Weitere Informationen finden Sie beim [IQB](https://www.iqb.hu-berlin.de/vera/) und bei der [Kultusministerkonferenz](https://www.kmk.org/fileadmin/Dateien/veroeffentlichungen_beschluesse/2015/2015_06_11-Gesamtstrategie-Bildungsmonitoring.pdf). 

Die Testaufgaben und auch die Zusammenstellungen der Aufgaben (Module, Testhefte) werden vom IQB geliefert. Die Durchführung selbst liegt in der Hand der Länder, d. h. es gibt hier keine gemeinsame Infrastruktur. Beim bisherigen papierbasierten Verfahren übergibt das IQB Druckvorlagen (pdf), die in Länderregie gedruckt und verteilt werden. Hier kommen mitunter Online-Portalsysteme zum Einsatz, um die Logistik zu bewältigen, aber auch um die Antworten der Schülerinnen und Schüler einzugeben und zu bewerten. Die Lehrkräfte erhalten außerdem über diese Portale die Ergebnisse der Datenanalysen, aus denen sie für den Unterricht Verbesserungen ableiten können (sog. Rückmeldungen).

Die ersten Ansätze der Online-Durchführung sehen eine manuelle Übertragung der Papierversion der Aufgaben in ein Online-Format vor. Das jeweilige vorhandene Portalsystem wird um einen Onlinetest erweitert. Diese Übertragung der Aufgaben erfolgt für jedes Portalsystem für jedes Jahr. Auf diese Art können viele Länder seit einigen Jahren den Schulen parallel eine Online-Durchführung von VERA anbieten.

Der nächste Schritt ist die Lieferung der Aufgaben durch das IQB im Online-Format. Angesichts der Vielfalt der vorhandenen technischen Lösungen ist dies ein anspruchsvolles [Vorhaben](https://www.iqb.hu-berlin.de/tba/online/) und wird viele Jahre in Anspruch nehmen.

![Schema Online-Durchführung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Running-VERA.png)

---

<!--+++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.7-Technische-Details">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.5-Copyright,-Lizenz">
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

# 1.7 Technische Details

```yaml
Dokumentstatus: Entwurf
Stand: 6.4.2021
todo: - weitere techn. details einbringen
```

Ideen zu vielleicht hier gesetzten Verlinkungen:

* [Verona Interface Einführung](https://box.hu-berlin.de/f/a6de8bd03626451a93d0/)

## Verona Interfaces

[Text von:](http://iqbstaff.pbworks.com/w/page/143201397/TBA-Tools#VeronaInterfaces)

Zum Abspielen, Tests durchführen, Daten ausgeben, Logins festlegen usw. (alles was zum TBA-testen nötig ist) kann man entweder das IQB-Testcenter benutzen ("Auswertuns-/Kodierungsgmodul" fehlt allerdings noch) oder eine Verona Interface Schnittstelle nutzen um ein eigens programmiertes Testcenter zu nutzen und die IQB-Tests "abzuspielen". Ein Video von Martin auf GitHub (ca. 9 Minuten) Testcenter oder Verona? erläutert beide Szenarien (sehr technisch bzw. konzeptionell, wohl eher für auswertenden Einrichtungen relevant) 

    Verona steht für VERA-Online 
    Verona Interfaces sind Schnittstellen zu Programmen/Modulen vom IQB zur VERA-Testungen im TBA-Format
    daher fand Modularisierung der Komponenten des Testcenters statt
    Grund: Flexibilität z.B. in Verwendung neuer Aufgabenformate zu haben 
    dazu Entkopplung innerhalb des Testcenters von Präsentation der Aufgabe (Player) & Testsystem (Login, Aufgabe laden, Antworten/Log speichern usw.)
    zwischen Testsystem und Player muss Kommunikation bestehen, passiert in Form von Schnittstelle (=Plug-In-Schnittstelle)
    IQB liefert also immer auch den Player aus (+ Testsystem), Länder müssen Schnittstellendefinition noch leisten
    der Player ändert sich also, wenn beispielsweise ein neues Testformat entwickelt wurde, das Testsystem muss jedoch nicht "nachprogrammiert" werden, allerdings die Schnittstelle 
    das IQB hat ein Testsystem (dies heißt Testcenter, siehe oben) für seine eigenen Bedürfnisse, die Länder können ein (oder mehrere) eigene/andere Testsysteme haben, dafür muss nur die Schnittstelle bedient werden und nicht grundsätzlich eine neues Testsystem aufgebaut werden (Ansteuerung und Anpassung des Testsystems über eine Schnittstelle) 
    die Schnittstelle ist vor allem auch dafür verantwortlich, dass Antworten, die in Form von Rohdaten vorliegen, in ein Standardformat umgewandelt werden (Response Converter)
    auch muss die Antwortverarbeitung vorab geplant werden (im VERA-Paper-Pencil-Prozess heißt es Antwortschema), ein Responce Scheme (wie es hier im TBA-Kontext genannt wird) ist als extra Modul also auch notwendig 
    insgesamt besteht die Schnittstelle aus 4 Modulen: Editor, Player, Response Scheme, Response Converter
    ein Testsystem (z.B. Testcenter zu nennen, wie im IQB) in dem der Test durchgeführt werden kann (Pilotierung im IQB, Hauptdurchgang in einem Land) bräuchte einen Player und einen Response Converter
    ein Teststudio in dem die Aufgaben und Tests entwickelt werden, bräuchte Editor (Authoring), Response Scheme und Player (für Demo-Voransicht der Aufgaben) 
    Video Verona Interfaces: Einführung auf GitHub von Martin (ca. 14 Minuten)
    weitere Videos in der Reihe zeigen 
         Aufbau und Funktionsweise des Players (ca. 17 Minuten): Verona Interfaces 2. Player: Modell 
        weiteres zum Player und Beschreibung des API (Backend-Programmierung) (ca. 24 Minuten): Verona Interfaces 3. Player: API

               (alle Videos sind auch eher technisch bzw. konzeptionell, wohl auch eher für auswertenden Einrichtungen relevant) 
---
<!--+++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.6-Herausforderung-Vera">
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