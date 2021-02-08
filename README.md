[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)


**Das IQB auf GitHub - Code, Wissen, Dialog**

Das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) nutzt GitHub für die Veröffentlichung von Programmcode. Zusätzlich pflegen wir hier Dokumentationen zu diesen Programmierungen, die es Interessierten erleichtern, mit diesen Anwendungen zu arbeiten und diese zu installieren und anzupassen. Außerdem geben wir an vielen Stellen die Möglichkeit, mit uns in den Dialog zu treten. 

Diese Seite bietet einen groben Überblick über das Angebot. Mit einem Klick auf die Links begeben Sie sich in Wikis, Code-Repositorien und Foren oder zu einer Videopräsentation zum jeweiligen Thema.


# <a name="cba"></a>Computerbasiertes Testen
#### Verstehen und Anwenden
* [Einführung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki): Dieses Wiki gibt einen Überblick über das Instrumentarium zum Online-Testen am IQB. Hier finden sich zahlreiche Verweise auf andere Quellen bzw. zu den Wiki-Seiten der jeweiligen Anwendungen.
* **IQB-Testcenter**: Diese Webanwendung wird zur Durchführung von Befragungen oder Kompetenztests benutzt.
  * [Wiki zum IQB-Testcenter](https://github.com/iqb-berlin/testcenter-frontend/wiki): 
Diese Wiki-Seiten beschreiben im Detail die Bedienung und die Möglichkeiten der Konfiguration dieser Web-Anwendung.
  * [Testcenter-Forum](https://github.com/iqb-berlin/testcenter-frontend/discussions): Hier finden Sie häufig gestellte Fragen mit Antworten sowie Berichte über Einsätze des IQB-Testcenters.
  * [itc-Toolbox](https://github.com/iqb-berlin/itc-toolbox/blob/master/README.md): Windows-Desktop-Anwendung zur Unterstützung der Nutzung des IQB-Testcenters (vb.net). Man erhält Unterstützung bei der Erstellung von Steuerdateien (Logins, Testheft-Xml) und bei der Aufbereitung der Ergebnisse.
  * [IQB-Daten-Spezifikationen](https://github.com/iqb-berlin/verona-data-specifications/blob/main/README.md): Spezifikationen zu den Datenformaten "iqb-scripted" und "iqb-key-value" 
* **IQB-Teststudio-Lite**: Mit dieser Webanwendung erstellt man Aufgaben für die Befragungen bzw. Kompetenztests.
  * [Wiki zum IQB-Teststudio](https://github.com/iqb-berlin/teststudio-lite-frontend/wiki): 
Diese Wiki-Seiten beschreiben im Detail die Bedienung und die Möglichkeiten der Konfiguration dieser Web-Anwendung.

#### Programmieren und Installieren
* IQB-Testcenter:
  * Programmcode: [Frontend](https://github.com/iqb-berlin/testcenter-frontend) (Angular), [Backend](https://github.com/iqb-berlin/testcenter-backend) (php), [Server für Testleitungskonsole](https://github.com/iqb-berlin/testcenter-broadcasting-service) (node.js), [Docker-Setup](https://github.com/iqb-berlin/testcenter-setup)
  * Installation (Video-Präsentationen auf HU-Box): [Einführung in die Architektur](https://box.hu-berlin.de/f/a8f7aea9c751493c8d35/), [Optionen der Einbindung](https://box.hu-berlin.de/f/d23af87168fa4e9f9bb0/)  
* IQB-Teststudio-Lite: [Frontend](https://github.com/iqb-berlin/teststudio-lite-frontend) (Angular), [Backend](https://github.com/iqb-berlin/teststudio-lite-backend) (php), [Docker-Setup](https://github.com/iqb-berlin/teststudio-lite-setup)
* [itc-Toolbox](https://github.com/iqb-berlin/itc-toolbox): Windows-Desktop-Anwendung zur Unterstützung der Nutzung des IQB-Testcenters (vb.net)
* [Verona-Player-Testbed](https://github.com/iqb-berlin/verona-player-testbed): IQB-Anwendung zum schnellen Testen eines Verona-Players bzw. dessen Unit-Definitionen
* IQB-Verona-Player: [abi](https://github.com/iqb-berlin/verona-player-abi), [dan](https://github.com/iqb-berlin/verona-player-dan), [simple](https://github.com/iqb-berlin/verona-player-simple)
* [IQB-Daten-Spezifikationen](https://github.com/iqb-berlin/verona-data-specifications): Ergänzende Spezifikationen zu Datenformaten rund um Verona 

#### Konzipieren: Verona-Interfaces
* Video-Präsentationen: [Einführung](https://box.hu-berlin.de/f/a6de8bd03626451a93d0/), [Player-Modell](https://box.hu-berlin.de/f/8f4b50975e9645af803b/), [Player-API](https://box.hu-berlin.de/f/6c71fcdb9d7944d69dec/)
* [Player-Spezifikation](https://github.com/verona-interfaces/player)
* [Editor-Spezifikation](https://github.com/verona-interfaces/editor)
* [IQB-Daten-Spezifikationen](https://github.com/iqb-berlin/verona-data-specifications): Ergänzende Spezifikationen zu Datenformaten rund um Verona 
 
# Metadaten-Kataloge
* [Spezifikation und Erläuterung](https://github.com/iqb-berlin/mdc-schemadefinition)
* Aktive Kataloge: [Kernkatalog](https://github.com/iqb-berlin/mdc-core), [Copyright-Datenbank](https://github.com/iqb-berlin/mdc-copyright), [Forschungsdaten](https://github.com/iqb-berlin/mdc-researchdata)
* [vb-metadata](https://github.com/iqb-berlin/vb-metadata): vb.Net-Module zum Auslesen eines Metadatenkatalogs sowie Komponenten zur Darstellung und Änderung von Metadaten in einer Windows-Desktop-Anwendung; außerdem `IQB-MD-CatAdmin` Windows-Anwendung zum Lesen und Speichern eines Kataloges

# Übergreifende Programmierungen / Spezifikationen:
* [IQB-Components](https://github.com/iqb-berlin/iqb-components): Angular-Komponenten zur Verwendung in Web-Anwendungen
* [IQB-Dev-Components](https://github.com/iqb-berlin/iqb-dev-components): Sammlung von Scripten zur Unterstützung der Programmierung bzw. des Deployments von Web-Anwendungen
* [eslint-config](https://github.com/iqb-berlin/eslint-config): TypeScript Syntax-Regeln (linting)
* [distpacker](https://github.com/iqb-berlin/distpacker): Script zum Packen von Html-, Css- und JavaScript-Dateien zu einer Html-Datei
* [vb-lib](https://github.com/iqb-berlin/vb-lib): Sammlung verschiedener Module zur Programmierung von Windows-Desktop-Anwendungen (vb.Net-Code); diese Module sind auf nuget.org als Package veröffentlicht
* [Version-Compare](https://github.com/iqb-berlin/version-compare): Kleines Tool für Windows  


# <a name="rcode"></a> R-Programmierungen zur Datenanalyse (GitHub, CRAN) 
* [eatPrep](https://github.com/sachseka/eatPrep): Aufbereitung von Datensätzen (Einlesen, Plausibilitätsprüfungen, Zusammenführen von Datensätzen, Missingbehandlung, Rekodieren, Aggregieren, Scoren und Schreiben von gelabelten SPSS-Datensätzen) unter Verwendung von in der IQB-Datenbank hinterlegten Informationen zu den Items und zum Testdesign. Diese werden mithilfe des ZKDaemon (siehe unten) aus der Datenbank extrahiert und in ein standardisiertes xlsx-Format geschrieben. Dieses xlsx-Format nutzt `eatPrep`, um die Informationen aus der Datenbank nach R zu übertragen.
* [eatModel](https://github.com/weirichs/eatModel): Dient als Interface für die Software ConQuest. Die benötigten Steuerdateien (Skript, Labels, Datensatz im "fixed width"-Format) werden automatisch erzeugt und ConQuest über die Kommandozeile aufgerufen. Die Ergebnisdateien (Showfile, WLEs, PVs, etc.) können wieder nach R importiert und weiterverarbeitet werden. Neuere Versionen von `eatModel` erlauben auch die Einbindung des R-Pakets `tam` sowie Parallelisierung.
* [eatRep](https://cran.r-project.org/web/packages/eatRep/index.html): Berechnet Mittelwerte, Standardabweichungen, Varianzen, Häufigkeitstabellen, Perzentile und lineare (logistische) Regressionen sowie Trends für alle diese Analysen in geclusterten Mehrebenenstrukturen mit imputierten Daten. Das Paket implementiert einen Teil der Funktionsweise der Computersoftware WesVar in R und ist im Wesentlichen für die IQB-Bildungstrendstudien relevant.
* [eatGADS](https://cran.r-project.org/web/packages/eatGADS/index.html): Erzeugt den Gesamtanalysedatensatz (GADS) für IQB-Bildungstrendstudien als SQLite3-Datenbank. Teile des Datensatzes können mithilfe des Pakets dann in R geladen werden. Erlaubt außerdem den Import und Export von SPSS Dateien in und aus R. Beinhaltet die Anonymisierungsfunktionen des FDZ
* [eatTools](https://cran.r-project.org/web/packages/eatTools/index.html): verschiedene Hilfsfunktionen, die unter anderem auch von den Paketen `eatPrep`, `eatModel` und `eatRep` benötigt werden.
* [eatAnalysis](https://github.com/beckerbenj/eatAnalysis): verschiedene nützliche Hilfsfunktionen, wie zum Speichern von Excel-Datein, Speichern von Analyse-Ergebnissen von lm4 und Simulieren von IRT-Responses
* [eatATA](https://github.com/beckerbenj/eatATA): automatisierte Blockbesetzung/automatisierte Testhefterstellung
* [eatFDZ](https://github.com/beckerbenj/eatFDZ): automatisierte Anonymisierung von Datensätzen; Abgleich von pdf-Dokumenten (z. B. Skalenhandbüchern) und Datensätzen
