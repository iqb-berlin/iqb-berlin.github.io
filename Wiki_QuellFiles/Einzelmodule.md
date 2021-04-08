<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# IQB Konventionen
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
# Arbeiten mit Xml-Dateien
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

> XML ist ein Standardformat und wird durch Texteditoren sehr gut unterstützt. Daher sind einige Dateien für die Definition von Daten in den IQB-Anwendungen in diesem Format hinterlegt. Der folgende Text soll Neulingen dieses Format nahebringen.

XML ist ein textbasiertes Dateiformat. Die Daten können also einfach mittels eines Texteditors bearbeitet werden. Beispiele sind Notepad++ oder Sublime. Viele Editoren bieten Ergänzungsmodule für die Arbeit mit XML-Dateien. Dann sind z. B. die Schlüssel-Zeichen in anderen Farben dargestellt und es werden Fehler in der Syntax (z. B. schließendes Element fehlt) gemeldet.

Damit die Daten im Text gefunden werden können, muss eine bestimmte Struktur eingehalten werden. Anschließend kann eine entsprechende Gegenstelle - z. B. das IQB-Testcenter, mittels eindeutiger Schlüsselwörter (Tags oder Elemente) die Daten im Text finden und nutzen.
* Elemente: XML-Dateien bestehen immer aus Elementen und ggf. mehreren Unterelementen. Der Beginn eines Elements wird mit zwei spitzen Klammern `<Element>` eingeleitet und wie folgt beendet: `</Element>`.
* Attribute: Jedes Element kann außer den eigentlichen Daten, welche sich im Elementenkörper befinden, Attribute enthalten. Attribute werden immer in der folgenden Form ausgedrückt: `Name Attribut = "Attributwert"` und befinden sich innerhalb des Elementenaufrufs (`<Element Attribut="Attributwert">`). Es gibt auch Elemente, die Attribute aber keine Daten enthalten und umgekehrt.

### Beispiele

1. Element ohne Attribute mit Daten:

   Daten sind in diesem Fall der Text zwischen den spitzen Klammern, dem Elementenkörper: `"Sekundarstufe I Englisch Ansichtsaufgaben"`.

  ```xml
    <Label>Sekundarstufe I Englisch Ansichtsaufgaben</Label>
  ```

2. Element mit Attributen ohne Daten:

   Hier gibt es 3 Attribute: `id`, `lable` und `lableshort`. Alle 3 Attribute enthalten in diesem Fall Attributwerte.<br>
   Diese sind in Hochkommata gefasst und werden mit einem Gleichheitszeichen dem Attribut zugeordnet. 
   Das keine Daten enthalten sind, ist gut an dem Schließen des Elementes **Unit** zu erkennen. Denn das Element endet nicht mit: 
   `</Unit>`, sondern nur mit: `/>`. Diese Syntax gibt an, dass keine Daten folgen.

```xml
   <Unit id="Unit1" label="1. Postcard" labelshort="1" />
```

3. Element mit Daten und Attributen:

   Attribut ist hier: `key`. Dieses bekommt den Attributwert `force_presentation_complete` zugewiesen.
   Datum ist der Wert: `ON`.

```xml
    <Config key="force_presentation_complete">ON</Config>
````

### Validierung

Die Abfolge der Elemente und Attribute einer IQB-XML-Datei ist streng geregelt. Damit ist sichergestellt, dass die Informationen durch alle beteiligten Komponenten korrekt interpretiert werden. Damit nicht erst bei der Verarbeitung oder beim Hochladen einer XML-Datei die Fehler bemerkt werden, kann man die Prüfung auf syntaktische Fehler (sog. "Validierung") auch automatisieren. Hierzu wurden sog. "Schema-Dateien" eingeführt. Eine Schema-Datei enthält in einer speziellen Beschreibungssprache alle Festlegungen zur Gestaltung der XML-Datei.

Um eine Validierung anzustoßen, fügt man zunächst in den Kopf der XML-Datei (also in das Wurzelelement) einen Verweis auf die Schema-Datei ein. Das IQB hat für alle XML-Dateien solche Schema-Dateien entwickelt. Für eine Unit-Xml wäre z. B. das Hauptelement folgendermaßen zu ändern:

```xml
    <Unit
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Unit.xsd">
```
Es sollte stets die aktuelle Version im Pfad zur Schema-Datei benutzt werden.

Außerdem muss für die automatische Validierung ein Editor verwendet werden, der diese Validierung unterstützt. Das IQB empfiehlt Notepad++.


<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Booklet-Xml
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

Die Testheft-Definition besteht aus einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Arbeiten-mit-Xml%E2%80%90Dateien).

Es ist möglich Booklets zu konfigurieren. Hierfür stehen einige Attribute zur Verfügung, die in der Booklet.xml 
(wenn gewünscht) anzugeben sind. Alle verwendbaren Attribute befinden sich in einer separaten Konfiguraionsdatei 
(booklet-config.json) auf die das Testcenter zugreifen kann. Möchten Sie einzelne Attribute nutzen, 
müssen Sie das Attribut und den gewünschten Wert (Datum) in der Booklet.xml unter "BookletConfig" angeben. 

Nachfolgend sehen Sie die entsprechend benötigte Struktur in der Booklet.xml:

```xml
<Booklet>
  <Metadata>
      ...
  </Metadata>

  `<BookletConfig>`
      <Config key="force_responses_complete">OFF</CustomText>
      <Config key="unit_navibuttons">ARROWS_ONLY</CustomText>
      ...
  </BookletConfig>

  <Units>
      ...
  </Units>

