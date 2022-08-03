# 3 Studio

Das IQB-Studio ist eine Webanwendung für den Entwurf von Kompetenztests oder Befragungen. Nach der Installation auf einem Webserver wählt man diesen Server über seine Adresse an. Dazu wird die Serveradresse in die Adresszeile eines Internet-Browsers eingegeben. Anschließend wird die Webanwendung geladen und es wird ein Formular zur Anmeldung angezeigt.

In themenspezifischen Arbeitsbereichen können dann mithilfe eines intergrierten Editors Aufgaben entworfen und organisiert  werden. Auch eine Vorschau der Aufgaben ist möglich. Nach einem abgeschlossenen Entwurf können die fertigen Aufgaben vom **Studio** in definierten Formaten ausgegeben werden.

Das IQB bietet folgende [Video-Präsentationen](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Teststudio) bzgl. des Studios an:

**Installation**

Das IQB hat alle Programmierungen unter einer Open-Source-Lizenz veröffentlicht und erleichtert die Installation durch Containervirtualisierung (Docker). Für die Installation muss man einen Linux-Server bereitstellen und dieser Server muss dann über eine Internet-Adresse erreichbar sein. Die Installation sollte erfahrenes IT-Fachpersonal durchführen. Die Dokumentation hierzu setzt Wissen vor allem zur Virtualisierungssoftware Docker voraus. Es ist weiterhin Wissen bzgl. Datensicherheit nötig, denn sobald ein Server öffentlich verfügbar ist, müssen Maßnahmen gegen Angriffe durch Schadsoftware ergriffen werden. Das IQB ist bemüht, die Installationspakete gut abzusichern, übernimmt aber im Schadensfall keine Verantwortung.

**Organisation**

Um Autoren die Möglichkeit zu bieten an Aufgabenentwürfen zu arbeiten, ist eine Aufteilung bzw. Organisation in Bereichsgruppen und Arbeitsbereiche sinnvoll. Die Aufgabenentwürfe (Units) werden dann in den Arbeitsbereichen organisiert. Im Sinne einer besseren Übersichtlichkeit können auch die Aufgaben in einem Arbeitsbereich themenspezifisch gruppiert werden. Zugriffsrechte regeln den Zugriff auf diese Bereiche. So können Personen nur Bereiche sehen, die von der IT, also den Administrator\*innen, für diese Personen freigegeben wurden.
Bsph. können dann nur alle zum Team Englisch gehörenden Autor\*innen die Bereichsgruppe des Fachbereichs Englisch sehen.

**Rechte**

Jeder Zugriff auf das **Studio** kann mit bestimmten Rechten ausgestattet werden. Hiermit kann sichergestellt werden, dass nur festgelegte Personengruppen auf bestimmte Bereiche zugreifen können.

**Ausblick**

In zukünftigen Versionen wird auch eine entsprechende Kodierung der entworfenen Aufgaben mithilfe des **Studios** möglich sein. Somit wird dann Entwurf und Kodierung in einer Anwendung stattfinden und es bedarf keiner weiteren Zwischenschritte oder Hilfsmitteln mehr.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Organisation-und-Zugriffsrechte">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 3.1 Organisation

Die Organisation findet in **Bereichsgruppen** und **Arbeitsbereichen** statt. **Arbeitsbereiche** werden dabei immer einer **Bereichsgruppe** zugeordnet. Innerhalb der **Arbeitsbereiche** können dann die eigentlichen **Aufgaben**, auch genannt **Units**, entworfen und organisiert werden. Nachfolgend ist diese Struktur noch einmal verdeutlicht dargestellt. 

![Studio:Bereiche theoretisch](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Bereiche_theoretisch_04.png)

Im **Studio** sieht die Übersicht dann wie nachfolgend dargestellt anhand eines Beispiels aus. Mit einem Klick auf den jeweiligen Arbeitsbereich öffnet sich dieser und die enthaltenen Aufgaben (Units) sind in Gruppen sortiert zu sehen.

![Studio:Bereiche praktisch](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Bereiche_praktisch_04.png)

Im nächsten Bild ist einmal bsph. der Arbeitsbereich "Hören und verstehen" in der Bereichsgruppe "Deutsch" mit den enthaltenen Aufgaben (Units) zu sehen. In diesem Arbeitsbereich befinden sich 2 Gruppen mit den Namen "Templates" und "Vorlagen". Außerdem ist die Aufteilung eines Arbeitsbereichs einmal dargestellt und näher beschrieben.

