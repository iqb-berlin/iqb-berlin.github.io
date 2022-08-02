# 1. Einführung

## Zum Begriff TBA

TBA steht für Technology Based Assessment, also technologie- oder technikbasiertes Testen. Damit ist nicht nur der Computer als Testinstrument gemeint, sondern auch andere digitale Hilfsmittel wie z. B. Stifte, die beim Schreiben scannen. Am IQB wird zur Zeit nur der Computer (Desktop, Tablet, Notebook) als Medium eingesetzt. Daher kann man CBA - Computer Based Assessement - hier als Synonym betrachten für TBA. Andere Begriffe wie Digital Assessment sind ebenfalls zutreffend.

## Projektbezug

Nach zahlreichen Vorarbeiten arbeitet das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de)
seit 2018 gezielt im Auftrag der Länder an der Umstellung der papierbasierten Kompetenzerhebung auf eine technologiebasierte Durchführung. 
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

Hier finden Sie einführende Videos zu den IQB-Anwendungen
* [Einführung in die IQB TBA-Systeme](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-TBA-Einf%C3%BChrung)

![iqb applications: testcenter, teststudio, codingbox](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/einfuehrung_2.png)

#### IQB-Studio

Das **Studio** besteht vereinfacht ausgedrückt aus einer Datenbank und einer Benutzeroberfläche.
Letztere kann mittels einer Adresse in einem Internetbrowser geöffnet werden. Anschließend erfolgt eine Anmeldung mit den entsprechenden 
Zugangsdaten. In die Benutzeroberfläche ist ein Editor eingebettet, mit dessen Hilfe die interaktiven Einheiten eines Kompetenztests 
(Units) bearbeitet und erstellt werden können. Nähere Informationen zur Bearbeitung und Erstellung von Aufgaben sind dem Kapitel:
**Studio** zu entnehmen. Nach finaler Editierung der Aufgaben erzeugt das **Studio** die Einheiten eines Kompetenztests 
(Units und weitere für den Test erforderliche Dateien) in einem komprimierten Dateiformat (Zip-Datei). Die Einheiten können bei Bedarf 
nachträglich bearbeitet und an die entsprechende Testumgebung angepasst werden. Anschließend können die Testdateien dann im **Testcenter** 
geladen und wiedergegeben werden.
> **Das Studio für die Aufgaben befindet sich noch in einer Entwicklungsphase und wird im Projektzeitraum 2021-2023 grundlegend überarbeitet. 
> Die derzeitige Version nennt sich Studio Lite. Die finale Version wird dann nur noch Studio heißen.**

#### IQB-Testcenter

Mit dieser Anwendung werden Kompetenztests durchgeführt und von den Testorganisator\*innen in den Abläufen getestet. Das **Testcenter**
besteht wieder vereinfacht ausgedrückt aus einer Datenbank und einer Benutzeroberfläche. Letztere wird mittels Adresseingabe in einem 
Internetbrowser geöffnet. Nach Anmeldung mit den entsprechenden Zugangsdaten unterscheidet das System zwischen Testperson (die Aufgaben/Seiten werden zur Bearbeitung präsentiert) und Verwaltung (die zuvor im **Studio** generierten Einheiten 
eines Tests werden geladen, gelöscht oder Antwortdaten heruntergeladen). Die Einheiten, Metadaten und Konfigurationen des Tests, sowie die gegebenen Antworten, werden dabei in der Datenbank gespeichert und verwaltet.

Mehr zum Thema **Testcenter** erfahren Sie im gleichnamigen Kapitel.

#### IQB-Kodierbox