</Booklet>
```
---

### Booklet Konfiguration

Nachfolgend finden Sie eine Übersicht über die verwendbaren Attribute und deren Bedeutung. 
**Achten Sie bei der Verwendung dieser Parameter auf die richtige Schreibweise (Groß-/Kleinschreibung)!**

|Attribut &nbsp; &nbsp;| Bedeutung     | Wert (Datum)    |
| :----------------| :----------| :--------|
|`loading_mode`|Ladeverhalten beim Start| **LAZY(default):** Start sobald wie möglich, Laden im Hintergrund fortsetzen;<br>**EAGER:** Testheft erst dann starten, wenn alle Inhalte geladen sind |
|`logPolicy`|Erfassen und Speichern von Log-Daten| **disabled:** Ausgeschaltet;<br>**lean:** Nur wichtige Meldungen;<br>**rich(default):** Alles außer debug-informationen;<br>**debug:** Auch debug-informationen |
|`pagingMode`|pagingMode (https://verona-interfaces.github.io/player/#operation-publish-vopStartCommand)|**separate(default):** pages are separated;<br>**concat-scroll:** concat-scroll;<br>**concat-scroll-snap:** concat-scroll-snap |
|`stateReportPolicy`|stateReportPolicy (https://verona-interfaces.github.io/player/#operation-publish-vopStartCommand)|**none:** pages are separated;<br>**eager(default):** concat-scroll;<br>**on-demand:** concat-scroll-snap|
|`page_navibuttons`|Navigationsbuttons für die Seitennavigation (innerhalb einer Aufgabe)|**OFF:** Keine Seitennavigation unterstützen (übernimmt ggf. die Aufgabe selbst);<br>**MERGED:** Die Seitennavigation wird durch die Aufgabennavigation mit übernommen;<br>**SEPARATE_TOP:** Seitennavigation über getrennte Button-Leiste - oben;<br>**SEPARATE_BOTTOM(default):** Seitennavigation über getrennte Button-Leiste - unten|
|`unit_navibuttons`|Navigationsbuttons für die Navigation zwischen den Aufgaben|**OFF:** Keine Buttons für Aufgabennavigation anzeigen (übernimmt ggf. die Aufgabe selbst);<br>**ARROWS_ONLY:** Nur die Buttons für 'Weiter' und 'Zurück' anzeigen;<br>**FULL(default):** Buttons für 'Weiter' und 'Zurück' und dazwischen kleine Buttons für jede Aufgabe anzeigen|
|`unit_menu`|Extra-Seite mit großen Buttons für Aufgaben zum direkten Springen|**OFF(default):** Ausgeschaltet;<br>**ENABLED_ONLY:** Eingeschaltet - nur die Aufgaben anzeigen, die noch freigegeben sind;<br>**FULL:** Eingeschaltet - auch die Aufgaben anzeigen, die nicht mehr freigegeben sind (gegraut)|
|`force_presentation_complete`|Verhalten, wenn noch nicht alle Elemente der Aufgabe angezeigt wurden|**OFF(default):** Ignorieren - Weiterblättern möglich;<br>**ON:** Weiterblättern verhindern, bis Anzeige vollständig|
|`force_responses_complete`|Verhalten, wenn noch nicht alle Antworten der Aufgabe vollständig gegeben wurden|**OFF(default):** Ignorieren - Weiterblättern möglich;<br>**SOME:** Weiterblättern erst möglich, wenn einige Antworten gegeben wurden;<br>**COMPLETE:** Weiterblättern erst möglich, wenn alle Antworten gegeben wurden;<br>**COMPLETE_AND_VALID:** Weiterblättern erst möglich, wenn alle Antworten gegeben wurden und als gültig eingeschätzt wurden|
|`unit_screenheader`|Legt fest, ob im obersten Seitenbereich Platz für Logo, Navigations-Buttons u. ä. gelassen wird.|**OFF:** Kein Seitenkopf. Achtung: Logo bleibt sichtbar (überlappt);<br>**WITH_UNIT_TITLE:** Seitenkopf wird angezeigt mit Titel der Unit (s. Booklet-XML);<br> **WITH_BOOKLET_TITLE:** Seitenkopf wird angezeigt mit Titel des Booklets (s. Booklet-XML);<br>**EMPTY (default):** Seitenkopf wird angezeigt (leer)|
|`unit_title`|Festlegung, ob oberhalb des Unitbereiches eine Zeile mit dem Unit-Titel gezeigt werden soll| **OFF:** Keine Titelzeile;<br> **ON(default):** Eine Zeile wird eingeblendet mit dem Unit-Titel (s. Booklet-XML)|
|`unit_show_time_left`|Festlegung, ob im obersten Seitenbereich bei einer festgelegten Maximalzeit für einen Testbereich die verbleibende Zeit angezeigt wird.| **OFF(default):** Die verbleibende Zeit wird nicht angezeigt;<br>**ON:** Die verbleibende Zeit wird angezeigt|

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# itc-Toolbox: Antworten und Logs
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

In Csv-Dateien, die aus dem IQB-Testcenter heruntergeladen werden, sind Werte in einer bestimmten Art und Weise aufgelistet und voneinander abgegrenzt. Die Abgrenzung erfolgt mittels
Semikolon, Hochkommata und Komma. Tabellenkalkulationsprogramme, wie bspw. Excel, können dieses Format lesen und erkennen über die 
entsprechende Zeichensetzung, welche Werte bspw. in den Tabellenkopf, in eine bestimmte Zeile oder Spalte gehören. 
Eine Csv-Datei ist vorwiegend als Werteransportmittel gedacht und ist daher nur schlecht für den Menschen lesbar. 
Daher ist es sinnvoll diese Csv-Datei in eine entsprechende Tabelle zu überführen. Damit erhöht sich die Lesbarkeit deutlich und macht 
die Auswertung zudem deutlich weniger fehleranfällig. Das IQB bietet zur Tabellenkonvertierung ein kleines Tool mit dem Namen: 
**ITC-Toolbox** für Windows an. Dieses ist frei verfügbar und kann von Anwender\*innen genutzt werden. Sie können das 
Programm über die IQB-Website herunterladen:<br>
https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox

Nach dem Öffnen des Programms stehen folgende Optionen zur Auswahl:

* Booklet-Xlsx
* Login-Xlsx
* SysCheck csv- > xlsx
* Antworten und Logs csv -> xlsx

Mittels des letzten Punktes können Csv-Dateien in Exceldateien (xlsx-Dateien) konvertiert werden. 
Wenn Sie zuvor heruntergeladenen Antworten und Logs eines Probanden in ein Xlsx-Format konvertieren möchten, 
betätigen Sie einfach den Button: *Antworten und Logs csv -> xlsx*. Anschließend wählen Sie den Ort aus an welchem sich die 
Dateien befinden und wählen einen Namen und einen Speicherort für die zu generierende Excel-Tabelle aus. 

Wie sind die Inhalte in diesen 2 Tabellen zu deuten?

### Tabelle Anworten

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 27.03.2021
Prio: high
todo:
  - Die Tabellenwerte entstammen einem alten Text auf GitHub. Nach Download einer 
    Antwort-/ und Logdatei vom Testcenter und Konvertierung in Excel
    haben die Spalten andere Namen als die in der Tbl aufgeführten. Sind diese Angaben nachfolgend sicher noch gültig??? 
```