:information_source:> **Die Benennung der Arbeitsbereiche richtet sich günstigerweise nach dem Zweck dieses Arbeitsbereichs. So könnte bspw. eine Aufteilung in unterschiedliche Fachbereiche sinnvoll sein.**

![Studio:Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Arbeitsbereich.png)

* rot markiert:<br>
	Hier können Units gelöscht, neu erzeugt, exportiert/importiert, kopiert und verschoben werden.

* grün markiert:<br>
	Hier können die Eigenschaften einer Unit verändert, neue Aufgabenelemente mittels Editor erzeugt und Aufgaben in einer Vorschau dargestellt werden. In späteren Versionen des **Studios** kann hier auch die Kodierung der Aufgabenelemente vorgenommen werden.

Folgende Funktionen stehen in der Unit Organisation zur Verfügung:

![Studio:Unit_Funktionen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Unit_Funktionen.png)

* Import von Datei(en)
 * jjjjj




Hat eine Person Zugriff auf eine Bereichsgruppe (siehe Zugriffsrechte) kann diese Person Arbeitsbereiche innerhalb dieser Bereichsgruppe anlegen und kann in der Anwendung gelisteten Personen Zugriff darauf geben. So kann eine verantwortliche Person den Zugriff der zuvor bestimmten Teammitglieder auf relevante Arbeitsbereiche und die darin enthaltenen Aufgaben regeln. So können sich Teams unabhängig von den Systemadministrator\*innen innerhalb ihrer Bereichsgruppe selber  organisieren. 

Jede in der Anwendung hinterlegte Person kann nach Anmeldung am **Studio** personenspezifische Daten, wie bspw. eine E-Mailadresse angeben. Die Person kann dann im Weiteren festlegen, ob diese Informationen für andere ersichtlich sind oder nicht. Außerdem können zu jeder angelegten Aufgabe Kommentare hinterlegt werden. Dies ermöglicht Teammitgliedern auf unterschiedlichen Wegen miteinander in Kontakt zu treten.

Nachfolgend ist zu erfahren, wie der Zugriff auf Bereichsgruppen und Arbeitsbereiche geregelt ist.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Unit-Organisation">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3-Studio">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---


## 3.2 Zugriffsrechte

Die Zugriffsrechte sind über zwei Anmeldetypen geregelt. Zum einen den sogenannten **SuperAdmin** und zum anderen den **WorkspaceAdmin**. Der **SuperAdmin** kann, wie der Name vielleicht schon andeutet, so ziemlich alles im **Studio** freigeben. Er kann Personen anlegen und grundlegende Zugriffsrechte auf Bereichsgruppen und Arbeitsbereiche vergeben. Alle Personen, die vom **SuperAdmin** hinterlegt wurden und nicht als **SuperAdmin** angelegt wurden, sind automatisch **WorkspaceAdmins**. Diese können dann Arbeitsbereiche innerhalb einer Bereichsgruppe für andere Personen freigeben und spezifische Einstellungen an den Arbeitsbereichen vornehmen.

**Was kann der SuperAdmin?**

Über die folgenden Schaltflächen kann der **SuperAdmin** die aufgelisteten Tätigkeiten vornehmen:

![Studio:SuperAdmin](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_SuperAdmin_02.png)

* Personen anlegen, bearbeiten und löschen
* Bereichsgruppen anlegen, bearbeiten und bestimmten Personen Zugriff darauf geben
* Arbeitsbereiche in den Bereichsgruppen anlegen, bearbeiten und Personen Zugriff darauf geben
* spezifische Änderungen an der Anwendung **Studio** vornehmen, bspw. Texte, Farben und Logos der Anwendung ändern
* Module eines Players und Editors in die Anwendung laden und somit dem Aufgabenentwurf zur Verfügung stellen
* außerdem alles was der WorkspaceAdmin auch kann

**Was kann der WorkspaceAdmin?**

![Studio:WorkspaceAdmin](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_WorkspaceAdmin.png)

* Änderungen an der für den angemeldeten WorkspaceAdmin freigegebenen Bereichsgruppen vornehmen
* Arbeitsbereiche anlegen und Einstellungen des Arbeitsbereichs bearbeiten
* Aufgaben innerhalb eines Arbeitsbereichs organisieren (exportieren, kopieren, importieren usw.)
* Personen für bestimmte Arbeitsbereiche freigeben