Die Antworten müssen geprüft und aufbereitet werden. Hierzu stehen für die Beteiligten entsprechend ihrer Rolle Funktionen wie Kodierung, 
Verifizierung, beschreibende Statistik oder Export als Excel-Datei zur Verfügung. Aus den aufbereiteten Daten werden schließlich 
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
* Ausbau der Dokumentation/ Wissensbasis, z. B. Entwicklung typischer Einsatzszenarien mit ausführlicher Verfahrensbeschreibung einschl. Datensicherheitskonzept
* Einsatz eingebettet in eine fremde Anwendungsumgebung: Das Einspielen von Testinhalten und das Auslesen von Testantworten erfolgt nicht über das Verwaltungsportal des IQB-Testcenters, sondern durch Drittanwendungen über das API des IQB-Testcenters.
* Verbesserung des Lastverhalten bei der Anmeldung
* Download der Antworten bereits teilweise kodiert und bewertet

## IQB-Studio

Diese Anwendung liegt derzeit als Prototyp vor. Kleine eingearbeitete Teams können hinreichend schnell Aufgaben gestalten. Diese einfache Version des IQB-Studio wird als IQB-Studio-Lite weitergeführt. Nächste Entwicklungsschritte:
* Verbesserung der Import/Export-Funktionen
* Editieren des Antwortschemas zur Unterstützung der automatisierten Kodierung
* Konzeption eines IQB-Studio mit komplexen Arbeitsabläufen, differenzierten Rollen, Projektmanagement und Definition der Antwortverarbeitung

## IQB-Kodierbox

