<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# itc-Toolbox: Antworten und Logs (Abschnittsmarker)
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
# itc-Toolbox: SysCheck (Abschnittsmarker)
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
# itc-Toolbox: Booklets (Abschnittsmarker)
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
# itc-Toolbox: Logins (Abschnittsmarker)
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