Nach der Erstinstallation durch die IT, ist in der Anwendung ein **SuperAdmin** angelegt. Mit diesem können dann weitere Personen angelegt und deren Zugriffrechte (WorkspaceAdmin oder SuperAdmin) gesetzt werden. Im Vorfeld sollte festgelegt werden, wer welche Rechte erhält. Sollen bspw. weitere Personen hinzukommen, kann es ungünstig sein, wenn immer erst die IT benachrichtigt werden muss. Besser ist es dann vielleicht jemanden aus dem eigenen Team mit entsprechenden **SuperAdmin**-Rechten auszustatten.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Unit-Organisation">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3-Studio">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 3.3 Unit Organisation


Ein geöffneter Arbeitsbereich teilt sich in zwei Fenster auf:

![iqb online assessment applications with relations: Teststudio Funktionen Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Aufteilung_Arbeitsbereich_final.png)


In den nachfolgenden Kapiteln wird detailiert auf diese Aufteilung eingegangen.


> **Die Unit Organisation erfolgt im rot markierten Fenster des Arbeitsbereiches. Siehe Bild im Kapitel: 3 Teststudio.**

In diesem Bereich können Units verwaltet bzw. organisiert werden. Nachdem eine Unit markiert wurde, kann diese über die unten angeordneten Funktionschaltflächen gelöscht, exportiert, verschoben oder deren Eigenschaften verändert werden. Das kleine Pluszeichen legt eine neue Unit an. Oberhalb der Unit Auflistung im linken Bereich des Portals befinden sich zwei weitere Funktionsschaltflächen. Diese ermöglichen das Speichern bzw. Verwerfen von Änderungen an einer gewählten Unit.

![iqb online assessment applications with relations: Teststudio Funktionen Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Funktionen_Arbeitsbereich_final.png)

**Unit verschieben**

Es ist möglich Units zu verschieben. Verschoben kann dabei nur in andere für die angemeldete Person freigegebene Arbeitsbereiche.

**Unit kopieren**

Markierte Units können kopiert werden. Alle Inhalte dieser Unit werden dabei in eine neu zu benennende Unit kopiert.

**Unit importieren**

Der Import von bestehenden Units ist ebenso möglich. Besteht die zu importierende Unit aus einer XML-/ und einer VOUD-Datei, sollten diese zuvor in einem Zip-Format gepackt werden. Anschließend kann die Zip-Datei ausgewählt und importiert werden. Der gewählte Name der Zip-Datei spielt dabei keine Rolle, sollte aber einer gewissen Logik folgen um den Überblick zu behalten.

> **VOUD-Dateien können nicht einzeln importiert werden. Sie müssen immer zusammen mit der zugehörigen XML-Datei (`Unit.xml`) importiert werden. Daher sollten diese Dateien zuvor immer in einem Zip-Format verpackt und dann importiert werden!**

**Unit exportieren**

Werden Units exportiert, verpackt das **Teststudio** die zu dieser Unit gehörenden Dateien in einer Zip-Datei. Eine Unit besteht dabei aus einer XML-Datei und einer VOUD-Datei. Die Zip-Datei wird automatisch wie folgt benannt:<br> **aktuelles Datum***UnitDefs.voud.zip*. Es ist auch möglich eine passende `Testtakers.xml` und `Booklet.xml` mit ausgeben zu lassen. In der `Booklet.xml` sind dann bspw. alle zum Paket gehörenden Units bereits eingebunden. Um diese Dateien zu erzeugen, muss im Exportfenster der Haken bei "Als Paket für Testcenter" gesetzt werden.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Unit-Bearbeitung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Allgemeine-Organisation-und-Zugriffsrechte">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 3.3 Unit Bearbeitung

Die Unit Organisation erfolgt im grün markierten Fenster des Arbeitsbereich. Siehe Bild im Kapitel: 3 Teststudio.

![iqb online assessment applications with relations: Teststudio Funktionen Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Unit_bearbeiten_fina.png)

### Tab Eigenschaften

Unter den Eigenschaften einer Unit werden einerseits Metadaten, wie Namen und Beschreibung festgelegt und andererseits werden der zu verwendende Editor und der zugehörige Player bestimmt.

**Kurzname**

Eindeutiger (ID-fähiger )und schlüssiger Kurzname der Unit. Dieser sollte keine Leerzeichen oder Unterstriche enthalten. Über diesen Namen wird die Aufgabe im Testheft identifiziert.

**Name**

Dieser Name wird im **Testcenter** beim Abspielen dieser Aufgabe angezeigt. Dieser Name kann aber auch nachträglich noch geändert werden.