| Spaltenbezeichnung | Bedeutung |
| :------------- | :---------- |
|ID|Kombination aus anderen (nachfolgenden) Informationen. Diese ID wird benötigt, um eine Zeile eindeutig zu identifizieren. Es handelt sich um eine Testsitzung, also eine Testperson beantwortet ein konkretes Booklet. Diese Kombination ist nötig, weil eine Testperson mehrere Booklets haben könnte und in einem Booklet theoretisch dieselbe Unit enthalten sein kann (z. B. Motivationsabfrage). Es muss eindeutig sein, in welchem Booklet diese Unit platziert war.<br> Diese ID wird auch in den anderen zwei Tabellen verwendet, so dass hierüber eine Zusammenführung der Informationen erfolgen kann.|
|Group|Gruppe, in der das Anmelde-Login platziert war. Dies ist normalerweise nur ein Ordnungsmerkmal für das Monitoring der Durchführung.|
|Login+Code|Entsprechend der Anmeldung der Testperson|
| Booklet | ID des Booklets |
| Variablen nach dem Schema<br>`<Unit-ID>##<innere ID>`<br>z. B. `EL105R##canvasElement10` | Der Player des Testcenters speichert im bisherigen Modell die Antwortdaten als Paarung ID->Wert ab, wobei nicht definiert ist, was ID kennzeichnet (Item, Aspekt eines Items, Eingabeelement des Formulars usw.; hier mal als innere ID bezeichnet). Sicher ist nur, dass diese ID innerhalb der Unit eindeutig ist, und da die Unit-ID eindeutig für das Testheft ist, erlaubt die Kombination Unit-ID mit dieser inneren ID eine eindeutige Zuordnung des Antwort-Wertes zu einer Testperson in einem Booklet, wodurch sich die übliche zweidimensionale Struktur der Antwortdaten ergibt.<br> Es werden nur Units berücksichtigt, die tatsächlich Antwortdaten produziert haben. Reine Textseiten, die z. B. nur Instruktionen enthalten, werden nicht in die Tabelle aufgenommen.<br>Die Variablenspalten werden alphabetisch sortiert ausgegeben.<br>Sollte eine Unit mehrfach in einem Test vorkommen, fügt das System ab dem zweiten Vorkommen der Unit automatisch ein Suffix hinzu:<br>`<Unit-ID>%<n>`<br>n steht hier für die fortlaufende Nummerierung, beginnend mit 1 bei dem zweiten Vorkommen der Unit|

Die Zeilen dieser Tabelle sind nach ID sortiert. Sollte eine Testperson den Test nur gestartet, aber keine Antwortdaten abgeschickt haben, erscheint sie nicht in der Liste.


### Tabelle Logs

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 21.03.2021
Prio: high
todo:
  - Die Tabellenwerte entstammen einem alten Text auf GitHub. 
    Nach Download einer Antwort-/ und Logdatei vom Testcenter und Konvertierung in Excel
    haben die Spalten andere Namen als die in der Tbl aufgeführten. Sind die nachfolgenden Angaben sicher noch gültig?
