<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Verona Dan Editor v3.1 (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

> **[Hier](https://github.com/iqb-berlin/verona-editor-dan)** der Link zum GitHub Repository.<br>
> **[Hier](https://github.com/iqb-berlin/verona-editor-dan/releases)** finden Sie die letzten aktuellen Versionsstände.

Die folgenden Videos werden direkt zum **Dan-Editor** angeboten:

* [Schulung Teststudio Editor Dan2](https://box.hu-berlin.de/f/edc2409b79954dc3b3a1/)  

Die folgenden Videos beschäftigen sich vorwiegend mit dem Aufgabenentwurf, aber auch hier werden Aufgaben mit den **Dan-Editor** erzeugt:

* [Aufgabenentwurf mit dem Teststudio](https://moodle.hu-berlin.de/course/view.php?id=107279)
  
### Übersicht

Der Editor wird über den Tab: **Editor** im Bereich der Unitbearbeitung geöffnet. Nachfolgend wird dann die Editoransicht angezeigt:

![iqb online assessment applications with relations: Teststudio Editieransicht](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Editoransicht_final.png)

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

![iqb online assessment applications with relations: Teststudio Elemente](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Elemente_Eigenschaften_final.png)

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

````

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
#  Verona Editor Aspect (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Entwurf(THuste)
Stand: 11.01.2022
todo: 
```
> **[Hier](https://github.com/iqb-berlin/verona-modules-aspect)** ist der Link zum GitHub Repository.<br>
> **[Hier](https://github.com/iqb-berlin/verona-modules-aspect/releases/tag/editor%2F1.21.0%2Bplayer%2F1.15.0)** sind die letzten aktuellen Versionsstände zu finden.

Einführende Videos zum Aspect Editor sind [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/SCHULUNGSVIDEOS) zu finden.

## Überblick

Hier soll ein grundlegender Überblick über den Editor verschafft werden.

### Aufbau

Der Editor ist wie folgt aufgebaut:

**Mitte:** Leinwand, auch genannt Abschnitt
* hier erfolgt die Anordnung der Aufgabenelemente, auch genannt Items
* die Anordnung kann dabei dynamisch oder auch statisch erfolgen

**Links:** Elemente oder auch Items
* Auswahl aller von diesem Editor zur Verfügung gestellten Items
* Aufteilung der Items nach Funktionalität oder auch Einsatzhäufigkeit
Tab 1 beinhaltet Standardelemente die häufig zu Einsatz kommen und Tab 2 enthält Elemente die etwas spezieller sind und weniger häufig zur Anwendung kommen

**Rechts:** Eigenschaften/ Einstellungen zu den Items
* Aufführung der Item-Parameter, aufgeteilt in Funktionen (Verhalten, Positionierung Layout) 
* Grundlegende Funktionen wie Duplizieren und Löschen eines Items

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Aufbau_05.gif)


### Dynamisch vs statisch

Dieser Editor bietet die Möglichkeit Aufgaben statisch oder dynamisch anzulegen. 

Worin besteht der Unterschied?

Werden Aufgaben statisch angelegt, sind die Items dieser Aufgabe fix mit einem bestimmten Pixelwertes (x, y) auf der Leinwand bzw. Abschnitt angeordnet. Verändert sich das Endgerät auf dem die Aufgabe angezeigt wird und steht damit bspw. ein kleinerer Monitor zur Verfügung, passen sich die Items der neuen Größe nicht an. In einem solchen Fall wird die Aufgabe schnell unübersichtlich und verliert ihren ursprünglich angedachten Gesamteindruck. Benutzer\*innen müssen dann mittels vertikaler und horizontaler Schieber in der Aufgabe navigieren.
Werden hingehen dynamische Abschnitte ausgewählt, werden die Items nicht mehr fix im Abschnitt angeordnet, sondern passen sich immer den gegebenen Bildschirm-/ und Fenstergrößen an. 

Ob der Abschnitt statisch oder dynamisch sein soll, wird in den Abschnittsoptionen festgelegt (siehe Bild Grid Layout).

### Grid Layout

Wird ein dynamischer Abschnitt angelegt, kann dieser in Zeilen und Spalten aufgeteilt werden.
Das wird dann auch Grid Layout genannt.

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_dynamisch_03.gif)

In den so entstandenen Zellen können anschließend Items positioniert werden.

Wozu wird das Grid Layout verwendet?

Da die dynamische Anordnung der Items ein entsprechender Algorithmus übernimmt und dieser erst in der eigentlichen Vorschau bzw. während der Wiedergabe der Aufgabe aktiv wird, müssen Benutzer\*innen schon im Vorfeld die Möglichkeit haben die Anordnung in irgendeiner Weise festzulegen. Damit es möglich ist Items bestimmten Bereichen im Abschnitt und somit auf dem Bildschirm zuzuweisen, wird das Grid Layout verwendet.

### Aufteilung einer Aufgabe

Aufgaben, auch genannt Units, können in Seiten aufgeteilt werden. Jede Unit kann aus 1 oder mehreren Seiten bestehen.<br> Der Seitenwechsel innerhalb der Unit kann dann mittels einer Schaltfläche in der Vorschau oder Wiedergabe erfolgen. Für jede Seite können bestimmte Einstellungen vorgenommen werden. Zum einen kann Einfluss auf die Darstellung der Seite genommen werden (Randabstand etc.), zum anderen kann festgelegt werden, wie sich die Seite bei der Wiedergabe verhalten soll. Es kann dann bspw. eine Seite immer angezeigt (fixiert) und ihr Anteil auf dem Bildschirm festgelegt werden. 

![iqb online assessment applications: workflow](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/AE_Seiten.gif)
