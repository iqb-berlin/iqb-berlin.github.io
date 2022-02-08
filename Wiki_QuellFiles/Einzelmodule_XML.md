<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Arbeiten mit Xml-Dateien (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

> XML ist ein Standardformat und wird durch Texteditoren unterstützt. Daher sind einige Dateien für die Definition von Daten in den IQB-Anwendungen in diesem Format hinterlegt. Der folgende Text soll Neulingen dieses Format nahebringen.

XML ist ein textbasiertes Datenformat. Die Daten können einfach mittels eines Texteditors bearbeitet werden. Beispiele sind Notepad++ oder Sublime. Viele Editoren bieten Ergänzungsmodule für die Arbeit mit XML-Dateien. Diese erleichtern die Bearbeitung durch farbliche Hervorhebung der XML typischen Bestandteile und erkennen Fehler in der XML-Syntax (z. B. schließendes Element fehlt) gemeldet.

Damit die Daten im Text gefunden werden können, muss eine bestimmte Struktur eingehalten werden. Anschließend kann eine entsprechende Gegenstelle z.B. das IQB-Testcenter mittels eindeutiger Schlüsselwörter (Tags oder Elemente) die Daten im Text finden und nutzen.
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

Um eine Validierung anzustoßen, fügt man zunächst in den Kopf der XML-Datei (also in das Wurzelelement) einen Verweis auf die Schema-Datei ein. Das IQB hat für alle XML-Dateien solche Schema-Dateien entwickelt. Für eine `Unit-Xml` wäre z. B. das Hauptelement folgendermaßen zu ändern:

```xml
    <Unit
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Unit.xsd">
```
Es sollte stets die aktuelle Version im Pfad zur Schema-Datei benutzt werden.

Außerdem muss für die automatische Validierung ein Editor verwendet werden, der diese Validierung unterstützt. Das IQB empfiehlt Notepad++.


<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Booklet-Xml (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

<table>
  <tr>
    <td><a href="#Attr_Daten">Attribute und Daten</a></td>    
	<td><a href="#Konfiguration">Booklet Konfiguration</a></td>
  </tr>
</table>

Die Testheft-Definition besteht aus einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](Arbeiten-mit-Xml‐Dateien).

> **Die in der Xml-Datei angelegten Attribute und Elemente sind nicht frei wählbar, sondern orientieren sich an einer Schema-Definition. Diese gibt vor, welche Elemente und Attribute verwendet werden dürfen. Die Schema Definition für die Booklet.xml ist [hier](https://github.com/iqb-berlin/testcenter-backend/blob/master/definitions/vo_Booklet.xsd) ersichtlich.**

Nachfolgend werden die Attribute und deren Bedeutung beschrieben. Die Zuordnung der Attribute erfolgt nach Element.

### <a name="Attr_Daten"></a>Attribute und Daten

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

`UNITS`

<table>

<tr>
    <td>Unit:</td>
    <td>ID</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert. Wert muss in gleicher Schreibweise auch in der entsprechenden Unit unter ID aufgeführt sein!</td>
</tr>
<tr>
    <td>Unit:</td>
    <td>Label</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert zur Bezeichnung der Unit.</td>
</tr>
<tr>
    <td>Unit:</td>
    <td>labelshort</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert zur Bezeichnung der Navigationsleiste im Testcenter.</td>
</tr>
<tr>
    <td>Unit:</td>
    <td>alias</td>
    <td>Attribut</td>
    <td></td>
</tr>

</table>

```xml
<Unit id="Unit_Start" label="Beispielhafte Startseite" labelshort="1" alias=""/>
```

<table>

<tr>
    <td>Testlet:</td>
    <td>ID</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert.</td>
</tr>
<tr>
    <td>Testlet:</td>
    <td>Label</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert zur Bezeichnung des Testlets.</td>
</tr>

</table>

```xml
<Testlet id="Examples" label="Beispiele">
	
</Testlet>
```

Ein _Testlet_ ist eine Gruppe von Units mit gemeinsamen Restriktionen, beispielsweise einer gemeinsamen Zeitbegrenzung. _Testlets_ können auch rekursiv geschachtelt werden, mit anderen Worten: Ein Testlet kann weitere Testlets enthalten. 

Die Testlets der obersten Ebene werden auch Test_blöcke_ genannt.

Zeitbegrenzungen (Restrictions/TimeMax) in geschachtelten Testlets werden ignoriert, sofern diese ebenfalls eine Zeitbegrezung haben.

<table>

<tr>
	<td>Restrictions:</td>
    <td>CodeToEnter:</td>
    <td>code</td>
    <td>Attribut</td>
    <td>Frei wählbarer Code.</td>
</tr>
<tr>
	<td>Restrictions:</td>
    <td>CodeToEnter:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Frei wählbarer Text. Wird als Text zur Codeeingabe angegeben.</td>
</tr>
<tr>
	<td>Restrictions:</td>
    <td>TimeMax:</td>
    <td>minutes</td>
    <td>Attribut</td>
    <td>Frei wählbarer Wert in Minuten.</td>
</tr>

</table>

```xml
<Restrictions>
	<CodeToEnter code="Hase">Bitte 1. Freigabewort eingeben!</CodeToEnter>
	<TimeMax minutes="20"/>
</Restrictions>
```
---

`BOOKLETCONFIG`

<table>

<tr>
    <td>Config:</td>
    <td>key</td>
    <td>Attribut</td>
    <td>Vordefinierter Wert. Ermöglicht eine Booklet Konfiguration. Die möglichen zu verwendenden Werte sind im nächsten Abschnitt zu finden.</td>
</tr>
<tr>
    <td>Config:</td>
    <td>>xxx<</td>
    <td>Datum</td>
    <td>Vordefinierter Wert. Die möglichen zu verwendenden Werte sind im nächsten Abschnitt zu finden.</td>
</tr>

</table>


```xml
<BookletConfig>
  <Config key="force_response_complete">OFF</Config>
</BookletConfig>
```

---

### <a name="Konfiguration"></a>Booklet Konfiguration

Es ist möglich Booklets zu konfigurieren. Hierfür stehen einige Parameter (Attribute) zur Verfügung, die in der Booklet.xml 
angegeben werden können. Alle verwendbaren Parameter befinden sich in einer separaten Konfiguraionsdatei 
(booklet-config.json) auf die das Testcenter zugreifen kann. Möchten Sie die Bookletkonfiguration bzgl. spezifisches Eigenschaften ändern, 
müssen Sie den gewünschten Parameter mit dem gewünschten Wert in der Booklet.xml unter `BookletConfig` angeben. Ein Parameter setzt sich zusammen aus einem Attribut, einem Attributwert und einem entsprechenden Datum. Wie am nachfolgenden Bsp. zu sehen ist, ist `key` das Attribut. Als Attribuwerte können nur vordefinierte Werte verwendet werden. Diese sind der weiter unten aufgeführten Tabelle zu entnehmen. Im nachfolgenden Code wäre der Attributwert bspw. `force_response_complete`. Das Datum ist in diesem Fall `OFF`. Auch das mögliche Datum für den jeweiligen Attributwert, ist der unten aufgeführten Tabelle zu entnehmen. Alle Parameter werden global in der Booklet.xml angelegt. Sie gelten dann für jedes in der Booklet.xml definierte Testlet. Eine Ausnahme stellen die beiden Parameter: `force_response_complete` und `force_presentation_complete` dar. Diese können auch Testletspezifisch angelegt werden. 

Nachfolgend ist eine Bookletkonfiguration zu sehen, die global für das gesamte Booklet und damit für alle Testlets gilt:

```xml
<Booklet>
  <Metadata>
      ...
  </Metadata>

  `<BookletConfig>`
      <Config key="force_response_complete">OFF</Config>
      <Config key="unit_navibuttons">ARROWS_ONLY</Config>
      ...
  </BookletConfig>

	<Units>
  
		<Unit id="Startunit" label="Startunit" />
		
		<Testlet id="Examples" label="Beispiele">
			<Restrictions>
				<CodeToEnter code="Hase">Bitte 1. Freigabewort eingeben!</CodeToEnter>
			</Restrictions>
			<Unit id="Unit_Allg_Anweisung" label="Platzhalter Allgemeine Anweisungen" />
		</Testlet>
	
	</Units>

</Booklet>
```
Nachfolgend ist zu sehen wie die Parameter: `force_response_complete` und `force_presentation_complete` Testletspezifisch angelegt werden können:

```xml
	
    <Testlet id="Examples" label="Beispiele">
		<Restrictions>
			<CodeToEnter code="Hase">Bitte 1. Freigabewort eingeben!</CodeToEnter>
			<DenyNavigationOnIncomplete presentation="ON" response="OFF" />
		</Restrictions>
		<Unit id="Unit_Allg_Anweisung" label="Platzhalter Allgemeine Anweisungen" />
	</Testlet>
	
```

** Werden Parameter nicht in der Bookelt.xml angegeben, gelten die Default-Werte (siehe Tabelle unten)!**

---

**[Hier](https://github.com/iqb-berlin/testcenter-frontend/blob/master/docs/booklet-config.md) finden Sie eine Übersicht über die verwendbaren Parameter (Attribute) und deren Bedeutung.**

**Achten Sie bei der Verwendung dieser Parameter auf die richtige Schreibweise (Groß-/Kleinschreibung)!**

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Testtaker-Xml (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

<table>
  <tr>
    <td><a href="#Attr_Daten">Attribute und Daten</a></td>    
	<td><a href="#CustomText">Custom Text Konfigurationen</a></td>
	<td><a href="#Einr_Tlk">Einrichten der Testleitkonsole</a></td>
  </tr>
</table>

Die Testtaker-Definition besteht aus einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](Arbeiten-mit-Xml‐Dateien).

> **Die in der XML-Datei angelegten Attribute und Elemente sind nicht frei wählbar, sondern orientieren sich an einer Schema-Definition. Diese gibt vor, welche Elemente und Attribute verwendet werden dürfen. Die Schema Definition für die `Testtakers.xml` ist [hier](https://github.com/iqb-berlin/testcenter-backend/blob/master/definitions/vo_Testtakers.xsd) ersichtlich.**

### <a name="Attr_Daten"></a>Attribute und Daten

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

### <a name ="CustomText"></a>Custom Text Konfigurationen

Diese Anwendung ermöglicht es zur Laufzeit Änderungen an Texten durchzuführen. 
Dies kann notwendig sein, wenn Standardtitel, Eingabeaufforderungen oder Erklärungen nicht zur spezifischen Umgebung, in welcher das **Testcenter** ausgeführt wird, passen. Welche Textteile innerhalb des **Testcenters** ersetzt werden sollen, wird mit dem Attribut: `key` festgelegt. Dazu werden dem Attribut: `key` definierte Atributwerte zugewiesen. Die möglichen Attributwerte entnehmen Sie bitte der Tabelle weiter unten. Nach Festlegung, welcher Text innerhalb des **Testcenters** auf diese Weise verändert werden soll, kann der gewünschte Text dann als Datum (gefasst in Hochkommata) angegeben werden. Nachfolgend ein Bsp..

```xml
<CustomTexts>
    <CustomText key="login_testEndButtonText">Test beenden</CustomText>
    <CustomText key="login_bookletSelectPrompt">Bitte wählen</CustomText>
...
</CustomTexts>
```
Hier wird nun also der Text für den "Test beenden"-Button in den Text: "Test beenden" geändert. Außerdem wird der Text: "Bitte wählen" für die Booklet-Auswahl-Anzeige festgelegt.

Innerhalb des **Testcenters** kann auch ein System-Check durchgeführt werden. Auch Texte innerhalb dieses System-Checks können auf die gleichen Weise individualisiert werden. Dazu nachfolgend ein Bsp.:

```xml
<Config>
    <UploadSpeed ...
    <DownloadSpeed ...
    <CustomText key="syscheck_questionsintro">"Bitte beantworten Sie alle Fragen"</CustomText>
    <CustomText key="app_intro1">"Willkommen zu diesem System-Check"</CustomText>
...
</Config>
```
Hier werden zwei Texte festgelegt, die innerhalb des System-Checks angezeigt werden. Einmal der Text auf der System-Check eigenen Frageseite und des Weiteren der Text innerhalb der Einführungsseite des System-Checks.

---

**[Hier](https://github.com/iqb-berlin/testcenter-frontend/blob/master/docs/custom-texts.md) finden Sie eine Übersicht über die verwendbaren Parameter (Attribute) und deren Bedeutung.**

**Achten Sie bei der Verwendung dieser Parameter auf die richtige Schreibweise (Groß-/Kleinschreibung)!**

---

### <a name="Einr_Tlk"></a>Einrichten der Testleitkonsole

Die Testleitung kann in der `Testtaker.xml` über den Modus: **Monitor-Group** (mehr Informationen zum Thema Modi der Testdurchführung finden Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung) festlegen welche Testgruppen der Testleitkonsole hinzugefügt werden sollen. Dazu wird in der entsprechenden Gruppe dieser Modus angegeben. Nachfolgend finden Sie zwei Beispiele wie Gruppen angelegt werden können:

Ohne Passwort. Sinnvoll wenn nur Links an die Testpersonen versendet werden.

```xml
<Group id="iqb-intern1" label="IQB intern Gruppe 1">
		
	<Login mode="run-hot-return" name="Testgruppe-1">
		<Booklet codes="Testperson_a Testperson_b Testperson_c">THETLK</Booklet>
	</Login>

	<Login mode="monitor-group" name="group-monitor_1" />

</Group>

```

Jede Testperson erhält ein eigenes Passwort. Dies stellt die gängigste Methode dar.


```xml
<Group id="iqb-intern1" label="IQB intern Gruppe 1">
			
	<Login mode="run-hot-return" name="Testperson_a" pw="123">
		<Booklet>THETLK</Booklet>
	</Login>
	<Login mode="run-hot-return" name="Testperson_b" pw="124">
		<Booklet>THETLK</Booklet>
	</Login>
	<Login mode="run-hot-return" name="Testperson_c" pw="125">
		<Booklet>THETLK</Booklet>
	</Login>
						
	<Login mode="monitor-group" name="group-monitor_1" />
</Group>
```

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Unit-Xml (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

Die Unitdefinition besteht aus mindestens einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](Arbeiten-mit-Xml‐Dateien).

> **Die in der Xml-Datei angelegten Attribute und Elemente sind nicht frei wählbar, sondern orientieren sich an einer Schema-Definition. Diese gibt vor, welche Elemente und Attribute verwendet werden dürfen. Die Schema Definition für die Unit.xml ist [hier](https://github.com/iqb-berlin/testcenter-backend/blob/master/definitions/vo_Unit.xsd) ersichtlich.**

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

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Workaround Unit-Xml (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

Das aktuelle IQB-Teststudio wurde zwar bereits für diverse Studien verwendet, befindet sich aber noch im Entwicklungsstadium "Prototyp". Es ist völlig klar, dass viele Funktionen fehlen oder nicht die erwarteten Ergebnisse liefern. Im Projektzeitraum 2021-2023 wird diese Web-Anwendung grundlegend überarbeitet und die aktuelle Version "IQB-Teststudio-Lite" nur bei dringendem Bedarf geändert.

In der Zwischenzeit ist es punktuell erforderlich, Mängel manuell auszugleichen. 

Die folgenden Workarounds beschreiben dies:

### Metadaten reduzieren

Die aktuelle Version des Teststudios erzeugt Unit-Xmls, die nicht vom aktuellen Testcenter akzeptiert werden. Das liegt daran, dass die zulässigen Metadaten auf das Nötigste reduziert wurden. Die Elemente Lastchange, Owner und Project müssen entfernt werden:

**Vorher**

    <Unit>\
      \<Metadata>
      <Id>Yoyo</Id>
       <Label>Geobrettfigur auslegen</Label>
       <Lastchange>2020-07-02T00:41:16+02:00</Lastchange>
       <Owner>Institut zur Qualit&#xE4;tsentwicklung im Bildungswesen IQB</Owner>
       <Project>Demo-Aufgaben f&#xFC;r die &#xD6;ffentlichkeit</Project>
     </Metadata>
    <DefinitionRef player="IQBVisualUnitPlayerV2">Yoyo.voud</DefinitionRef>
    </Unit>

**Nachher**

    <Unit>
     <Metadata>
      <Id>Yoyo</Id>
      <Label>Geobrettfigur auslegen</Label>
     </Metadata>
     <DefinitionRef player="IQBVisualUnitPlayerV2">Yoyo.voud</DefinitionRef>
    </Unit>

### Empfehlung: Verweis zur Validierung

Nach dem Hochladen in das Testcenter erhält man noch eine Warnung "File has no link to XSD-Schema...". Diese Warnung bedeutet, dass die Xml-Datei keinen expliziten Verweis auf eine Xsd-Datei enthält. Eine solche Xsd-Datei definiert die möglichen Elemente und Attribute einer Xml-Datei und kann daher zur Prüfung der Xml-Datei auf Korrektheit verwendet werden. Das IQB stellt solche Xsd-Dateien bereit.

Die Deklaration der Xsd-Datei erfolgt im Haupt-Element einer Xml-Datei. Für die Unit-Xml heißt das Hauptelement Unit und muss folgendermaßen geändert werden:

    <Unit>
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Unit.xsd">

Ein nützlicher Nebeneffekt hierbei ist, dass auch Editoren zur Bearbeitung von Xml-Dateien (z. B. Notepad++, Sublime) nun eine Validierung vornehmen können. Man kann also vor dem Hochladen eine Validierung bereits beim Schreiben einer Xml-Datei vornehmen lassen.