Diese Anwendung wird derzeit konzipiert. Die Ergebnisverarbeitung unterstützt aktuell eine Windows-Desktop-Anwendung mit dem Namen: **itc-Toolbox**. Mehr Informationen dazu erhalten Sie [hier](https://github.com/iqb-berlin/itc-toolbox#readme)

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
    <td><a href="#backend">Backend</a></td>
	<td><a href="#frontend">Frontend</a></td>
	<td><a href="#player">Player</a></td>
	<td><a href="#responsivität">Responsivität</a></td>
    <td><a href="#testheft">Testheft/ Booklet</a></td>
    <td><a href="#testperson">Testperson/ Testtaker</a></td>	
	<td><a href="#unit">Unit</a></td>
	<td><a href="#verona">Verona</a></td>
	<td><a href="#voud">Voud</a></td>
		
  </tr>
</table>

## <a name="backend"></a>Backend

Die Online-Programmierungen des IQB bestehen stets aus einer Serverkomponente ("Backend") und einer Clientkomponente ("Frontend"). Die Serverkomponente besteht aus Code, enthält aber auch eine Datenbank. Die Funktionen des Backends sind verdeckt: Anwender\*innen interagieren nur mit dem was im Browser geladen ist. Die Kommunikation mit dem Server (Anmeldeprozess, Holen von Daten, Speichern von Änderungen usw.) läuft im Hintergrund.

## <a name="frontend"></a>Frontend

Die Online-Programmierungen des IQB bestehen stets aus einer Serverkomponente ("Backend") und einer Clientkomponente ("Frontend"). Die Clientkomponente ist der Programmcode, der beim Aufruf einer Seite in den Browser geladen wird und mit dem danach die Anwender\*innen interagieren. Das IQB gestaltet diese Seiten so, dass jeder Klick oder jede Eingabe zunächst durch Programmcode im Browser verarbeitet wird und erst später je nach Bedarf ein Datentransfer mit dem Server angestoßen wird. Diese Art Webanwendungen nennt man "Single Page Application", da ein Klick keine wirkliche Navigation im Sinne einer Webseite auslöst, sondern die Programmierung die Ansicht wechselt.

## <a name="player"></a>Player

Ein Player ist eine Html-Datei mit JavaScript-Programmierung. Diese wird in einer Webanwendung (z. B. Testcenter, Studio) für die Darstellung der Aufgaben / Units / Seiten verwendet. Das "Abspielen" der Unit deckt auch sämtliche Interaktionen der Testperson ab, z. B. Texteingaben. Zwischen Player und Webanwendung ist der Datenaustausch standardisiert (sog. Verona-Schnittstelle). Dadurch ist gesichert, dass die Antworten gespeichert werden.

Die Trennung der Programmierung an dieser Stelle hat den großen Vorteil, dass sehr verschiedene Aufgabentypen in einem Test flexibel verwendet werden können. Von einfachen Formularen bis zu komplexen Zeichnungen können Aufgaben passend zu den Anforderungen gestaltet werden. Jede Verona-kompatible Webanwendung kann neue und exotische Aufgaben ohne eine Neuinstallation einsetzen. Es müssen nur jeweils zu den Aufgabendefinitionen passende Player bereitgestellt werden.

## <a name="responsivität"></a>Responsivität

In der Webprogrammierung bezeichnet dieser Begriff die Fähigkeit einer Website auf unterschiedliche Bildschirmgrößen zu reagieren. Die Inhalte verhalten sich dynamisch und werden an die aktuelle Bildschirmauflösung angepasst (skaliert). Bei Webanwendungen für Kompetenztests spielt die Steuerung dieser Anpassung eine große Rolle, da sie großen Einfluss auf die Antworten hat.

## <a name="syscheck"></a>System-Check

Computerbasierte Lernstandserhebungen stellen bestimmte Anforderungen an die Hardware und Software sowie die Internet-Verbindung vor Ort an der Schule. Über einen System-Check lassen sich diese Anforderungen überprüfen. Daher bieten viele TBA-Systeme diese Funktion an.

## <a name="testheft"></a>Testheft / Booklet / Testablauf / Aufgabenfolge

Für die Testdurchführung ist es notwendig die Abfolge der Aufgaben/Seiten/Units festzulegen. Es können außerdem Festlegungen getroffen werden wie
* Zeitbeschränkung: Die Testperson hat nur eine bestimmte Zeit für die Beantwortung
* Freigabewort: Die Navigation wird erst erlaubt, wenn ein (von der Testleitung angesagtes) Codewort eingegeben wird. Darüber kann der Testablauf innerhalb einer Testgruppe (Klasse) zeitlich synchronisiert werden.
* Bedingte Fortsetzung/Filterführung: Nur bei bestimmten Antworten ist die Navigation insgesamt oder zu bestimmten Testblöcken erlaubt.

## <a name="testperson"></a>Testperson / Testtaker / Testee / Befragte*r

Mit diesen Begriffen wird die Person bezeichnet, die als Endzweck der Studie befragt bzw. getestet wird. Die Antworten dieser Person bilden den Rohdatensatz der Studie. Um einen Testablauf zu erproben oder zu evaluieren, kann natürlich auch jemand aus dem Autorenteam diese Rolle einnehmen. Dann könnte die Durchführung modifiziert werden, damit z. B. nicht alle Hörtexte jedesmal gehört werden müssen oder die Navigation ist unbeschränkt. 

## <a name="unit"></a>Unit / Aufgabe / Seite

Eine Frage an die Testperson ist stets auf einer Seite platziert. Es ist nun meist nicht ökonomisch nur eine Frage pro Seite vorzusehen, besser man gruppiert mehrere Fragen zusammen auf eine Seite. Es gibt noch weitere Seitenelemente, z. B. Fotos oder Sachtexte, die gleichzeitig zu den Fragen präsentiert werden sollen. In den IQB-Anwendungen nennen wir eine solche Gruppe von Elementen, die stets zusammen mit der Testperson präsentiert werden sollen, eine *Unit*. Diese Unit wird als Ganzes entwickelt, also in den Anwendungen als ein Paket editiert, importiert, exportiert usw..

Es kann sich bei der Unit um eine einzelne *Seite nur mit Text* handeln - dann dient die Unit z. B. als Begrüßungsseite am Beginn des Tests oder als Ankündigung von Hörverstehensaufgaben mit der Aufforderung bspw. die Kopfhörer aufzusetzen. Es können auch Frage-Elemente enthalten sein, deren Antworten für Kompetenztests ausgewertet werden - dann kann man die Unit eine *Aufgabe* nennen. Sollte es sich nicht um einen Kompetenztest, sondern um eine Befragung handeln, dann wird die Unit vielleicht *Abschnitt* genannt, denn es sind hier keine Aufgaben zu lösen.

Innerhalb einer Unit kann es sinnvoll sein die Frage-Elemente auf mehrere Seiten zu verteilen. Bspw. soll ein Lesetext links ständig zu sehen sein, und rechts sollen nach und nach Seiten mit Fragen dazu präsentiert werden. Im Schulkontext ist dies weit verbreitet. In diesem Fall gibt es für den Gesamttest eine Navigation zwischen den Units und innerhalb einer Unit, außerdem eine Navigation zwischen den Seiten einer Unit.

## <a name="verona"></a>Verona

Lernstandserhebungen in den Ländern als Teil des nationalen Bildungsmonitorings gibt es papierbasiert seit 2003. Diese Vergleichsarbeiten werden mit der Abkürzung VERA bezeichnet. Die Bemühungen um computerbasierte Erhebungen von Kompetenzen starteten zuerst im VERA-Kontext. Aus der Verbindung mit "Online" wurde dann die Bezeichnung "Verona" für VERA Online.

Inzwischen werden die technischen Spezifikationen und auch die Webanwendungen so offen gestaltet, dass auch Tests aus anderen Projekten möglich sind. Beispielsweise können auch Befragungen damit durchgeführt werden, die nichts mit VERA zu tun haben. Trotzdem hat sich die Bezeichnung für Anwendungen und Module erhalten, die sich an die Verona-Spezifikationen für Schnittstellen und Datenformate halten.

## <a name="voud"></a>Voud

Bei diesem Dateiformat handelt es sich um eine IQB-Definition zur Speicherung von Aufgabeninhalten (Aufgabenlementen) wie bspw. Audio, Grafiken, Multiple-Choice Elementen und mehr. Die Bezeichnung **voud** steht für: **VerOna Unit Definition**. Bei der Erzeugung einer Unit mittels **Studio** generiert das **Studio** meist eine Unit.xml und eine Unit.voud. Die Unit.xml enthält Metadaten zur allgemeinen Beschreibung der Unit, z. B. Name, Titel und Zeitpunkt der letzten Änderung. Die Voud-Datei enthält alle Daten, die bei der Ausführung der Unit durch den Player erforderlich sind.

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

Dieser Text fasst alle Schritte zusammen, die für eine kleinere Studie nötig sind. Es werden dabei nicht nur technische Aspekte angesprochen, sondern es fließen auch Erfahrungen im allgemeinen Testmanagement ein. Voraussetzung für diese Schritte sind die erfolgreichen Installationen der IQB-Anwendungen: **IQB-Studio** und **IQB-Testcenter**. 

Nachfolgend finden Sie eine grobe Übersicht wie die IQB Instrumentarien zusammenarbeiten:

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/EF_Datenaust_TS_TC_final.png)

