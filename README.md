[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

Das [Institut zur Qualitätsentwicklung im Bildungswesen](https://www.iqb.hu-berlin.de) nutzt GitHub für die Veröffentlichung von Programmcode. Zusätzlich pflegen wir hier Dokumentationen zu diesen Programmierungen, die es Interessierten erleichtern, mit diesen Anwendungen zu arbeiten und diese zu installieren und anzupassen. Außerdem geben wir an vielen Stellen die Möglichkeit, mit uns in den Dialog zu treten. 

# Computerbasiertes Testen (TBA)
## Verstehen und Anwenden: [Wiki IQB TBA](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki)

<hr/>

* IQB-Testcenter - Webanwendung zum Durchführen von Leistungstests und Befragungen; [Installation/Code](https://github.com/iqb-berlin/testcenter#readme), [Dokumentation für Anwendung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2-Testcenter), [Aktuelle Vorhaben](https://github.com/iqb-berlin/testcenter/issues)
* IQB-Teststudio - Webanwendung zum Erstellen von Testaufgaben bzw. Seiten mit Frage-Items; [Installation/Code](https://github.com/iqb-berlin/studio-lite#readme), [Dokumentation für Anwendung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3-Studio), [Aktuelle Vorhaben](https://github.com/iqb-berlin/studio-lite/issues)
* ict-ToolBox - Windows-Programm zur Vor- und Nachbereitung von Testcenter-Daten; [Installieren](https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox), [Dokumentation/Code](https://github.com/iqb-berlin/itc-toolbox#readme)
* Verona-Module – zur Verwendung im IQB-Testcenter oder im IQB-Teststudio
  * [Aspect Player und Editor](https://github.com/iqb-berlin/verona-modules-aspect/releases) - Player und Editor für komplexe Testaufgaben oder Seiten (IQB-Standard, VERA)
  * [Abi Player](https://github.com/iqb-berlin/verona-player-abi/releases) - Player für eine spezielle Scriptsprache
  * [Speed Test Player](https://github.com/iqb-berlin/verona-player-speedtest/releases) - Player für Lesegeschwindigkeitstests
  * [Simple Player](https://github.com/iqb-berlin/verona-player-simple/releases/latest) - Universeller Player für Html-Definitionen
  * [Plain Text Editor](https://github.com/iqb-berlin/verona-editor-plaintext/releases/latest) - Universeller Editor, Bearbeitung der Unit-Definitionen als Text
  * [IQB-Schemer](https://github.com/iqb-berlin/coding-components/releases/latest) - Editieren eines Kodierschemas - Standard für IQB-Aufgaben
* Für Entwickler:innen:
  * [Verona-Player-Testbed](https://github.com/iqb-berlin/verona-player-testbed#readme): Anwendung zum Testen von Playern oder Unit-Definitionen
  * [iqb-dev-components](https://github.com/iqb-berlin/iqb-dev-components#readme): Einige allgemeine Tools zur Webentwicklung

## Verona Interfaces
Das IQB implementiert die Spezifikationen, die im Rahmen der Verona-Initiative entwickelt werden. Dokumentationen und die Spezifikationen selbst finden Sie hier: [verona-interfaces.github.io](https://verona-interfaces.github.io/).
 
# <a name="metadata"></a>Metadaten
* [Spezifikation und Erläuterung](https://github.com/iqb-berlin/mdc-schemadefinition)
* Aktive Kataloge: [Kernkatalog](https://github.com/iqb-berlin/mdc-core), [Copyright-Datenbank](https://github.com/iqb-berlin/mdc-copyright), [Forschungsdaten](https://github.com/iqb-berlin/mdc-researchdata)
* Kataloge Entwurfsstadium: [Bildungsstandards](https://github.com/iqb-berlin/mdc-educational-standards)
* [vb-metadata](https://github.com/iqb-berlin/vb-metadata): vb.Net-Module zum Auslesen eines Metadatenkatalogs sowie Komponenten zur Darstellung und Änderung von Metadaten in einer Windows-Desktop-Anwendung; außerdem `IQB-MD-CatAdmin` Windows-Anwendung zum Lesen und Speichern eines Kataloges
* [Wiki](https://github.com/iqb-berlin/mdc-testunits/wiki) zur Entwicklung eines Metadaten-Profils für Testaufgaben

# <a name="rcode"></a> R-Programmierungen zur Datenanalyse
Das IQB stellt Programmierungen öffentlich zur Verfügung, die der Datenanalyse im weiteren Sinne dienen. Dazu gehören Verfahren der klassischen Testtheorie ebenso wie IRT-Verfahren. Es werden auch Module zur Datenaufbereitung (cleaning, plot) veröffentlicht. Weitere Informationen finden Sie hier: [iqb-research.github.io](https://iqb-research.github.io/). 

# Repositories alphabetisch:
{% for repository in site.github.public_repositories %}{% if repository.archived != 'true' %}
* [{{ repository.name }}]({{ repository.html_url }}) {{ repository.description }} {% endif %}{% endfor %}
