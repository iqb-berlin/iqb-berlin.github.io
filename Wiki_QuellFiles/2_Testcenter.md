# 2.Testcenter

**Vorab:**

Grundlegende Informationen zum Testcenter Frontend erhalten Sie auch im TBA Einführungskapitel.
Das Testcenter besteht aus einem Back- und einem Frontend. In diesem Kapitel wird nur auf das Frontend eingegangen,
da Anwender vorwiegend damit in Berührung kommen.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="">
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

Das Testcenter beinhaltet eine Datenbank, die zur Speicherung von Test und Metadaten verwendet wird.
Des Weiteren werden mithilfe des Testcenters die interaktiven Inhalte eines Tests wiedergegeben. 
Wobei nicht nur finale Tests durchgeführt werden können, sondern auch Probedurchläufe, die den Organisator\*innen einen Überblick 
verschaffen an welchen Stellen des Test eventuelle noch Änderungen durchgeführt werden sollten. 
Nachfolgend ist noch einmal aufgelistet welche Möglichkeiten das Testcenter bietet:

**Testdurchführung**

* finale oder probeweise Testdurchführung (abspielen der Aufgaben)

**Anlegen eines Tests**

* upload, löschen und download der Testdateien

**Administration**

* Testverwaltung
* Benutzerverwaltung/ Benutzerzugänge

Detailliert betrachtet besteht das Testcenter aus weiteren softwaretechnischen Komponenten, die hier, obwohl die meisten Andwender\*innen
damit nicht in Kontakt kommen dürften, einmal erwähnt werden sollten. Eine für die meisten Anwender\*innen häufig vorkommende Begrifflichkeit
dürfte der so genannte Verona Player sein. Dieser Player ist in das Testcenter intergriert und ist für die Wiedergabe der Aufgabeninhalte
zuständig. Über eine definierte Schnittstelle meldet dieser außerdem jegliche Interaktionen auf den Testseiten an das Testcenter.  
Näheres zum Thema Verona entnehmen Sie bitte dem gleichnamigen Kapitel. Es gibt weitere Schnittstellen und Umgebungsmodule, 
die direkt oder indirekt mit dem Testcenter zusammenarbeiten, diese sind für Interessierte nachfolgend dargestellt.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Umgebungsmodule_final.png)

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.2 Anmeldung und Laden eines Tests

### Anmeldung am Testcenter

Wie dem Einführungskapiteln bereits zu entnehmen war, besteht ein Technologiebasierter Test aus mehreren Datei.
Jede dieser Dateien bietet spezifische Möglichkeiten den Test bzgl. Aussehen und Ablauf zu beeinflussen. Um einen Test im Testcenter 
abspielen zu können oder Dateien eines Tests in das Testcenter zu laden, zu löschen, oder aus dem Testcenter herunterzuladen, 
bedarf es unterschiedlicher Anmeldearten. Dabei muss in zwei Gruppen unterschieden werden: 

* der oder die Testorganisator\*in
* die Testperson

Der oder die Testorganisator\*in übernimmt die administrative Rolle einer Testdurchführung, kann Dateien eines Tests bearbeiten, in das 
Testcenter laden, Ablauf und auch Zugang zum Test für die Testpersonen festlegen. Es wird also ein Zugang zum Testcenter benötigt. Dieser Zugang
kann nur von den Administrator\*innen des Testcenters angelegt werden. Wer ist nun aber der Administrator des Testcenters?<br> 
Derzeitig werden die meisten Testdurchführenden auf das Testcenter zugreifen, welches die hausinternen IT-Strukturen 
(Server, Netzwerke) des IQB nutzt. Mit der weiteren Etablierung des Technologiebasierten Testens in den Bildungseinrichtungen, 
wird der Betrieb beider Systeme, sowohl Teststudio als auch Testcenter, zunehmend in den eigenene IT-Strukturen der jeweiligen Bildungseinrichtungen 
zum Einsatz kommen. Administrator\*innen des Testcenters und auch des Teststudios sind somit diejenigen, die für die IT-Struktur, in welcher
die Systeme betrieben werden, verantwortlich sind. Sobald Sie die entsprechenden Zugangsdaten von administrativer Seite erhalten haben, können Sie
nach Aufruf einer entsprechenden Internetadresse in einem Webbrowser, die Anmeldung am Testcenter vornehmen. Auch die einzugebene Internetadresse ist
wiederum abhängig von der IT-Struktur in welcher das Testcenter betrieben wird. Möchten Sie das Testcenter in der IQB IT-Strukut nutzen, ist folgende
Adresse im Browser einzugeben: https://www.iqb-testcenter.de. Nach erfolgreicher Anmeldung können dann Daten geladen oder auch gelöscht werden.


