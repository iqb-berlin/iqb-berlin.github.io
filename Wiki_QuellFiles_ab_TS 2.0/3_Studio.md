# 3 Studio

:information_source: **Es gibt eine ältere Version des Studios mit dem Namen **Teststudio**. Nach und nach wird diese Version aber ersetzt durch die aktuelle Version **Studio**. Da sich sowohl Aussehen, als auch Funktionsumfang geändert haben, finden Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Dokumentation-zur-%C3%A4lteren-Version:-Teststudio) zur Dokumentation der älteren Version **Teststudio**.**

Das IQB-Studio ist eine Webanwendung für den Entwurf von Kompetenztests oder Befragungen. Nach der Installation auf einem Webserver wählt man diesen Server über seine Adresse an. Dazu wird die Serveradresse in die Adresszeile eines Internet-Browsers eingegeben. Anschließend wird die Webanwendung geladen und es wird ein Formular zur Anmeldung angezeigt.

In themenspezifischen Arbeitsbereichen können dann mithilfe eines intergrierten Editors Aufgaben entworfen und organisiert  werden. Auch eine Vorschau der Aufgaben ist möglich. Nach einem abgeschlossenen Entwurf können die fertigen Aufgaben vom **Studio** in definierten Formaten ausgegeben werden.

Das IQB bietet folgende [Video-Präsentationen](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Studio) bzgl. des Studios an:

**Installation**

Das IQB hat alle Programmierungen unter einer Open-Source-Lizenz veröffentlicht und erleichtert die Installation durch Containervirtualisierung (Docker). Für die Installation muss man einen Linux-Server bereitstellen und dieser Server muss dann über eine Internet-Adresse erreichbar sein. Die Installation sollte erfahrenes IT-Fachpersonal durchführen. Die Dokumentation hierzu setzt Wissen vor allem zur Virtualisierungssoftware Docker voraus. Es ist weiterhin Wissen bzgl. Datensicherheit nötig, denn sobald ein Server öffentlich verfügbar ist, müssen Maßnahmen gegen Angriffe durch Schadsoftware ergriffen werden. Das IQB ist bemüht, die Installationspakete gut abzusichern, übernimmt aber im Schadensfall keine Verantwortung.

**Ausblick**

In zukünftigen Versionen wird auch eine entsprechende Kodierung der entworfenen Aufgaben mithilfe des **Studios** möglich sein. Somit wird dann Entwurf und Kodierung in einer Anwendung stattfinden und es bedarf keiner weiteren Zwischenschritte oder Hilfsmittel mehr.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Verwaltung-und-Organisation">
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

## 3.1 Verwaltung und Organisation

### Bereichsgruppen und Arbeitsbereiche

Die Organisation findet in **Bereichsgruppen** und **Arbeitsbereichen** statt. **Arbeitsbereiche** werden dabei immer einer **Bereichsgruppe** zugeordnet. Innerhalb der **Arbeitsbereiche** können dann die eigentlichen **Aufgaben**, auch genannt **Units**, entworfen und organisiert werden. Nachfolgend ist diese Struktur noch einmal verdeutlicht dargestellt. 

![Studio:Bereiche theoretisch](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Bereiche_theoretisch_04.png)

Im **Studio** sieht die Übersicht dann wie nachfolgend dargestellt anhand eines Beispiels aus. Mit einem Klick auf den jeweiligen Arbeitsbereich öffnet sich dieser und die enthaltenen Aufgaben (Units) sind in Gruppen sortiert zu sehen.

![Studio:Bereiche praktisch](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Bereiche_praktisch_02.png)

Im nächsten Bild ist einmal bsph. der Arbeitsbereich "Hören und verstehen" in der Bereichsgruppe "Deutsch" mit den enthaltenen Aufgaben (Units) zu sehen. In diesem Arbeitsbereich befinden sich 2 Gruppen mit den Namen "Templates" und "Vorlagen". Außerdem ist die Aufteilung eines Arbeitsbereichs einmal dargestellt und näher beschrieben.

:information_source: **Die Benennung der Arbeitsbereiche richtet sich günstigerweise nach dem Zweck dieses Arbeitsbereichs. So könnte bspw. eine Aufteilung in unterschiedliche Fachbereiche sinnvoll sein.**

![Studio:Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Arbeitsbereich_01.png)

**rot markiert:**<br>
Hier können Units gelöscht, neu erzeugt, exportiert/importiert, kopiert und verschoben werden.

