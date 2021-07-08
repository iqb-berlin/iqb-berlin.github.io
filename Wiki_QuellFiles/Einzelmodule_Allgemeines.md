<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# IQB Konventionen (Abschnittsmarker)
<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

### Seitenlayout

    Seitenrand stets 30 px

#### Volle Seite

* eine oder mehrere Seiten, die die gesamte Bearbeitungsfläche beim Test ausfüllen
* Breite 1.100 px, Höhe beliebig
* ab einer Höhe von 1.000 px ist damit zu rechnen, dass nicht alles während des Tests dargestellt wird; daher sollte dann ein Viewpoint am Ende der Seite (links) platziert werden

#### Geteilte Seite

* links Seite ständig zu sehen, Breite ca. 530 px; hier werden die Textvorgaben (Stimulus) sowie die Audio-Elemente platziert
* rechts andere Seite, ggf. Blättern durch mehrere Seiten; Breite ca. 530 px
* die Teilung kann auch anders liegen, wenn z. B. eine Audioaufgabe links nicht viel Platz braucht
* ab einer Höhe von 1.000 px ist damit zu rechnen, dass nicht alles während des Tests dargestellt wird; daher sollte dann ein Viewpoint am Ende der Seite (links) platziert werden

### Textformatierung

#### Stimulustext

* Times New Roman 22 px, Höhe Anzahl Zeilen x 27
* Überschriften: fett, Textausrichtung zentriert
* Quellenangabe: extra Textfeld einfügen, Arial 10 px, unter dem Stimulustext platzieren
* bei nummerierten Textteilen mit hängendem Einzug: Erste Zeile -23 px, wenn Nummerierung zweistellig -33 px
* Fußnoten über html: Verweis im Text `<sup>1</sup>`, Fußnote unten mit horizontaler Linie `<hr><sup>1</sup><i>Text, Artikel</i>`

#### Instruktion

* Arial 24 px, fett, Höhe Anzahl Zeilen x 30

#### Itemtext, Antwortoptionen, Textbox zur Eingabe von Kurzantworten

* Arial 20 px, Höhe 30 px
* bei nummerierten Textteilen mit hängendem Einzug: Erste Zeile -23 px, wenn Nummerierung zweistellig -33 px

#### Abstände