Die eigentliche Testdurchführung oder auch ein Probelauf für Testorganisator\*innen erfolgt mit separaten Zugangsdaten. 
Diese Zugangsdaten legen allein die Testorganisator\*innen fest. Dies erfolgt durch Anpassung einer bestimmten Datei, 
die Bestandteil eines jeden Tests ist. Diese Datei trägt den Namen: *Testtakers.xml*. In dieser können Zugangsdaten festgelegt und zusätzlich ein 
Modi gesetzt werden. Der Modi bestimmt den Testablauf, also ob es sich z.B. um einen finalen Test oder nur einen Probedurchlauf für die Testorganisator\*innen
handelt. Nachdem die Dateien eines Tests inklusive, der bzgl. des Logins angepassten *Testtakers.xml*, in das Testcenter geladen wurden, 
können bei einer Neuanmeldung im Testcenter die in der *Testtakers.xml* gesetzten Zugangsdaten zur Anmeldung genutzt werden. 
Anschließend wird der Test auf die über den Modi gewünschte Art und Weise abgespielt. 

Bsp.:<br>
Nehmen wir an Sie als Organisator\*in wollen für den Schüler Jakob einen finalen Test vorbereiten. 
So ist in der *Texttakers.xml* des gewünschten Tests ein `Username` für Jakob, ein `pw` (Passwort) und der Modi, wie der Test ablaufen soll,
auszuwählen und einzutragen. Nachdem der Test inklusive der *Testtakers.xml* in das Testcenter geladen wurde, kann Jakob sich mit diesen von Ihnen
eingetragenen Zugangsdaten am Testcenter anmelden und seinen Test in der von Ihnen gewünschten Art und Weise durchlaufen.

Mehr zu diesem Thema erfahren Sie auch im Kapitel: [Testcenter / Bearbeiten eines Tests](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Bearbeiten-eines-Tests)

### Laden eines Tests

Nach der Anmeldung als Testorganisator\*in am Testcenter, können die Bestandteile (Dateien) des Tests geladen werden.
Auch die Löschung einzelner Datei und das Herunterladen ist möglich. Während des Hochladens in das Testcenter findet eine 
Plausibilitätsprüfung statt. Dabei wird überprüft ob die deklarierten Dateien in einer Datei während des Hochladens auch gefunden werden. 
Ein einfaches Beispiel: In der Booklet.xml werden die gewünschten Units deklariert. Laden Sie zuerst die Booklet.xml und erst anschließend
die Unit.xml wird eine Fehlermeldung generiert, weil die in der Booklet.xml deklarierten Units nicht gefunden werden. Es ist daher wichtig
die richtige Reihefolge beim Upload einzuhalten. Eine Übersicht verschafft das nachfolgende Bild:

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Upload_Dateien_final.png)

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.3 Bearbeiten eines Tests

Die im Teststudio erzeugten Dateien können vor dem Upload in das Testcenter berarbeitet werden.<br>
Betrachten Sie dazu auch noch einmal das Kapitel:

[TBA Einführung -> Ablauf Entwurf und Durchführung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2-Ablauf-Entwurf-und-Durchführung)

---

**Bevor es los geht ein paar Grundlagen:**

