# 2.Testcenter

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 21.03.2021
Prio: low
todo:
  - Was gehört hier noch her? Spezielle Infos zum Testcenter, wie z.B. Ansprechpartner, Entwicklungststände etc?
```

Das **Testcenter** gehört zu einem der wesentlichen TBA Bestandteile.
Grundlegende Informationen zum **Testcenter** erhalten Sie auch im TBA Einführungskapitel.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.1-Testcenter-Einf%C3%BChrung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.1 Testcenter Einführung

Eine grobe Einführung geben die nachfolgenden Verlinkungen.                         
Das IQB bietet folgende Video-Präsentationen bzgl. des Testcenters an:
* [Einführung in das IQB-Testcenter](https://box.hu-berlin.de/f/a8f7aea9c751493c8d35/)
* [Diskussion der Optionen Testcenter-Einsatz oder Implementation der Verona-Schnittstelle](https://box.hu-berlin.de/f/d23af87168fa4e9f9bb0/)

Des Weiteren besteht das folgende Forum:
[Testcenter-Forum](https://github.com/iqb-berlin/testcenter-frontend/discussions)                      
Hier finden Sie häufig gestellte Fragen und Antworten sowie Berichte über Einsätze des IQB-Testcenters.

---

### Einsatz und Aufbau des Testcenters

Das **Testcenter** beinhaltet eine Datenbank, die zur Speicherung von Tests und Metadaten verwendet wird.
Des Weiteren werden mithilfe des **Testcenters** die interaktiven Inhalte eines Tests wiedergegeben. 
Wobei nicht nur finale Tests, sondern auch Probedurchläufe durchgeführt werden können. Letztere verschaffen den Organisator\*innen einen Überblick 
bzgl. eventueller Fehlabläufe und damit nötiger Nachbearbeitungen eines Tests. Nachfolgend ist noch einmal aufgelistet, welche Möglichkeiten 
das **Testcenter** bietet:

**Testdurchführung**

* finale oder probeweise Testdurchführung (abspielen der Aufgaben)

**Anlegen eines Tests**

* upload, löschen und download der Testdateien

**Administration**

* Testverwaltung
* Benutzerverwaltung/ Benutzerzugänge

Detailliert betrachtet besteht das **Testcenter** aus weiteren softwaretechnischen Komponenten, die hier, obwohl die meisten Andwender\*innen
damit nicht in Kontakt kommen dürften, einmal Erwähnung finden sollten. Eine für die meisten Anwender\*innen häufig vorkommende Begrifflichkeit
dürfte der so genannte Verona Player sein. Dieser Player ist in das **Testcenter** intergriert und ist für die Wiedergabe der Aufgabeninhalte
zuständig. Über eine definierte Schnittstelle meldet dieser außerdem jegliche Interaktionen auf den Testseiten an das **Testcenter**. 
Näheres zum Thema Verona entnehmen Sie bitte dem gleichnamigen Kapitel. Es gibt weitere Schnittstellen und Umgebungsmodule, 
die direkt oder indirekt mit dem **Testcenter** zusammenarbeiten, diese sind für Interessierte nachfolgend dargestellt.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Umgebungsmodule_final.png)

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.2-Anmeldung-und-Laden-eines-Tests">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.-Testcenter">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.2 Anmeldung und Laden eines Tests

### Anmeldung am Testcenter

Wie dem Einführungskapiteln bereits zu entnehmen ist, besteht ein Technologiebasierter Test aus mehreren Dateien.
Jede dieser Dateien bietet spezifische Möglichkeiten den Test bzgl. Struktur und Ablauf zu beeinflussen. Um einen Test im **Testcenter** 
abspielen zu können oder Testdateien in das **Testcenter** zu laden, zu löschen, oder aus dem **Testcenter** herunterzuladen, 
bedarf es unterschiedlicher Anmeldearten. Dabei muss in zwei Gruppen unterschieden werden: 

* Testorganisator\*innen
* Testpersonen

---

#### Testorganisator\*in

Der oder die Testorganisator\*in übernimmt die administrative Rolle einer Testdurchführung. Dazu gehört die Bearbeitung von Testdateien, 
das Laden und Löschen der Testbestandteile, die Benutzerverwaltung für die Probanden und das Festlegen der Testmodi, 
sprich wie der Test im **Testcenter** ablaufen soll. Testorganisator\*innen benötigen dafür einen Zugang zum **Testcenter**. 
Dieser Zugang kann nur von den Administrator\*innen des **Testcenters** angelegt werden.

  
*Wer ist nun aber Administrator\*in des Testcenters?*

Derzeitig werden die meisten Testdurchführenden auf das **Testcenter** zugreifen, welches die hausinternen IT-Strukturen 
(Server, Netzwerke) des IQB nutzt. Mit der weiteren Etablierung des Technologiebasierten Testens in den Bildungseinrichtungen, 
wird der Betrieb beider Systeme, sowohl **Teststudio** als auch **Testcenter**, zunehmend in den eigenen IT-Strukturen 
der jeweiligen Bildungseinrichtungen zum Einsatz kommen. Administrator\*innen des **Testcenter** und auch des **Teststudios** 
sind somit diejenigen, die für die IT-Strukturen in welcher die Systeme betrieben werden, verantwortlich sind. 

Sobald Sie die entsprechenden Zugangsdaten von administrativer Seite erhalten haben, können Sie
nach Aufruf einer entsprechenden Internetadresse in einem Webbrowser die Anmeldung am **Testcenter** vornehmen. 
Auch die einzugebene Internetadresse ist wiederum abhängig von der IT-Struktur in welcher das **Testcenter** betrieben wird. 
Möchten Sie das **Testcenter** in der IT-Strukur des IQB nutzen, ist folgende Adresse im Browser einzugeben: https://www.iqb-testcenter.de.<br>
Nach erfolgreicher Anmeldung können dann Daten geladen oder auch gelöscht werden.

---

#### Testperson

Die eigentliche Testdurchführung, oder auch ein Probelauf für Testorganisator\*innen, erfolgt mit separaten Zugangsdaten. 
Diese Zugangsdaten legen allein die Testorganisator\*innen fest. Dies erfolgt durch Anpassung einer bestimmten Datei, 
die Bestandteil eines jeden Tests ist. Diese Datei trägt den Namen: *Testtakers.xml*. In dieser können Zugangsdaten festgelegt 
und zusätzlich ein Modi gesetzt werden. Der Modi bestimmt den Testablauf, also ob es sich z.B. um einen finalen Test oder nur um einen 
Probedurchlauf für die Testorganisator\*innen handelt. Nach der Bearbeitung der *Testtakers.xml* bzgl. des angepassten Logins und Modis, 
können die Testdateien in das **Testcenter** geladen werden. Anschießend können die so angelegten Zugangsdaten bei einer Neuanmeldung 
im **Testcenter** angegeben werden. Der Test wird dann entsprechend des gesetzten Modis abgespielt.
Für die Testperson sollte dann also ein finaler Testdurchlauf gestartet werden.


**Bsp.:**<br>
Nehmen wir an Sie als Organisator\*in wollen für den Schüler Jakob einen finalen Test vorbereiten. 
So ist in der *Texttakers.xml* des gewünschten Tests ein `Username` für Jakob, ein `pw` (Passwort) und der Modi wie der Test ablaufen soll,
auszuwählen und einzutragen. Nachdem der Test inklusive der *Testtakers.xml* in das **Testcenter** geladen wurde, 
kann Jakob sich mit diesen von Ihnen eingetragenen Zugangsdaten am **Testcenter** anmelden und seinen Test in der von Ihnen 
gewünschten Art und Weise durchlaufen.

Mehr zu diesem Thema erfahren Sie auch im Kapitel: 
[Testcenter / Vorbearbeitung Testdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Vorbearbeitung-der-Testdateien)

---

### Laden eines Tests

Nach der Anmeldung als Testorganisator\*in am **Testcenter** können die Testbestandteile geladen werden.
Auch die Löschung einzelner Datei und das Herunterladen ist möglich. Während des Hochladens in das **Testcenter** findet eine 
Plausibilitätsprüfung statt. Dabei wird überprüft ob die definierten Bestandteile in einer Datei während des Hochladens auch gefunden werden. 

Ein einfaches Beispiel: In der Booklet.xml werden die gewünschten Units deklariert. Laden Sie zuerst die Booklet.xml und erst anschließend
die Unit.xml wird eine Fehlermeldung generiert, weil die in der Booklet.xml deklarierten Units nicht gefunden werden. 

Um die Plausibilitätsprüfung beim Upload in das **Testcenter** zu bestehen, müssen die Dateien in der richtigen Reihenfolge geladen werden.
Des Weiteren ist vor dem Upload zu prüfen ob die IDs in den Dateien richtig geschrieben (Groß-/Kleinschreibung beachten!) bzw. die Dateien 
richtig benannt sind. In welcher Reihenfolge die Dateien zu laden sind, ist im nachfolgenden Bild zu erkennen. Außerdem ist die Abhängigkeit 
der IDs und der Dateinamen bzgl. der Definitionen ersichtlich.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Upload_Ablauf_final.png)

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Vorbearbeitung-der-Testdateien">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.1-Testcenter-Einführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.3 Vorbearbeitung der Testdateien

Die im **Teststudio** erzeugten Dateien können vor dem Upload in das **Testcenter** berarbeitet werden.<br>
Betrachten Sie dazu auch noch einmal das Kapitel:

[TBA Einführung -> Ablauf Entwurf und Durchführung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2-Ablauf-Entwurf-und-Durchführung)

Die Testdateien können einzeln "händisch" bearbeitet und die vorgenommenen Änderungen später im Testcenter abgespielt werden.
Diese Methode verlangt etwas Basiswissen bzgl. der Syntax der einzelnen Dateien, hat aber den Vorteil Änderungen direkt und bewusst herbeizuführen.
Diese Methode soll an dieser Stelle als: **Direktes Bearbeiten** bezeichnet werden.

Eine weitere Methode ist das Verwenden von Hilfsmitteln. Eines dieser Hilfsmittel stellt das IQB zur freien Verfügung.<br>
Es trägt den Namen **ITC-Toolbox** und kann über den folgenden Link heruntergeladen werden:<br>
https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox. Diese Methode der Bearbeitung soll an dieser Stelle als **Indirektes Bearbeiten** 
bezeichnet werden. Die Dateien werden also indirekt über das Tool **ITC-Toolbox** bearbeitet. Das Tool konvertiert dabei Excelinhalte in die 
für Testdateien benötigten Formate, in unserem Fall Xml-Formate. Vorteil dieser Methode: Sie müssen nicht direkt in der Testdatei arbeiten, 
sondern können die Werte der Testdatei mittels Excel beinflussen. Dies erhöht für einige Anwender\*innen die Übersichtlichkeit, 
eventuell verlangt es aber entsprechende Nachkontrollen der Testdatei.

---

### Direktes Bearbeiten

**Bevor es los geht ein paar Grundlagen zu XML:**

Bei den zu bearbeitenden Dateien handelt es sich um Xml-Dateien. Xml ist ein textbasiertes Datenformat.   
Die Daten werden also in Textform in einem Text hinterlegt. Xml-Dateien können daher auch einfach mittels eines Texteditors bearbeitet werden.
Damit die Daten im Text gefunden werden können, muss eine bestimmte Struktur eingehalten werden. Anschließend kann eine entsprechende Gegenstelle, 
in unserem Fall das **Testcenter**, mittels eindeutiger Schlüsselwörter (Tags oder Elemente) die Daten im Text finden und nutzen. 
Xml-Dateien bestehen immer aus Elementen und ggf. mehreren Unterelementen. Der Beginn eines Elements wir mit zwei spitzen 
Klammern `<Element>` eingeleitet und wie folgt beendet: `</Element>`. Jedes Element kann außer den eigentlichen Daten, welche sich im 
Elementenkörper befinden, zusätzliche Attribute enthalten. Attribute werden immer in der folgenden Form ausgedrückt: 
`Name Attribut = "Attributwert"` und befinden sich innerhalb des Elementenaufrufs (`<Element Attribut="Attributwert">`). 
Es gibt auch Elemente die Attribute aber keine Daten enthalten und umgekehrt. Einfache Bsp. sind nachfolgend aufgeführt:

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


Manche Attributwerte können frei gewählt werden, manche müssen sich an Vorgaben halten.<br> 
Nachfolgend wird nun auf die Elemente unserer Testdateien und deren Attribute und Daten eingegangen.<br>
In der Tabelle finden Sie immer das entsprechende Unterelement eines Hauptelementes und dessen Attribute und Daten (falls vorhanden).

Wie zu Beginn bereits erwähnt, können Sie xml-Dateien mit einem normalen Texteditor öffnen und bearbeiten.
Zur besseren Übersichtlichkeit wird jedoch ein Xml-Editor empfohlen, da dieser die Xml typische Syntax farblich hervorhebt und 
somit die Arbeit deutlich erleichert wird. Da es sehr viele Editoren gibt, kann an dieser Stelle nur eine Empfehlung unsererseits erfolgen. 
Letztlich müssen Anwender\*innen den für sich geeigneten Editor finden. Wir können den Editor Notepad++ empfehlen. 
Dieser kann auch noch andere Syntax darstellen, wie z.B. Html und ist frei verfügbar.
  
---

#### Attribute und Daten TESTTAKERS.xml

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
    <td>Vordefinierter Wert. Erzeugt einen Custom Text. Siehe <b>Custom Text Configuration</b> im Kapitel:
	<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Konfiguration-der-Testdurchf%C3%BChrung">Testcenter / Konfiguration der Testdurchführung</a></td   
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
    <td>Vordefinierter Wert. Bestimmt wie ein Test ablaufen soll (finaler Test oder Probetest etc.). Siehe: <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Modi-der-Testdurchf%C3%BChrung">Modi der Testdurchführung</a></td>
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

---

#### Attribute und Daten BOOKLET.xml

`METADATA`

<table>

<tr>
    <td>Id:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Wert. Der Name muss in gleicher Schreibweise auch in der Testtakers.xml aufgeführt sein damit dieses Booklet aufgerufen werden kann!</td>
</tr>
<tr>
    <td>Label:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Wert zur Bezeichnung des Booklets.</td>
</tr>
<tr>
    <td>Description:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Wert zur weiteren Beschreibung dieses Booklets.</td>
</tr>

</table>

```xml
<Metadata>
  <Id>Booklet1</Id>
  <Label>Sekundarstufe I Englisch Ansichtsaufgaben</Label>
  <Description>Sekundarstufe I Englisch Ansichtsaufgaben</Description>
