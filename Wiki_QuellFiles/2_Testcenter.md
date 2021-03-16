# 2.Testcenter
**Vorab:**

Grundlegende Informationen zum Testcenter Frontend erhalten Sie auch im TBA Einführungskapitel.
Das Testcenter besteht aus einem Back- und einem Frontend. In diesem Kapitel wird nur auf das Frontend eingegangen,
da Anwender vorwiegend damit in Berührung kommen.

---

> **In Bearbeitung**
> 
> THuste
> 

## 2.1 Testcenter Einführung

Eine grobe Einführung geben die nachfolgenden Verlinkungen.                         
Das IQB bietet folgende Video-Präsentationen bzgl. des Testcenters an:
* [Einführung in das IQB-Testcenter](https://box.hu-berlin.de/f/a8f7aea9c751493c8d35/)
* [Diskussion der Optionen Testcenter-Einsatz oder Implementation der Verona-Schnittstelle](https://box.hu-berlin.de/f/d23af87168fa4e9f9bb0/)

Des Weiteren gibt besteht folgende Forum:
[Testcenter-Forum](https://github.com/iqb-berlin/testcenter-frontend/discussions)                      
Hier finden Sie häufig gestellte Fragen und Antworten sowie Berichte über Einsätze des IQB-Testcenters.

### Aufbau

Nachfolgend ist der grobe Aufbau des Testcenters zu sehen. Dieses besteht aus einem Frontend und einem Backend.
Das Frontend wird von den Endbenutzer\*innen, sprich den Testdurchführenden (Lehrer\*innen, Schüler\*innen und andere Verantwortlichkeiten), verwendet. Hier erfolgt das Hochladen, Herunterladen und Löschen der einzelnen Dateien eines Tests, die finale oder probeweise Testdurchführung und im administrativen Bereich das Verwalten von Benutzer\*innen und deren Rechten. 
Das Backend ist der softwaretechnisch Unterbau des Frontends. Hier werden die Daten eines Tests, Benutzer\*in Daten und Metadaten gespeichert.
Endbenutzer\*innen kommen mit diesem Teil des Testcenters nicht direkt in Berührung!

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Aufbau_final.png)

Detailliert betrachtet besteht das Testcenter Frontend aus weiteren Komponenten. An dieser Stelle sei einmal der Verona Player genannt, da dessen Funktion innerhalb des Testcenter Frontend auch den Anwender\*innen bekannt sein sollte. Der Verona Player und seine definierte Schnittstelle zum Testcenter stellt die Aufgabeninhalte im Testcenter dar. Näheres zum Thema Verona entnehmen Sie bitte dem gleichnamigen Kapitel. Weitere Schnittstellen und Umgebungsmodule, die direkt oder indirekt mit dem Testcenter zusammenarbeiten, sind nachfolgend dargestellt.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Umgebungsmodule_final.png)

 
---

> **In Bearbeitung**
> 
> THuste
> 
> Stand:09.03.2021

---

## 2.2 Laden eines Tests

Nach der Anmeldung im Testcenter können Sie auf Ihren Workspace oder andere vom Administrator für Sie freigegebene Arbeitsbereiche, wie z.B Beispielaufgaben, zugreifen.
                  
**Der Workspace und andere Arbeitsbereiche müssen zuvor von einem IQB Administrator für Sie angelegt oder freigegeben werden!**

Anschließend ist es Ihnen möglich Dateien eines Tests in das Testcenter zu laden oder Testbestandteile aus dem Testcenter herunterzuladen. Auch die Löschung einzelner Datei ist möglich. Während des Hochladens findet eine Plausibilitätsprüfung statt. Dabei wird überprüft ob die deklarierten Dateien in einer Datei während des Hochladens auch gefunden werden. Ein einfaches Beispiel: In der Booklet.xml werden die gewünschten Units deklariert. Laden Sie zuerst die Booklet.xml und erst anschließend die Unit.xml wird eine Fehlermeldung generiert, weil die in der Booklet.xml deklarierten Units nicht gefunden werden. Es ist daher wichtig die richtige Reihefolge beim Upload einzuhalten. Eine Übersicht verschafft das nachfolgende Bild:

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Upload_Dateien_final.png)