**Editor**
	
Für die Aufgabengestaltung können je nach Bedarf unterschiedliche Editoren genutzt werden. Diese unterscheiden sich hinsichtlich Funktionalität und Ausstattung. Prinzipiell kann man die angebotenen Editoren in zwei Gruppen einteilen:

* grafischer Entwurf
	* Alle für den Entwurf benötigten Elemente einer Aufgabe (Textfelder, Grafiken, Multiple-Choice-Felder etc.) stehen über ein Menu symbolisch zur Verfügung und können mittels drag-and-drop in der Aufgabe positioniert werden. Die Eigenschaften der Elemente können über entsprechende Menus verändert werden.
	
* textueller Entwurf
	* Alle für den Entwurf benötigten Elemente einer Aufgabe können über eine Scriptsprache erstellt werden. Es gibt keine vorgefertigten Elemente, alle Eigenschaften werden rein textuell beschrieben. Kenntnisse bzlg. Syntax der Scriptsprache sind zwingend erforderlich.

Welcher Editor gewählt wird, orientiert sich an den Anforderungen an die Aufgabe, sprich welche Aufgabenelemente müssen enthalten sein und welcher Editor stellt diese Elemente bereit. Können mehrere Editoren die erforderlichen Elemente liefern, ist die Entscheidung für einen Editor allein von der gewünschten Entwurfsmethode (rein grafischer oder rein textueller Entwurf) abhängig. Die Auswahl des Editors erfolgt dann im rechten Teil der Eigenschaftsbearbeitung.

> Mehr zur Arbeit mit dem Editor entnehmen Sie bitte dem Kapitel **Editor**

**Player**

Damit eine entworfene Aufgabe sowohl in der Vorschau, als auch später im Testcenter abgespielt werden kann, wird ein Player benötigt. Dieser ist in die jeweilige Webanwendung integriert und gibt die Aufgabe mit all ihren Elementen wieder. Der Player muss dabei zwingend zum Editor passen mit dem die Aufgabe entworfen wurde. Wurde eine Aufgabe bspw. mit einem Script Editor entworfen, muss auch ein Script Player verwendet werden.

> Mehr zum Thema Player entnehmen Sie bitte dem Kapitel **Player.**

### Tab Editor

> Detailierte Informationen zur Arbeit mit den Editoren finden Sie im Kapitel **Editor.**

### Tab Vorschau

Während der Erstellung einer Aufgabe kann die Aufgabe ohne Speicherung aktueller Änderungen in der Voransicht begutachtet werden.

> **Um die Aufgabe auch in der Vorschau korrekt darstellen zu können, müssen in den Eigenschaften gewählter Editor und Player zueinander passen!**

Nachfolgendes Bild zeigt die Voransicht und deren Bestandteile:

![iqb online assessment applications with relations: Teststudio Funktionen Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Editor_Voransicht_final.png)

Beschreibung des grün markierten Bereiches:<br>

**P:** zeigt die Vollständigkeit der Präsentation/Anzeige an, d. h. es wird angezeigt, ob alle Audios abgespielt wurden und/oder ob alle Viewpoints (unsichtbar) angezeigt wurden (d. h. ob gescrollt und alle Textteile, Items etc. gesehen wurden): grün = ja, vollständig; rot = nein, unvollständig;<br>
**R:** zeigt die Vollständigkeit der Reaktionen an, d. h. es wird angezeigt, ob alle Input-Felder/Anklick-Optionen bedient wurden: grün = ja, alle; gelb = ja, teilweise; rot = nein, keine.<br>
**F:** zeigt an, ob sich der Fokus noch im aktuellen Fenster befindet. Dient der Kontrolle bei der späteren Testdurchführung, ob sich die Testperson immer noch im Fenster der Testdurchführung befindet oder ob diese das Testfenster verlassen hat und stattdessen ein anderes Fenter geöffnet hat (andere Website etc.)

### Anlegen einer Unit

Nach Auswahl und öffnen des gewünschten Arbeitsbereichs kann mithilfe der Plus-Schaltfläche im linken Teil des Arbeitsbereichs (rot markiert) eine neue Unit angelegt werden. Nach Anlage sollten die Eigenschaften hinsichtlich Namensgebung, Auswahl des Editors und Players im rechten Fenster erfolgen. Anschließend können die Editierfunktionen geöffnet werden mittels Klick auf den Tab: Editor. Die gewünschte Aufgabenelemente können dann auf den Seiten einer Unit platziert werden und deren Eigenschaften angepasst werden.