</Metadata>
```

---

`BOOKLETCONFIG`

<table>

<tr>
    <td>Config:</td>
    <td>key</td>
    <td>Attribut</td>
    <td>Vordefinierter Wert. Ermöglicht eine Booklet Konfiguration. Die möglichen zu verwendenden Werte entnehmen Sie bitte der <b>Booklet Konfiguration</b> im Kapitel: 
	 <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Konfiguration-der-Testdurchf%C3%BChrung">Konfiguration der Testdurchführung</a></td>
</tr>
<tr>
    <td>Config:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Vordefinierter Wert. Die möglichen zu verwendenden Werte entnehmen Sie bitte der <b>Booklet Konfiguration</b> im Kapitel: 
	 <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Konfiguration-der-Testdurchf%C3%BChrung">Konfiguration der Testdurchführung</a></td>
</tr>

</table>


```xml
<BookletConfig>
  <Config key="force_responses_complete">OFF</Config>
</BookletConfig>
```

---

`UNITS`

<table>

<tr>
    <td>Unit:</td>
    <td>id</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert. Bezeichnet die Unit, die eingebunden werden soll. Die ID innerhalb der Unit.xml muss den selben Namen tragen (Groß/-Kleinschreibung beachten!).</td>
</tr>
<tr>
    <td>Unit:</td>
    <td>label</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert.</td>
</tr>
<tr>
    <td>Testlet:</td>
    <td>id</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert.</td>
</tr>
<tr>
    <td>Testlet:</td>
    <td>label</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert.</td>
</tr>
<tr>
    <td>CodeToEnter:</td>
    <td>code</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert. Dieser Code wird im Testcenter abgefragt. Dies kann z.B. verwendet werden um nach Codeeingabe in eine weitere Unit zu gelangen.</td>
</tr>
<tr>
    <td>CodeToEnter:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Wert. Dieser Text wird für die Codeabfrage verwendet.</td>
</tr>

</table>

```xml
<Units>
  <Unit id="Unit1" label="erste Unit" />
  <Testlet id="Testlet1" label="erstes Testlet">
    <Restrictions>
      <CodeToEnter code="Hase">Bitte geben Sie den Code ein!</CodeToEnter>
    </Restrictions>
  </Testlet>
