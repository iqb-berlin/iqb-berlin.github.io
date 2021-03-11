[![Back Home](https://img.shields.io/badge/Zurück--KapComputerbasiertesTesten-blueviolet)](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.--Computerbasiertes-Testen-(TBA))

![Back Home](https://img.shields.io/badge/Haupt--Kapitel-ComputerbasiertesTesten-brightgreen)

---

**Vorab:**

Nach zahlreichen Vorarbeiten arbeitet seit 2018 das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) gezielt im Auftrag der Ländern an der Umstellung papierbasierter Kompetenzerhebungen auf technologiebasierte Durchführung. Details zu den Projekten bzw. zu weiteren Planungen entnehmen Sie bitte hier:
* [TBA-Projekt 2018-2020](https://www.iqb.hu-berlin.de/research/dm/tba/)
* [TBA-Projekt 2021-2023](https://www.iqb.hu-berlin.de/research/dm/tba21/)
* [VERA online](https://www.iqb.hu-berlin.de/vera/online/)

---

**Inhalt:**
  * [1.1.1 TBA Module Aufbau](1.1.1-TBA-Module-Aufbau)
  * [1.1.2 Datenhandshake Testcenter Teststudio](1.1.2-Datenhandshake-Testcenter-Teststudio)
  * [1.1.3 Aktueller Entwicklungsstand](1.1.3-Aktueller-Entwicklungsstand)
  * [1.1.4 Studiendurchführung](1.1.4-Studiendurchführung)
  * [1.1.5 Verfügbarkeit IQB Programmierung](1.1.5-Verfügbarkeit-IQB-Programmierung)
  * [1.1.6 Was macht VERA so speziell?](1.1.6-Was-macht-VERA-so-speziell%3F)

---



## 1.1.1 TBA Module Aufbau

[![Back Home](https://img.shields.io/badge/Zurück--KapTBAEinführung-blue)](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-TBA-Einf%C3%BChrung)

![Back Home](https://img.shields.io/badge/Haupt--Kapitel-TBAEinführung-brightgreen)

---
Nachfolgend wird ein Überblick über die wesentlichen softwarebasierten Bestandteile des Computerbasierten Testens gegeben.
Detaillierte Informationen zu den Software Modulen entnehmen Sie bitte den gleichnamigen Kapiteln.
Die meisten Anwender werden im Rahmen einer Testgestaltung und Testdurchführung vorwiegend mit den Modulen **Teststudio** und **Testcenter** in Berührung kommen. 

![iqb online assessment applications with relations: testcenter, Teststudio, conding, data analysis, archive, taskpool](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/IQB-OnlineTest-Apps.png)

* **IQB-Teststudio**: Es handelt sich hierbei um eine Datenbank mit einer Editierfunktion, welche den Aufgabenentwurf und eine Nachbearbeitung ermöglicht. Mittels dieses Editors werden die interaktiven Einheiten eines Kompetenztests oder einer Befragung entworfen. Die einzelnen Einheiten eines Testheftes werden Unit genannt. Diese sog. Units bestehen aus einem oder mehreren Eingabefeldern, Auswahlboxen, Klappfeldern oder ähnlichen Elementen einer Internet-Seite mit denen die Testperson eine Antwort auf Fragen geben kann. Im Teststudio wird von den Autoren außerdem die Aneinanderreihung der Units festgelegt, das sog. Testheft. Des Weiteren muss eine Vorschrift hinterlegt werden, wie die Antworten ggf. umgeformt werden sollen. Alle Beteiligten erhalten eine spezielle Sicht auf den Entwicklungsprozess entsprechend ihrer Rolle.                            
*Das Teststudio für die Technologie basierten Aufgaben befindet sich noch in einer Entwicklungsphase und wird im Projektzeitraum 2021-2023 grundlegend überarbeitet. Die derzeitige Version nennt sich Teststudio Lite. Die überarbeitete Version wird dann den Namen Teststudio Pro tragen.*

* **IQB-Testcenter**: Mit dieser Anwendung wird der Online-Test durchgeführt. Das Testcenter besteht aus einem Front-/ und einem Backend. Das Backend besteht aus einer entsprechenden Schnittstelle zum Frontend und einer Datenbank, in welcher Metadaten und die Testaufgaben entsprechend gespeichert werden. Der Anwender kommt nur mit dem Frontend in Berührung. Das Frontend wird über eine Internetadresse geladen. Hier können Aufgaben hochgeladen werden und "abgespielt" werden. Das Abspielen der Aufgabeninhalte übernimmt dabei ein so genannter Verona Player. Mehr zum Thema Verona finden Sie im gleichnamigen Kapitel. Die Testpersonen wählen sich über die angegebene Internet-Adresse ein und geben Anmeldenamen und Kennwort ein. Die Verantwortlichen für die Testdurchführung können die Units, Testhefte und Personendaten (Logins) hochladen, sowie die Ergebnisse herunterladen. Außerdem kann man für eine Testgruppe (z. B. Klasse/Kurs) den Fortschritt der Bearbeitung beobachten.

* **IQB-Dateneditor**: Die Antworten müssen geprüft und aufbereitet werden. Hierzu stehen für die Beteiligten entsprechen ihrer Rolle Funktionen wie Kodieren, Verifizieren, beschreibende Statistik abrufen oder Export als Excel-Datei zur Verfügung. Aus den aufbereiteten Daten werden schließlich die gewünschten Ergebnisse der Unternehmung erzeugt: Berichte, Publikationen, Rückmeldungen an Schulen.

* **IQB-Testarchiv**: Eine Testung, Befragung oder allgemein "Studie" sollte gut dokumentiert werden. Hierzu zählen die verwendeten Units, Testhefte, Roh-/Primärdaten, Analysedaten, Berichte - aber auch Protokolle der Testdurchführung, eine Kritik der Analyseverfahren, Verweise auf Bildungsstandards u. ä. Diese dann zu archivierende Dokumentation kann auch als Basis für eine Veröffentlichung der Daten für Sekundäranalysen in einem Forschungsdatenzentrum dienen. Im Testarchiv wird besonderer Wert auf eine Langzeitarchivierung gelegt (besondere Speicherverfahren, besondere Formate für die Dateien usw.).

* **IQB-Testdepot**: Wenn Aufgaben bzw. Fragebögen verwendet wurden, haben sie ihre Eignung für bestimmte Fragestellungen unter Beweis gestellt. Man weiß, unter welchen Bedingungen sie bei welchen Testpersonen mit welcher Genauigkeit Erkenntnisse liefern. Diese wertvollen Informationen werden als Metadaten mit den Units und Testheften in einer Datenbank gespeichert. Über Suchformulare oder auch über Algorithmen können sie für andere Studien ausgewählt werden. Diese Studien mögen als Großprojekte in einem Jahrgang der Schulen eines Landes angelegt sein, es kann sich aber auch um einzelne Lehrkräfte handeln, die für einen kurzen Test in ihrem Kurs Aufgaben zusammenstellen.



## 1.1.2 Datenhandshake Testcenter Teststudio

[![Back Home](https://img.shields.io/badge/Zurück--TBAEinführungHome-blue)](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-TBA-Einf%C3%BChrung)

![Back Home](https://img.shields.io/badge/Haupt--Kapitel-TBAEinführung-brightgreen)

---
Nachfolgend wird der grundsätzliche Handshake zwischen den Hauptmodulen Teststudio und Testcenter, 
beginnend mit der Dateierzeugung bis zur Dateneingabe und Bearbeitung, aufgezeigt.

![iqb online assessment applications with relations: Einführung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/EF_Datenaust_TS_TC_final.png)


### Dateierzeugung
Die Dateierzeugung erfolgt mittels Teststudio (Item-Datenbank und intergriertem Editor). 
Nach finaler Editierung der Aufgaben und Anforderung der Daten im Teststudio, erzeugt dieses die folgenden Dateien verpackt in einem Zip-Format:

![iqb online assessment applications with relations: Einführung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Datenstruktur_Out_final.png)

### Dateibearbeitung
Die einzelnen Datei bzgl. Unit, Booklet etc. können hinsichtlich bestimmter Parameter bearbeitet werden.
Nachfolgend finden Sie eine Übersicht welche Parameter in den einzelnen Dateien verändert werden können. 

**TESTTAKERS.xml**
* Aufruf gewünschtes Booklet mittels eindeutiger Booklet ID (!ID muss entsprechend im Booklet vorhanden sein)
* Definition User und Testmodi
* Definition Test Gruppe


**BOOKLET.xml**
* Layout des Booklets
* Namen des Testheftes
* Aufruf der gewünschten Units mittels eindeutiger Unit-ID (!ID muss entsprechend in der Unit vorhanden sein)
* Name der Unit
* Beschränkungen mittels Codewort

**UNIT.xml**
* Definition des zu verwendenden Players
* Definition der zu verwendenden Ressourcen Datei


### Dateieingabe
Wie die Dateien in das Testcenter zu laden sind, entnehmen Sie bitte dem Kapitel zum Testcenter Frontend.



Weitere Bearbeitung erforderlich! Stand: 01.03.21 T.Huste

---



## 1.1.3 Aktueller Entwicklungsstand

[![Back Home](https://img.shields.io/badge/Zurück--TBAEinführungHome-blue)](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-TBA-Einf%C3%BChrung)

![Back Home](https://img.shields.io/badge/Haupt--Kapitel-TBAEinführung-brightgreen)

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
**In Bearbeitung**

THuste

Änderung des Links, wenn es zu diesem Thema eine eigene Wikiseite gibt!

Diese Anwendung wird derzeit konzipiert. Die Ergebnisverarbeitung unterstützt aktuell eine Windows-Desktop-Anwendung [ict-Toolbox](https://github.com/iqb-berlin/itc-toolbox/blob/master/README.md).

### IQB-Testarchiv IQB-Testdepot
Diese Anwendungen werden derzeit konzipiert. 

---



## 1.1.4 Studiendurchführung

[![Back Home](https://img.shields.io/badge/Zurück--TBAEinführungHome-blue)](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1-TBA-Einf%C3%BChrung)

![Back Home](https://img.shields.io/badge/Haupt--Kapitel-TBAEinführung-brightgreen)

---

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