#### Unit Bezeichner

Jedes Aufgabenelement, sei es ein Textfeld, ein Button etc., erhält einen eindeutigen Bezeichner. Dieser setzt sich wie folgt zusammen: *canvasElement* + *fortlaufende Nummer*

Das erste Element einer Unitseite erhält somit den Bezeichner canvasElement1. Der Bezeichner eines Elements ist auch immer im Eigenschaftenfenster des Elementes ersichtlich. Dieser Bezeichner muss einer im Sinne der Auswertung relevanten Aufgabe zugeordnet werden, bspw: Aufgabe 1a = canvasElement9. Es sollten also während der Aufgabenerstellung immer parallel eine Liste geführt werden, die diese Zuordnung aufzeigen.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.4-Editor">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Unit-Organisation">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 3.4 Editor

Zum Zeitpunkt der Erstellung dieser Dokumentation stehen die drei folgenden Editoren zur Verfügung:<br>

**Verona Editor Plain Text**<br>
Aufgaben können mittels einer Scriptsprache (deshalb auch der Name "...Plain Text..") erstellt werden. Es stehen keine grafischen Elemente zur Erstellung eines Textfeldes, Schaltflächen oder anderen Elementen zur Verfügung. Die Erzeugung solcher Elemente wird rein textuell realisiert. Auch die Beschreibung der Eigenschaften eines Elementes erfolgt auf diese Weise.

Detailierte Informationen zum Plain Text Editor finden Sie in dem gleichnamigen [Einzeldokument](Verona-Editor-Plaintext-v1.0).
	
**Verona Editor Dan**<br>
Komplexe Aufgaben können mittels Auswahl von vorgefertigten Elementen erstellt werden. Die bereitgestellten Elemente können dabei einfach mittels Drag-and-Drop der Aufgabe hinzugefügt werden. Anschließend können diese Elemente in ihren Eigenschaften verändert werden. Es können dann bspw. Größe, Farbe, Position und weitere Eigenschaften der Elemente über entsprechende Toolboxen verändert werden. 

Detailierte Informationen zum **Dan-Editor** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Editor-Dan-v3.1).

**Verona Aspect Editor**<br>
Komplexe Aufgaben können mittels Auswahl von vorgefertigten Elementen erstellt werden. Die bereitgestellten Elemente können dabei einfach mittels Drag-and-Drop der Aufgabe hinzugefügt werden. Anschließend können diese Elemente in ihren Eigenschaften verändert werden. Es können dann bspw. Größe, Farbe, Position und weitere Eigenschaften der Elemente über entsprechende Toolboxen verändert werden. Bzgl. Responsivität ist es auch möglich dynamische Felder zu erzeugen und Elemente in diesen anzuordnen. Die angelegten Elemente skalieren sich dann automatisch und passen sich an veränderte Fenstergrößen oder wechselnde Bildschirme an.

Detailierte Informationen zum **Aspect-Editor** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Editor-Aspect-v1.21).

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.5-Player-Vorschau-(Verona)">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Unit-Bearbeitung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 3.5 Player Vorschau (Verona)

Damit die Aufgabe in der Vorschau wiedergegeben werden kann, muss der zum Editor passende Player gewählt werden. Eine Aufgabe die bspw. mit dem **PlainText-Editor** erstellt wurde, kann nicht von einem **Dan-Player** wiedergegeben werden, da ihm schlicht die enthaltenen Elemente nicht bekannt sind. Zum Zeitpunkt der Erstellung dieser Dokumentation stehen die zwei folgenden Player zur Verfügung:<br>
	
**Verona Player Dan**<br>
Dieser Player kann Aufgaben wiedergeben, deren Erstellung mittels **Dan-Editor** erfolgte.<br>
Detailierte Informationen zum **Dan-Player** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Player-Dan-v3.0).
	
**Verona Player Abi**<br>
Dieser Player kann Aufgaben wiedergeben, deren Erstellung mittels **PlainText-Editor** erfolgte.<br>
Detailierte Informationen zum **Abi-Player** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Player-Abi-v3.3).

**Verona Player Aspect**<br>
Dieser Player kann Aufgaben wiedergeben, deren Erstellung mittels **Aspect-Editor** erfolgte.<br>
Detailierte Informationen zum **Aspect-Player** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Player-Aspect-v1.15).

---
<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.6-Portal-zur-Verwaltung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.4-Editor">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 3.6 Portal zur Verwaltung

## Arbeitsbereich

