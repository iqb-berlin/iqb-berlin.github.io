[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

Das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) nutzt GitHub für die Veröffentlichung von Programmcode. Zusätzlich pflegen wir hier Dokumentationen zu diesen Programmierungen, die es Interessierten erleichtern, mit diesen Anwendungen zu arbeiten und diese zu installieren und anzupassen. Außerdem geben wir an vielen Stellen die Möglichkeit, mit uns in den Dialog zu treten. 

Diese Seite bietet einen groben Überblick über das Angebot. Mit einem Klick auf die Links begeben Sie sich in Wikis, Code-Repositorien und Foren oder zu einer Videopräsentation zum jeweiligen Thema.

# Computerbasiertes Testen
## Verstehen und Anwenden: [Wiki IQB TBA](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki)

## Installieren
* [IQB-Testcenter](https://github.com/iqb-berlin/testcenter-setup#readme) - Webanwendung zum Durchführen von Leistungstests und Befragungen 
* [IQB-Teststudio](https://github.com/iqb-berlin/teststudio-lite-setup#readme) - Webanwendung zum Erstellen von Testaufgaben bzw. Seiten mit Frage-Items
* [ict-ToolBox](https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox) - Windows-Programm zum Aufbereiten der Ergebnisse u. a.
* Verona-Player – zur Verwendung im IQB-Testcenter oder im IQB-Teststudio (Voransicht)
  + [Aspect Player](https://github.com/iqb-berlin/verona-modules-aspect/releases/latest) - Player für komplexe Testaufgaben oder Seiten (IQB-Standard, VERA)
  + [Simple Player](https://github.com/iqb-berlin/verona-player-simple/releases/latest) - Universeller Player für Html-Definitionen
  + [Abi Player](https://github.com/iqb-berlin/verona-player-abi/releases/latest) - Player für eine spezielle Scriptsprache
* Verona-Editoren – zur Verwendung im IQB-Teststudio
  + [Aspect Editor](https://github.com/iqb-berlin/verona-modules-aspect/releases/latest) - Editor für komplexe Testaufgaben oder Seiten (IQB-Standard, VERA)
  * [Plain Text Editor](https://github.com/iqb-berlin/verona-editor-plaintext/releases/latest) - Universeller Editor, Bearbeitung der Unit-Definitionen als Text 

## Entwicklung/Quellcode
* IQB-Testcenter: [Frontend](https://github.com/iqb-berlin/testcenter-frontend) (Angular), [Backend](https://github.com/iqb-berlin/testcenter-backend) (php), [Server für Testleitungskonsole](https://github.com/iqb-berlin/testcenter-broadcasting-service) (node.js), 
* IQB-Teststudio-Lite: [Frontend](https://github.com/iqb-berlin/teststudio-lite-frontend) (Angular), [Backend](https://github.com/iqb-berlin/teststudio-lite-backend) (php), 
* [itc-Toolbox](https://github.com/iqb-berlin/itc-toolbox) (vb.net)
* [Verona-Player-Testbed](https://github.com/iqb-berlin/verona-player-testbed): IQB-Anwendung zum schnellen Testen eines Verona-Players bzw. dessen Unit-Definitionen
* Verona-Module: [aspect](https://github.com/iqb-berlin/verona-modules-aspect), [abi-player](https://github.com/iqb-berlin/verona-player-abi), [simple-player](https://github.com/iqb-berlin/verona-player-simple), [plaintext-editor](https://github.com/iqb-berlin/verona-editor-plaintext)

## Verona Interfaces Specification
* [Player](https://github.com/verona-interfaces/player), [Editor](https://github.com/verona-interfaces/editor), [Metadaten](https://github.com/verona-interfaces/metadata)
* Video-Präsentationen: [Einführung](https://box.hu-berlin.de/f/a6de8bd03626451a93d0/), [Player-Modell](https://box.hu-berlin.de/f/8f4b50975e9645af803b/), [Player-API](https://box.hu-berlin.de/f/6c71fcdb9d7944d69dec/)
 
# <a name="metadata"></a>Metadaten
* [Spezifikation und Erläuterung](https://github.com/iqb-berlin/mdc-schemadefinition)
* Aktive Kataloge: [Kernkatalog](https://github.com/iqb-berlin/mdc-core), [Copyright-Datenbank](https://github.com/iqb-berlin/mdc-copyright), [Forschungsdaten](https://github.com/iqb-berlin/mdc-researchdata)
* Kataloge Entwurfsstadium: [Bildungsstandards](https://github.com/iqb-berlin/mdc-educational-standards)
* [vb-metadata](https://github.com/iqb-berlin/vb-metadata): vb.Net-Module zum Auslesen eines Metadatenkatalogs sowie Komponenten zur Darstellung und Änderung von Metadaten in einer Windows-Desktop-Anwendung; außerdem `IQB-MD-CatAdmin` Windows-Anwendung zum Lesen und Speichern eines Kataloges

# <a name="rcode"></a> R-Programmierungen zur Datenanalyse (GitHub, CRAN) 
* [eatPrep](https://github.com/sachseka/eatPrep): Aufbereitung von Datensätzen (Einlesen, Plausibilitätsprüfungen, Zusammenführen von Datensätzen, Missingbehandlung, Rekodieren, Aggregieren, Scoren und Schreiben von gelabelten SPSS-Datensätzen) unter Verwendung von in der IQB-Datenbank hinterlegten Informationen zu den Items und zum Testdesign.
* [eatModel](https://github.com/weirichs/eatModel): Dient als Interface für die Software ConQuest. Die benötigten Steuerdateien (Skript, Labels, Datensatz im "fixed width"-Format) werden automatisch erzeugt und ConQuest über die Kommandozeile aufgerufen. Die Ergebnisdateien (Showfile, WLEs, PVs, etc.) können wieder nach R importiert und weiterverarbeitet werden. Neuere Versionen von `eatModel` erlauben auch die Einbindung des R-Pakets `tam` sowie Parallelisierung.
* [eatRep](https://cran.r-project.org/web/packages/eatRep/index.html): Berechnet Mittelwerte, Standardabweichungen, Varianzen, Häufigkeitstabellen, Perzentile und lineare (logistische) Regressionen sowie Trends für alle diese Analysen in geclusterten Mehrebenenstrukturen mit imputierten Daten. Das Paket implementiert einen Teil der Funktionsweise der Computersoftware WesVar in R und ist im Wesentlichen für die IQB-Bildungstrendstudien relevant.
* [eatGADS](https://cran.r-project.org/web/packages/eatGADS/index.html): Erlaubt Import und Datenaufbereitungen von SPSS Datensätzen in R. Erzeugt den Gesamtanalysedatensatz (GADS) für IQB-Bildungstrendstudien als SQLite3-Datenbank. Teile des Datensatzes können mithilfe des Pakets dann in R geladen werden. Erlaubt außerdem den Export von SPSS Dateien in und aus R.
* [eatTools](https://cran.r-project.org/web/packages/eatTools/index.html): verschiedene Hilfsfunktionen, die unter anderem auch von den Paketen `eatPrep`, `eatModel` und `eatRep` benötigt werden.
* [eatAnalysis](https://github.com/beckerbenj/eatAnalysis): verschiedene nützliche Hilfsfunktionen, wie zum Speichern von Excel-Datein, Speichern von Analyse-Ergebnissen von `lm4` und Simulieren von IRT-Responses
* [eatATA](https://cran.r-project.org/web/packages/eatATA/index.html): automatisierte Blockbesetzung/automatisierte Testhefterstellung
* [eatFDZ](https://github.com/beckerbenj/eatFDZ): automatisierte Anonymisierung von Datensätzen; Abgleich von pdf-Dokumenten (z. B. Skalenhandbüchern) und Datensätzen

# <a name="components"></a>Übergreifende Programmierungen / Spezifikationen
* [IQB-Components](https://github.com/iqb-berlin/iqb-components): Angular-Komponenten zur Verwendung in Web-Anwendungen
* [IQB-Dev-Components](https://github.com/iqb-berlin/iqb-dev-components): Sammlung von Scripten zur Unterstützung der Programmierung bzw. des Deployments von Web-Anwendungen
* [eslint-config](https://github.com/iqb-berlin/eslint-config): TypeScript/JavaScript Syntax-Regeln (linting)
* [distpacker](https://github.com/iqb-berlin/distpacker): Script zum Packen von Html-, Css- und JavaScript-Dateien zu einer Html-Datei
* [vb-lib](https://github.com/iqb-berlin/vb-lib): Sammlung verschiedener Module zur Programmierung von Windows-Desktop-Anwendungen (vb.Net-Code); diese Module sind auf nuget.org als Package veröffentlicht
* [Version-Compare](https://github.com/iqb-berlin/version-compare): Kleines Tool (Windows legacy)  

# Repositories alphabetisch:
{% for repository in site.github.public_repositories %}{% if repository.archived == false %}
* [{{ repository.name }}]({{ repository.html_url }}) {% endif %}{% endfor %}