## Planung

Die Beteiligten brauchen rechtzeitig klare Anweisungen, wie die Studie vorbereitet, durchgeführt und ausgewertet wird. Hierzu sind zunächst eine Reihe von Fragen zu beantworten und ggf. bestimmte Schritte vorzuziehen. Mitunter müssen die Festlegungen in Dokumenten festgehalten und verschickt werden: allg. Handreichungen, Manual für die Testleitung, Anschreiben für System-Check, Anträge beim Datenschutz, Elternanschreiben, usw.

* Soll ein System-Check durchgeführt werden?
* Wie genau erfolgt die Anmeldung der Testperson (durch die Testaufsicht, oder nur teilweise, oder nur durch Link usw.)?
* Soll der Testablauf einer Testgruppe beobachtet oder gesteuert werden (Testleitungskonsole)?
* Erhalten die Schulen eine Rückmeldung? Wie sieht diese aus?
* Welche Zusatzmaterialien werden vor Ort benötigt: Taschenrechner, Lineal, Notizpapier, Kopfhörer?
* Stehen für die Durchführung Testleiterinnen oder Testleiter oder zumindest Coaches zur Verfügung?
* Soll es eine Hotline geben? Für welchen Zeitraum?
* Wie hoch ist das Risiko für technische Probleme? Soll jemand aus der Systemadministration oder Programmierung ständig greifbar sein?
* Wie lautet die genaue Internet-Adresse für die Testung bzw. Befragung?