</Units>
```

---

#### Attribute und Daten UNIT.xml

`UNIT`

<table>

<tr>
    <td>Id:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Wert. Der verwendete Wert muss in gleicher Schreibweise auch in der <b>Booklet.xml</b> unter <b>Units</b> eingetragen werden.</td>
</tr>
<tr>
    <td>Label:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Wert zur Bezeichnung der Unit.</td>
</tr>
<tr>
    <td>DefinitionRef:</td>
    <td>player</td>
    <td>Attribut</td>
    <td>Auswahl des Players, welcher die Inhalte der zugehörigen <b>voud-Datei</b> abspielen kann. Dieser Player muss als Ressource mit in das Testcenter geladen werden.</td>
</tr>
<tr>
    <td>DefinitionRef:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Name der zugehörigen <b>voud-Datei</b>. Die eigentliche <b>voud-Datei</b> muss den selben Namen tragen (Groß/-Kleinschreibung beachten!).</td>
</tr>

</table>


```xml
<Unit>
  <Metadata>
    <Id>Unit1</Id>
    <Label>erste Unit</Label>
  </Metadata>
  <DefinitionRef player="IQBVisualUnitPlayerV2">ER513.voud</DefinitionRef>
</Unit>
```

---

### Indirektes Berabeiten

#### IQB ITC-Toolbox

Wie eingangs bereits erwähnt können Sie mithilfe des Tools: **ITC-Toolbox** die *Booklet.xml* indirekt bearbeiten bzw. erzeugen.
**ITC-Toolbox** benötigt dafür eine Excel-Datei in welcher die zukünftigen Inhalte der Xml-Datei
in einer bestimmten Anordnung zu finden sind. Nachfolgend können Sie sich eine entprechende Excel-Vorlage herunterladen: 

[Excel-Vorlage für die ITC-Toolbox](https://github.com/iqb-berlin/itc-toolbox/blob/master/Booklet-Template.xlsx)

Nach der Installation und dem Start der **ITC-Toolbox** können Sie zwischen verschiedenen Optionen wählen:

* Booklet-Xlsx
* Login-Xlsx
* SysCheck csv- > xlsx
* Antworten und Logs csv -> xlsx

In diesem Kapitel interessieren uns vor allem die beiden Punkte *Booklet-Xlsx* (erzeugt eine Booklet.xml) 
und *Login-Xlsx* (unterstützt bei der Login-Datenverwaltung). Die letzten beiden Punkte sind für die Nachbearbeitung, 
sprich die Bearbeitung nach Abschluss eines Tests, bestimmt und werden daher im nachfolgenden Kapitel behandelt:

[Testcenter / Nachbearbeitung der Testdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Nachbearbeitung-der-Testdateien)

Damit die ITC-Toolbox die Werte entsprechend in der Excel-Tabellen finden und zuordnen kann, darf die Grundstruktur der Excel-Vorlage 
nicht verändert werden. Ändern Sie bitte nicht die Bezeichnungen von Zellen der Tabellenköpfe oder Bezeichner der Excel Blattseiten.

---

**Erzeugen / Bearbeiten der Booklet.xml**

Nach Auswahl des ersten Punktes: *Booklet-Xlsx* muss der Speicherort der entsprechende Excel-Datei angegeben werden.
**ITC-Toolbox** überprüft anschließend die Struktur der Excel-Datei und versucht die dort angegebenen Zusatzinformationen auf den anderen
Excel Blattseiten zu finden. Können Bezeichner nicht gefunden oder zugeordnet werden, werden entsprechende Fehlermeldung generiert.
Wurden alle Bezeichner gefunden und konnten entsprechend zugeordnet werden, erscheint eine Meldung über die erfolgreiche Erzeugung
einer *Booklet.xml*. Die *Booklet.xml* wird dann im selben Verzeichnis gespeichert in dem sich auch die Excel-Datei, die als Vorlage diente, 
befindet.

Um die Inhalte und Strukturen dieser Vorlage besser zu verstehen, betrachten Sie bitte die nachfolgenden Abbildungen. Diese gehen näher 
auf die Strukturen der Excel-Inhalte und den Auswirkungen auf die so generierte *Booklet.xml* ein. Achten Sie auch die farbliche Hervorhebung 
auf den Excel-Blättern und im generierten Code.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_ToolBox_Excel_final.png)

Auf der Grundlage dieser im obigen Bild dargestellten Excel-Datei und deren Inhalten wird die folgende *Booklet.xml* erzeugt:

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_ToolBox_BookletXml_final.png)

---

**Login-Datenverwaltung**

Über den Admin-Bereich des Testcenters sind die Zugangsdaten für 
Testpersonen, aber auch für Reviewer und die Testleitung zu hinterlegen. Struturiert 
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

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Nachbearbeitung-der-Testdateien">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.2-Anmeldung-und-Laden-eines-Tests">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.4 Nachbearbeitung der Testdateien

Das Testcenter gibt je nach gewähltem Durchführungsmodi am Ende eines Tests verschiedene Dateien aus. Diese dienen der Auswertung
einer Studie. Die Dateien können im Testcenter unter der jeweiligen durchgeführten Studie gefunden werden.
Nach Anmeldung als Testorganisator\*in stehen die Dateien in der abgeschlossenen Studie unter dem Punkt: *Ergebnisse/ Antworten* 
zum Download bereit. Setzen Sie anschließend einen Haken bei dem Probanden dessen Auswertungsdaten Sie einsehen möchten. 
Nachfolgend werden Ihnen 3 Datensätze angeboten:

* Anworten
* Logs
* Kommentare

Alle 3 Datensätze können heruntergeladen und als Csv-Datei am gewählten Ziehlort gespeichert werden.

---

### Nachberabeitung mittels Itc-Toolbox

In Csv-Dateien werden Werte in einer bestimmten Art und Weise aufgelistet und voneinander abgegrenzt. Die Abgrenzung erfolgt mittels
Semikolon, Hochkommata und Komma. Tabellenkalkulationsprogramme, wie bspw. Excel, können dieses Format lesen und erkennen über die 
entsprechende Zeichensetzung, welche Werte bspw. in den Tabellenkopf, in eine bestimmte Zeile oder Spalte gehören. 
Eine Csv-Datei ist vorwiegend als Werteransportmittel gedacht und ist daher nur schlecht für den Menschen lesbar. 
Daher ist es sinnvoll diese Csv-Datei in eine entsprechende Tabelle zu überführen. Damit erhöht sich die Lesbarkeit deutlich und macht 
die Auswertung zudem deutlich weniger fehleranfällig. Das IQB bietet zur Tabellenkonvertierung ein kleines Tool mit dem Namen: 
**ITC-Toolbox** für Windows an. Dieses ist frei verfügbar und kann von Anwender\*innen genutzt werden. Sie können das 
Programm über die IQB-Website herunterladen:

https://www.iqb.hu-berlin.de/institut/ab/it/itc-ToolBox

Nach dem Öffnen des Programms stehen folgende Optionen zur Auswahl:

* Booklet-Xlsx
* Login-Xlsx
* SysCheck csv- > xlsx
* Antworten und Logs csv -> xlsx

Mittels der ersten beiden Punkte ist es zum einen möglich aus einer Excel-Tabelle eine *Booklet.xml* zu erzeugen und zum 
anderen die Logindaten übersichtlicher zu organisieren. Näheres dazu entnehmen Sie bitte dem Kapitel:

[Testcenter / Vorbearbeitung Testdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Vorbearbeitung-der-Testdateien)

Mittels der letzten beiden Punkte können Csv-Dateien in Exceldateien (xlsx-Dateien) konvertiert werden. 
Wenn Sie zuvor heruntergeladenen Antworten und Logs eines Probanden in ein Xlsx-Format konvertieren möchten, 
betätigen Sie einfach den Button: *Antworten und Logs csv -> xlsx*. Anschließend wählen Sie den Ort aus an welchem sich die 
Dateien befinden und wählen einen Namen und einen Speicherort für die zu generierende Excel-Tabelle aus. 
Selbiges können Sie auch für zuvor heruntergeladene SysCheck-Dateien tun. Am Ende werden somit 3 Excel-Tabellen erzeugt, 
die Sie frei bezeichnen können.

Wie sind die Inhalte in diesen 3 Tabellen zu deuten?

**Tabelle Anworten:**

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 27.03.2021
Prio: high
todo:
  - Die Tabellenwerte entstammen einem alten Text auf GitHub. Nach Download einer 
    Antwort-/ und Logdatei vom Testcenter und Konvertierung in Excel
    haben die Spalten andere Namen als die in der Tbl aufgeführten. Martin berfragen ob die Angaben nachfolgend sicher noch gültig sind???? 
```