```

Für die weitere Beurteilung der Antworten schickt das IQB-Testcenter eine größere 
Menge zeitpunktbezogener Daten, sog. Log-Daten. Hierbei wird stets ein Zeitstempel 
mitgeliefert (Datum und Uhrzeit auf dem Computer der Testperson) sowie Art des 
Ereignisses und ggf. weitere Informationen. Aus dieser Folge von Ereignissen lässt 
sich die Navigation zwischen Units und Seiten und somit die Zeit ermitteln, die eine 
Testperson während des Tests auf einer bestimmten Seite verbracht hat.

Die Tabelle TimeOnUnit listet alle Zeiten auf, die die Testpersonen auf einer Unit 
verbracht hat. Dabei kann der Besuch einer Unit mehrfach auftreten. Folgende Spalten 
enthalten Informationen hierzu:

* `Start At`: Zeitstempel des Starts der Navigation in die Unit
* `Player Load Time`: Anzahl Millisekunden nach Start bis zu dem Zeitpunkt, an 
dem der Player "RUNNING" meldet
* `Stay Time`: Verweildauer bei dieser Unit in Milisekunden. Das Verweilen beginnt 
erst nach Laden des Players und der Unit-Daten und wird 
als beendet angesehen, wenn eine andere Unit angewählt wurde oder der Test terminiert. 
Achtung: Sollte der Controller ein PAUSE-Commando geben, läuft die Zeit weiter.
* `Was Paused`: (True/False) Der Controller hat zwischendurch ein PAUSE-Commando geben.
* `Lost Focus`: (True/False) Die Test hat einen Fokusverlust festgestellt, d. h. 
die Testperson hat im Browser das Test-Tab verlassen oder den Browser
* `Responses Some Time`: Zeit in Millisekunden nach Laden des Players und der 
Unitdaten bis der Player "Responses Progress: Some" meldet
* `Responses Complete Time`: Zeit in Millisekunden nach Laden des Players und der 
Unitdaten bis der Player "Responses Progress: Complete" meldet

### Konfiguration über YAML-Datei

Eine YAML-Datei ist eine einfache Textdatei, in der über eine spezielle Syntax Informationen 
hinterlegt sind. Es können drei Konfigurationseinträge `bookletSizes`, `omitUnits`und `variables` definiert werden. 
Hier ein Beispiel:

```
bookletSizes:
  THETLK: 19138814
omitUnits:
- Ex_MC
- Ex_SA
- Ex_MM
- Ex_Audio
variables:
  EL639v2:
    EL639v201:
    - canvasElement10
    - canvasElement11
    - canvasElement12
    - canvasElement13
    EL639v202:
    - canvasElement14
    - canvasElement15
    - canvasElement16
    - canvasElement17
    __omit__:
    - canvasElement3
    - canvasElement4
    - pagesViewed
    - responsesGiven
  EL666:
    EL66601:
    - canvasElement18
    EL66602:
    - canvasElement19
    EL66604:
    - canvasElement20
    EL66605:
    - canvasElement21
    EL66606:
    - canvasElement22
    __omit__:
    - canvasElement17
    - canvasElement34
    - canvasElement51
    - canvasElement37
    - pagesViewed
    - responsesGiven
```

#### bookletSizes

Hier wird eine ID eines Testheftes erwartet, Doppelpunkt, und dahinter die Größe des Testheftes in Bytes.
Die Größe der Testhefte erhält man im IQB-Testcenter über die Admin-Funktion `Arbeitsbereich prüfen`. Bitte 
vor dem Übertragen jeweils die Punkte aus der Zahl entfernen. Mit Hilfe der Testheftgröße kann die 
Download-Geschwindigkeit berechnet werden (s. oben).

#### omitUnits

Die hier aufgeführten Units werden bei der Berichtstransformation ignoriert. Normalerweise sind den eigentlichen 
Testaufgaben Probe- bzw. Trainingsaufgaben vorgeschaltet, die der Einstellung der Lautstärke usw. dienen. Deren 
Ergebnisse interessieren üblicherweise nicht.

#### variables

Für jede Unit (Angabe der ID) werden neue Variablen definiert. Die darunter jeweils aufgeführten Bezeichner 
entsprechen IDs von Daten, die in den Csv zu finden sind. Hier gibt es die Fälle
* Umbenennen: Wenn nur eine einzige Csv-ID genannt ist, erhält die neue Variable deren Wert
* Transformation von Radiobutton-Gruppen: Wenn mehrere Csv-IDs aufgeführt sind geht der Transformator davon aus, dass 
es sich um Radiobuttons handelt, bei denen nur ein Wert true (also ausgewählt) ist. Dann wird der neuen Variable 
eine Zahl zugewiesen, die der Position der Csv-ID in der Liste entspricht. Eine 0 oder leer zeigt an, dass 
keine Option ausgewählt wurde.
* Ignorieren: Wenn das Schlüsselwort `__omit__` verwendet wird, dann ignoriert der Transformator die hier gelisteten 
IDs. Damit kann man z. B. Audioelemente oder Beispielitems entfernen, deren Wert nicht interessiert.

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# itc-Toolbox: SysCheck
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

In Csv-Dateien, die aus dem IQB-Testcenter heruntergeladen werden, sind Werte in einer bestimmten Art und Weise aufgelistet und voneinander abgegrenzt. Die Abgrenzung erfolgt mittels
Semikolon, Hochkommata und Komma. Tabellenkalkulationsprogramme, wie bspw. Excel, können dieses Format lesen und erkennen über die 
entsprechende Zeichensetzung, welche Werte bspw. in den Tabellenkopf, in eine bestimmte Zeile oder Spalte gehören. 
Eine Csv-Datei ist vorwiegend als Werteransportmittel gedacht und ist daher nur schlecht für den Menschen lesbar. 
Daher ist es sinnvoll diese Csv-Datei in eine entsprechende Tabelle zu überführen. Damit erhöht sich die Lesbarkeit deutlich und macht 
die Auswertung zudem deutlich weniger fehleranfällig. Das IQB bietet zur Tabellenkonvertierung ein kleines Tool mit dem Namen: 
**itc-Toolbox** für Windows an. Dieses ist frei verfügbar und kann von Anwender\*innen genutzt werden. Sie können das 
Programm über die IQB-Website herunterladen:<br>
https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox

Nach dem Öffnen des Programms stehen folgende Optionen zur Auswahl:

* Booklet-Xlsx
* Login-Xlsx
* SysCheck csv- > xlsx
* Antworten und Logs csv -> xlsx

Mittels des vorletzten Punktes können Csv-Dateien in Exceldateien (xlsx-Dateien) konvertiert werden. 
Wenn Sie zuvor heruntergeladene Syscheck-Dateien in ein Xlsx-Format konvertieren möchten, 
betätigen Sie einfach den Button: *SysCheck csv -> xlsx*. Anschließend wählen Sie den Ort aus an welchem sich die 
Dateien befinden und wählen einen Namen und einen Speicherort für die zu generierende Excel-Tabelle aus. 

Wie sind die Inhalte in dieser Tabelle zu deuten?

### Tabelle Syscheck

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 27.03.2021
Prio: high
todo:
  - Von Martin prüfen lassen ob Tbl+Werte noch gültig sind.
```

