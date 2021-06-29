<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Verona Dan Editor v3.1 (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Review (THuste)
Stand: 18.06.2021
todo: - Weiter abgleichen mit Informationen die sich bereits in PbWorks befinden!
      
```

[Hier](https://github.com/iqb-berlin/verona-editor-dan) der Link zum GitHub Repository. Hier sind der aktuelle Versionsstand und weitere Informationen zu finden.

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
2.3 Füge Element ein.Fügt das zwischengespeicherte Element ein.<br>
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

### IQB Konventionen

Für Interessierte bzgl. der am IQB gesammelten Erfahrungen im Aufgabenentwurf, steht ein Zusatzdokument mit IQB Emfehlungen bereit. Zu finden ist diese Dokument [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/IQB-Konventionen-Aufgabengestaltung).


<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
#  Verona Editor PlainText v1.0(Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Review (THuste)
Stand: 18.06.2021
todo: - Weiter mit Leben füllen! Wo finde ich Informationen bzgl. Syntax Scriptsprache???
      
```

[Hier](https://github.com/iqb-berlin/verona-editor-plaintext) der Link zum GitHub Repository. Hier sind der aktuelle Versionsstand und weitere Informationen zu finden.