Bei den zu bearbeitenden Dateien handelt es sich um Xml-Dateien. Xml ist ein textbasiertes Datenformat.   
Die Daten werden also in Textform in einem Text hinterlegt. Xml-Dateien können daher auch einfach mittels eines Texteditors bearbeitet werden.
Damit die Daten im Text gefunden werden können, muss eine bestimmte Struktur eingehalten werden. Anschließend kann eine entsprechende Gegenstelle, 
in unserem Fall das Testcenter, mittels eindeutiger Schlüsselwörter (Tags oder Elemente) die Daten im Text finden und nutzen. 
Xml-Dateien bestehen immer aus Elementen und ggf. mehreren Unterelementen. Der Beginn eines Elements wir mit zwei spitzen Klammern `<Element Start>` eingeleitet und wie folgt beendet: `</Element Ende>`. 
Jedes Element kann außer den eigentlichen Daten, welche zwischen zwei spitzen Klammern stehen, zusätzliche Attribute enthalten. 
Attribute werden immer in der folgenden Form ausgedrückt: `Name Attribut = "Attributwert"` und befinden sich innerhalb eines Elementenblocks, sprich innerhalb der beiden spitzen Klammern. 
Es gibt auch Elemente die Attribute aber keine Daten enthalten und umgekehrt. Einfache Bsp. sind nachfolgend aufgeführt:

1. Element ohne Attribute mit Daten:<br>

   Daten sind in diesem Fall der Text zwischen den spitzen Klammern: `"Sekundarstufe I Englisch Ansichtsaufgaben"`.

  ```xml
    <Label>Sekundarstufe I Englisch Ansichtsaufgaben</Label>
  ```

2. Element mit Attributen ohne Daten:<br>

   Hier gibt es 3 Attribute: `id`, `lable` und `lableshort`. Alle 3 Attribute enthalten in diesem Fall Attributwerte.<br>
   Diese sind in Hochkommata gefasst und werden mit einem Gleichheitszeichen dem Attribut zugeordnet. 
   Das keine Daten enthalten sind, ist gut an dem Schließen des Elementes **Unit** zu erkennen. Denn das Element endet nicht mit: `</Unit>`, sondern nur mit: `/>`. 
   Diese Syntax gibt an, dass keine Daten folgen.

```xml
   <Unit id="Unit1" label="1. Postcard" labelshort="1" />
```

3. Element mit Daten und Attributen:<br>

   Attribut ist hier: `key`. Dieses bekommt den Attributwert `force_presentation_complete` zugewiesen.
   Datum ist der Wert: `ON`.

```xml
    <Config key="force_presentation_complete">ON</Config>
````


Manche Attributwerte können frei gewählt werden, manche müssen sich an Vorgaben halten.<br> 
Nachfolgend wird nun auf die Elemente unserer Testdateien und deren Attribute und Daten eingegangen.<br>
In der Tabelle finden Sie immer das entsprechende Unterelement eines Hauptelementes und dessen Attribute und Daten (falls vorhanden).
  
---

### Attribute und Daten TESTTAKERS.xml

`METADATA`<br>

<table>
	
<tr>
    <td>Description:</td>
    <td>>xxx<</td>
	<td>Datum</td>
    <td>frei wählbarer Text für die Metadaten Beschreibung</td>
</tr>

</table>

```xml
<?xml version="1.0"?>
<Testtakers>
  <Metadata>
    <Description>
     Diese Datei enthält Informationen zur Art des Logins und der Testdurchführung.
    </Description>		
  </Metadata>
  ...
```
---

`CUSTOMTEXTS`<br>

<table>
	
<tr>
    <td>CustomText:</td>
    <td>key</td>
    <td>Attribut</td>
    <td>Vordefinierter Wert. Erzeugt einen Custom Text. Siehe <b>Custom Text Configuration</b> im Kapitel:
	<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Konfiguration-der-Testdurchf%C3%BChrung">TBA Einführung / Konfiguration der Testdurchführung</a></td   
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
  ...
```
---