In dieser Tabelle sind weitere eventuell interessante Daten einer Testsitzung 
aufgelistet:

| Spaltenbezeichnung | Bedeutung |
| :------------- | :---------- |
|ID|ID der Testsitzung wie in den anderen Tabellen|
|Start at|Beginn des ersten Ladens der Testinhalte nach Auswahl des Booklets durch die Testperson (Zeitstempel).|
|loadcomplete after|Dauer des Ladevorganges in Millisekunden|
|loadspeed|Ladegeschwindigkeit als Quotient aus Bookletgröße (aus der zusätzlich zugewiesenen txt-Datei) und Ladedauer. Wenn die Bookletgröße in Bytes und die Dauer in Millisekunden angegeben werden (wie hier aktuell im Testcenter), dann ist die Einheit des Wertes kBytes/sec|
|firstUnitRunning after|Zeit zwischen Start des Ladens der Testinhalte und Eintritt in die erste Unit. Achtung: In Abhängigkeit von Testhefteinstellungen kann die erste Unit angezeigt werden, bevor alle Testinhalte geladen wurden.|
|os|Betriebssystem (operating system)|
|browser|Name und Version|
|screen|Breite x Höhe in Pixels|

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# itc-Toolbox: Booklets
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

Die Windows-Software **itc-Toolbox** konvertiert Excelinhalte in das für die *Booklet.xml* benötigte Format. 
Das Tool steht zur freien Verfügung und kann über folgenden Link heruntergeladen werden:
https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox

Vorteil dieser Methode: Sie müssen nicht direkt in der *Booklet.xml* arbeiten, sondern können die Werte dieser Datei mittels Excel beinflussen. 
Dies erhöht für einige Anwender\*innen die Übersichtlichkeit, eventuell verlangt es aber entsprechende Nachkontrollen der Testdatei.

Damit itc-Toolbox Excelinhalte entsprechend konvertieren kann, muss die Exceldatei über ein entsprechendes Format verfügen.
Eine Vorlage können Sie hier herunterladen: [Excel-Vorlage für die ITC-Toolbox](https://github.com/iqb-berlin/itc-toolbox/blob/master/Booklet-Template.xlsx)<br>
> **Beachten Sie bitte: Änderungen an Tabellenköpfen oder Blattbezeichner, können ein ordnungsgemäßes Einlesen der Excelinhalte durch ITC-Toolbox verhindern!**

Nach der Installation und dem Start der **itc-Toolbox** können Sie zwischen verschiedenen Optionen wählen:

* Booklet-Xlsx
* Login-Xlsx
* SysCheck csv- > xlsx
* Antworten und Logs csv -> xlsx

Hier interessiert uns vor allem der Punkt: *Booklet-Xlsx*.

**Erzeugen / Bearbeiten der Booklet.xml**

Nach Auswahl des ersten Punktes: *Booklet-Xlsx* muss der Speicherort der entsprechende Excel-Datei angegeben werden.
**ITC-Toolbox** überprüft anschließend die Struktur der Excel-Datei und versucht die dort angegebenen Zusatzinformationen auf den anderen
Excel Blattseiten zu finden. Können Bezeichner nicht gefunden oder zugeordnet werden, werden entsprechende Fehlermeldung generiert.
Wurden alle Bezeichner gefunden und konnten entsprechend zugeordnet werden, erscheint eine Meldung über die erfolgreiche Erzeugung
einer *Booklet.xml*. Die *Booklet.xml* wird dann im selben Verzeichnis gespeichert in dem sich auch die Excel-Datei, die als Vorlage diente, 
befindet.

Um die Inhalte und Strukturen dieser Vorlage besser zu verstehen, betrachten Sie bitte die nachfolgenden Abbildungen. Diese gehen näher 
auf die Strukturen der Excel-Inhalte und den Auswirkungen auf die so generierte *Booklet.xml* ein. Achten Sie auch die farbliche Hervorhebung 
in Bild und Code.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_ToolBox_Excel_final.png)