| Spaltenbezeichnung | Bedeutung |
| :------------- | :---------- |
|ID|Kombination aus anderen (nachfolgenden) Informationen. Diese ID wird benötigt, um eine Zeile eindeutig zu identifizieren. Es handelt sich um eine Testsitzung, also eine Testperson beantwortet ein konkretes Booklet. Diese Kombination ist nötig, weil eine Testperson mehrere Booklets haben könnte und in einem Booklet theoretisch dieselbe Unit enthalten sein kann (z. B. Motivationsabfrage). Es muss eindeutig sein, in welchem Booklet diese Unit platziert war.<br> Diese ID wird auch in den anderen zwei Tabellen verwendet, so dass hierüber eine Zusammenführung der Informationen erfolgen kann.|
|Group|Gruppe, in der das Anmelde-Login platziert war. Dies ist normalerweise nur ein Ordnungsmerkmal für das Monitoring der Durchführung.|
|Login+Code|Entsprechend der Anmeldung der Testperson|
| Booklet | ID des Booklets |
| Variablen nach dem Schema<br>`<Unit-ID>##<innere ID>`<br>z. B. `EL105R##canvasElement10` | Der Player des Testcenters speichert im bisherigen Modell die Antwortdaten als Paarung ID->Wert ab, wobei nicht definiert ist, was ID kennzeichnet (Item, Aspekt eines Items, Eingabeelement des Formulars usw.; hier mal als innere ID bezeichnet). Sicher ist nur, dass diese ID innerhalb der Unit eindeutig ist, und da die Unit-ID eindeutig für das Testheft ist, erlaubt die Kombination Unit-ID mit dieser inneren ID eine eindeutige Zuordnung des Antwort-Wertes zu einer Testperson in einem Booklet, wodurch sich die übliche zweidimensionale Struktur der Antwortdaten ergibt.<br> Es werden nur Units berücksichtigt, die tatsächlich Antwortdaten produziert haben. Reine Textseiten, die z. B. nur Instruktionen enthalten, werden nicht in die Tabelle aufgenommen.<br>Die Variablenspalten werden alphabetisch sortiert ausgegeben.<br>Sollte eine Unit mehrfach in einem Test vorkommen, fügt das System ab dem zweiten Vorkommen der Unit automatisch ein Suffix hinzu:<br>`<Unit-ID>%<n>`<br>n steht hier für die fortlaufende Nummerierung, beginnend mit 1 bei dem zweiten Vorkommen der Unit|