**grün markiert:**<br>
Hier können die Eigenschaften einer Unit verändert, neue Aufgabenelemente mittels Editor erzeugt und Aufgaben in einer Vorschau dargestellt werden. In späteren Versionen des **Studios** kann hier auch die Kodierung der Aufgabenelemente vorgenommen werden.

Folgende Funktionen stehen in der Unit Organisation zur Verfügung:

![Studio:Unit_Funktionen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Unit_Funktionen_04.png)

**Import von Datei(en)**
* Laden von Aufgaben von einem Speicherort. Zu einer Aufgabe gehört immer eine XML- und eine VOUD-Datei. Diese müssen pro Aufgabe gemeinsam geladen werden. Hierfür können diese zu einer ZIP-Datei verpackt werden. 

**Neu von vorhandener Aufgabe**
* Es können Aufgaben aus einem anderen Bereich als Vorlage kopiert werden. Außerdem können Aufgaben im aktiven Arbeitsbereich kopiert werden. 

**Neu (leer)**
* Erzeugen einer neuen Aufgabe

**Einstellungen**
* Einstellungen für den aktiven Arbeitsbereich. Hier kann festgelegt werden, welcher Editor und Player voreingestellt ist. Wird eine neue Aufgabe erzeugt, sind diese dann schon voreingestellt in den Eigenschaften der Aufgabe zu finden.

**Nutzer:innen**
* Übersicht und Kontaktdaten (falls von den jeweiligen Personen freigegeben) aller Personen, die Zugriff auf diesen Arbeitsbreich haben.

**Export**
* Exportieren von Aufgaben mit zusätzlichen Optionen. Wenn gewünscht können auch die beiden Steuerdateien: Booklet.xml und Testtakers.xml zusätzlich zu den Aufgaben ausgegeben werden. Es kann dann auch festgelegt werden, wie diese beiden Dateien konfiguriert sein sollen. Bspw. kann für die Testtakers.xml festgelegt werden, wie viele Testpersonen angelegt sind und in welchem Modus diese Testpersonen den Test durchführen können. Zusätzlich kann die für die Aufgaben festgelegte Player-Ressource mit ausgegeben werden.

**Verschieben**
* Aufgaben aus dem aktiven Arbeitsbereich in einen anderen Arbeitsbereich verschieben.

**Kopieren**
* Kopieren einer Aufgabe des aktiven Arbeitsbereich in einen anderen Arbeitsbereich.

:information_source: **Einige Funktionen bspw. das Verschieben in einen anderen Arbeitsbereich, können nur genutzt werden, wenn die entsprechenden Zugriffsrechte auf den Ziel-Arbeitsbereich auch vorhanden sind.**

### Arbeiten im Team

Hat eine Person Zugriff auf eine Bereichsgruppe (siehe Zugriffsrechte), kann diese Person Arbeitsbereiche innerhalb dieser Bereichsgruppe anlegen und angelegten Personen Zugriff darauf gewehren. So kann die für einen Bereich verantwortliche Person den Zugriff einzelner Mitglieder einer Fachgruppe auf Arbeitsbereiche und die darin enthaltenen Aufgaben regeln. Dies ermöglicht den Fachgruppen eine von den Systemadministrator\*innen unabhängige Organisation ihres Bereichs.

:information_source: In die Einstellungsebene für die Bereichsgruppe gelangt man über das Zahnradsymbol rechts neben der Bereichsgruppe.

Jede in der Anwendung hinterlegte Person kann nach Anmeldung am **Studio** personenspezifische Daten, wie bspw. eine E-Mailadresse angeben. Anschließend kann die Person festlegen, ob diese Informationen für andere ersichtlich sind oder nicht. 

![Studio:Kontaktdaten](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Kontaktdaten_01.png)

Weiterhin können zu jeder angelegten Aufgabe Kommentare hinterlegt werden. Dies ermöglicht Mitgliedern einer Fachgruppe auf unterschiedlichen Wegen miteinander in Kontakt zu treten. Kommentare zu einer Aufgaben können im Arbeitsbereich in den Eigenschaften einer Aufgabe geschrieben werden.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Zugriffsrechte">
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

Die Zugriffsrechte sind über zwei Anmeldeebenen geregelt. Zum einen den sogenannten **SuperAdmin** und zum anderen den **WorkspaceAdmin**. Der **SuperAdmin** kann, wie der Name vielleicht schon andeutet, so ziemlich alles im **Studio** freigeben. Er kann Personen anlegen und grundlegende Zugriffsrechte auf Bereichsgruppen und Arbeitsbereiche vergeben. Alle Personen, die vom **SuperAdmin** hinterlegt wurden und nicht als **SuperAdmin** angelegt wurden, sind automatisch **WorkspaceAdmins**. Diese können dann Arbeitsbereiche innerhalb einer Bereichsgruppe für andere Personen freigeben und spezifische Einstellungen an den Arbeitsbereichen vornehmen.

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
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Aufgabenbearbeitung-und-Erstellung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Verwaltung-und-Organisation">
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