Auf der Grundlage dieser im obigen Bild dargestellten Excel-Datei und deren Inhalten wird die folgende *Booklet.xml* erzeugt:

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_ToolBox_BookletXml_final.png)

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# itc-Toolbox: Logins
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

Die Windows-Software **itc-Toolbox** erzeugt Zufallsworte, die für Logins verwendet werden können.
Das Tool steht zur freien Verfügung und kann über folgenden Link heruntergeladen werden:
https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox

Nach der Installation und dem Start der **itc-Toolbox** können Sie zwischen verschiedenen Optionen wählen:

* Booklet-Xlsx
* Login-Xlsx
* SysCheck csv- > xlsx
* Antworten und Logs csv -> xlsx

Hier interessiert uns vor allem der Punkt: *Login-Xlsx*.

### Anforderungen an Login-Daten

Über den Admin-Bereich des Testcenters sind die Zugangsdaten für 
Testpersonen, aber auch für Reviewer und die Testleitung zu hinterlegen. Strukturiert 
in Gruppen, bestehen diese meist aus Benutzername und Kennwort, ggf. auch ergänzt 
durch Personencodes.

Die Verfahren zur Erzeugung und Verwaltung der Login-Daten sind sehr vielfältig. Mal 
hat man Monitor-Accounts, mal Code-basierte, mal nicht, und die Weiterverarbeitung bzw. 
Dokumentation (Verschicken an die Schulen, Zettelchen auf dem Platz) hat nochmal 
gesonderte Anforderungen. Außerdem kann man oft nicht alle Logins auf einmal erzeugen, 
weil die Rückmeldungen der Schulen nur schleppend eintreffen. Dann muss man zu 
vorhandenen Logins neue erzeugen. Eventuell sind Aspekte des Datenschutzes zu beachten.

Im Moment scheint es daher nicht sinnvoll, ein formales Verfahren für Logins festzulegen. Es 
gibt allerdings einen Schritt hierbei, der sehr anstrengend ist: Festlegen von Codes für 
Logins (Benutzername/-kennzeichen, Kennwort) oder Personencode. Hierbei 
sind eine Reihe von Kriterien zu beachten:

* Sie müssen eindeutig sein: Kein Login-Benutzername darf doppelt vorkommen.
* Die Zeichen müssen gut merkbar sein, damit bei der Übertragung vom Zettel in den Computer kein Fehler passiert.
* Die Tasten sollen auf der Computer-Tastatur gut findbar sein. Es sollte zur Eingabe nur eine Taste nötig sein. 
  Großbuchstaben und die meisten Sonderzeichen sind also ungünstig.
* Die Zeichen müssen gut lesbar sein: Optisch sehr ähnliche Zeichen wie "n" und "m" oder "1" und "l" sind zu vermeiden.
* Die Codes müssen gut sprechbar und akustisch verständlich sein: Sollte z. B. die Testleiterin einem Schüler den Code ansagen, 
  darf es keine Fehler geben.
* Es sollte keine Gefahr stehen, dass durch nicht erkannte Zeichenkodierung von Dateien Probleme mit Sonderzeichen (Umlaute!) auftreten.

### Nutzung der itc-ToolBox

Über die Funktion "Logins-Xlsx" erzeugt die itc-ToolBox eine Excel-Tabelle mit vier 
Spalten: Zweistellige, dreistellige, vierstellige und fünfstellige Codes. Das IQB 
verwendet eine Auswahl aus Kleinbuchstaben und Ziffern - keine Sonderzeichen und Umlaute. 
Kleinbuchstaben wechseln sich dabei mit Ziffern ab. Die Codes kommen in der Tabelle 
jeweils nur einmal vor.

Diese Tabelle soll für eine Studie als Quelle benutzt werden, aus 
der man nach Bedarf Codes entnimmt (Copy & Paste) und in die eigentlichen Dokumente zur 
Login-Verwaltung überträgt. Bei Codes für Logins (Eindeutigkeit erforderlich über die 
gesamte Studie) sollten die Codes in der Tabelle gelöscht oder markiert werden, um 
eine Mehrfachverwendung auszuschließen.

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Login: Modi der Testdurchführung
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
# Testtaker-Xml
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Überarbeitung THuste
Stand: 8.4.2021
```
Die Testtaker-Definition besteht aus einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](Arbeiten-mit-Xml‐Dateien).



`METADATA`

<table>
	
<tr>
    <td>Description:</td>
    <td>>xxx<</td>
	<td>Datum</td>
    <td>frei wählbarer Text für die Metadaten Beschreibung</td>
</tr>

</table>

```xml
<Metadata>
  <Description>
    Diese Datei enthält Informationen zur Art des Logins und der Testdurchführung.
  </Description>		
</Metadata>
  ...