Die Zeilen dieser Tabelle sind nach ID sortiert. Sollte eine Testperson den Test nur gestartet, aber keine Antwortdaten abgeschickt haben, erscheint sie nicht in der Liste.


**Tabelle Logs:**

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 21.03.2021
Prio: high
todo:
  - Die Tabellenwerte entstammen einem alten Text auf GitHub. 
    Nach Download einer Antwort-/ und Logdatei vom Testcenter und Konvertierung in Excel
    haben die Spalten andere Namen als die in der Tbl aufgeführten. Martin berfragen ob nachfolgende Angaben sicher noch Gültigkeit haben????
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

**Tabelle Syscheck:**

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


```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 21.03.2021
Prio: high
todo:
  - Im alten Text von Martin würde jetzt hier noch etwas von Yaml-Datei stehen 
    mit Martin klären was das ist und wofür es verwendet wird.

```

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Modi-der-Testdurchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Vorbearbeitung-der-Testdateien">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.5 Modi der Testdurchführung

Bei der Definition der Anmeldung zur Durchführung eines Tests können verschiedene Modi gewählt werden. Die Testhefte bleiben unverändert, 
es wird nur ein Modus für eine spezielle Testperson festgelegt. Verschiedene Anmeldungen können also mit denselben Testheften zu 
unterschiedlichem Verhalten führen.

---

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

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.6-Konfiguration-der-Testdurchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Nachbearbeitung-der-Testdateien">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.6 Konfiguration der Testdurchführung

### Booklet Konfiguration

Es ist möglich Booklets entsprechend zu konfigurieren. Hierfür stehen einige Attribute zur Verfügung, die in der Booklet.xml 
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

---

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

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.7-Anmeldeoptionen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Modi-der-Testdurchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.7 Anmeldeoptionen

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 21.03.2021
Prio: low
todo:
  - Was gehört hier noch her? Mit Martin klären.
```
---

Für eine Testdurchführung erlaubt das IQB-Testcenter verschiedene Arten der Anmeldung der Testperson:

---

### Klassisch: Anmeldename, Kennwort
Beim Aufruf der Internet-Seite und damit der Webanwendung wird ein Formular präsentiert zur Eingabe dieser Daten. 
Diese Anmeldeform wird üblicherweise erwartet. Der Anmeldename wird im Klartext gezeigt, die Eingabe des Kennwortes erzeugt 
aber nur Punkte, d. h. man kann nicht mitlesen.

---

### Kurz: Nur Anmeldename
Das Kennwort kann weggelassen werden. Hier hat man keine geringere Sicherheit, wenn die Länge und Zeichenzusammensetzung 
des Namens hinreichend ungewöhnlich ist. Eine laufende Nummer am Ende ist z. B. problematisch, denn sie kann bei Kenntnis eines Namens 
erraten werden. Diese Anmeldeform sollte gewählt werden, wenn das Verbergen des Kennwortes stört.

---

### Noch kürzer: Link
Wenn nur ein Anmeldename ohne Kennwort als Login festgelegt wurde, dann kann man auch einen Link an die Testpersonen verschicken. 
Wenn "u8h5m2a4c3x2f2g8" der Anmeldename ist würde der Link so aussehen:
```
https://www.iqb-testcenter.de/#/u8h5m2a4c3x2f2g8
```
Dadurch macht man es noch einfacher: Auf den Link klicken, und man muss nur noch das Testheft wählen. Diese Form der 
Anmeldung kann z. B. bei Befragungen in Kombination mit dem Durchführungsmodus `run-hot-restart` verwendet werden: 
Es wird nur ein Login in einer Einladungs-E-Mail verschickt, und eine vorher unbekannte Anzahl Personen kann die Befragung starten.

---

### Länger: Anmeldename, Kennwort, Personencode
Es kann sein, dass die Testleitung Zeit hat, vor Eintreffen der Schülerinnen und Schüler alle Computer zu starten, 
einen Standard-User anzumelden, den Browser zu starten und die richtige Internet-Adresse aufzurufen. Dann ist es auch hilfreich, 
wenn auf jedem Computer schon Anmeldename und Kennwort eingegeben werden kann und also ein Anmeldeprozess gestartet wird. 
Anmeldename und Kennwort sind dann für die Gruppe gleich. Es reicht dann anschließend die Eingabe eines kurzen Personencodes durch die Testperson, 
um eine eindeutige Identifizierung sicherzustellen. Man spart so Testzeit und vermeidet Fehleingaben. Dieses Szenario bietet sich z. B. an, 
wenn man den Test nicht in der Schule, sondern in dem eigenen oder einem angemieteten Computer-Lab durchführt.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.8-IQB-Daten-Spezifikationen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.6-Konfiguration-der-Testdurchführung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.8 IQB Daten Spezifikationen

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 21.03.2021
todo:
  - Gehört das Kapitel hierher? Ist der Inhalt vollständig? Mit Martin klären.
```
---

