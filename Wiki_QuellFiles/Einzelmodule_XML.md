<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Arbeiten mit Xml-Dateien (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

> XML ist ein Standardformat und wird durch Texteditoren sehr gut unterstützt. Daher sind einige Dateien für die Definition von Daten in den IQB-Anwendungen in diesem Format hinterlegt. Der folgende Text soll Neulingen dieses Format nahebringen.

XML ist ein textbasiertes Dateiformat. Die Daten können also einfach mittels eines Texteditors bearbeitet werden. Beispiele sind Notepad++ oder Sublime. Viele Editoren bieten Ergänzungsmodule für die Arbeit mit XML-Dateien. Dann sind z. B. die Schlüssel-Zeichen in anderen Farben dargestellt und es werden Fehler in der Syntax (z. B. schließendes Element fehlt) gemeldet.

Damit die Daten im Text gefunden werden können, muss eine bestimmte Struktur eingehalten werden. Anschließend kann eine entsprechende Gegenstelle - z. B. das IQB-Testcenter, mittels eindeutiger Schlüsselwörter (Tags oder Elemente) die Daten im Text finden und nutzen.
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

Um eine Validierung anzustoßen, fügt man zunächst in den Kopf der XML-Datei (also in das Wurzelelement) einen Verweis auf die Schema-Datei ein. Das IQB hat für alle XML-Dateien solche Schema-Dateien entwickelt. Für eine Unit-Xml wäre z. B. das Hauptelement folgendermaßen zu ändern:

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

Die Testheft-Definition besteht aus einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](Arbeiten-mit-Xml‐Dateien).

Es ist möglich Booklets zu konfigurieren. Hierfür stehen einige Attribute zur Verfügung, die in der Booklet.xml 
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
      <Config key="force_responses_complete">OFF</Config>
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
	
	<Testlet id="Deutsch" label="Deutsch lesen">
		<Restrictions>
			<CodeToEnter code="Deutschland">Bitte 1. Freigabewort eingeben!</CodeToEnter>
		</Restrictions>
		<Unit id="Deutsch Teil 1" label="Platzhalter Allgemeine Anweisungen" />
	</Testlet>
	
  </Units>

</Booklet>
```
---

### Booklet Konfiguration

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

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Testtaker-Xml (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Überarbeitung THuste
Stand: 8.4.2021
```
Die Testtaker-Definition besteht aus einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](Arbeiten-mit-Xml‐Dateien).



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


<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# Unit-Xml (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

```yaml
Dokumentstatus: Überarbeitung MM
Stand: 7.4.2021
todo:
  - noch einzubinden
```
Die Unitdefinition besteht aus mindestens einer XML-Datei. Hinweise zur Bearbeitung von XML-Dateien erhalten Sie [hier](Arbeiten-mit-Xml‐Dateien).
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