## 3.3 Aufgabenbearbeitung und Erstellung

Nach Öffnen eines Arbeitsbereichs kann in der Unit-Organisation eine neue Aufgabe angelegt oder eine bestehende Aufgaben bearbeitet werden. Wird eine Aufgabe neu angelegt, können alle relevanten Eigenschaften zu dieser Aufgabe vorab in einem Formular eingegeben werden. Es ist auch möglich diese Eigenschaften nachträglich zu ändern. Dazu ist die entsprechende Aufgabe in der Liste zu markieren. Anschließend erscheinen im oberen Teil einige Reiter. Über den Reiter "Eigenschaften" können die Eigenschaften nachträglich geändert werden. Alle weiteren Reiter werden nachfolgend beschrieben.

![Unit Bearbeitung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Unit_Bearbeitung_01.png)

### Reiter: Eigenschaften

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

### Reiter: Editor

> Detailierte Informationen zur Arbeit mit den Editoren finden Sie im Kapitel **Editor.**

### Reiter: Vorschau

Während der Erstellung einer Aufgabe kann die Aufgabe ohne Speicherung aktueller Änderungen in der Voransicht begutachtet werden.

> **Um die Aufgabe auch in der Vorschau korrekt darstellen zu können, müssen in den Eigenschaften gewählter Editor und Player zueinander passen!**

Nachfolgendes Bild zeigt die Voransicht und deren Bestandteile:

![Editor Vorschau](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Editor_Vorschau_01.png)

Beschreibung des grün markierten Bereiches:<br>

**P:** zeigt die Vollständigkeit der Präsentation/Anzeige an, d. h. es wird angezeigt, ob alle Audios abgespielt wurden und/oder ob alle Viewpoints (unsichtbar) angezeigt wurden (d. h. ob gescrollt und alle Textteile, Items etc. gesehen wurden): grün = ja, vollständig; rot = nein, unvollständig;<br>
**R:** zeigt die Vollständigkeit der Reaktionen an, d. h. es wird angezeigt, ob alle Input-Felder/Anklick-Optionen bedient wurden: grün = ja, alle; gelb = ja, teilweise; rot = nein, keine.<br>
**F:** zeigt an, ob sich der Fokus noch im aktuellen Fenster befindet. Dient der Kontrolle bei der späteren Testdurchführung, ob sich die Testperson immer noch im Fenster der Testdurchführung befindet oder ob diese das Testfenster verlassen hat und stattdessen ein anderes Fenter geöffnet hat (andere Website etc.)

### Reiter: Kodierung

In den nächsten Versionen des **Studios** wird es an dieser Stelle möglich sein eine Kodiervorlage für die Aufgabenelemente anzulegen.

### Reiter: Kommentare

Hier können Kommentare zu den Aufgaben hinterlegt werden. Auf diesem Weg können Mitgliedern einer Fachgruppe Informationen zu einer Aufgabe austauschen.

:information_source: Gegebene Kommentare können nur von den Autor\*innen wieder gelöscht werden!

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.4-Editor">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Zugriffsrechte">
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

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.5-Player-Vorschau-(Verona)">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Aufgabenbearbeitung-und-Erstellung">
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
Detailierte Informationen zum **Dan-Player** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Player-Dan).
	
**Verona Player Abi**<br>
Dieser Player kann Aufgaben wiedergeben, deren Erstellung mittels **PlainText-Editor** erfolgte.<br>
Detailierte Informationen zum **Abi-Player** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Player-Abi).

**Verona Player Aspect**<br>
Dieser Player kann Aufgaben wiedergeben, deren Erstellung mittels **Aspect-Editor** erfolgte.<br>
Detailierte Informationen zum **Aspect-Player** finden Sie in dem gleichnamigen [Einzeldokument](Verona-Player-Aspect).

---
<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.6-Kodierung-(Schemer)">
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

# 3.6 Kodierung (Schemer)

```yaml
Dokumentstatus: Review (THuste)
Stand: 05.08.2022
todo: - In Bearbeitung
      
```
Informationen zum Schemer sind dem [folgenden](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schemer-Vxx) Einzeldokument zu entnehmen.

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