### IQB-Definitionen für Verona-Daten

In diesem Repository sind alle Datenformate beschrieben, die das IQB im Zusammenhang 
mit Verona-Anwendungen nutzt. Verona steht hier für eine Initiative zur Spezifizierung 
von Schnittstellen, die im computerbasierten Testen genutzt werden können. Weitere 
Informationen zu Verona-Schnittstellen [hier](https://github.com/verona-interfaces/introduction).

#### Unit-Definitionen
Die Fragen eines Tests werden üblicherweise gruppiert. Obwohl auch eine Frage einzeln
auf einer Seite präsentiert werden kann, nimmt man oft mehrere Fragen, die inhaltlich 
eine Einheit bilden, zusammen. Diese sogenannte Unit kann man mit einer Aufgabe 
vergleichen, die mehrere Teilaufgaben hat.

Der Verona-Ansatz sieht vor, dass ein Testsystem jeweils die Daten einer Unit lädt 
und dann eine dazu passende Komponente zur Präsentation wählt (den sog. Player). Folgende 
Datentypen verwendet das IQB für seine Player:

* [iqb-scripted](unit-defs/manual_iqb-scripted.md): Die Unit-Definition besteht aus einem Script. 
Diese Folge von Anweisungen ist eine einfache Text-Datei, die in einem Texteditor bearbeitet
werden kann oder aus einem Hilfsprogramm automatisiert erzeugt wird. Es gibt keine Vorschriften zur 
Verarbeitung der Antworten (richtig/falsch usw.). Dieses Format wird vorrangig für 
Befragungen genutzt (z. B. Evaluationen oder Protokolle von Testsitzungen).

#### Player-Antwortdaten
Während der Durchführung eines Tests oder einer Befragung gibt der Player die 
Antwortdaten an das Testsystem zur Speicherung. Die Spezifikation dieser 
Antwortdaten ist wichtig, um nachfolgend eine korrekte Datenverarbeitung (Kodierung,
Analyse) zu gewährleisten:
* [iqb-key-value](responses/manual_iqb-key-value.md): Dieses JSON-Format speichert Antworten als 
Schlüssel-Wert-Paare in JSON-Notation. Der Schlüssel ist stets ein String, der Wert (aktuell in 
Version 1.0) ebenfalls. Da dieses Format keine weiteren Festlegungen
enthält, ist es zwar universell, aber erst mit vielen Zusatzinformationen aus dem 
Erhebungszusammenhang sinnvoll zu verarbeiten.

#### Steuerung für Tests/Befragungen
Die Verona-Schnittstellen beziehen sich jeweils auf eine Unit. Das IQB wird aber auch Konventionen
definieren, die sich auf die Unit-Abfolge im Rahmen eines Tests bzw. einer Befragung beziehen. Eine 
IQB-Software soll dann deklarieren, ob oder wie diese Konventionen umgesetzt sind.

Folgende Dokumentationen sind hierzu verfügbar:
* (IQB-Testcenter): Optionen zur Steuerung der Testdurchführung über die Booklet-Xml 
[hier](https://github.com/iqb-berlin/testcenter-frontend/blob/master/docs/booklet-config.md). 
* (IQB-Testcenter): Modi der Testdurchführung (festgelegt über Testtaker-Xml)
[hier](https://github.com/iqb-berlin/testcenter-frontend/blob/master/docs/test-mode.md). 
 

### IQB Verona Data Specifications

Verona interfaces are specifications concerning computer based assessment. You can learn 
more about this German initiative [here](https://github.com/verona-interfaces/introduction).

The IQB uses these interface specs for it's own applications. One important feature of these 
Verona interfaces is the black box approach for data exchange. Although the 
applications communicate via well defined channels, the structure of the transferred 
data is unknown. Only the name and version of data specification is needed to select 
the matching component.  

Nevertheless, every producer of data should document data structures. For the IQB, we 
do this in this repository. The manuals are in German language, because most of the 
people involved in data supply and processing welcome this language very much.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.9-Verona-Player">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.7-Anmeldeoptionen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.9 Verona Player

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 17.03.2021
Prio: low
todo:
  - Eventuell dieses Thema hier nicht aufführen??? 
  - Inhaltlich vollständig?
  - Querverweise zum Repo Verona Interfaces setzen
```
---

### Verona Player Einführung
In Deutschland gibt es für internationale (z. B. PISA) und einheitliche nationale 
Erhebungen (z. B. Bildungstrend) jeweils zentrale Einrichtungensdsadasdasda oder Firmen zur 
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

Da die Testsysteme eine Anpassung erfahren müssten, wenn Aufgabenformate geändert werden, 
kommt ein Player mit einer definierten Schnittstelle zum Einsatz. 
Der zu verwendende Player wird in der jeweiligen Unit definiert und mit der Unit geladen. Dieser spielt dann die in der 
Unit definierten Aufgabenformate ab. Die dazu gehörige Schnittstelle des Players gewährleistet eine Kompatibilität zu den Anwendungen, 
die bereits für die Vera Papierstudien genutzt wurden und weiterhin werden. 
Der Player wird daher auch Verona-Player und die Schnittstelle auch Verona-Schnittstelle genannt. 
Ändert sich ein Aufgabenformat, muss somit nur noch ein dazu passender Player geladen werden, 
der dieses Format auch abspielen kann. Durch den modularen Aufbau des Testcenters entfällt somit eine Anpassung 
der gesamten Testumgebung, wenn sich Aufgabenformate ändern. Stattdessen 
wird einfach der entsprechende Player für das Format geladen und in die Oberfläche des Testcenters intergriert.

Nachfolgend finden Sie einige Videos zum Thema:

* [Verona-Interfaces: 1.Einführung](https://box.hu-berlin.de/f/a6de8bd03626451a93d0/)
* [Verona-Interfaces: 2.Player-Model](https://box.hu-berlin.de/f/8f4b50975e9645af803b/)
* [Verona-Interfaces: 3.Player-API](https://box.hu-berlin.de/f/6c71fcdb9d7944d69dec/)

---

### Grundsätze Player Programmierung

Die folgenden Grundsätze bestimmen aktuell die Entwicklung von Verona-Playern am IQB. Sie sind nicht mit anderen Partnern bzw. Institutionen 
abgestimmt. Die Grundsätze sind teilweise noch nicht umgesetzt, sondern werden bei künftigen Änderungen implementiert.

#### Datenformat der Unit-Definition

Aus der Unit-Definition müssen Anwendungen erkennen, welcher Player benutzt werden soll, um die Unit anzuzeigen bzw. auszuführen. 
Das IQB hinterlegt hier nicht eine ID eines Players, sondern benennt das Datenformat. Dies ist universeller, 
denn es mag verschiedene Player geben, die das Datenformat unterstützen. Außerdem ergibt sich daraus auch der notwendige Editor 
bzw. die Liste der möglichen Editoren für die Änderung der Unit-Defintion.
Das Datenformat besteht aus einer ID und einer Version nach Semantic Versioning 2.0.0, getrennt durch Leerzeichen. Beispiel: `iqb-dan 3.2.3`. 
Es werden Player bzw. andere Programmierungen als kompatibel angesehen, die mindestens diese Version unterstützen sowie 
maximal die letzte Version des major-Elementes der Version. Für das Beispiel würde das bedeuten, dass ein Player mit dokumentiertem 
Datenformat `iqb-dan 3.4.0` oder `iqb-dan 3.34.7` als zulässig angesehen wird, aber die Versionen `iqb-dan 3.2.1` sowie `iqb-dan 4.0.0` nicht.

#### Player-Registry

Für Player und andere Module sollten Metadaten hinterlegt werden, die die Eignung für bestimmte Use Cases und Datenformate 
anzeigen und die Auswahl durch eine Anwendung unterstützen. Wir stellen uns einen Server vor, über dessen API Anfragen gestellt 
und Referenzen auf Player zurückgegeben werden können. Diese Referenzen sollten vorzugsweise DOI-Kennungen sein, 
die dann auf GitHub-Dateien aufgelöst werden. Dieses Verfahren ist in Vorbereitung, wird aber aktuell als übertrieben 
angesehen angesichts der geringen Anzahl der Player. Wer Anwendungen für Verona-Plugins erstellt, 
sollte ein manuelles Einspielen der erforderlichen Player/Editoren usw. vorsehen.

#### Kleine fokussierte Player

Das IQB wird für verschiedene Studien bzw. Befragungen unterschiedliche Player einsetzen. Man könnte Player konzipieren, 
die alle möglichen Interaktionselemente abdecken, das IQB möchte aber eher typische Interaktionselemente als Basisausstattung 
umsetzen und dann zusätzliche Player bereitstellen, die spezielle Interaktionselemente implementieren. 
Wir möchten z. B. eine GeoGebra-Implementation nicht auch bei Sprachtests laden oder Formate zur Kommasetzung in Mathematik-Tests bereitstellen. 
Wo dann genau die Grenze zu ziehen ist wird sich zeigen, aber tendenziell möchten wir kleine fokussierte Player bereitstellen.

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.10-System-Check">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.8-IQB-Daten-Spezifikationen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.10 System Check

### Was ist ein System-Check?

Es ist bitter, wenn man erst während der Studiendurchführung bemerkt, dass die Hardware oder die Software-Ausstattung für einen 
Online-Test nicht geeignet ist. Der System-Check ist ein Weg, vorab diese Eignung zu prüfen. Man kann natürlich nicht alle Probleme erkennen 
und vielleicht hat man für bestimmte Probleme auch keine Lösung parat, aber man kann die Ausfall- und damit die Frustrate deutlich senken.

### Planung

Nach dem Einrichten eines Systemchecks erscheint auf der Seite der Webanwendung (hier: IQB-Testcenter) ein neuer Schalter `System-Check`. 
Man kann alle Interessierten einladen, darüber zumindest eine Prüfung der Internetanbindung vorzunehmen (Bandbreite) und eine Anzahl von 
Hardware- und Softwareinformationen anzuzeigen. Außerdem stehen folgende Optionen zur Verfügung:

* Probeweises Aufrufen einer Testaufgabe: Eine speziell dafür entwickelte Testaufgabe wird gezeigt und man kann die Bearbeitungselemente auswählen,
  ändern und so prüfen, ob die Aufgabenelemente wie erwartet funktionieren.
* Fragebogen beantworten: Die Person, die den System-Check durchführt, kann eine Liste von Fragen beantworten. 
  Die Fragen können sich zunächst auf die vorherige Testaufgabe beziehen (wurde die Audio-Datei abgespielt? 
  Passte alles auf den Bildschirm? usw.), aber auch weitere Informationen zur Ausstattung vor Ort können erfragt werden 
  (wieviele Plätze sind im PC-Lab?, Können die Testpersonen sich gegenseitig auf den Bildschirm schauen?, Gibt es ein Whiteboard? usw.)
* Bericht abschicken: Es kann festgelegt sein, dass die Daten gespeichert werden zur späteren Auswertung. 
  Dazu sollte ein Kennwort vergeben werden und eine weitere Kennung, anhand der die Zuordnung der Daten z. B. 
  zu einer bestimmten Schule möglich ist.

### XML-Definition schreiben

Ein System-Check wird über eine XML-Datei gesteuert. Außerdem kann eine Unit-Definition hinzugelegt werden (XML-Datei, 
VOUD-Datei und zugehöriger Player). All diese Dateien sind über einen beliebigen Arbeitsbereich in das Testcenter zu laden. 
Die Berichte des System-Checks werden dann auch in diesem Arbeitsbereich gespeichert.

Der genaue Aufbau und die möglichen Parameter der System-Check-XML sind in einer 
[Schemadefinition](https://github.com/iqb-berlin/testcenter-backend/blob/master/definitions/vo_SysCheck.xsd) festgelegt. 
Anhand einer Beispieldatei sollen nachfolgend die Optionen beschrieben werden:

```xml
<?xml version="1.0" encoding="utf-8"?>
<SysCheck xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_SysCheck.xsd">
	<Metadata>
		<Id>LAL8_2021</Id>
		<Label>System-Check für LAL8 2021</Label>
		<Description>Version 4.2.2021</Description>
	</Metadata>
	<Config unit="SC3" savekey="fichtelgebirge">
		<UploadSpeed min="1024" good="2048" maxDevianceBytesPerSecond="10000" maxErrorsPerSequence="0" maxSequenceRepetitions="15">100000, 200000, 400000, 800000</UploadSpeed>
		<DownloadSpeed min="1024" good="2048" maxDevianceBytesPerSecond="200000" maxErrorsPerSequence="0" maxSequenceRepetitions="15">400000, 800000, 1600000, 3200000</DownloadSpeed>		
		<Q id="1" type="header" prompt="Abschnitt I: Computerübergreifende Fragen – diese müssen nur einmal online eingegeben werden."></Q>
		<Q id="2" type="radio" prompt="1. Wer ist an der Schule die Ansprechperson für technische Fragen?">der Schulkoordinator/die Schulkoordinatorin selbst#eine andere Person (Eingabe nächstes Feld)#es gibt keine Ansprechperson</Q>
		<Q id="2a" type="text" prompt="Weitere Informationen zur Ansprechperson"/>
		<Q id="3" type="string" prompt="2. In welchem Raum wurde die Systemdiagnose durchgeführt? Bitte geben Sie die Raumbezeichnung an."/>
		<Q id="4" type="text" prompt="3. Bitte notieren Sie ggf. Informationen zur Erreichbarkeit des Raumes."/>
		<Q id="5" type="string" prompt="4. Wie viele Computer gibt es im Raum?"/>
		<Q id="6" type="string" prompt="5. Wie viele funktionstüchtige Computer gibt es im Raum?"/>
		<Q id="7" type="text" prompt="6. Wie würden Sie den allgemeinen Zustand der Computer (und Bildschirme, Mäuse, Tastaturen) beschreiben? 
	z. B. modern, veraltet, gut instandgehalten etc."/>

		<Q id="8" type="header" prompt="Abschnitt II: Fragen zum Account für die Systemdiagnose"></Q>
		<Q id="9" type="radio" prompt="1. Ist dies ein allgemeiner Account?">der Account kann für alle PC verwendet werden#der Account ist nur für bestimmte PC zur Anmeldung möglich#konnte Reichweite des Accounts nicht ermitteln</Q>
		<Q id="10" type="radio" prompt="2. Ist dies ein Account mit Zugriff auf USB?">ein mobiler Browser konnte direkt von USB gestartet werden#ein mobiler Browser konnte auf den Desktop kopiert und ausgeführt werden#ein mobiler Browser konnte nicht gestartet werden</Q>
		<Q id="11" type="text" prompt="3. Gibt es Änderungen dieser Situation im Testzeitraum bis Mai? Bitte beschreiben!"/>

		<Q id="12" type="header" prompt="Abschnitt III: Fragen zum Funktionieren der Aufgabe"></Q>
		<Q id="13" type="text" prompt="1. Besonderheiten beim Starten des Browsers und beim Zugriff auf das Testcenter"/>
		<Q id="14" type="text" prompt="2. Allgemeine Auffälligkeiten bei der Darstellung der Aufgabe"/>
		<Q id="15" type="text" prompt="3. Probleme beim Abspielen der Audio-Sequenz"/>
		<Q id="16" type="text" prompt="4. Klarheit der Darstellung der Grafik"/>
		<Q id="17" type="text" prompt="5. Auffälligkeiten beim Scrollen"/>
		<Q id="18" type="text" prompt="6. Auffälligkeiten beim Navigieren zwischen Seiten"/>
		<Q id="19" type="text" prompt="7. Anmerkungen zur Kästchendarstellung der Ankreuzoptionen"/>
		<Q id="20" type="check" prompt="8. Nutzung des mobilen Browsers.">Beim Systemcheck musste der mobile Browser benutzt werden.</Q>
	</Config>
</SysCheck>
```
#### Kopfdeklarationen

Die XML-Datei sollte man mit einem Editor bearbeiten, der zumindest eine Validierung vornehmen kann. 
Das bedeutet, dass nicht nur die allgemeine Syntax geprüft wird (stets schließende Tags, keine Leerzeichen 
vor/hinter einem Attribut usw.), sondern nur Elemente und Attribute akzeptiert werden, die in einer System-Check-XML erlaubt sind. 
Dazu muss der Editor die Schemadatei kennen. Dies erfolgt üblicherweise über die Deklaration `noNamespaceSchemaLocation` wie im Beispiel gezeigt.
Gute Editoren unterstützen die Bearbeitung dann außerdem mit automatischer Vervollständigung.

#### Metadaten

Zur Kennzeichnung und Beschreibung der Datei sollen eine ID und ein Label vergeben werden. Ersteres dient der internen Zuordnung auch der 
Berichte, letzteres wird bei der Beschriftung des Start-Schalters verwendet. Eine Beschriftung kann helfen, verschiedene Versionen eines 
Systemchecks zu unterscheiden.

#### Netzwerkverbindung

Die Angaben in den Bereichen `UploadSpeed` und `DownloadSpeed` sind rein technischer Natur und sollten nur angepasst werden, 
wenn die Ergebnisse überwiegend unerwartet sind. Bitte fragen Sie die Spezifikation beim Entwickler-Team nach!

#### Unit

Wenn im Element `Config` ein Attribut `unit` gefunden wird, dann erfolgt nach dem Test der Verbindungsqualität die Anzeige einer Unit. 
Diese Befragungsseite bzw. Testaufgabe soll möglichst alle Element-Typen enthalten, die später auch im Test bzw. der Befragung benutzt werden. 
Es ist also z. B. hier unnötig, eine Audio-Datei einzubauen, wenn im Test keine Hörverstehensaufgabe vorkommt.

Es muss natürlich in den Arbeitsbeich auch eine Unit mit dieser ID hochgeladen werden. Außerdem ist der in der Unit-Definition genannte 
Player im Arbeitsbereich bereitzustellen.

#### Bericht speichern

Wenn im Element `Config` ein Attribut `savekey` gefunden wird, dann können die Ergebnisse des System-Checks abschließend gespeichert werden. 
Die letzte Seite enthält dann einen Schalter `Bericht senden` und es wird ein Kennwort erfragt.

#### CustomTexts (in Vorbereitung)

Hierüber werden einige Textbausteine geliefert. Bitte wählen Sie aus 
[dieser Liste](https://github.com/iqb-berlin/testcenter-frontend/blob/master/docs/custom-texts.md) die Schlüsselworte mit dem Präfix `syscheck_`.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.11-Versionsstand">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.9-Verona-Player">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.11 Versionsstand

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 29.03.2021
Prio: low
todo:
  - Was kann zum Versionsstand geschrieben werden -> mit Martin besprechen!

```
---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.10-System-Check">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---