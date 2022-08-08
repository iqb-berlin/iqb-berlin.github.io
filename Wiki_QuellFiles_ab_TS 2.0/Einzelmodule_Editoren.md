<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Verona Dan Editor v3.1 (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

> **[Hier](https://github.com/iqb-berlin/verona-editor-dan)** der Link zum GitHub Repository.<br>
> **[Hier](https://github.com/iqb-berlin/verona-editor-dan/releases)** finden Sie die letzten aktuellen Versionsstände.

Die folgenden [Videos](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Editor:-Dan) werden direkt zum **Dan-Editor** angeboten

Das folgende [Video: Vom Entwurf zum Test](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-TBA-Einf%C3%BChrung) beschäftigt sich vorwiegend mit dem Aufgabenentwurf, aber auch hier werden auch Aufgaben mit den **Dan-Editor** erzeugt:

### Übersicht

:information_source: Zu beachten ist: Das **Studio** und auch der Editor haben noch einmal optische Veränderungen erfahren. Die nachfolgenden Bilder können bzgl. Optik vom aktuellen Stand des Editors und des Studios abweichen. Funktional hat sich aber nichts geändert.

Der Editor wird über den Tab: **Editor** im Bereich der Unitbearbeitung geöffnet. Nachfolgend wird dann die Editoransicht angezeigt:

![iqb online assessment applications with relations: Studio Editieransicht](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Editoransicht_final.png)

* Grün markiert:<br>
	Im oberen Bereich die Elemente, die auf einer Seite hinzugefügt werden können. Dies sind bspw. Schaltflächen, Textfelder, Grafiken, Multiple-Choice-Felder etc. Im mittleren Bereich Optionen zur Formatübertragung und zum Kopieren und Einfügen markierter Elemente. Im unteren Bereich Pfeil-Schaltflächen, mit denen man alle Elemente auf einer Seite um 10px verschieben kann. Ganz unten die Option zum Löschen eines aktiven Elements und Optionen zum Up- und Download von Dateien. Eine detailierte Beschreibung der Elemente und Funktionen erfolgt weiter unten. 
	 
* Gelb markiert:<br>
	Wenn eine Unit neu angelegt wird, besteht diese zu Anfang immer nur aus einer Seite. Die Seiten können anschließend mithilfe des kleinen Pluszeichens im gelb markierten Bereich beliebig erhöht werden.

* Blau markiert:<br>
	Eigenschaften eines Elements. Wird bspw. ein Textfeld Element einer Seite hinzugefügt, kann über die Eigenschaften das Textfeld nachträglich bearbeitet werden. Es kann die Größe, Position etc. angepasst werden. 

#### Erstellung Aufgabenelemente

Aufgabenelemente stehen über eine kleine Box (im oberen Bild grün markiert) bereit. Diese Box stellt nicht nur die Elemente, sondern auch weitere Funktionen zur Verfügung.
Nachfolgend eine Übersicht aller Elemente und weiterer Funktionen (die Nummerierung bezieht sich auf den grün markierten Bereich im oberen Bild):

1 Elemente zum Einfügen<br>
1.1 Text hinzufügen<
Zum Erstelllen einer Textbox für jeglichen Text (Aufgabenstellung, Stimulus, Fragen, ...).<br>
1.2 Bild hinzufügen<br>
1.3 Audio hinzufügen<br>
1.4 Video hinzufügen<br>
1.5 Textbox hinzufügen. Für einzeilige Antwortfelder mit erwarteten Antworten von 3-4 Wörtern Länge<br>
1.6 Multiline Textbox hinzufügen. Für (mehrzeilige) Antwortfelder mit längeren erwarteten Antworten<br>
1.7 Checkbox hinzufügen. Für Multiple-Choice-Aufgaben bei der mehrere Optionen ausgewählt werden sollen<br>
1.8 Multiple Choice hinzufügen. Für Multiple-Choice-Aufgaben bei denen nur eine Option ausgewählt werden soll. Zu einer Option gehörende Buttons müssen hierbei denselben Gruppennamen bekommen.<br>
1.9 Dropdown hinzufügen<br>
1.10 Tabelle hinzufügen. Bitte wenn möglich vermeiden<br>
1.11 html-Element hinzufügen<br>
1.12 Viewpoint hinzufügen. Bei einer Seitenlänge von mehr als 1000 px im unteren Bereich einen Viewpoint platzieren. Dadurch wird sichergestellt, dass alle Teile einer Aufgabe gesehen werden bevor Seitenwechsel folgt.<br>
1.13 Button hinzufügen<br>

2 Kopieren<br>
2.1 Eigenschaften übertragen. Überträgt die Eigenschaften des ausgewählten Elements auf alle Elemente der Seite<br>
2.2 Kopiere Element. Kopiert das ausgewählt Element in den Zwischenspeicher<br>
2.3 Füge Element ein. Fügt das zwischengespeicherte Element ein.<br>
2.4 Kopieren und wiedereinfügen. Kopiert das ausgewählte Element und fügt es direkt wieder ein<br>

3 Elemente verschieben<br>
3.1 Verschiebe alle Elemente auf der Seite um 10 px nach oben<br>
3.2 Verschiebe alle Elemente auf der Seite um 10 px nach unten<br>
3.3 Verschiebe alle Elemente auf der Seite um 10 px nach rechts<br>
3.4 Verschiebe alle Elemente auf der Seite um 10 px nach links<br>

4 Element löschen<br>

5 Backup<br>
5.1 lade eine Aufgabendatei hoch (vom eigenen Computer)<br>
5.2 lade die Aufgabendatei runter (auf den eigenen Computer)<br>

### Textelement hinzufügen

Nachdem ein Textelement auf der Seite platziert und markiert wurde, erscheint auf der rechten Seite ein Eigenschaftenfenster. In diesem können die Eigenschaften wie nachfolgend aufgelistet angepasst werden. Die aufgeführten Werte orientieren sich an den Erfahrungen der IQB Entwicklerteams.

![iqb online assessment applications with relations: Studio Elemente](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Elemente_Eigenschaften_final.png)

> Die nachfolgende Beschreibung enthält Vorschlagswerte, die auf Erfahrungen des IQB beruhen und daher nur als Empfehlung anzusehen sind.

1. Breite: Die Breite des Textfeldes, höchstens Breite der Seite - 60
2. Erste Zeile: Die Einrückung der ersten Zeile
3. Fettgedruckt: Wenn das gesamte Textfeld fettgedruckt sein soll "true" auswählen, für einzelne Wörter siehe 13
4. Hintergrundfarbe: Standard: durchsichtig, für Beispiele: hellgrau
5. Höhe: für einzeilige Texte normalerweise 30, bei mehrzeiligen Texten 25xAnzahl Zeilen, bei Stimulustexten 27xAnzahl Zeilen
6. Kursivgedruckt: Wenn das gesamte Textfeld kursivgedruckt sein soll "true" auswählen, für einzelne Wörter siehe 13
7. Navigate to: Als Hyperlink zwischen Seiten benutzbar, normalerweise nicht verwenden
8. Schriftart: Für Stimulustexte Times New Roman, ansonsten immer Arial
9. Schriftfarbe
10. Schriftgröße: Stimulustexte 22; Quellenangaben 10 (Arial); Überschriften 24 (fett); Standard 20
11. Sichtbar
12. Style
13. Text: Hier den eigentlichen Text einfügen. Für das bearbeiten des Stils einzelner Wörter gängige HTML-Befehle verwenden, z.B. **Dieser Text ist fett**, *Dieser Text ist kursiv*  weitere Beispiele hier.
14. Sonderzeichen: Zum Kopieren und Einfügen im Text
15. Textausrichtung
16. Unterstrichen: Wenn das gesamte Textfeld unterstrichen sein soll "true" auswählen, für einzelne Wörter siehe 13
17. Zeilenhöhe: Bei mehrzeiligen Textfeldern, Standard 120%
18. x-Koordinate: horizontale Position des Textfeldes auf der Seite, mindestens 30
19. y-Koordinate: vertikale Position des Textfeldes auf der Seite, mindestens 30<
20. z-Index
21. Neue Eigenschaften einsetzen: "Speichern" Taste für die Eigenschaften, muss nach Verändern eines Elements zum Speichern gedrückt werden, sonst gehen alle Änderungen verloren

### Wiedergabe der Inhalte

Die mit diesem Editor erstellten Aufgabenelemente können sowohl in einer Vorschau, als auch im finalen System zur Testdurchführung wiedergegeben werden. Damit die Inhalte dargestellt werden können, bedarf es eines bestimmten Players. Dieser muss zwingend zu diesem Editor passen. Für den **Dan-Editor** muss der **Verona Dan-Player** verwendet werden. Detailierte Informationen zu diesem Player finden Sie im gleichnamigen [Einzeldokument](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Verona-Player-Dan-v3.0).

### IQB Konventionen

Für Interessierte bzgl. der am IQB gesammelten Erfahrungen im Aufgabenentwurf, steht ein Zusatzdokument mit IQB Emfehlungen bereit. Zu finden ist diese Dokument [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/IQB-Konventionen-Aufgabengestaltung).

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
#  Verona Editor PlainText v1.0(Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

> **[Hier](https://github.com/iqb-berlin/verona-editor-plaintext)** der Link zum GitHub Repository.<br>
> **[Hier](https://github.com/iqb-berlin/verona-editor-plaintext/releases)** finden Sie die letzten aktuellen Versionsstände.

:information_source: Zu beachten ist: Das **Studio** und auch der Editor haben noch einmal optische Veränderungen erfahren. Die nachfolgenden Bilder können bzgl. Optik vom aktuellen Stand des Editors und des Studios abweichen. Funktional hat sich aber nichts geändert.

## Erstellung der Aufgabenelemente

 > Vorab: Dieser Editor verwendet eine Scriptsprache zur Erstellung von Elementen. Für die Aufgabengestaltung mit diesem Editor sind also zwingend Kenntnisse bzgl. Aufbau und Struktur dieser Scriptsprache erforderlich.

Bei der Unit-Definition handelt es sich um eine normale Text-Datei. Jede Zeile enthält die Definition eines Eingabeelementes, eines Textes oder eines Elementes zur Strukturierung.

### Grundsätzlicher Aufbau einer Zeile

Jede Zeile enthält als Erstes ein Schlüsselwort und kann dahinter weitere Parameter enthalten, jeweils getrennt mit ::.

* Die erste Zeile MUSS lauten iqb-scripted::1.0.
* Am Ende einer Definitionszeile kann nach ?? noch weiterer Text angefügt werden, der als Hilfe-/Hinweistext verwendet wird (mouse-over).
* Eine leere Zeile erzeugt einen Abstand im Formular in der Höhe eines Text-Elementes.
* Vor dem Schlüsselwort können Leer- oder Tabzeichen eingefügt werden, um die Lesbarkeit des Scriptes zu erhöhen. Sie werden bei der Auswertung ignoriert.

### Statische Texte, Linien, Kommentare

<table>
	<thead>
		<tr>
		<th>Schlüsselwort</th>
		<th>Bedeutung</th>
		<th>Parameter</th>
		</tr>
	</thead>
	<tbody>
		<tr>
		<td><code>title</code></td>
		<td>eine Zeile Text als oberste Gliederungsüberschrift</td>
		<td><I>Text des Titels (optional)</I></td>
		</tr>
		<tr>
		<td><code>header</code></td>
		<td>eine Zeile Text als zweite Gliederungsüberschrift</td>
		<td><I>Text der Überschrift (optional)</I></td>
		</tr>
		<tr>
		<td><code>text</code></td>
		<td>Standard-Text</td>
		<td><I>Text (optional)</I></td>
		</tr>
		<tr>
		<td><code>html</code></td>
		<td>wird genau so in das Formular übernommen; dient der Lösung besonderer Layout-Probleme; Achtung: unsichere Inhalte wie Links werden herausgefiltert</td>
		<td><I>Html-Text (optional)</I></td>
		</tr>
		<tr>
		<td><code>hr</code></td>
		<td>stellt eine horizontale Linie dar</td>
		<td><I>keine</I></td>
		</tr>
		<tr>
		<td><code>rem</code></td>
		<td>leitet einen Kommentar ein, der bei der Verarbeitung ignoriert wird</td>
		<td></td>
		</tr>
	</tbody>
</table>


**Beispiele:**

```
title::na sowas!
html::And now <strong>this text here is bolded</strong>
hr
text::Einfach nur so mal Text, der aber - wenn zu wenig Platz ist - auch mal umgebrochen wird.??Aber nicht vergessen: Ab und zu mit der Maus drüber!
rem::ab hier noch Nummern der Fragen prüfen!!!!!
header::Abschnitt 223
```

### Eingabe von Text oder Zahl

<table>
	<thead>
	<tr>
		<th>Schlüsselwort</th>
		<th>Parameter</th>
		<th>Standardwert</th>
	</tr>
	</thead>
	<tbody>
		<tr>
		<td><code>input-text</code></td>
		<td>1. Name der Variablen, in die die Eingabe gespeichert werden soll</td>
		<td><I>Angabe ist erforderlich</I></td>
		</tr>
		<tr>
		<td></td>
		<td>2. Pflichtfeld: 0=nein, 1=ja</td>
		<td><I>0</I></td>
		</tr>
		<tr>
		<td></td>
		<td>3. Text vor dem Eingabefeld (Eingabeaufforderung)</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>4. Text nach dem Eingabefeld</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>5. Anzahl von Zeilen (>1 bedeutet mehrzeiliges Eingabefeld)</td>
		<td><I>1</I></td>
		</tr>
		<tr>
		<td></td>
		<td>6. maximale Anzahl von Zeichen bei der Eingabe</td>
		<td><I>unbegrenzt</I></td>
		</tr>
		<tr>
		<td><code>input-number</code></td>
		<td>1. Name der Variablen, in die die Eingabe gespeichert werden soll</td>
		<td><I>Angabe ist erforderlich</I></td>
		</tr>
		<tr>
		<td></td>
		<td>2. Pflichtfeld: 0=nein, 1=ja</td>
		<td><I>0</I></td>
		</tr>
		<tr>
		<td></td>
		<td>3. Text vor dem Eingabefeld (Eingabeaufforderung)</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>4. Text nach dem Eingabefeld</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>5. Minimalwert</td>
		<td><I>kein</I></td>
		</tr>
		<tr>
		<td></td>
		<td>6. Maximalwert</td>
		<td><I>kein</I></td>
		</tr>
	</tbody>
</table>
 
  
**Beispiele:**

```
input-number::task12ahmfA::1::Teilaufgabe 1.2a (Analysis)::::0::10
input-text::note::0::Weitere Kommentare zu den Prüfungsaufgaben (optional)::::20??Abschließend haben Sie an dieser Stelle die Möglichkeit, zusätzliche Hinweise und Kommentare zu den Prüfungsaufgaben und Erwartungshorizonten festzuhalten.
input-number::A155f::1::Wieviel wiegt ungefähr eine Kuh?::kg::1::1000

```
  
Mehrzeilige Eingabefelder sind mindestens zwei Zeilen hoch, auch wenn sie leer sind. Bei der Eingabe vergrößert sich dann das Eingabefeld nach Bedarf. Die angegebene Obergrenze gilt nur für die Darstellung, nicht für den Inhalt, d. h. sollte mehr eingegeben werden, als in die angegebenen Zeilen passt, wird ein Scrollbalken eingeblendet und die weitere Eingabe ist nicht blockiert.

Ungültige Eingaben (z. B. Grenze des numerischen Feldes überschritten) erzeugen einen roten Hinweistext. Der eingegebene Wert wird nicht gespeichert.

Bei numerischen Eingaben ist als Dezimaltrennzeichen sowohl ein Komma als auch ein Punkt erlaubt. Bei der Auswertung muss beides vorgesehen werden.

Ein Pflichtfeld ist zunächst nicht hervorgehoben. Erst wenn das Eingabefeld besucht und ohne eine Eingabe verlassen wurde, ist ein roter Hinweistext eingeblendet.
  
### Ankreuzen/Auswählen

Bei einer `checkbox` kreuzt man nur an. Bei `multiple-choice` werden die Optionen untereinander dargestellt und es kann nur eine Option ausgewählt werden. Bei `drop-down` werden die Optionen in eine Klappbox gepackt, was Platz spart.

<table>
	<thead>
	<tr>
		<th>Schlüsselwort</th>
		<th>Parameter</th>
		<th>Standardwert</th>
	</tr>
	</thead>
	<tbody>
		<tr>
		<td><code>checkbox</code></td>
		<td>1. Name der Variablen, in die die Eingabe gespeichert werden soll</td>
		<td><I>Angabe ist erforderlich</I></td>
		</tr>
		<tr>
		<td></td>
		<td>2. Pflichtfeld: 0=nein, 1=ja</td>
		<td><I>0</I></td>
		</tr>
		<tr>
		<td></td>
		<td>Achtung: Pflichtfeld bedeutet hier, dass die Checkbox ausgewählt/angekreuzt sein muss (z. B. Zustimmung zu Datenschutzfragen).</td>
		<td></td>
		</tr>
		<tr>
		<td></td>
		<td>3. Text vor dem Eingabefeld (Eingabeaufforderung)</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>4. Text nach dem Eingabefeld</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>Achtung: Als Wert der Variablen wird 'true' oder 'false' gespeichert. Der Wert der Variable ist im Ausgangszustand immer 'false'.</td>
		<td></td>
		</tr>
		<tr>
		<td><code>multiple-choice</code> oder <code>drop-down</code></td>
		<td>1. Name der Variablen, in die die Eingabe gespeichert werden soll</td>
		<td><I>Angabe ist erforderlich</I></td>
		</tr>
		<tr>
		<td></td>
		<td>2. Pflichtfeld: 0=nein, 1=ja</td>
		<td><I>0</I></td>
		</tr>
		<tr>
		<td></td>
		<td>3. Text vor Optionsliste (Eingabeaufforderung)</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>4. Liste der Optionen, jeweils getrennt durch ##</td>
		<td><I>keine</I></td>
		</tr>
		<tr>
		<td></td>
		<td>Achtung: Als Wert der Variablen wird die Position der gewählten Option gespeichert, beginnend mit 1.</td>
		<td></td>
	</tbody>
</table>

**Beispiele:**

```
checkbox::task162ahmfF::0::Sie fühlen sich beunruhigt
multiple-choice::task3wtrtimeS::1::Ich fühle mich heute großartig::trifft gar nicht zu##trifft eher nicht zu##trifft eher zu##trifft voll zu
drop-down::ta33S::1::Ich fühlte mich gestern großartig::##trifft gar nicht zu##trifft eher nicht zu##trifft eher zu##trifft voll zu

```

### Likert-Skala

Mit dem `likert` Element kann eine Liste von Fragen mit einer einheitlichen Antwortskala definiert werden. Sie funktioniert ähnlich wie eine Liste von exklusiven Checkboxen mit dem Unterschied, dass Antworten-Optionen nur einmal im Tabellenkopf definiert werden müssen. Diese Form ist sehr platzsparend und kann schnell beantwortet werden.

<table>
	<thead>
		<tr>
		<th>Schlüsselwort</th>
		<th>Parameter</th>
		<th>Standardwert</th>
		</tr>
	</thead>
	<tbody>
		<tr>
		<td><code>likert-start</code></td>
		<td>1. Liste der Antwortoptionen jeweils getrennt durch ##</td>
		<td><I>Angabe erforderlich</I></td>
		</tr>
		<tr>
		<td><code>likert</code></td>
		<td>1. Name der Variable, in die die Eingabe gespeichert werden soll 2. (Frage)Text</td>
		<td><I>mindestens eine Angabe erforderlich</I></td>
		</tr>
		<tr>
		<td><code>likert-end</code></td>
		<td>1.keine</td>
		<td><I>Angabe ist erforderlich</I></td>
		</tr>
		<tr>
		<td><code>html</code></td>
		<td>wird genau so in das Formular übernommen; dient der Lösung besonderer Layout-Probleme; Achtung: unsichere Inhalte wie Links werden herausgefiltert</td>
		<td><I>Html-Text (optional)</I></td>
		</tr>
		<tr>
		<td><code>hr</code></td>
		<td>stellt eine horizontale Linie dar</td>
		<td><I>keine</I></td>
		</tr>
		<tr>
		<td><code>rem</code></td>
		<td>leitet einen Kommentar ein, der bei der Verarbeitung ignoriert wird</td>
		<td></td>
		</tr>
	</tbody>
</table>


**Beispiele:**

```
likert-start::sehr hilfreich##eher hilfreich##teilweise hilfreich##eher nicht hilfreich##nicht hilfreich
    likert::task2useA::Abschnitt 1: Einleitung
    likert::task2useB::Abschnitt 2: Starten der Computer
    likert::task2useC::Abschnitt 3: Anmeldung
    likert::task2useD::Abschnitt 4: Steuerung über Testleitungskonsole
    likert::task2useE::Abschnitt 5: Speichern/Beenden
likert-end

```

### Schleifen

`repeat-start` und `repeat-end` markieren einen Block von Elementen, der während der Beantwortung dynamisch mehrfach erzeugt wird. Dazu muss die befragte Person eine Zahl eingeben, die die Anzahl der Wiederholungen steuert. Alle Variablennamen der im Block befindlichen Eingabeelemente erhalten für den jeweiligen Blockdurchlauf einen Suffix: `_ +` laufende Nummer des aktuellen Blockdurchlaufes, beginnend mit `_1`.

Innerhalb des Blocks ist es möglich Ein- und Ausblendungen vorzunehmen (s. u.). Hierbei ist möglich sich auf Variablen innerhalb des Blocks oder Variablen auf höchster Ebene zu beziehen. Bei Verschachtelung mehrerer Schleifen kann man sich nicht auf Variablen anderer Schachtelungsebenen beziehen.

<table>
	<thead>
		<tr>
		<th>Schlüsselwort</th>
		<th>Parameter</th>
		<th>Standardwert</th>
		</tr>
	</thead>
	<tbody>
		<tr>
		<td><code>repeat-start</code></td>
		<td>1. Name der Variablen, in die die Eingabe (Anzahl) gespeichert werden soll</td>
		<td><I>Angabe erforderlich</I></td>
		</tr>
		<tr>
		<td></td>
		<td>2. Text vor dem Eingabefeld (Eingabeaufforderung)</td>
		<td><I>kein Text</I></td>
		</tr>
		<tr>
		<td></td>
		<td>3. Text für die Überschrift zu Beginn jeden Blockes (Blocknummer wird jeweils dynamisch dahinter gesetzt)</td>
		<td>`Block`</td>
		</tr>
		<tr>
		<td></td>
		<td>4. Maximalwert für die Anzahl der Blöcke</td>
		<td><I>10</I></td>
		</tr>
		<tr>
		<td><code>repeat-end</code></td>
		<td>keine</td>
		<td></td>
		</tr>
	</tbody>
</table>


**Beispiel:**

```
rem::Schleife für alle Prüflinge
repeat-start::examineecount::Wie viele Prüflinge gibt es?::Angaben zu Prüfling::20??Sie können Angaben zu maximal 20 Prüflingen eintragen. Sollten sich im Kurs mehr als 20 Prüflinge befinden, ist eine Auswahl vorzunehmen. Diese Auswahl sollte so erfolgen, dass ein möglichst breites Leistungsspektrum abgebildet wird. Vermieden werden sollte eine selektive Berücksichtigung bzw. Nichtberücksichtigung bestimmter Gruppen (z. B. besonders leistungsschwache oder leistungsstarke Prüflinge, Schülerinnen und Schüler mit nichtdeutscher Herkunftssprache).
    input-number::task1::1::Teilaufgabe 1::::0::10
    input-number::task2::1::Teilaufgabe 2::::0::10
    input-number::task3::1::Teilaufgabe 3::::0::10
repeat-end

```

führt z. B. zu folgenden Daten:

```

examineecount;3
task1_1;3
task2_1;4
task3_1;5
task1_2;3
task2_2;1
task3_2;5
task1_3;1
task2_3;4
task3_3;6

```

### Ausblenden/Einblenden

`if-start` und `if-end` markieren einen Block von Elementen, der in Abhängigkeit des Wertes einer Variablen gezeigt oder ausgeblendet wird. Dabei wird der eingegebene Wert mit einem Sollwert verglichen. Mit `if-else` können Elemente ein-/ausgeblendet werden, wenn der Wert **nicht** mit dem Sollwert übereinstimmt.

<table>
	<thead>
		<tr>
		<th>Schlüsselwort</th>
		<th>Parameter</th>
		</tr>
	</thead>
	<tbody>
		<tr>
		<td><code>if-start</code></td>
		<td>1. Name der Variablen, der Wert geprüft werden soll</td>
		</tr>
		<tr>
		<td></td>
		<td>2. Wert</td>
		</tr>
		<tr>
		<td><code>if-else</code></td>
		<td>keine</td>
		</tr>
		<tr>
		<td><code>if-end</code></td>
		<td>keine</td>
		</tr>
	</tbody>
</table>

### Navigation

nav-button-group ermöglicht das Einfügen von Navigationselementen. Art und Reihenfolge können gewählt werden. Mögliche Bedienelemente sind: `next`, `previous`, `first`, `last` und `end`.

<table>
	<thead>
		<tr>
		<th>Schlüsselwort</th>
		<th>Parameter</th>
		</tr>
	</thead>
	<tbody>
		<tr>
		<td><code>nav-button-group</code></td>
		<td>1. Liste der Optionen, jeweils getrennt durch ##</td>
		</tr>
	</tbody>
</table>

**Beispiel:**

```
nav-button-group::previous##next##first##last##end
nav-button-group::next

```

### Wiedergabe der Inhalte

Die mit diesem Editor erstellten Aufgabenelemente können sowohl in einer Vorschau, als auch im finalen System zur Testdurchführung wiedergegeben werden. Damit die Inhalte dargestellt werden können, bedarf es eines bestimmten Players. Dieser muss zwingend zu diesem Editor passen. Für den **PlainText-Editor** muss zwingend der Player **Verona Abi-Player** verwendet werden. Detailierte Informationen zu diesem Player finden Sie im gleichnamigen [Einzeldokument](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Verona-Player-Abi-v3.3).


<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
#  Verona Editor Aspect v1.30 (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

---

<table>
	<tr>
		<td><a href="#Element:Text">Text</a></td>
		<td><a href="#Element:Eingabefeld">Eingabefeld</a></td>
		<td><a href="#Element:Optionsfeld (Bild)">Optionsfeld (Bild)</a></td>
		<td><a href="#Element:Ablegeliste">Ablegeliste</a></td>
		<td><a href="#Element:Bild">Bild</a></td>
		<td><a href="#Element:Audio">Audio</a></td>
		<td><a href="#Element:Video">Video</a></td>
		<td><a href="#Element:Optionstabelle">Optionstabelle</a></td>
		<td><a href="#Element:Lückentext">Lückentext</a></td>
	</tr>
</table>

---

> **[Hier](https://github.com/iqb-berlin/verona-modules-aspect)** ist der Link zum GitHub Repository.

> **[Hier](https://github.com/iqb-berlin/verona-modules-aspect/releases/tag/editor%2F1.21.0%2Bplayer%2F1.15.0)** sind die letzten aktuellen Versionsstände zu finden.

> **[Hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Editor:-Aspect)** sind Videos zu finden.<br>

## <a name="Überblick"></a>Überblick

An dieser Stelle soll ein allgemeiner Überblick bzgl. Aufbau, Bedienung und Funktion des Aspect Editors stattfinden. 

### Aufbau

Der Editor ist wie folgt aufgebaut:

**Mitte:** Seitenansicht mit Abschnitt
* Seitenansicht einer Unit mit den enthaltenen Abschnitten
* auf einer Seite können mehrere Abschnitte angelegt und Elemente darin angeordnet werden
* die Abschnitte können dynamisch oder statisch angelegt werden

**Links:** Aufgabenelemente
* Aufgabenelemente gruppiert nach Funktion

**Rechts:** Eigenschaftenbereich der Elemente
* Aufführung der Eigenschaften eines Elements, aufgeteilt in Gruppen (spez. Parameter des Elements, Positionierung und Dimensionierung, Gestaltung) 
* Grundlegende Funktionen wie Duplizieren und Löschen eines Elements

![Aspect Editor Aufbau](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Aufbau_01.gif)

### Aufteilung einer Unit in Seiten

Units können in Seiten aufgeteilt werden. Jede Unit kann aus einer oder mehreren Seiten bestehen.<br> Der Seitenwechsel innerhalb der Unit kann dann mittels einer Schaltfläche in der Vorschau oder Wiedergabe erfolgen. Für jede Seite können bestimmte Einstellungen vorgenommen werden. Zum einen kann Einfluss auf die Darstellung der Seite genommen werden (Randabstand etc.), zum anderen kann festgelegt werden wie sich die Seite bei der Wiedergabe verhalten soll. Es kann dann bspw. eine Seite immer angezeigt (fixiert) und ihr Anteil auf dem Bildschirm festgelegt werden.

![Aspect Editor Aufbau Seiten](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Seiten_01.png)

### Aufteilung einer Seite in Abschnitte

Wird ein Abschnitt auf einer Seite angelegt muss eine wesentliche Festlegung getroffen werden, wie sich der Abschnitt verhalten soll. Der Editor bietet die Möglichkeit Abschnitte statisch oder dynamisch anzulegen. Ob ein Abschnitt statisch oder dynamisch ist, wird in den Abschnittsoptionen (rotes Menu zum Abschnitt) festgelegt.

Ein Abschnitt ist statisch solange der Haken bei "dynamisch" in den Abschnittsoptionen <u>nicht</u> gesetzt ist. 

#### Statisch

Werden Abschnitte statisch angelegt, sind die Elemente fix mit einem bestimmten Pixelwertes (x, y) im Abschnitt angeordnet. Verändert sich das Endgerät auf dem die Unit angezeigt wird und steht damit bspw. ein kleinerer Monitor zur Verfügung, passen sich die Elemente der neuen Größe nicht an. In einem solchen Fall wird die Unit schnell unübersichtlich und verliert ihren ursprünglich angedachten Gesamteindruck. Benutzer\*innen müssen dann mittels vertikaler und horizontaler Bildlaufleisten in der Unit navigieren.

#### Dynamisch

Wird ein dynamischer Abschnitt angelegt, werden die Elemente nicht mehr fix im Abschnitt angeordnet sondern passen sich immer den gegebenen Bildschirm-/ bzw. Fenstergrößen an.

Da die dynamische Anordnung der Elemente ein entsprechender Algorithmus übernimmt und dieser erst in der eigentlichen Vorschau bzw. während der Wiedergabe der Aufgabe aktiv wird, müssen Benutzer\*innen schon im Vorfeld die Möglichkeit haben, die Anordnung in irgendeiner Weise festzulegen. Damit es möglich ist Elemente bestimmten Bereichen im Abschnitt und somit auf dem Wiedergabebildschirm zuzuweisen, kann in den Eigenschaften eines Elements die Position im Abschnitt festgelegt werden. Auf diese Weise findet eine Unterteilung des Abschnittes in Zeilen und Spalten statt. Um die Gestaltungsmöglichkeiten auf einer Seite offen zu halten, können weitere Abschnitte mit unterschiedlichen Rastern angelegt werden.

![AE_Dynamsich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_dynamisch_01.gif)

Es ist auch möglich teildynamisch zu arbeiten. Die Spaltenbreite und Zeilenhöhe kann auch <u>statische</u> Werte erhalten. Diese Werte können entweder in Bildanteilen oder in Bildpunkten angegeben werden.

![AE_Statisch_Settings](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Settings_dynamisch_02.png)

## <a name="Die Aufgabenelemente"></a>Die Aufgabenelemente

Nach der Auswahl eines Elements, linke Maustaste, wird es im Abschnitt angelegt. Ist der Abschnitt dynamisch, wird das zuerst gewählte Element in der ersten Abschnittszeile angelegt. Kommen weitere Elemente hinzu, werden diese aufsteigend der nächsten Zeile innerhalb des Abschnittes zugeordnet. Die so angelegten Elemente haben noch keine feste Positionszuordnung im Abschnitt. Sie werden erst einmal in eine freie Zeile des Abschnittes gelegt, damit sie dort markiert und deren Eigenschaften verändert werden können. In den Eigenschaften des Elements kann dann die finale Position festgelegt werden. Die Positionierung erfolgt innerhalb eines dynamischen Abschnitts in Zeilen und Spalten. Innerhalb eines statischen Abschnitts erfolgt die Positionierung in X-, und Y-Position.

### Elementen Eigenschaften (Parameter)

:information_source: Zu beachten ist: Das **Studio** und auch der Editor haben noch einmal optische Veränderungen erfahren. Die nachfolgenden Bilder können bzgl. Optik vom aktuellen Stand des Editors und des Studios abweichen. Funktional hat sich aber nichts geändert.

Im Eigenschaftenbereich sind die Eigenschaften eines Elements zu finden. Das Eigenschaftenfenster unterteilt sich in 3 Gruppen oder Reiter (hier gekennzeichnet mit A,B,C). Die nachfolgend beschriebenen Parameter im Eigenschaftenbereich sind diesen 3 Reitern entsprechend zugeordnet.

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Eigenschaften_Tabs_02.gif)

**A** <br>
Hier sind die spezifischen Parameter eines Elements zu finden. Am Bsp. eines Text-Elements könnte hier der enthaltene Text festgelegt und Markierungsoptionen aktiviert werden.

**B** <br>
Hier können Parameter zur Positionierung und Dimensionierung des Elements bedient werden.

**C** <br>
Hier können Einstellungen bzgl. der Gestaltung eines Elements vorgenommen werden, bspw. können hier Hintergrundfarben, Schriftgrößen usw. gesetzt werden.

> **Alle nachfolgend beschriebenen Parameter beginnen immer mit dem Buchstaben des Reiters unter dem  sie zu finden sind (A,B,C).**

> **Da die meisten Parameter selbsterklärend sind, werden wir an dieser Stelle nicht auf jeden Parameter eingehen. Bspw. dürfte klar sein, was der Parameter: *Schriftfarbe* zu bedeuten hat.**

#### Basis-Parameter

Einige Parameter sind in jedem Element zu finden. Bspw. hat jedes Element eine ID und Parameter, die die Position eines Elementes angeben. Diese Parameter werden an dieser Stelle als **Basis-Parameter** beschrieben. Die meisten **Basis-Parameter** sind unter den Reitern **B** und **C** zu finden. Außerdem gibt es **spezifische Parameter** die nur dem entsprechenden Element zur Verfügung stehen. Damit nicht für jedes Element die **Basis-Parameter** beschrieben werden müssen, diese weisen ja immer die selbe Funktionalität auf, soll vorab eine Zusammenstellung und Beschreibung dieser erfolgen. Die **spezifischen Parameter** und deren Funktionen werden dann in den Beschreibungen zu den Elementen gesondert behandelt.

**A:** `ID:` <br>
Jedes Element besitzt eine eindeutige ID. Über diese ID wird das Element identifiziert. Bei der Auswertung können die Antworten so einem Element zugeordnet werden.
Die ID kann individuell angepasst werden. 
> **IDs können nicht doppelt vergeben werden innerhalb einer Unit.**

**A:** `Pflichtfeld:` <br>
Wird dieser Parameter aktiviert, kann bei der späteren Testdurchführung im **Testcenter** die Navigation zur nächsten Aufgabe blockiert werden. Die Navigation ist dann erst möglich, wenn dieses Element bedient wurde. Bspw. gilt ein *Eingabefeld* als bedient, wenn in dieses ein oder mehrere Zeichen eingegeben wurden.

**A:** `Schreibschutz:` <br>
Dieser Parameter ist eigentlich selbsterklärend. Er weist allerdings einige Besonderheiten auf, die an dieser Stelle genannt werden sollten.
 
Wird dieser Parameter aktiviert, werden Eingaben mittels Tastatur nicht angenommen. Auch wenn der Parameter: `Tastatur einblenden` aktiviert ist, wird die virtuelle Tastatur nicht eingeblendet. Einzige Eingabemöglichkeit stellt die Auswahl einer *Eingabehilfe* dar. Ist eine Eingabehilfe aktiviert, wird diese auch bei Schreibschutz eingeblendet und entsprechende Zeichen können in das Feld eingegeben werden. Hintergrund: Auf diese Weise ist es möglich nur bestimmte gewünschte Eingaben für ein Inputfeld zuzulassen. <br>

**A:** `Tastatur einblenden:` <br>
Dieser Parameter wird hauptsächlich für die Nutzung an einem Tablet verwendet. Es kann gewünscht sein, dass Eingaben über die Tablet eigene Tastatur nicht erlaubt sind. Bspw. können die Automatismen bzgl. Groß-/ Kleinschreibung, die auf einer Tablet-Tastatur zum Einsatz kommen können, während einer Deutsch Rechtschreibtestung problematisch sein. Das IQB hat für diesen Zweck eine eigene Tastur programmiert, die an dieser Stelle einmal als IQB-Tastatur bezeichnet werden soll. Ist diese Tastatur aktiv, wird die Tastatur nur an Geräten angezeigt an denen keine "echte" Tastatur erkannt wird. An einem Tablet ohne angeschlossene Tastatur würde somit die Tablet eigene Tastatur unterdrückt und nur die IQB-Tastatur angezeigt werden. Ist an einem Tablet zusätzlich noch eine "echte" Tastatur angeschlossen, wird bei einem Klick in das entsprechende Eingabefeld zuerst die IQB-Tastatur angezeigt. Erfolgt ein Tastendruck auf der "echten" Tastatur, wird diese erkannt und die IQB-Tastatur wird wieder ausgeblendet.

**A:** `Eingabehilfe:` <br>
Es können verschiedene Eingabehilfen aus einer Liste gewählt werden. Wurde eine Eingabehilfe gewählt, wird diese auch bei Elementen mit Schreibschutz eingeblendet.

**B:** `Feste Abmessungen: Mindestbreite:` <br>
Legt die Mindestbreite eines Elements fest. Wird im dynamischen Abschnitt das Wiedergaberfenster oder der Bildschirm verkleinert, verkleinert sich dieses Element nur bis zu diesem festgelegten Wert. Ist das Fenster kleiner als dieser Wert erscheint eine horizontale Bildlaufleiste, über diese kann im Element navigiert werden.

**B:** `Mindesthöhe:` <br>
Gleich wie Mindestbreite, nur bezogen auf die Höhe des Elements.

**B:** `Raster:` <br>
Die hier enthalten Parameter: *Spalte, Zeile, Spalten- und Zeilenspanne* legen fest, in welcher Zeile und Spalte sich das Element befinden soll. Hier kann auch festgelegt werden, ob sich das Element über mehrere Spalten bzw. Zeilen erstrecken soll.

**B:** `Abstand:` <br>
Legt die X-/ Y-Position eines Elements innerhalb einer Zelle (Zeile, Spalte) fest. Auf diese Weise kann ein Element zu benachbarten Elementen positioniert werden.

**B:** `Z-Index:` <br>
Werden Elemente übereinander gestapelt kann mit diesem Index festgelegt werden, an welcher Stelle im Stapel sich das Element befinden soll. 

### <a name="Element:Text"></a>Element: Text

**A:** `Anzahl der Spalten:` <br>
Es ist möglich den im Textelement enthaltenen Text in Spalten anzuordnen. Um den Text sinnvoll einer Spalte zuordnen zu können, müssen an den gewünschten Stellen im Text Zeilenumbrüche vorhanden sein.

![Text:Spalten](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Text_Spalten.gif)

### <a name="Element:Eingabefeld"></a>Element: Eingabefeld

**A:** `Muster:` <br>
Hier können reguläre Ausdrücke eingetragen werden. Mittels dieser kann dann bestimmt werden, welche Eingaben im Eingaberfeld erlaubt sind.

**A:** `Minimallänge:` <br>
Werden weniger Zeichen eingegeben, als hier festgelegt ist, erscheint eine Warnung.

**A:** `Maximalwert:` <br>
Werden mehr Zeichen eingegeben, als hier festgelegt ist, erscheint eine Warnung.

**A:** `Eingabehilfe:` <br>
Siehe Beschreibungen zu den Basis-Parameter.

**A:** `Tastatur einblenden:` <br>
Siehe Beschreibungen zu den Basis-Parameter.

### <a name="Element:Optionsfeld (Bild)"></a>Element: Optionsfeld (Bild)

Dieses Element unterteilt sich noch einmal in "einfach" und "komplex". Ein "einfaches" Optionsfeld bietet die Möglichkeit einzelne Felder anzulegen und anschließend die Ausrichtung (Spalte, Zeile) dieser Felder festzulegen. In "komplexen" Optionsfeldern können die Felder nur in Spalten angeordnet werden. Der jeweiligen Spalte können dann noch zusätzlich Bilder hinzugefügt werden. Nachfolgend wird gezeigt wie ein Bild für ein komplexes Optionsfeld einer Spalte zugeordnet werden kann.

**A:** `Spalten:` *Einstellungen:*

![Optionsfeld komplex Spalteneinstellungen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Optionsfeld_Bild_02.gif)

### <a name="Element:Ablegeliste"></a>Element: Ablegeliste

**Gut zu wissen:** Wie können Bilder eingefügt werden?

**A:** `Vorbelegung:` <br>
In den erweiterten Einstellungen einer Vorbelegung können Bilder hinzugefügt werden.<br>
Zu beachten ist dabei: Eingefügte Bilder überdecken den Text der Vorbelegung, dieser ist dann nicht mehr sichtbar.<br> Auch bei sehr kleinen Bildern wird der Text überdeckt.

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Ablegeliste_Bilder.png)

**A:** `Verbundene Ablegeliste:` <br>
Es ist möglich ein oder mehrere Listen miteinander zu verbinden. Sind Listen miteinander verbunden, können Inhalte via drag-and-drop von einer in die andere Liste bewegt werden. Zur Verbindung muss die ID der jeweiligen Liste eingetragen und anschließend das Pluszeichen betätigt werden.

> Die ID muss in gleicher Schreibweise (auch Groß-/ Kleinschreibung beachten) angegeben werden wie sie im Eigenschaftenbereich der jeweiligen Liste zu finden ist! Es reicht nicht aus die ID hinter das Pluszeichen zu setzen. Das Pluszeichen muss auch betätigt werden damit die ID final übernommen wird.

### <a name="Element:Bild"></a>Element: Bild

**A:** `Skalieren:` <br>
Ist diese Funktion aktiv und ist genügend Platz für ein Bild vorhanden, kann das Bild aufskaliert werden. Es kann dann auch seine ursprüngliche Größe überschreiten. Eventuell leidet darunter aber die Qualität des Bildes.

### <a name="Element:Audio"></a>Element: Audio

Hier ist eine Vielzahl spezifischer Parameter zu finden. Wie bereits erwähnt sind die meisten jedoch selbsterklärend und werden daher an dieser Stelle nicht beschrieben.

**A:** `Symbol Schraubenschlüssel: Verhalten: Abspielbar nach:` <br>
Hier kann ein Audio angegeben werden, welches zuvor abgespielt werden muss. Solange dieses nicht abgespielt wird, ist der Play-Button inaktiv.

**A:** `Symbol Schraubenschlüssel: Verhalten: Minimale Anzahl Durchläufe:` <br>
Hierüber kann festgelegt werden wie oft das Audio mindestens abgespielt werden muss, damit der Player bei der Wiedergabe "Presentation complete" meldet.

### <a name="Element:Video"></a>Element: Video

**A:** `Symbol Schraubenschlüssel: Verhalten: Abspielbar nach:` <br>
Hier kann ein Video angegeben werden, welches zuvor abgespielt werden muss. Solange dieses nicht abgespielt wird, ist der Play-Button inaktiv.

**A:** `Symbol Schraubenschlüssel: Verhalten: Minimale Anzahl Durchläufe:` <br>
Hierüber kann festgelegt werden wie oft das Video mindestens abgespielt werden muss, damit der Player bei der Wiedergabe "Presentation complete" meldet.

### <a name="Element:Optionstabelle"></a>Element: Optionstabelle

**Gut zu wissen:** Ändern der Zeilen-ID und hinzufügen von Bildern:

**A:** `Zeilen:` <br>
In den erweiterten Einstellungen zu den Zeilen (Schraubenschlüsselsymbol) kann die ID der Zeile individuell vergeben werden.
Außerdem können hier auch Bilder hinzugefügt werden.

**A:** `Spalten:` <br>
Bilder können einzelnen Spalten zugewiesen werden. Sollen Bilder eingefügt werden kann dies über die erweiterten Spalteneinstellungen (Schraubenschlüsselsymbol) erfolgen.

**Gut zu wissen:** Ändern der Breite der ersten Spalte:

**A:** `Anteil der ersten Spalte:`
Hier kann das Verhältnis der ersten Spalte in Bildanteilen angegeben werden.

### <a name="Element:Lückentext"></a>Element: Lückentext

**A:** Symbol: Schraubenschlüssel: <br>
Hier wird ein Lückentext erstellt. Die Lücken im Text können mit bestimmten Elementen besetzt werden.
Dazu gehören die folgenden 3:

* Eingabefeld
* Ablegeliste
* Optionsfeld

Diese Elemente können wie gewünscht im Text eingeordnet werden. Dazu werden die Elemente mittels Schaltfläche an gewünschter Stelle im Text positioniert.
Nachdem der Lückentext gespeichert wurde, kann durch Markierung der Elemente im Text auf deren Parameter zugegriffen werden.

> Die so eingefügten Elemente enthalten die gleichen Parameter wie die Einzelelemente: Eingabefeld, Ablegeliste und Optionsfeld.

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Lückentext_Part_01.png)

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Lückentext_Part_02.gif)