## Units gestalten mit IQB-Studio

### Vorbereitung

* Zugangsdaten erhalten
* Neuen Arbeitsbereich (Workspace) anlegen lassen
* Testablauf planen: Welche Units, welche Zwischenseiten?
* Entscheidungen treffen: Welcher Player, welcher Editor?, ggf. in das IQB-Studio hochladen lassen
* ggf. Audios aufbereiten: Größe reduzieren, Exif-Metadaten eintragen
* ggf. Grafikdateien aufbereiten (Farben prüfen, Auflösung bei Zoom)
* Konventionen festlegen (Einrückung, Schriftart/-größe, Zeilenabstand, Formulierung bei Instruktionen, Benennung der Units usw.). Mehr dazu finden Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/IQB-Konventionen-Aufgabengestaltung)

### Übertragung organisieren

* Trello, CryptPad, Kanban o. ä. einrichten, um für jede Unit den aktuellen Status zu dokumentieren
* Workflow definieren: Wer macht ersten Entwurf, wer schaut drüber, wer prüft psychometrisch, wer prüft fachdidaktisch usw.
* Schulungen und Austausch der Autorinnen und Autoren untereinander planen

### Gestaltung

* Gute Kurznamen für Units wählen, sprechende Titel
* Voransicht nutzen, um Layout und Verhalten zu prüfen
* Erzeugte IDs der Interaktionselemente prüfen, um die Antwortverarbeitung zu steuern (z. B. über Excel- oder CryptPad-Tabelle)
* Beteiligte sollten sich regelmäßig ihre Units zeigen und Erfahrungen austauschen
* frühzeitig einige Units in das IQB-Testcenter übertragen, um deren Verhalten zu überprüfen
* Units regelmäßig als Dateien exportieren als Backup

### Export

* Units exportieren mit XML und Voud
* Der Export im Studio erlaubt es, eine Booklet-XML und eine Testtaker-XML zu erzeugen, die zu den exportierten Units passt. Diese Dateien sind allerdings nur ein Vorschlag und sollten bearbeitet werden.

## Testcenter konfigurieren

### Vorbereitung

* Zugangsdaten erhalten
* Neuen Arbeitsbereich (Workspace) anlegen lassen
* System-Check ggf. einrichten und freigeben

### Units und Testhefte hochladen

* Hier ist Reihenfolge der Dateien wichtig, da eine Prüfung der Abhängigkeiten der Dateien untereinander erfolgt und ggf. das Hochladen abgelehnt wird.
* Eine xlsx-Datei für die **ict-Toolbox** kann helfen, das Testdesign transparent zu 
  planen: Units, Blöcke, Testhefte sind hier einzutragen und dann die daraus erzeugten XML-Dateien hochzuladen.
* Sollten Units im Testheft mehrfach auftauchen (z. B. Fragen zur Motivation) bitte darauf achten, dass die Units unterschiedliche Aliase bekommen!
* Bitte [diese Hinweise](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren) zu Logins beachten.

### Review und Probelauf

* Die XML zu Testteilnehmer\*innen (die sog. Testtaker.xml) ersteinmal nur für [Review-Modus](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung) anlegen und für alle Verantwortlichen der Studie hochladen.
* Nach jeder Review-Schleife die Kommentare aus dem Testcenter-Admin-Portal herunterladen und auswerten, Änderungen an den Units vornehmen, neu exportieren und NUR DIE 
  neuen VOUD-Dateien ins Testcenter hochladen (sonst überschreibt man die XML-Änderungen).
* Auch Logins im hot-restart-Modus anlegen, Real-Time-Tests durchführen und sorgfältig auswerten

## Studie durchführen

