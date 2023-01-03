[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

Das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) nutzt GitHub für die Veröffentlichung von Programmcode. Zusätzlich pflegen wir hier Dokumentationen zu diesen Programmierungen, die es Interessierten erleichtern, mit diesen Anwendungen zu arbeiten und diese zu installieren und anzupassen. Außerdem geben wir an vielen Stellen die Möglichkeit, mit uns in den Dialog zu treten. 

# Computerbasiertes Testen (TBA)
## Verstehen und Anwenden: [Wiki IQB TBA](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki)

<hr/>

* IQB-Testcenter - Webanwendung zum Durchführen von Leistungstests und Befragungen; [Installation/Code](https://github.com/iqb-berlin/testcenter#readme), [Dokumentation für Anwendung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2-Testcenter), [Aktuelle Vorhaben](https://github.com/iqb-berlin/testcenter/issues)
* IQB-Teststudio - Webanwendung zum Erstellen von Testaufgaben bzw. Seiten mit Frage-Items; [Installation/Code](https://github.com/iqb-berlin/studio#readme), [Dokumentation für Anwendung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3-Studio), [Aktuelle Vorhaben](https://github.com/iqb-berlin/studio/issues)
* ict-ToolBox - Windows-Programm zur Vor- und Nachbereitung von Testcenter-Daten; [Installieren](https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox), [Dokumentation/Code](https://github.com/iqb-berlin/itc-toolbox#readme)
* Verona-Module – zur Verwendung im IQB-Testcenter oder im IQB-Teststudio
  * [Aspect Player und Editor](https://github.com/iqb-berlin/verona-modules-aspect/releases) - Player und Editor für komplexe Testaufgaben oder Seiten (IQB-Standard, VERA)
  * [Abi Player](https://github.com/iqb-berlin/verona-player-abi/releases) - Player für eine spezielle Scriptsprache
  * [Speed Test Player](https://github.com/iqb-berlin/verona-player-speedtest/releases) - Player für Lesegeschwindigkeitstests
  * [Simple Player](https://github.com/iqb-berlin/verona-player-simple/releases/latest) - Universeller Player für Html-Definitionen
  * [Plain Text Editor](https://github.com/iqb-berlin/verona-editor-plaintext/releases/latest) - Universeller Editor, Bearbeitung der Unit-Definitionen als Text
  * [IQB-Schemer](https://github.com/iqb-berlin/schemer-autocoder/releases/latest) - Editieren eines Kodierschemas - Standard für IQB-Aufgaben
* Für Entwickler:innen:
  * [Verona-Player-Testbed](https://github.com/iqb-berlin/verona-player-testbed#readme): Anwendung zum Testen von Playern oder Unit-Definitionen
  * [iqb-dev-components](https://github.com/iqb-berlin/iqb-dev-components#readme): Einige allgemeine Tools zur Webentwicklung

## Verona Interfaces
Das IQB implementiert die Spezifikationen, die im Rahmen der Verona-Initiative entwickelt werden. Dokumentationen und die Spezifikationen selbst finden Sie [hier](https://verona-interfaces.github.io/).
 
# <a name="metadata"></a>Metadaten
* [Spezifikation und Erläuterung](https://github.com/iqb-berlin/mdc-schemadefinition)
* Aktive Kataloge: [Kernkatalog](https://github.com/iqb-berlin/mdc-core), [Copyright-Datenbank](https://github.com/iqb-berlin/mdc-copyright), [Forschungsdaten](https://github.com/iqb-berlin/mdc-researchdata)
* Kataloge Entwurfsstadium: [Bildungsstandards](https://github.com/iqb-berlin/mdc-educational-standards)
* [vb-metadata](https://github.com/iqb-berlin/vb-metadata): vb.Net-Module zum Auslesen eines Metadatenkatalogs sowie Komponenten zur Darstellung und Änderung von Metadaten in einer Windows-Desktop-Anwendung; außerdem `IQB-MD-CatAdmin` Windows-Anwendung zum Lesen und Speichern eines Kataloges
* [Wiki](https://github.com/iqb-berlin/mdc-testunits/wiki) zur Entwicklung eines Metadaten-Profils für Testaufgaben

# <a name="rcode"></a> R-Programmierungen zur Datenanalyse (GitHub, CRAN) 
* [eatPrep](https://github.com/sachseka/eatPrep): Aufbereitung von Datensätzen (Einlesen, Plausibilitätsprüfungen, Zusammenführen von Datensätzen, Missingbehandlung, Rekodieren, Aggregieren, Scoren und Schreiben von gelabelten SPSS-Datensätzen) unter Verwendung von in der IQB-Datenbank hinterlegten Informationen zu den Items und zum Testdesign.
* [eatModel](https://github.com/weirichs/eatModel): Dient als Interface für die Software ConQuest. Die benötigten Steuerdateien (Skript, Labels, Datensatz im "fixed width"-Format) werden automatisch erzeugt und ConQuest über die Kommandozeile aufgerufen. Die Ergebnisdateien (Showfile, WLEs, PVs, etc.) können wieder nach R importiert und weiterverarbeitet werden. Neuere Versionen von `eatModel` erlauben auch die Einbindung des R-Pakets `tam` sowie Parallelisierung.
* [eatRep](https://cran.r-project.org/web/packages/eatRep/index.html): Berechnet Mittelwerte, Standardabweichungen, Varianzen, Häufigkeitstabellen, Perzentile und lineare (logistische) Regressionen sowie Trends für alle diese Analysen in geclusterten Mehrebenenstrukturen mit imputierten Daten. Das Paket implementiert einen Teil der Funktionsweise der Computersoftware WesVar in R und ist im Wesentlichen für die IQB-Bildungstrendstudien relevant.
* [eatGADS](https://cran.r-project.org/web/packages/eatGADS/index.html): Erlaubt Import und Datenaufbereitungen von SPSS Datensätzen in R. Erzeugt den Gesamtanalysedatensatz (GADS) für IQB-Bildungstrendstudien als SQLite3-Datenbank. Teile des Datensatzes können mithilfe des Pakets dann in R geladen werden. Erlaubt außerdem den Export von SPSS Dateien in und aus R.
* [eatTools](https://cran.r-project.org/web/packages/eatTools/index.html): verschiedene Hilfsfunktionen, die unter anderem auch von den Paketen `eatPrep`, `eatModel` und `eatRep` benötigt werden.
* [eatAnalysis](https://github.com/beckerbenj/eatAnalysis): verschiedene nützliche Hilfsfunktionen, wie zum Speichern von Excel-Datein, Speichern von Analyse-Ergebnissen von `lm4` und Simulieren von IRT-Responses
* [eatATA](https://cran.r-project.org/web/packages/eatATA/index.html): automatisierte Blockbesetzung/automatisierte Testhefterstellung
* [eatFDZ](https://github.com/beckerbenj/eatFDZ): automatisierte Anonymisierung von Datensätzen; Abgleich von pdf-Dokumenten (z. B. Skalenhandbüchern) und Datensätzen


# Repositories alphabetisch:
{% for repository in site.github.public_repositories %}{% if repository.archived == false %}
* [{{ repository.name }}]({{ repository.html_url }}) {% endif %}{% endfor %}