---

> **In Bearbeitung**
> 
> Bearbeiter: Huste
> Stand: 1.3.21

## 2.3 Bearbeiten eines Tests

Die im Teststudio erzeugten Dateien können vor dem Upload in das Testcenter berarbeitet werden.<br>
Betrachten Sie dazu auch noch einmal das Kapitel:

[TBA Einführung -> Datenhandshake](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.1.2-Datenhandshake-Testcenter-Teststudio)

---

**Bevor es los geht ein paar Grundlagen:**
<p>

Bei den zu bearbeitenden Dateien handelt es sich um Xml-Dateien. Xml ist ein textbasiertes Datenformat.   
Die Daten werden also in Textform in einem Text hinterlegt. Xml-Dateien können daher auch einfach mittels eines Texteditors bearbeitet werden.
Damit die Daten im Text gefunden werden können, muss eine bestimmte Struktur eingehalten werden. Anschließend kann eine entsprechende Gegenstelle, in unserem Fall das Testcenter, mittels eindeutiger Schlüsselwörter (Tags oder Elemente) die Daten im Text finden und nutzen. Xml-Dateien bestehen immer aus Elementen und ggf. mehreren Unterelementen. Der Beginn eines Elements wir mit zwei spitzen Klammern **<*Element Start*>** eingeleitet und wie folgt beendet:**</*Element Ende*>**. Jedes Element kann außer den eigentlichen Daten zusätzliche Attribute enthalten. Attribute werden immer in der folgenden Form ausgedrückt: *Name Attribut* = "*Attributwert*" und befinden sich innerhalb eines Elementenblocks, sprich innerhalb der beiden spitzen Klammern. Es gibt auch Elemente die Attribute aber keine Daten enthalten und umgekehrt. Einfache Bsp. sind nachfolgende aufgeführt:

Element ohne Attribute mit Dateninhalt.<br>
*Daten sind in diesem Fall der Text zwischen den spitzen Klammern: "Sekundarstufe I Englisch Ansichtsaufgaben".*

```
<Label>Sekundarstufe I Englisch Ansichtsaufgaben</Label>
```

Element mit Attributen ohne Daten.<br>
*Hier gibt es 3 Attribute: id, lable und labelshort. Alle 3 Attribute enthalten in diesem Fall Attributwerte.<br>
Diese sind in Hochkommata gefasst und werden mit einem Istgleichzeichen dem Attribut zugeordnet. Das keine Daten enthalten sind, ist gut am Schließen des Elementes: Unit zu erkennen. Denn das Element endet nicht mit: `</Unit>`, sondern nur mit: `/>`. Diese Syntax gibt an, dass keine Daten folgen.*

```
<Unit id="Unit1" label="1. Postcard" labelshort="1" />
```

Element mit Daten und Attributen.<br>
*Attribut ist hier: key. Dieses bekommt den Attributwert "force_presentation_complete" zugewiesen.
Datum ist der Text: ON.*
````
<Config key="force_presentation_complete">ON</Config>
````


Manche Attributwerte können frei gewählt werden, manche müssen sich an Vorgaben halten.<br> 
Nachfolgend wird nun auf die Elemente unserer Testdateien und deren Attribute und Daten eingegangen.
  
</p>

---

### Die Datei TESTTAKERS.xml

**Element: Metadata/ Describition**<br>
Datum: frei wählbar

```
<?xml version="1.0"?>
<Testtakers>
  <Metadata>
    <Description>
     This file contains some logins for testing and works a a sample for developers.
    </Description>		
  </Metadata>
  ...
```
---

**Hauptelement: CustomTexts
  Unterelement: CustomText<br>
    Attribute:<br>
    key:<br> Attributwert: Vordefiniert, siehe: [Testcenter->Konfiguration der Testanwendung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2.5-  Konfiguration-der-Testdurchf%C3%BChrung)<br> 
Datum: frei wählbar 
```
  <CustomTexts>
    <CustomText key="somestr">string</CustomText>
  </CustomTexts>
  ...
```
---

**Element: Group/ Login**<br>
* Attribut
  * name<br>
  frei wählbar
  * mode<br>
  Vordefiniert, siehe: [Modi der Testdurchführung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2.4-Modi-der-Testdurchf%C3%BChrung)
  * pw<br>
  frei wählbar
  


```
 <Group id="frei wählbare ID" label="frei wählbarer Text Label">
    <Login name="user1" mode="run-demo" pw="123">
      <Booklet>Booklet1</Booklet>
    </Login>
 </Group>
</Testtakers>

```
 
![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Xml_Testtakers_final.png)

---



---
| Parameter_B<br>*(CustomTexts)*|Beschreibung|         
| :-----------| :--------- |
| CustomText | Welche Parameter genutzt werden können entnehmen Sie bitte dem Kapitel:<br> *[Testcenter Frontend -> Konfiguration der Testanwendung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2.5-Konfiguration-der-Testdurchf%C3%BChrung)*|
---
| Parameter_C<br>*(Group)*|Beschreibung|
| :-----------| :--------- |
|name| Username ist frei wählbar und ist zusammen mit dem Passwort im Testcenter einzugeben |
|mode| Es dürfen nur vordefinierte Modi verwendet werden. Welche Modi das sind,<br>entnehmen Sie bitte dem Kapitel: *[Modi der Testdurchführung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2.4-Modi-der-Testdurchf%C3%BChrung)*|
|pw| Das Passwort ist frei wählbar und wird zusammen mit dem Namen im Testcenter angegeben |
|booklet| Hier wird das Booklet gewählt, welches für den entsprechenden Test (angelegter User) verwendet werden soll. Dabei ist zu beachten, dass der Name der ID in der Booklet.xml entspricht (Achten Sie auf Groß-Kleinschreibung!!!)|

### BOOKLET.xml

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Xml_Booklet_final.png)

---

| Parameter_A<br>*(Metadaten)*|Beschreibung|
| :-----------| :--------- |
| Id | Frei wählbare ID. Die Booklet.xml wird über die Testtakers.xml aufgerufen. In der Testtakers.xml<br>muss somit zwingend die gewählte Booklet ID unter Beachtung der Groß-/Kleinschreibweise angegeben werden |
| Label| Frei wählbar |
| Describtion| Frei wählbar |
---
| Parameter_B<br>*(BookletConfig)*|Beschreibung|
| :-----------| :--------- |
| Config| Welche Parameter genutzt werden können, entnehmen Sie bitte dem nachfolgenden Kapitel: *[Testcenter Frontend -> Konfiguration der Testanwendung](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/1.2.5-Konfiguration-der-Testdurchf%C3%BChrung)* |
---
| Parameter_C<br>*(Units)*|Beschreibung|
| :-----------| :--------- |
| | |

---

> **in Bearbeitung**
> 
> T.Huste
> 
> Stand: 3.3.21

## 2.4 Modi der Testdurchführung

Bei der Definition der Anmeldung zur Durchführung eines Tests können verschiedene Modi gewählt werden. Die Testhefte bleiben unverändert, es wird nur ein Modus für eine spezielle Testperson festgelegt. Verschiedene Anmeldungen können also mit denselben Testheften zu unterschiedlichem Verhalten führen.

### Wo wird das festgelegt?
Die Festlegung erfolgt in der Testtaker-Xml im Element `Login` im Attribut `mode`:

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

## 2.5 Konfiguration der Testdurchführung

### Booklet Konfiguration

Es ist möglich Booklets entsprechend zu konfigurieren. Hierfür stehen einige Attribute zur Verfügung, die in der Booklet.xml (wenn gewünscht) anzugeben sind. Alle verwendbaren Attribute befinden sich in einer separaten Konfiguraionsdatei (booklet-config.json) auf die das Testcenter zugreifen kann. Möchten Sie einzelne Attribute nutzen, müssen Sie das Attribut und den gewünschten Wert (Datum) in der Booklet.xml unter "BookletConfig" angeben. 

Nachfolgend sehen Sie die entsprechend benötigte Struktur in der Booklet.xml:

```
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

```
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

```
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