* Logins für Durchführung hochladen, ggf. Zeitfenster gut dokumentieren
* täglich Antworten und Logs herunterladen und speichern
* Probeauswertungen vornehmen: Nur so erkennt man früh, wenn bestimmmte Variablen nicht ankommen
* Test auswerten, auch erste Testprotokolle analysieren

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

Das IQB ist länderfinanziert und erhält daher Aufträge stets mit Blick auf den Nutzen für die Länder der Bundesrepublik Deutschland. Dies ist insbesondere beim computerbasierten Testen im Bildungswesen der Fall. Denn wenn bisher die Aufgaben als Druckvorlagen an die Länder geliefert wurden, die jede Druckerei vervielfältigen kann, sind Testaufgaben im Online-Format nur durch spezielle Testsysteme nutzbar. Das Speicherformat muss kompatibel sein.

Viele der Kompetenztestungen finden durch die Länder selbst statt ohne Beteiligung des IQB. Daher sind alle Programmierarbeiten am IQB mit der *Auflage verbunden, die Nutzbarkeit der Aufgaben durch die Länder sicherzustellen*.

## Software ist frei nutzbar

Der erste Schritt hierzu ist die Veröffentlichung des Codes und der Dokumentationen sowie der Installationspakete aller IQB-Anwendungen hier auf GitHub. Alle Interessierten können die Software installieren und ohne Kenntnis des IQB einsetzen. Gemäß des o. g. Auftrages sind wir sehr daran interessiert, die Nutzung durch Dritte zu unterstützen, insbesondere durch die Länder.

## Aufgabenaustausch

Wie sieht es aber mit Einrichtungen aus, die eigene Anwendungen (weiter-)nutzen? Wie können hier die Aufgaben eingesetzt werden? Eine länderübergreifende Fachgruppe evaluierte die Optionen. Zunächst wurde die Nutzung eines vorhandenen Speicherstandards verworfen. Entweder erfüllt ein Standard nicht alle Anforderungen (nicht alle Interaktionsformate können abgebildet werden), oder zu dessen Verwendung ist Software nötig, die zu teuer oder nur über spezialisierte Dienstleister nutzbar ist. Einen neuen Standard für ein Speicherformat zu entwickeln, wurde ebenfalls verworfen.

Die Lösung liegt darin, viele Speicherformate zuzulassen und jeweils Programmcode mitzuliefern, der zwischen Testsystem und der Aufgabe vermittelt. Für spezielle Anforderungen können also jederzeit neue Speicherformate entwickelt werden, solange der erforderliche Programmcode mitgeliefert wird. Ein vorhandenes Testsystem muss nur einmalig die Schnittstelle zu derartigem Programmcode implementieren.

Weitere technische Informationen finden Sie [hier](1.7-Technische-Details).

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

## Modelle der Durchführung

### Nutzung des IQB-Testcenters