```
---

`CUSTOMTEXTS`

<table>
	
<tr>
    <td>CustomText:</td>
    <td>key</td>
    <td>Attribut</td>
    <td>Vordefinierter Wert. Erzeugt einen Custom Text. Siehe <b>Custom Text Configuration.</a></td   
</tr>
<tr>
    <td>CustomText:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>frei wählbar Text zur Anzeige eines Custom Text</td>
</tr>

</table> 

```xml
<CustomTexts>
  <CustomText key="app_title">Hier steht ein Custom Text</CustomText>
</CustomTexts>
```
---

`GROUP`

<table>

<tr>
    <td>Group:</td>
    <td>id</td>
    <td>Attribut</td>
    <td>frei wählbarer Wert</td>
</tr>
<tr>
    <td>Group:</td>
    <td>label</td>
    <td>Attribut</td>
    <td>frei wählbarer Wert</td>
</tr>
<tr>
    <td>Login:</td>
    <td>name</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert. Wird zur Anmeldung am Testcenter benötigt, um entsprechend des gewählten Testmodi einen Test durchzuführen.</td>
</tr>
<tr>
    <td>Login:</td>
    <td>mode</td>
    <td>Attribut</td>
    <td>Vordefinierter Wert. Bestimmt wie ein Test ablaufen soll (finaler Test oder Probetest etc.).
	Siehe: <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung">Modi der Testdurchführung</a></td>
</tr>
<tr>
    <td>Login:</td>
    <td>pw</td>
    <td>Attribut</td>
    <td>Frei wählbares Passwort. Wird zur Anmeldung am Testcenter benötigt, um entsprechend des gewählten Testmodi einen Test durchzuführen.</td>
</tr>
<tr>
    <td>Booklet:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Wert. Die ID in der Booklet.xml muss den selben Namen tragen (Groß-/Kleinschreibung beachten!)</td>
</tr>

</table>

```xml
<Group id="Gruppe1" label="Dies ist die erste Gruppe.">
  <Login name="user1" mode="run-demo" pw="123">
    <Booklet>Booklet1</Booklet>
  </Login>
</Group>

```

### Custom Text Konfigurationen

Diese Anwendung ermöglicht es zur Laufzeit Änderungen an Texten durchzuführen. 
Dies kann notwendig sein, wenn Standardtitel, Eingabeauffforderungen oder Erklärungen nicht zur spezifischen Umgebung, 
in welcher das **Testcenter** ausgeführt wird, passen. Alle möglichen CustomText Attribute sind in einer Konfigurationsdatei deklariert, 
die das **Testcenter** ausliest. Daher können auch nur CustomText Attribute verwendet werden, die in dieser Datei 
deklariert sind. Eine Übersicht der verfügbaren Attribute und deren Bedeutung entnehmen Sie bitte der Liste weiter unten. 
Nach dem Attribut kann dann ein frei gewählter Text angegeben werden. 
In dem unteren Code würde nun der Titel der Hauptwanwendung (Attribut: app_title) wie folgt lauten: "Titel der Anwendung". 
CustomText kann in der Login.xml (Testtakers.xml) oder im Systemcheck konfiguriert werden.

Nachfolgend sind die benötigten Strukuren für CustomText via `Login.xml` (Testtakers.xml) aufgeführt:

```xml
<Testtakers>
  <Metadata>
    ...		
  </Metadata>
	
  <CustomTexts>
    <CustomText key="app_title">Titel der Anwendung</CustomText>
    ...
  </CustomTexts>
	
  <Group id="frei wählbare ID" label="frei wählbarer Text Label">
    ...	
  </Group>

</Testtakers>
```

Nachfolgend sind die benötigten Strukuren für `Custom Check` aufgeführt:

```xml
<Config>
    <UploadSpeed ...
    <DownloadSpeed ...
    <CustomText key="syscheck_questionsintro">...</CustomText>
    <CustomText key="app_intro1">...</CustomText>