`GROUP`<br>

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
    <td>Vordefinierter Wert. Bestimmt wie ein Test ablaufen soll (finaler Test oder Probetest etc.).<br>Siehe: <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Modi-der-Testdurchf%C3%BChrung">Modi der Testdurchführung</a></td>
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
    <td>Frei wählbarer Wert. Die zugehörige Booklet.xml muss den selben Namen tragen (Groß-/Kleinschreibung beachten!)</td>
</tr>

</table>

```xml
 <Group id="Gruppe1" label="Dies ist die erste Gruppe.">
    <Login name="user1" mode="run-demo" pw="123">
      <Booklet>Booklet1</Booklet>
    </Login>
 </Group>
</Testtakers>

```

---

### Attribute und Daten BOOKLET.xml

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
    <td>Frei wählbarer Wert. Bezeichnet die Unit. Die zugehörige Unit.xml muss den selben Namen tragen (Groß/-Kleinschreibung beachten!).</td>
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

### Attribute und Daten UNIT.xml

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

### Namensgebung

```yaml
Dokumentstatus: Entwurf (Tobias Huste)
Stand: 17.03.2021
to do:
  - Wie sind die Dateien zu benamen, wie wird aufgerufen ID oder Dateinamen
  
```
---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.4 Modi der Testdurchführung

Bei der Definition der Anmeldung zur Durchführung eines Tests können verschiedene Modi gewählt werden. Die Testhefte bleiben unverändert, 
es wird nur ein Modus für eine spezielle Testperson festgelegt. Verschiedene Anmeldungen können also mit denselben Testheften zu unterschiedlichem Verhalten führen.

### Wo wird das festgelegt?
Die Festlegung erfolgt in der Testtaker-Xml im Element `Login` im Attribut `mode`:

```xml
<?xml version="1.0" encoding="utf-8"?>
  <Testtakers
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Testtakers.xsd">

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

### Welche Modi gibt es?
| Modus | Erläuterung |
| ----- | -------- |
| run-hot-return | Es wird angenommen, dass die finale Testperson den Test durchführt. Alle Beschränkungen der Testheftdefinition sind aktiv. Die Testperson kann bei einem Browserabsturz oder halt später zurückkehren und erhält alle gegebenen Antworten wieder angezeigt. |
| run-hot-restart | Wie oben, nur dass bei einer erneuten Anmeldung die vorherigen Daten nicht geladen werden. Statt dessen wird eine neue Person angenommen und die Antworten unter einer neuen Kennung gespeichert. Dadurch ist es möglich, dieselben Zugangsdaten an viele Menschen zu schicken (z. B. bei Befragungen einer nicht genau bekannten Gruppe). |
| run-trial | Zum Ausprobieren: Viele Beschränkungen gelten (s. u.). |
| run-review | Zum Ausprobieren: Einige Beschränkungen gelten nicht (s. u.). |
| run-demo | Kein Speichern, keine Beschränkungen (s. u.). |
| monitor-group | Reserviert zur Nutzung der Testleitungskonsole. |

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
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.5 Konfiguration der Testdurchführung

### Booklet Konfiguration

Es ist möglich Booklets entsprechend zu konfigurieren. Hierfür stehen einige Attribute zur Verfügung, die in der Booklet.xml (wenn gewünscht) anzugeben sind. Alle verwendbaren Attribute befinden sich in einer separaten Konfiguraionsdatei (booklet-config.json) auf die das Testcenter zugreifen kann. Möchten Sie einzelne Attribute nutzen, müssen Sie das Attribut und den gewünschten Wert (Datum) in der Booklet.xml unter "BookletConfig" angeben. 

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


Nachfolgend finden Sie eine Übersicht über die verwendbaren Attribute und deren Bedeutung. **Achten Sie bei der Verwendung dieser Parameter auf die richtige Schreibweise (Groß-/Kleinschreibung)!**

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

Diese Anwendung ermöglicht es zur Laufzeit Änderungen an Texten durchzuführen. Dies kann notwendig sein, wenn Standardtitel, Eingabeauffforderungen oder Erklärungen nicht zur spezifischen Umgebung, in welcher das Testcenter ausgeführt wird, passen.
Alle möglichen CustomText Attribute sind in einer Konfigurationsdatei deklariert, die das Testcenter ausliest. Daher können auch nur CustomText Attribute verwendet werden, die in dieser Datei deklariert sind. Eine Übersicht der verfügbaren Attribute und deren Bedeutung entnehmen Sie bitte der Liste weiter unten. Nach dem Attribut kann dann ein frei gewählter Text angegeben werden. In dem unteren Code würde nun der Titel der Hauptwanwendung (Attribut: app_title) wie folgt lauten: "Titel der Anwendung". CustomText kann in der Login.xml (Testtakers.xml) oder im Systemcheck konfiguriert werden.

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

Nachfolgend finden Sie eine Übersicht über die verwendbaren Attribute und deren Bedeutung. **Achten Sie bei der Verwendung dieser Attribute auf die richtige Schreibweise (Groß-/Kleinschreibung)!**


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
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

## 2.6 Anmeldeoptionen

Für eine Testdurchführung erlaubt das IQB-Testcenter verschiedene Arten der Anmeldung der Testperson:

### Klassisch: Anmeldename, Kennwort
Beim Aufruf der Internet-Seite und damit der Webanwendung wird ein Formular präsentiert zur Eingabe dieser Daten. Diese Anmeldeform wird üblicherweise erwartet. Der Anmeldename wird im Klartext gezeigt, die Eingabe des Kennwortes erzeugt aber nur Punkte, d. h. man kann nicht mitlesen.

### Kurz: Nur Anmeldename
Das Kennwort kann weggelassen werden. Hier hat man keine geringere Sicherheit, wenn die Länge und Zeichenzusammensetzung des Namens hinreichend ungewöhnlich ist. Eine laufende Nummer am Ende ist z. B. problematisch, denn sie kann bei Kenntnis eines Namens erraten werden. Diese Anmeldeform sollte gewählt werden, wenn das Verbergen des Kennwortes stört.

### Noch kürzer: Link
Wenn nur ein Anmeldename ohne Kennwort als Login festgelegt wurde, dann kann man auch einen Link an die Testpersonen verschicken. Wenn "u8h5m2a4c3x2f2g8" der Anmeldename ist würde der Link so aussehen:
```
https://www.iqb-testcenter.de/#/u8h5m2a4c3x2f2g8
```
Dadurch macht man es noch einfacher: Auf den Link klicken, und man muss nur noch das Testheft wählen. Diese Form der Anmeldung kann z. B. bei Befragungen in Kombination mit dem Durchführungsmodus `run-hot-restart` verwendet werden: Es wird nur ein Login in einer Einladungs-E-Mail verschickt, und eine vorher unbekannte Anzahl Personen kann die Befragung starten.

### Länger: Anmeldename, Kennwort, Personencode
Es kann sein, dass die Testleitung Zeit hat, vor Eintreffen der Schülerinnen und Schüler alle Computer zu starten, einen Standard-User anzumelden, den Browser zu starten und die richtige Internet-Adresse aufzurufen. Dann ist es auch hilfreich, wenn auf jedem Computer schon Anmeldename und Kennwort eingegeben werden kann und also ein Anmeldeprozess gestartet wird. Anmeldename und Kennwort sind dann für die Gruppe gleich. Es reicht dann anschließend die Eingabe eines kurzen Personencodes durch die Testperson, um eine eindeutige Identifizierung sicherzustellen. Man spart so Testzeit und vermeidet Fehleingaben. Dieses Szenario bietet sich z. B. an, wenn man den Test nicht in der Schule, sondern in dem eigenen oder einem angemieteten Computer-Lab durchführt.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---