Für die Testdurchführung kann das IQB-Testcenter verwendet werden. Die [Lizenz MIT](https://opensource.org/licenses/MIT) erlaubt dies ohne Einschränkungen. Allerdings bietet das IQB keinen Serverdienst an, d. h. die Testungen laufen nicht am IQB. Es muss das IQB-Testcenter auf einem landeseigenen oder angemieteten Server installiert werden. Dafür stellt das IQB ein [Setup-Paket](https://github.com/iqb-berlin/testcenter-setup#readme) zur Verfügung.

Die Installation kann weitgehend an das Länder-Design angepasst werden: Durch Änderung von Farben, Bezeichnungen und dem Logo merken die Testpersonen nicht, dass es sich um eine IQB-Programmierung handelt. Die Bezeichnung "IQB-Testcenter" z. B. ist ersetzbar.

Die Definitionen für die Aufgaben, Tests, Testpersonen und ggf. System-Checks können über das Verwaltungsportal der Anwendung in das Testcenter übertragen werden. Soll dieser Datentransfer und auch das Herunterladen der Antworten nicht manuell, sondern über andere Programmierungen erfolgen (z. B. Schulportale), dann kann das IQB-Testcenter auch über ein API angesprochen werden. Die Dokumentation dazu finden Sie [hier](https://iqb-berlin.github.io/testcenter-backend/api/).

### Durchführung in eigenem Testsystem

Wenn die gelieferten IQB-Aufgaben in einer eigenen Testanwendung genutzt werden sollen, dann muss diese die Verona-Schnittstelle unterstützen. Vor dem Laden einer Aufgabe wird dann das zugehörige Player-Modul geladen. Die Dokumentation der Schnittstelle finden Sie [hier](https://github.com/verona-interfaces/player/#readme).


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

Die Anwendungen des IQB sind so programmiert und veröffentlicht, dass es möglichst einfach ist, sie zu installieren, anzupassen und ggf. neue Versionen einzuspielen.

## Installation

Wir veröffentlichen sog. Docker-Setups. Ein Server muss nur die Virtualisierungslösung [Docker](https://www.docker.com/) unterstützen. Durch die Installation werden dann automatisch die einzelnen Systeme (Frontend, Datenbank, Backend, ggf. zweites Backend, Routing über Traefik) installiert. Die Installationsanleitung (z. B. für das Testcenter [hier](https://github.com/iqb-berlin/testcenter-setup#readme)) gibt dann detaillierte Hinweise für Anpassungen nach der Installation.

### Update

Es werden kontinuierlich neue Versionen veröffentlicht. Es handelt sich dann um Funktionserweiterungen, aber auch Fehler werden regelmäßig zu beheben sein. Im Installationspaket sind Skripte für den Update-Vorgang hinterlegt, die die lokalen Einstellungen und die vorhandenen Daten erhalten. Sollten Änderungen der Datenbank erforderlich sein, werden diese gezielt so vorgenommen, dass die alten Daten erhalten oder ggf. transformiert werden.

## Verona-Module

Programmierungen, die die Darstellung einzelner Aufgaben betreffen, sind nicht fester Bestandteil der Installationen. Auch das Editieren eines speziellen Aufgabentyps ist in separate Programm-Module ausgelagert. Diese Module müssen nach der Installation über das Verwaltungsportal in das System eingespielt werden. Ein solches Plug-In-Verfahren hat den großen Vorteil, dass Änderungen an den Programmierungen nicht über die Serveradministration eingespielt werden müssen, sondern die inhaltlich Verantwortlichen jederzeit diese Programmteile hinzufügen oder ersetzen können.

Voraussetzung für dieses Modul-System ist die Definition einer Schnittstelle, die wir in Zusammenhang mit dem computerbasierten Testen "Verona" nennen. Definitionen finden Sie [hier](https://verona-interfaces.github.io/).

## Computersprachen

Wir programmieren die Frontends und die Verona-Module in *Angular*. Dieses Framework benutzt TypeScript als Sprache und erzeugt sehr effizienten JavaScript-Code. Es gibt Erweiterungen für das Styling (Angular Material, Flex-Layout). Im Backend haben wir bis 2021 *php* mit der Erweiterung *Slim* genutzt. Jetzt kommt zunehmend *NestJS* zum Einsatz, das node.js erweitert und womit man TypeScript auf eine Angular-ähnliche Art nutzen kann.

Als Datenbank haben wir bisher MySQL oder PostgreSQL genutzt. Neue Anwendungen (Studio, Kodierbox) speichern die Daten in MongoDB. Auch SQLite kommt punktuell zum Einsatz, vor allem als Austauschformat für die Ergebnisdaten.

Die Prototypen der Webanwendungen sind ohne Unit- und E2E-Tests entstanden, was wir schrittweise beheben. Wir sehen eine hohe Testabdeckung als Voraussetzung für hohe Codequalität. Im Rahmen der Pull-Requests und damit des Peer-Reviews beachten wir die Grundsätze des Clean Code. Viele Prozesse sind automatisiert (Continuous Integration).

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