...
</Config>
```

---

Nachfolgend finden Sie eine Übersicht über die verwendbaren Attribute und deren Bedeutung. 
**Achten Sie bei der Verwendung dieser Attribute auf die richtige Schreibweise (Groß-/Kleinschreibung)!**


| Key (Attribut)  | Used for | Default |
| :------------- | :---------- | :----------- |
|`app_intro1`|Begrüßungstext auf der Startseite (Text nach IQB-Link)|betreibt auf diesen Seiten eine Anwendung für das computerbasierte Leistungstesten von Schülerinnen und Schülern. Der Zugang zu einem Test ist nur möglich, wenn Sie von Testverantwortlichen Zugangsdaten erhalten haben. Es sind keine weiteren Seiten öffentlich verfügbar.|
|`app_title`|Titel der Hauptanwendung|IQB-Testcenter|
|`booklet_codeToEnterPrompt`|Aufforderung für die Eingabe eines Freigabewortes (Dialog-Box)|Bitte gib das Freigabewort ein, das angesagt wurde!|
|`booklet_codeToEnterTitle`|Titel der Dialogbox für die Eingabe eines Freigabewortes|Freigabewort|
|`booklet_errormessage`|Nachricht an die Testperson, wenn ein schwerer Fehler aufgetreten ist|Es ist ein schwerer Fehler aufgetreten. Bitte rufe die Aufsichtsperson und beschreibe das Problem!|
|`booklet_msgPresentationNotCompleteTextNext`|Nachrichttext, dass nicht weitergeblättert werden kann, solange die Präsentation des Aufgabeninhaltes nicht abgeschlossen ist|Du kannst erst weiterblättern, wenn Audio-Dateien vollständig abgespielt wurden und wenn du in allen Fenstern bis ganz nach unten gescrollt hast.|
|`booklet_msgPresentationNotCompleteTextPrev`|Nachrichttext, dass nicht zurückgeblättert werden kann, solange die Präsentation des Aufgabeninhaltes nicht abgeschlossen ist|Eine Audio-Datei ist noch nicht bis zu Ende abgespielt oder Seiten wurden noch nicht vollständig gezeigt. Wenn du jetzt zurückblätterst, kannst Du später Audio-Dateien nicht nocheinmal starten.|
|`booklet_msgPresentationNotCompleteTitleNext`|Titel der Nachricht (Dialogbox), dass nicht weitergeblättert werden kann, solange die Präsentation des Aufgabeninhaltes nicht abgeschlossen ist|Weiterblättern nicht möglich!|
|`booklet_msgPresentationNotCompleteTitlePrev`|Titel der Nachricht (Dialogbox), dass nicht zurückgeblättert werden kann, solange die Präsentation des Aufgabeninhaltes nicht abgeschlossen ist|Zurückblättern - Warnung|
|`booklet_msgSoonTimeOver1Minute`|Nachricht, dass für die Bearbeitung eines Abschnittes noch 1 min Zeit ist|Du hast noch 1 Minute Zeit für die Bearbeitung der Aufgaben in diesem Abschnitt.|
|`booklet_msgSoonTimeOver5Minutes`|Nachricht, dass für die Bearbeitung eines Abschnittes noch 5 min Zeit sind|Du hast noch 5 Minuten Zeit für die Bearbeitung der Aufgaben in diesem Abschnitt.|
|`booklet_msgTimeOver`|Nachricht, dass die Bearbeitungszeit für einen Abschnitt abgelaufen ist.|Die Bearbeitung des Abschnittes ist beendet.|
|`booklet_msgTimerCancelled`|Nachricht, dass die Bearbeitung eines Abschnittes mit Timer abgebrochen wurde|Die Bearbeitung des Abschnittes wurde abgebrochen.|
|`booklet_msgTimerStarted`|Nachricht, dass der Timer für die Bearbeitung eines Abschnittes gestartet wurde|Die Bearbeitungszeit für diesen Abschnitt hat begonnen: |
|`booklet_pausedmessage`|Nachricht an die Testperson, wenn der Test vom System unterbrochen wurde|Der Test wurde kurz angehalten.|
|`booklet_tasklisttitle`|Titel für die Auflistung der Aufgaben (Schalter)|Aufgaben|
|`booklet_warningLeaveTimerBlockTextPrompt`|Schalterbeschriftung für 'Zurück zum Test'|Du verlässt einen zeitbeschränkten Bereich und kannst nicht zurückkehren. Trotzdem weiterblättern?|
|`booklet_warningLeaveTimerBlockTitle`|Titel für Warnung (Dialogbox) vor dem vorzeitigen Verlassen eines Abschnittes mit Timer|Aufgabenabschnitt verlassen?|
|`login_bookletSelectPromptMany`|Aufforderung, aus der Liste der gefundenen Tests einen auszusuchen (auf Schalter klicken)|Bitte klicke auf eine der Schaltflächen auf der linken Seite, um einen Test zu starten!|
|`login_bookletSelectPromptNull`|Nachricht für den Fall, dass Booklet(s) beendet wurden und keine weiteren zur Verfügung stehen|Beendet. Es können keine weiteren Testhefte gestartet werden.|
|`login_bookletSelectPromptOne`|Aufforderung, den einen gefundenen Test anzuklicken (auf Schalter klicken)|Bitte klicke auf die Schaltfläche auf der linken Seite, um den Test zu starten!|
|`login_codeInputPrompt`|Aufforderung, Code einzugeben (bei einem zweistufigen Login-Prozess)|Bitte Log-in eingeben, der auf dem Zettel steht!|
|`login_codeInputTitle`|Titel des Eingabeformulares für den Code|Log-in eingeben|
|`login_pagesNaviPrompt`|Aufforderungstext, weitere Seiten einer Unit auszuwählen, z. B. 'Wähle hier andere Seiten dieser Aufgabe:'|Weitere Seiten:|
|`login_testEndButtonLabel`|Schalterbeschriftung für 'Test beenden'|Test beenden|
|`syscheck_intro`|Text auf der ersten Seite des System-Checks|Dieser Systemcheck soll gewährleisten, dass der von Ihnen verwendete Computer für eine bestimmte Befragung oder Testung geeignet ist.|
|`syscheck_questionsRequiredMessage`|Nachricht an die Testperson, wenn einige Fragen, die als 'required' markiert sind, nicht beantwortet wurden|Bitte prüfen Sie die Eingaben (unvollständig):|
|`syscheck_questionsintro`|Aufforderung, die Fragen (Questionnaire) zu beantworten|Bitte bearbeiten Sie die nachfolgenden Fragen.|
|`syscheck_unitPrompt`|Titelzeile über der Aufgabe|Bitte prüfen Sie die folgenden Aufgaben-Elemente|