Damit mehrere Studien gleichzeitig im Teststudio bearbeitet bzw. vorbereitet werden können, sind sog. Arbeitsbereiche vorbereitet. Die Benennung richtet sich günstigerweise nach dem Zweck, also z. B. "Demo Deutsch Sek1" oder "Review Abi" oder "VERA Englisch". Für jedes Verwaltungskonto ist festgelegt, welche Arbeitsbereiche eingesehen (Nur-Lese-Modus) bzw. geändert werden können (Lesen-Und-Schreiben-Modus). Um die Übersichtlichkeit zu erhöhen, sind die Bereiche Gruppen zugeordnet. So gehören dann bspw. alle Arbeitsbereiche zum Thema Mathematik zur Gruppe Mathematik usw..

Nach der Anmeldung präsentiert das System eine Liste aller Arbeitsbereiche, die für diese Person freigegeben sind. Mit einem Klick auf den jeweiligen Arbeitsbereich wird dieser geöffnet. Zur Liste der Arbeitsbereiche kehrt man zurück, indem man auf das IQB-Logo links oben in der Ecke klickt.

In diesen Bereichen können dann Aufgaben angelegt, importiert oder bereits bestehende Aufgaben bearbeitet werden.

Die Vergabe von Zugriffsberechtigungen auf Bereiche und die Zuordnung von Bereichen zu bestimmten Personen, erfolgt durch den **SuperAdmin**.

## System-Admin (Super-Admin)

Wurden Ihnen Rechte für die Verwaltung des Gesamtsystems zugewiesen (sog. **Super-Admin**), wird zusätzlich zur Liste der Arbeitsbereiche ein System-Admin-Schalter eingeblendet. Über diesen Schalter gelangen Sie zur Systemverwaltung. Dort können Nutzerkonten (Benutzername und Kennwort) und Arbeitsbereiche angelegt werden. Auch der Zugriff auf diese Arbeitsbereiche kann für die jeweiligen Personenkreise festgelegt und grundsätzliche Systemeinstellungen (Hintergrundfarbe, Logo) vorgenommen werden.

Der System-Admin-Bereich wird in **4 Reiter** unterteilt:

* **Nutzer:**<br>
Hier können bestehende Benutzer\*innen verwaltet werden. Es können mittels Pluszeichen-Schaltfläche neue Benutzer\*innen hinzugefügt werden oder mit der Löschen-Schaltfläche gelöscht werden. Weiterhin stehen zwei Schaltflächen zur Änderungen von Kennwort und Zugriffebene bereit. Diese beide Schaltflächen sind mit einem Stift-Symbol gekennzeichnet. Ist eine Person als Super-Adminn angelegt, wird diese mit einem Stern gekennzeichnet. Wird in der Liste der angelegten Personen eine Person markiert, werden auf der rechten Seite alle Arbeitsbereiche angezeigt, auf die diese Person Zugriff hat. Die Berechtigung für einen Arbeitsbereich sind dabei noch einmal unterteilt in "read only" (RO) und "read and write" (RW).

* **Arbeitsbereiche:**<br>
Hier werden alle angelegten Bereiche aufgelistet. Es können neue Bereiche angelegt, gelöscht oder nachträglich bearbeitet werden. Durch Markierung eines Bereichs werden rechts alle Personen aufgelistet, die auf diesen Bereich Zugriff haben. Dabei wird noch einmal unterschieden, ob die Personen nur lesend (RO) oder lesend und schreibend (RW) auf den Bereich zugreifen darf. Sollen Personen einen Zugriff auf einen Bereich erhalten, ist der jeweilige Bereich zu markieren und die Person mit RO- oder RW-Zugriff auszuwählen. Anschließend muss zwingend das Speicher-Symbol oben rechts aktiviert werden, ansonsten werden die Änderungen nicht gespeichert.

* **Editor/Player:**<br>
Hier können neue Editor-bzw. Playerversionen geladen werden. Diese neuen Versionen können dann bei Benutzung des Editors angewählt werden. Die aktuellen Versionen sind in den entsprechenden GitHub-Repositories zu finden.

* **Einstellungen:**<br>
Hier können einige Bereiche des Teststudios an individuelle Bedürfnisse angepasst werden. Es ist bspw. möglich Texte der Anwendung anzupassen. Es ist auch möglich neue Gruppen für die Arbeitsbereiche anzulegen bzw. bestehende Gruppen zu löschen.

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.5-Player-Vorschau-(Verona)">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---