* zwischen Instruktion und Itemtext: 30 px
* (Itemtext) zwischen Frage und Antwortoptionen: 10 px
* zwischen zwei Antwortoptionen: kein Abstand
* zwischen zwei Items: 20 px

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Login: Modi der Testdurchführung (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

Bei der Definition der Anmeldung zur Durchführung eines Tests können verschiedene Modi gewählt werden. Die Testhefte bleiben unverändert, 
es wird nur ein Modus für eine spezielle Testperson festgelegt. Verschiedene Anmeldungen können also mit denselben Testheften zu 
unterschiedlichem Verhalten führen.

### Wo wird das festgelegt?

Die Festlegung erfolgt in der Testtaker-Xml im Element `Login` im Attribut `mode`:

```xml
<?xml version="1.0" encoding="utf-8"?>
  <Testtakers
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:noNamespaceSchemaLocation=
	 "https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Testtakers.xsd">

     <Metadata>
       <Description>Technischer Test Mechtel</Description>
     </Metadata>

     <Group id="check_mme" label="Mechtels Testgruppe">
       <Login mode="run-review" name="mme4r5t6" pw="d7u9">
         <Booklet>Booklet_Version1</Booklet>
       </Login>
       <Login mode="run-hot-return" name="susicheck12" pw="r4u2">
         <Booklet>Booklet_Version2</Booklet>
       </Login>
     </Group>
   </Testtakers>
```
---

### Welche Modi gibt es?

| Modus | Erläuterung |
| ----- | -------- |
| run-hot-return | Es wird angenommen, dass die finale Testperson den Test durchführt. Alle Beschränkungen der Testheftdefinition sind aktiv. Die Testperson kann bei einem Browserabsturz oder halt später zurückkehren und erhält alle gegebenen Antworten wieder angezeigt. |
| run-hot-restart | Wie oben, nur dass bei einer erneuten Anmeldung die vorherigen Daten nicht geladen werden. Statt dessen wird eine neue Person angenommen und die Antworten unter einer neuen Kennung gespeichert. Dadurch ist es möglich, dieselben Zugangsdaten an viele Menschen zu schicken (z. B. bei Befragungen einer nicht genau bekannten Gruppe). |
| run-trial | Zum Ausprobieren: Viele Beschränkungen gelten (s. u.). |
| run-review | Zum Ausprobieren: Einige Beschränkungen gelten nicht (s. u.). |
| run-demo | Kein Speichern, keine Beschränkungen (s. u.). |
| monitor-group | Reserviert zur Nutzung der Testleitungskonsole. |

---

### Die Modi konkret

* `DEMO` (default): Nur Ansicht (Demo)
* `HOT`: Durchführung Test/Befragung
* `REVIEW`: Prüfdurchgang ohne Speichern
* `TRIAL`: Prüfdurchgang mit Speichern


|  | `DEMO` | `HOT` | `REVIEW` | `TRIAL` | 
| :------------- | :-------------: | :-------------: | :-------------: | :-------------: |
|Es können Reviews abgegeben werden (Kommentare/Einschätzungen zur Unit bzw. zum Test)|  |  |X |  |
|Es werden Antworten und Logs gespeichert.|  |X |  |X |
|Alle Zeitbeschränkungen für Testabschnitte werden angewendet.|  |X |  |X |
|Alle Navigationsbeschränkungen des Booklets werden angewendet (z. B. erst weiter, wenn vollständig angezeigt).|  |X |  |X |
|Sollte ein Testabschnitt mit einem Freigabewort geschützt sein, wird dieses bei der Eingabebox schon eingetragen.|X |  |X |X |
|Sollte eine Maximalzeit für einen Testabschnitt festgelegt sein, wird die verbleibende Zeit angezeigt, auch wenn die Booklet-Konfiguration dies unterbindet.|X |  |X |  |
|Die Seite mit der Aufgaben-Übersicht wird erlaubt, auch wenn das Booklet dies unterbindet.|  |  |X |  |


<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Login: Anmeldeverfahren (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Standby
Stand: 6.4.2021
```
Für eine Testdurchführung erlaubt das IQB-Testcenter verschiedene Arten der Anmeldung der Testperson:

### Klassisch: Anmeldename, Kennwort

Beim Aufruf der Internet-Seite und damit der Webanwendung wird ein Formular präsentiert zur Eingabe dieser Daten. 
Diese Anmeldeform wird üblicherweise erwartet. Der Anmeldename wird im Klartext gezeigt, die Eingabe des Kennwortes erzeugt 
aber nur Punkte, d. h. man kann nicht mitlesen.

### Kurz: Nur Anmeldename

Das Kennwort kann weggelassen werden. Hier hat man keine geringere Sicherheit, wenn die Länge und Zeichenzusammensetzung 
des Namens hinreichend ungewöhnlich ist. Eine laufende Nummer am Ende ist z. B. problematisch, denn sie kann bei Kenntnis eines Namens 
erraten werden. Diese Anmeldeform sollte gewählt werden, wenn das Verbergen des Kennwortes stört.

### Noch kürzer: Link

Wenn nur ein Anmeldename ohne Kennwort als Login festgelegt wurde, dann kann man auch einen Link an die Testpersonen verschicken. 
Wenn "u8h5m2a4c3x2f2g8" der Anmeldename ist würde der Link so aussehen:
```
https://www.iqb-testcenter.de/#/u8h5m2a4c3x2f2g8
```
Dadurch macht man es noch einfacher: Auf den Link klicken, und man muss nur noch das Testheft wählen. Diese Form der 
Anmeldung kann z. B. bei Befragungen in Kombination mit dem Durchführungsmodus `run-hot-restart` verwendet werden: 
Es wird nur ein Login in einer Einladungs-E-Mail verschickt, und eine vorher unbekannte Anzahl Personen kann die Befragung starten.

### Länger: Anmeldename, Kennwort, Personencode

Es kann sein, dass die Testleitung Zeit hat, vor Eintreffen der Schülerinnen und Schüler alle Computer zu starten, 
einen Standard-User anzumelden, den Browser zu starten und die richtige Internet-Adresse aufzurufen. Dann ist es auch hilfreich, 
wenn auf jedem Computer schon Anmeldename und Kennwort eingegeben werden kann und also ein Anmeldeprozess gestartet wird. 
Anmeldename und Kennwort sind dann für die Gruppe gleich. Es reicht dann anschließend die Eingabe eines kurzen Personencodes durch die Testperson, 
um eine eindeutige Identifizierung sicherzustellen. Man spart so Testzeit und vermeidet Fehleingaben. Dieses Szenario bietet sich z. B. an, 
wenn man den Test nicht in der Schule, sondern in dem eigenen oder einem angemieteten Computer-Lab durchführt.

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Verona (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

<table>
  <tr>
    <td><a href="#Allgem">Allgemeines</a></td>    
	<td><a href="#TechnDetails">Technische Details</a></td>
  </tr>
</table>

## <a name="Allgem"></a>Allgemeines

In Deutschland gibt es für internationale (z. B. PISA) und einheitliche nationale 
Erhebungen (z. B. Bildungstrend) jeweils zentrale Einrichtungen oder Firmen zur 
Durchführung. Da für die Bildungspolitik aber jedes Bundesland einzeln zuständig ist, 
werden Kompetenzerhebungen oft in Länderregie durchgeführt. Entsprechend ist die 
Vielfalt an Anforderungen an ein technisches System zum computerbasierten Testen.    

Erhebungen zum Bildungsmonitoring erfordern nicht nur die eigentliche 
Computeranwendung zur unmittelbaren Durchführung des Tests, sondern auch komplexe Portale 
zur Vorbereitung (Eingabe der Daten der Testgruppen bzw. -personen, Festlegungen zum 
Inhalt und Ablauf der Tests) und zur Auswertung (anschauliche Präsentation der 
Ergebnisse, Anregungen zur Interpretation und zur Weiterarbeit). Die erhebliche Vielfalt 
und Komplexität der Anwendungen führt dazu, dass es keine einheitliche Software geben 
kann, die von allen genutzt wird. Statt dessen entwickeln die Länder gemeinsam eine 
offene und schrittweise wachsende Landschaft von Software-Modulen, die über 
wohldefinierte Schnittstellen durch alle Beteiligten genutzt werden können.

Lernstandserhebungen in den Ländern gibt es papierbasiert seit 2003. Diese 
Vergleichsarbeiten werden mit der Abkürzung VERA bezeichnet. Aus der Verbindung mit 
"Online" wurde dann die Bezeichnung "Verona" für VERA Online. Die nötigen Schnittstellen 
(engl. Interfaces) sind in diesem Dokumenten- bzw. Codeverwaltungssystem GitHub 
beschrieben.

Da die Testsysteme eine Anpassung erfahren müssten, wenn Aufgabenformate geändert werden, kommt ein Player mit einer definierten Schnittstelle zum Einsatz. Der zu verwendende Player wird in der jeweiligen Unit definiert und mit der Unit geladen. Dieser spielt dann die in der Unit definierten Aufgabenformate ab. Die dazu gehörige Schnittstelle des Players gewährleistet eine Kompatibilität zu den Anwendungen, die bereits für die Vera Papierstudien genutzt wurden und weiterhin werden. Der Player wird daher auch Verona-Player und die Schnittstelle auch Verona-Schnittstelle genannt. Ändert sich ein Aufgabenformat, muss somit nur noch ein dazu passender Player geladen werden, der dieses Format auch abspielen kann. Durch den modularen Aufbau des Testcenters entfällt somit eine Anpassung der gesamten Testumgebung, wenn sich Aufgabenformate ändern. Stattdessen wird einfach der entsprechende Player für das Format geladen und in die Oberfläche des Testcenters intergriert.

## <a name="TechnDetails"></a>Technische Details

Dieser Abschnitt richtet sich an technisch Interessierte. Hier erhalten Sie einen tieferen Einblick in die techn. Funktionsweisen und die techn. Strukturen.

### Verona Schnittstelle

Zum Abspielen, Tests durchführen, Daten ausgeben, Logins festlegen usw. (alles was zum TBA-testen nötig ist) kann man entweder das **IQB-Testcenter** benutzen ("Auswertuns-/Kodierungsgmodul" fehlt allerdings noch) oder eine Verona Interface Schnittstelle nutzen um ein eigens programmiertes Testcenter zu nutzen und die IQB-Tests "abzuspielen". Folgendes [Video](https://box.hu-berlin.de/f/d23af87168fa4e9f9bb0/) verschafft einen groben Überblick über dieses Thema.

* Verona steht für VERA-Online 
* Verona Interfaces sind Schnittstellen zu Programmen/Modulen vom IQB zur VERA-Testungen im TBA-Format
* daher fand Modularisierung der Komponenten des Testcenters statt
* Grund: Flexibilität z.B. in Verwendung neuer Aufgabenformate zu haben 
* dazu Entkopplung innerhalb des Testcenters von Präsentation der Aufgabe (Player) & Testsystem (Login, Aufgabe laden, Antworten/Log speichern usw.)
* zwischen Testsystem und Player muss Kommunikation bestehen, passiert in Form von Schnittstelle (=Plug-In-Schnittstelle)
* IQB liefert also immer auch den Player aus (+ Testsystem), Länder müssen Schnittstellendefinition noch leisten
* der Player ändert sich also, wenn beispielsweise ein neues Testformat entwickelt wurde, das Testsystem muss jedoch nicht "nachprogrammiert" werden, allerdings die Schnittstelle 
* das IQB hat ein Testsystem (Testcenter) für seine eigenen Bedürfnisse, die Länder können ein (oder mehrere) eigene/andere Testsysteme haben, dafür muss nur die Schnittstelle bedient werden und nicht grundsätzlich eine neues Testsystem aufgebaut werden (Ansteuerung und Anpassung des Testsystems über eine Schnittstelle) 
* die Schnittstelle ist vor allem auch dafür verantwortlich, dass Antworten, die in Form von Rohdaten vorliegen, in ein Standardformat umgewandelt werden (Response Converter)
* auch muss die Antwortverarbeitung vorab geplant werden (im VERA-Paper-Pencil-Prozess heißt es Antwortschema), ein Responce Scheme (wie es hier im TBA-Kontext genannt wird) ist als extra Modul also auch notwendig 
* insgesamt besteht die Schnittstelle aus 4 Modulen: Editor, Player, Response Scheme, Response Converter
* ein Testsystem (z.B. Testcenter zu nennen, wie im IQB) in dem der Test durchgeführt werden kann (Pilotierung im IQB, Hauptdurchgang in einem Land) bräuchte einen Player und einen Response Converter
* ein Teststudio in dem die Aufgaben und Tests entwickelt werden, bräuchte Editor (Authoring), Response Scheme und Player (für Demo-Voransicht der Aufgaben) 
    
Folgende Videos verschaffen weitere Einblicke:

* [Verona-Interfaces: 1.Einführung](https://box.hu-berlin.de/f/a6de8bd03626451a93d0/)
* [Verona-Interfaces: 2.Player-Model](https://box.hu-berlin.de/f/8f4b50975e9645af803b/)
* [Verona-Interfaces: 3.Player-API](https://box.hu-berlin.de/f/6c71fcdb9d7944d69dec/)
	
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# xIQB Grundsätze Player Programmierung (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Löschkandidat
Stand: 6.4.2021
```

Die folgenden Grundsätze bestimmen aktuell die Entwicklung von Verona-Playern am IQB. Sie sind nicht mit anderen Partnern bzw. Institutionen abgestimmt. Die Grundsätze sind teilweise noch nicht umgesetzt, sondern werden bei künftigen Änderungen implementiert.

### Datenformat der Unit-Definition

Aus der Unit-Definition müssen Anwendungen erkennen, welcher Player benutzt werden soll, um die Unit anzuzeigen bzw. auszuführen. Das IQB hinterlegt hier nicht eine ID eines Players, sondern benennt das Datenformat. Dies ist universeller, denn es mag verschiedene Player geben, die das Datenformat unterstützen. Außerdem ergibt sich daraus auch der notwendige Editor bzw. die Liste der möglichen Editoren für die Änderung der Unit-Defintion.

Das Datenformat besteht aus einer ID und einer Version nach Semantic Versioning 2.0.0, getrennt durch Leerzeichen. Beispiel: `iqb-dan 3.2.3`. Es werden Player bzw. andere Programmierungen als kompatibel angesehen, die mindestens diese Version unterstützen sowie maximal die letzte Version des major-Elementes der Version. Für das Beispiel würde das bedeuten, dass ein Player mit dokumentiertem Datenformat `iqb-dan 3.4.0` oder `iqb-dan 3.34.7` als zulässig angesehen wird, aber die Versionen `iqb-dan 3.2.1` sowie `iqb-dan 4.0.0` nicht.

### Player-Registry

Für Player und andere Module sollten Metadaten hinterlegt werden, die die Eignung für bestimmte Use Cases und Datenformate anzeigen und die Auswahl durch eine Anwendung unterstützen. Wir stellen uns einen Server vor, über dessen API Anfragen gestellt und Referenzen auf Player zurückgegeben werden können. Diese Referenzen sollten vorzugsweise DOI-Kennungen sein, die dann auf GitHub-Dateien aufgelöst werden.

Dieses Verfahren ist in Vorbereitung, wird aber aktuell als übertrieben angesehen angesichts der geringen Anzahl der Player. Wer Anwendungen für Verona-Plugins erstellt, sollte ein manuelles Einspielen der erforderlichen Player/Editoren usw. vorsehen.

### Kleine fokussierte Player

Das IQB wird für verschiedene Studien bzw. Befragungen unterschiedliche Player einsetzen. Man könnte Player konzipieren, die alle möglichen Interaktionselemente abdecken, das IQB möchte aber eher typische Interaktionselemente als Basisausstattung umsetzen und dann zusätzliche Player bereitstellen, die spezielle Interaktionselemente implementieren. Wir möchten z. B. eine GeoGebra-Implementation nicht auch bei Sprachtests laden oder Formate zur Kommasetzung in Mathematik-Tests bereitstellen. Wo dann genau die Grenze zu ziehen ist wird sich zeigen, aber tendenziell möchten wir kleine fokussierte Player bereitstellen.


<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Newsletter Archiv
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

# Newsletter IQB-Programmierungen zum computerbasierten Testen
## 2021/1 - 18.5.2021
### Teststudio-Lite 1.0
Die IQB-Anwendung zum Erstellen von Aufgaben bzw. Seiten hat den Status "Prototyp" verlassen und ist jetzt in der Version 1.0 verfügbar. Die Installation als "Docker-Setup" ist jetzt erweitert um ein Update-Script, um alte Inhalte oder Einstellungen zu respektieren. Neue Funktionen u. a.:
* Import von Aufgaben/Seiten
* Vereinfachtes Einspielen von Verona-Modulen
* Anpassbarkeit Startseite, Impressum 


