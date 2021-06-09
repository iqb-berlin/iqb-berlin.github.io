# 3 Teststudio

```yaml
Achtung: Noch nicht aktualisiert auf 1.0
Dokumentstatus: Review (THuste)
Stand: 02.06.2021
todo:
```

Das IQB-Teststudio ist eine Web-Anwendung für den Entwurf von Kompetenztests oder Befragungen. Nach der Installation auf einem Webserver wählt man diesen Server über seine Adresse an, d. h. man schreibt dessen Internet-Adresse in die Adresszeile eines Internet-Browsers. Dadurch werden die Programmierungen geladen und man sieht ein Formular zum Anmelden.

Eine grobe Einführung in das Teststudio geben auch die nachfolgenden Verlinkungen.
Das IQB bietet folgende Video-Präsentationen bzgl. des Testcenters an:

 * [IQB-Teststudio Intro](https://box.hu-berlin.de/f/e29f3e8d8c35480f8531/)
 * [Schulung Teststudio Editor Dan2](https://box.hu-berlin.de/f/edc2409b79954dc3b3a1/)    

Des Weiteren besteht das folgende Forum: [Teststudio-Forum](https://github.com/iqb-berlin/teststudio-lite-frontend/discussions)<br>
Hier finden Sie häufig gestellte Fragen und Antworten sowie Berichte über Einsätze des IQB-Teststudios.

**Installation**

Das IQB hat alle Programmierungen unter einer Open Source veröffentlicht und erleichtert die Installation durch ein sog. Docker-Setup. Für die Installation muss man einen Server bereitstellen (Linux oder Windows), und dieser Server muss dann über eine Internet-Adresse erreichbar sein. Die Installation sollte erfahrenes IT-Fachpersonal durchführen. Die Dokumentation hierzu setzt Wissen vor allem zur Virtualisierungssoftware Docker voraus. Es ist weiterhin Wissen zu Datensicherheit nötig, denn sobald ein Server öffentlich verfügbar ist, müssen Maßnahmen gegen Angriffe durch Schadsoftware ergriffen werden. Das IQB ist bemüht, die Installationspakete gut abzusichern, übernimmt aber im Schadensfall keine Verantwortung.

**Verwaltung der Tests**

Nach der Installation ist zunächst ein Standard-Konto für die Verwaltung von Tests angelegt. Mit diesem Zugang können dann entsprechende Arbeitsbereiche und Personenzugriffe angelegt werden. Meldet sich eine entsprechend freigegebene Person am Teststudio an, kann diese in ihrem Arbeitsbereich erste Aufgabenentwürfe starten. Bereits bestehende Aufgaben können auch in diesen Bereich importiert werden.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Stand-der-Entwicklung%3A-Teststudio‐Lite">
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

# 3.1 Stand der Entwicklung: Teststudio-Lite

```yaml
Dokumentstatus: Entwurf
Stand: 6.4.2021
```

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Portal-zur-Verwaltung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3-Teststudio">
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

# 3.2 Übersicht der Webanwendung

```yaml
Dokumentstatus: Entwurf T.Huste
Stand: 03.06.2021
```

<table>
  <tr>
    <td><a href="#Zugriffsrechte">Zugriffsrechte</a></td>
    <td><a href="#Arbeitsber">Arbeitsbereiche</a></td>    
	<td><a href="#Editor">Der Editor</a></td>
  </tr>
</table>

## Zugriffsrechte

### <a name="Zugriffsrechte"></a>System-Admin

Wenn das eigene Verwaltungskonto ein kleines Zahnradsymbol aufweist, ist über dieses Symbol ein Zugriff auf die Systemverwaltung möglich. In der Systemverwaltung werden Nutzerkonten und Arbeitsbereiche angezeigt. Hier können Zugriffsrechte auf Arbeitsbereiche für die angelegten Personen festgelegt werden. Es können auch neue Nutzer\*innen und Arbeitsbereiche angelegt werden.

> Personen die Zugriff auf die Systemverwaltung erhalten sollen, können nur von dem Administrator\*innen des Teststudios festgelegt werden!

### Standardzugriff

Verfügen Personen über einen Standardzugriff, können diese nach Anmeldung am Teststudio die Gruppen und Arbeitsbereich sehen, die für sie von dem System-Admin freigegeben wurden. Auf diese können dann zugergiffen und die enthaltenen Aufgaben bearbeitet werden.

## <a name="Arbeitsber"></a>Arbeitsbereiche

Um mehreren für die Aufgabenentwicklung verantwortlichen Personen die Möglichkeit zu bieten an Aufgabenentwürfen zu arbeiten, ist eine Aufteilung bzw. Organisation in Arbeitsbereiche sinnvoll. Die Aufgabenentwürfe (Units) werden dann in diesen Bereichen organisiert. Im Sinne einer besseren Übersichtlichkeit wird außerdem eine Gruppenaufteilung in entsprechende Themen vorgenommen. Zugriffsrechte regeln den Zugriff auf diese Bereiche. So können Personen nur Bereiche sehen, die von der Verwaltung, also den Administrator\*innen, für diese Personen freigegeben wurden.

> Die Benennung der Arbeitsbereiche richtet sich günstigerweise nach dem Zweck, also z. B. "Demo Deutsch Sek1" oder "Review Abi" oder "VERA Englisch".

Nach der Anmeldung präsentiert das System eine Liste aller Gruppen und der darin enthaltenen Arbeitsbereiche für die angemeldete Person (Zugriffsrechte). Mit einem Klick auf den jeweiligen Arbeitsbereich wird dieser geöffnet. Zur Liste der Arbeitsbereiche kehrt man zurück, indem man auf das IQB-Logo links oben in der Ecke klickt.


Ein geöffneter Arbeistbereich sieht dann wie folgt aus:

![iqb online assessment applications with relations: Teststudio Funktionen Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Aufteilung_Arbeitsbereich_final.png)

Das Fenster eines geöffneten Arbeitsbereichs unterteilt sich in zwei Bereiche:

 * rot markiert:<br>
   Organisation der Units. Hier können Units gelöscht, neu erzeugt, exportiert/importiert und verschoben werden.
 * grün markiert:<br>
   Bearbeiten einer Unit. Hier können die Eigenschaften einer Unit verändert, neue Aufgabenelemente mittels Editor erzeugt und Aufgaben in einer Vorschau dargestellt werden.

### Bereich der Unit Bearbeitung (grün markiert)

#### Eigenschaften

Unter den Eigenschaften einer Unit werden einerseits Metadaten, wie Namen und Beschreibung, festgelegt und andererseits werden der zu verwendende Editor und der zugehörige Player bestimmt.

Kurzname:<br>
Eindeutiger (ID-fähiger )und schlüssiger Kurzname der Unit. Dieser sollte keine Leerzeichen oder Unterstriche enthalten. Über diesen Namen wird die Aufgabe im Testheft identifiziert.

Name:<br>
Dieser Name wird im Testcenter beim Abspielen dieser Aufgabe angezeigt. Dieser Name kann aber auch nachträglich noch geändert werden.

Editor:<br>
Zum Zeitpunkt der Erstellung dieser Dokumentation stehen die zwei folgenden Editoren zur Verfügung:

* IQB Editor Plain Text v1.0.1<br>
  Aufgaben können mittels einer Scriptsprache (deshalb auch der Name "...Plain Text..") erstellt werden. Es stehen also bspw. keine grafischen Elemente zur Erstellung eines Textfeldes oder eines Buttons zur Verfügung. Die Erzeugung solcher Elemente wird rein textuell realisiert.

* IQB Editor Dan v3.1.0<br>
  Komplexe Aufgaben können mittels Auswahl von vorgefertigten Elementen erstellt werden. Die bereitgestellten Elemente können dabei einfach mittels Drag-and-Drop der Aufgabe hinzugefügt werden. Anschließend können diese Elemente in ihren Eigenschaften verändert werden. Es können dann bspw. Größe, Farbe, Position und weitere Eigenschaften der Elemente verändert werden.

Player:<br>
Damit die Aufgabe wiedergegeben werden kann, muss der zum Editor passende Player gewählt werden. Eine Aufgabe die bspw. mit dem IQB Editor Plain Text v1.0.1 erstellt wurde, kann nicht von einem Dan Player wiedergegeben werden, da ihm schlicht die enthaltene Syntax nicht bekannt ist.
Zum Zeitpunkt der Erstellung dieser Dokumentation stehen die zwei folgenden Player zur Verfügung:
 
* IQB Player Dan v3.0.0<br>
  Dieser Player kann Aufgaben wiedergeben, deren Erstellung mittels Dan Editor erfolgte.

* IQB Player Abi v3.3.3<br>
  Dieser Player kann Aufgaben wiedergeben, deren Erstellung mittels Plain Text Editor erfolgte.

#### Editor

Hierüber gelangt man zu den Funktionen des in den Eigenschaften festgelegten Editors. Mehr zu den Funktionen und dem Umgang mit diesem Editor sind dem Kapitel: [Allgemeine Arbeitsweise](3.3-Allgemeine-Arbeitsweise) zu entnehmen.

#### Vorschau

Während der Erstellung einer Aufgabe, kann die Aufgabe ohne Speicherung einer aktuellen Änderungen in der Voransicht begutachtet werden.<br>
> Um die Aufgabe auch in der Vorschau korrekt darstellen zu können, müssen in den Eigenschaften gewählter Editor und Player zueinander passen!

Nachfolgendes Bild zeigt die Voransicht und deren Bestandteile:

![iqb online assessment applications with relations: Teststudio Funktionen Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Editor_Voransicht_final.png)

Beschreibung des grün markierten Bereiches:<br>

**P:** zeigt die Vollständigkeit der Präsentation/Anzeige an, d. h. es wird angezeigt, ob alle Audios abgespielt wurden und/oder ob alle Viewpoints (unsichtbar) angezeigt wurden (d. h. ob gescrollt und alle Textteile, Items etc. gesehen wurden): grün = ja, vollständig; rot = nein, unvollständig;<br>
**R:** zeigt die Vollständigkeit der Reaktionen an, d. h. es wird angezeigt, ob alle Input-Felder/Anklick-Optionen bedient wurden: grün = ja, alle; gelb = ja, teilweise; rot = nein, keine.<br>
**F:** zeigt an, ob sich der Fokus noch im aktuellen Fenster befindet. Dient der Kontrolle bei der späteren Testdurchführung, ob sich die Testperson immer noch im Fenster der Testdurchführung befindet oder ob diese das Testfenster verlassen hat und stattdessen ein anderes Fenter geöffnet hat (andere Website etc.)

### Bereich der Unit Organisation (rot markiert)

In diesem Bereich können Units verwaltet bzw. organisiert werden. Nachdem eine Unit markiert wurde, kann diese über die unten angeordneten Funktionschaltflächen gelöscht, exportiert, verschoben oder deren Eigenschaften verändert werden. Das kleine Pluszeichen legt eine neue Unit an. Oberhalb der Unit Auflistung im linken Bereich des Portals befinden sich zwei weitere Funktionsschaltflächen. Diese ermöglichen das Speichern bzw. Verwerfen von Änderungen an einer gewählten Unit.

![iqb online assessment applications with relations: Teststudio Funktionen Arbeitsbereich](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Funktionen_Arbeitsbereich_final.png)

#### Unit verschieben

Es ist möglich Units zu verschieben. Verschoben kann dabei nur in andere für die angemeldete Person freigegebene Arbeitsbereiche.

#### Unit kopieren

Markierte Units können kopiert werden. Alle Inhalte dieser Unit werden dabei in eine neu zu benennende Unit kopiert.

#### Unit importieren

Der Import von bestehenden Units ist ebenso möglich. Besteht die zu importierende Unit aus einer xml-/ und einer voud-Datei, sollten diese zuvor in einem Zip-Format gepackt werden. Anschließend kann die Zip-Datei ausgewählt und importiert werden. Der gewählte Name der Zip-Datei spielt dabei keine Rolle.

> Voud-Dateien können nicht einzeln importiert werden. Sie müssen immer zusammen mit der zugehörigen Xml-Datei importiert werden. Daher sollten diese Dateien zuvor immer in einem Zip-Format verpackt und dann importiert werden!

#### Unit exportieren

Werden Units exportiert, verpackt das Teststudio die zu dieser Unit gehörenden Dateien in einer Zip-Datei. Eine Unit besteht dabei zumeist aus einer Xml-Datei und einer Voud-Datei. Die Zip-Datei wird automatisch wie folgt benannt: aktuelles Datum UnitDefs.voud.zip


## <a name="Editor"></a>Der Editor

> Vorab! Hier wird nur die Arbeit mit dem Editor: **IQB Editor Dan v3.1.0** aufgezeigt. Es wird nicht auf den Plain Text Editor eingegangen.

### Übersicht

Der Editor wird über den Tab: **Editor** im Bereich der Unitbearbeitung (grün markiert im oberen Bild) geöffnet. Nachfolgend wird dann die Editoransicht angezeigt:

![iqb online assessment applications with relations: Teststudio Editieransicht](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Editoransicht_final.png)

Grün markiert:
 * Im oberen Bereich die Elemente, die auf einer Seite hinzugefügt werden können. Dies sind bspw. Schaltflächen, Textfelder, Grafiken, Multiple-Choice-Felder etc..Eine detailierte Beschreibung der Elemente und Funktionen erfolgt weiter unten.
 * Im mittleren Bereich Optionen zur Formatübertragung und zum Kopieren und Einfügen markierter Elemente.
 * Im unteren Bereich Pfeil-Schaltflächen, mit denen man alle Elemente auf einer Seite um 10px verschieben kann.
 * Ganz unten die Option zum Löschen eines aktiven Elements und Optionen zum Up- und Download von Dateien. 
 
Gelb markiert:
Wenn eine Unit neu angelegt wird, besteht diese zu Anfang immer nur aus einer Seite. Die Seiten können anschließend mithilfe des kleinen Pluszeichens im gelb markierten Bereich beliebig erhöht werden.

### Elemente einer Aufgabe

Aufgabenelemente stehen über eine kleine Box (im oberen Bild grün markiert) bereit. Diese Box stellt nicht nur die Elemente, sondern auch weitere Funktionen zur Verfügung.
Nachfolgend eine Übersicht aller Elemente und weiterer Funktionen:


 












---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Allgemeine-Arbeitsweise">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Stand-der-Entwicklung%3A-Teststudio‐Lite">
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

# 3.3 Allgemeine Arbeitsweise

```yaml
Dokumentstatus: Review (THuste)
Stand: 03.06.2021
todo: - Verweis auf Konventionen erhalten
      - weiter mit Leben füllen
```
## Anlegen einer Unit

Nach Auswahl und öffnen des gewünschten Arbeitsbereichs kann mithilfe der Plus-Schaltfläche im linken Teil des Arbeitsbereichs eine neue Unit angelegt werden. Nach der Anlage sollten die Eigenschaften hinsichtlich Namensgebung, Auswahl des Editors und Players erfolgen. Anschließend können die Editierfunktionen geöffnet werden mittels Klick auf den Tab: Editor. 


## IQB Konventionen

Ein Zusatzdokument welches die IQB Konventionen beschreibt finden Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/IQB-Konventionen-Aufgabengestaltung)

## Workarounds

Das aktuelle IQB-Teststudio wurde zwar bereits für diverse Studien verwendet, befindet sich aber noch im Entwicklungsstadium "Prototyp". Es ist völlig klar, dass viele Funktionen fehlen oder nicht die erwarteten Ergebnisse liefern. Im Projektzeitraum 2021-2023 wird diese Web-Anwendung grundlegend überarbeitet und die aktuelle Version "IQB-Teststudio-Lite" nur bei dringendem Bedarf geändert.

### Metadaten reduzieren

Die aktuelle Version des Teststudios erzeugt Unit-Xmls, die nicht vom aktuellen Testcenter akzeptiert werden. Das liegt daran, dass die zulässigen Metadaten auf das Nötigste reduziert wurden. Die Elemente `Lastchange`, `Owner` und `Project` müssen entfernt werden:

#### Vorher
```
<Unit>
  <Metadata>
    <Id>Yoyo</Id>
    <Label>Geobrettfigur auslegen</Label>
    <Lastchange>2020-07-02T00:41:16+02:00</Lastchange>
    <Owner>Institut zur Qualit&#xE4;tsentwicklung im Bildungswesen IQB</Owner>
    <Project>Demo-Aufgaben f&#xFC;r die &#xD6;ffentlichkeit</Project>
  </Metadata>
  <DefinitionRef player="IQBVisualUnitPlayerV2">Yoyo.voud</DefinitionRef>
</Unit>
```
#### Nachher
```
<Unit>
  <Metadata>
    <Id>Yoyo</Id>
    <Label>Geobrettfigur auslegen</Label>
  </Metadata>
  <DefinitionRef player="IQBVisualUnitPlayerV2">Yoyo.voud</DefinitionRef>
</Unit>
```
### Empfehlung: Verweis zur Validierung
Nach dem Hochladen in das Testcenter erhält man noch eine Warnung "File has no link to XSD-Schema...". Diese Warnung bedeutet, dass die Xml-Datei keinen expliziten Verweis auf eine Xsd-Datei enthält. Eine solche Xsd-Datei definiert die möglichen Elemente und Attribute einer Xml-Datei und kann daher zur Prüfung der Xml-Datei auf Korrektheit verwendet werden. Das IQB stellt solche Xsd-Dateien bereit. 

Die Deklaration der Xsd-Datei erfolgt im Haupt-Element einer Xml-Datei. Für die Unit-Xml heißt das Hauptelement `Unit` und muss folgendermaßen geändert werden:
```
<Unit 
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Unit.xsd">
```
Ein nützlicher Nebeneffekt hierbei ist, dass auch Editoren zur Bearbeitung von Xml-Dateien (z. B. Notepad++, Sublime) nun eine Validierung vornehmen können. Man kann also vor dem Hochladen eine Validierung bereits beim Schreiben einer Xml-Datei vornehmen lassen.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.4-Wahl-des-Editors-(Verona)">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Übersicht-der-Webanwendung">
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

# 3.4 Wahl des Editors (Verona)

```yaml
Dokumentstatus: Entwurf
Stand: 6.4.2021
```

Einführungsvideo:
 * [IQB-Verona Editor Dan2](https://box.hu-berlin.de/f/edc2409b79954dc3b3a1/)

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Allgemeine-Arbeitsweise">
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

