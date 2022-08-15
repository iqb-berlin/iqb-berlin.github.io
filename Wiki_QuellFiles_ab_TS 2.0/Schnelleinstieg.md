# TBA Schnelleinstieg

Im Rahmen der digitalisierten Testung hat das **IQB** zwei webbasierte Anwendungen entwickelt.

Eine Anwendung wird für das Aufgabenmanagement und die Aufgabenentwicklung verwendet und trägt den Namen **Studio**. Ein integrierter **Editor** übernimmt dabei den eigentlichen Aufgabenentwurf. Eine weitere Anwendung trägt den Namen **Testcenter** und wird für die Testdurchführung und Auswertung einer Testung verwendet.

Sind Aufgaben mit dem **Studio** final entworfen, können diese abschließend in einem bestimmten Dateiformat vom **Studio** ausgegeben werden. Die so ausgegebenen Dateien können bei Bedarf nachträglich verändert werden. Zur Testdurchführung werden diese Dateien dann in das **Testcenter** geladen und wiedergegeben.


Lernen Sie beiden Anwendung **Studio** und **Testcenter** und die Bearbeitung der **Testdateien** doch einmal anhand eines vereinfachten Beispiels kurz kennen:

<table border=0 >
    <tr>
        <th align=center>
            <img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Symbol_004.png" alt="Alt-Text" title="Studio Symbol" />
        </th>
        <th align=center>
           <img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Output_Symbol_004.png" alt="Alt-Text" title="TS Output Symbol" />
        </th>
        <th align=center>
           <img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testdateien_Symbol_002.png" alt="Alt-Text" title="Die Testdateien" />
        </th>
        <th align=center>
           <img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_Input_Symbol_001.png" alt="Alt-Text" title="Output Symbol" />
        </th>
        <th align=center>
           <img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_Symbol_002.png" alt="Alt-Text" title="Testcenter Symbol" />
        </th>
    </tr>
    <tr>
        <th align=center>
            <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Studio">Studio</a>
        </th>
        <th align=center>
           <a href=""></a>
        </th>
        <th align=center>
           <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Testdateien">Testdateien</a>
        </th>
        <th align=center>
           <a href=""></a>
        </th>
        <th align=center>
           <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Testcenter">Testcenter</a>
        </th>
    </tr>
</table>

:information_source: Detailliertere Informationen zu den Anwendungen finden Sie in den gleichnamigen Kapiteln dieser Wiki.

<!--###################################################################################################################### -->
## Schnelleinstieg: Das Studio
<!--###################################################################################################################### -->

<table border=1>
<tr>
<th align=center>

### Entwerfen Sie Ihre erste Aufgabe mit dem Studio

</th>

</tr>
<tr>
<td>

### :heavy_check_mark: Vorweg

</td></tr>
<tr>
<td>

:information_source: Detaillierte Informationen zum **Studio** finden Sie im gleichnamigen Kapitel.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Studio öffnen

</td></tr>
<tr>
<td>

Eingabe der Adresse des Studios in einen Browser.
 
:heavy_exclamation_mark: **Das Studio muss dazu auf Ihrem Server installiert sein.**

Melden Sie sich anschließend mit Ihren Zugangsdaten am Studio an.

:information_source: Die Zugangsdaten erhalten Sie von Ihren Adminstrator\*innen.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Arbeitsbereich wählen

</td></tr>
<tr>
<td>

Wählen Sie Ihren Arbeitsbereich aus.

:information_source: Die Administrator\*innen geben die Bereiche für Sie frei.

![TS_AB_Auswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_AB_Auswahl_01.png)


</td></tr>
<tr>
<td>

### :heavy_check_mark: Aufgabe anlegen

</td></tr>
<tr>
<td>

Legen Sie eine neue Aufgabe an oder bearbeiten Sie eine bestehende Aufgabe durch Markierung der Aufgabe.

In diesem Beispiel befinden sich bereits einige Aufgaben im geöffneten Arbeitsbereich. Fügen Sie nun eine neue Aufgabe hinzu. Wählen Sie anschließend einen eindeutigen Namen für die Aufgabe. In diesem Beispiel wird er Name "MEA" vergeben. "MEA" soll für "Meine erste Aufgabe" stehen. Zur besseren Übersicht können Sie die Aufgabe abschließend noch einer Gruppe innerhalb des Arbeitsbereichs zuordnen.

:information_source: Eine Aufgabe wird übrigens im IQB-Umfeld auch **Unit** genannt!

![TS_Aufgabe_anlegen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Aufgabe_anlegen_01.gif)

:heavy_exclamation_mark: **Wählen Sie kurze ID-fähige Namen, die Ihre Aufgabe eindeutig identifizieren und diese von anderen Aufgaben sehr wahrscheinlich unterscheiden.**

</td></tr>
<tr>
<td>

### :heavy_check_mark: Auswahl Editor und Player

</td></tr>
<tr>
<td>

Bevor Sie mit dem Aufgabentwurf starten, müssen Sie festlegen mit welchem Editor Sie die Aufgabe entwerfen möchten. Jeder vom IQB angebotene Editor verfügt über spezifische Eigenschaften und Funktionen. Wählen Sie den Aspect-Editor, wenn Sie Ihre Aufgabe mittels vorgefertigter Elemente entwerfen wollen und wenn sich die Aufgabenansicht dynamisch an andere Bildschirmgrößen anpassen soll. Wählen Sie den Editor für Text, wenn Sie Ihre Aufgabe mittels einer Scriptsprache entwerfen möchten und auf eine dynamische Ansicht verzichten können.

Ist der Editor ausgewählt, muss auch ein zum Editor passender Player gewählt werden. Der Player gibt die Aufgabe mit Ihren Aufgabenelementen dann sowohl in der Vorschau als auch später bei der Testdurchführung im **Testcenter** wieder.

![TS_Editorwahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Editorwahl_01.png)


 Player und Editor werden in verschieden Versionständen angeboten. Wählen Sie immer die aktuellste Version.

:information_source: An dieser Stelle können Sie die Aufgabe auch schon einmal speichern.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Der Editor

</td></tr>
<tr>
<td>

Jetzt gehts los! Starten Sie den zuvor ausgewählten Editor mithilfe des gleichnamigen Reiters.

Soll sich Ihre Aufgabe dynamisch an entsprechende Bildschirmgrößen anpassen, wählen Sie zuvor einen dynamischen Abschnitt aus.

![TS_Editor_dynamisch](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Editor_dynamisch_02.png)

Legen Sie ihr erstes Aufgabenelement in Ihrer Aufgabe an und speichern Sie die Aufgabe. In diesem Beispiel wird ein Optionsfeld mit Text gewählt.

![TS_Elementenauswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Elementenauswahl_02.gif)

Sie können die Aufgabe vor der finalen Ausgaben durch das **Studio** in einer Vorschau betrachten. Klicken Sie dazu auf den Reiter "Vorschau". Dort wird Ihre Aufgabe genau so angezeigt, wie sie auch bei der Testdurchführung im **Testcenter** angezeigt werden würde. So erkennen Sie schon vor der Ausgabe Fehler und können diese beheben!

![TS_Vorschau](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Vorschau_03.gif)

</td></tr>
<tr>
<td>

### :heavy_check_mark: Ausgabe der Aufgabe

</td></tr>
<td>

Im nächsten Schritt lassen Sie Ihre Aufgabe mit dem **Studio** ausgeben.

Bei der Ausgabe kann festgelegt werden, welche Dateien ausgegeben werden sollen. Es können entweder nur die Dateien zu einer Aufgabe ausgegeben werden oder zusätzliche Dateien, die den Ablauf und grundlegende Funktionen der Testdurchführung beeinflussen. Nachfolgend sind diese optionalen Dateien aufgeführt und deren Funktion wird kurz beschrieben. 

**Player-Html**<br>
Wiedergabe der Aufgaben im **Testcenter**. Diese Datei wird auch als **Player-Ressource** bezeichnet.

**Booklet-Xml**<br>
Bündelung ausgewählter Aufgaben in Testlets, auch genannt Blöcken.

**Testtaker-Xml**<br>
Festlegungen in welchem Modus die Testung ablaufen soll und anlegen der Zugangsdaten für die Testpersonen.

Welche Dateien ausgegeben werden soll, kann im Ausgabeformular angegeben werden. Möchten Sie zusätzlich zur Aufgabe auch die oben aufgeführten optionalen Dateien ausgeben lassen, müssen Sie die Anzahl der Logins für die Testpersonen angeben. Dabei kann zwischen verschiedenen **Testmodi** gewählt werden. Der **Testmodus** legt fest wie eine Testung abläuft (Vorschau, finaler Test etc.). Welche Modi zur Verfügung stehen, finden Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung). 

![Studio Output Formular](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Output_Formular_02.png)

In diesem Fall werden 6 Logins im Review-Modus angelegt. Das **Studio** generiert dann automatisch Zeichenfolgen für den Namen und das Passwort in der **Testtaker-Xml** unter `Login`. Optional können die Logins auch ohne Passwort angelegt werden. Außerdem generiert das **Studio** eine Gruppe, der diese Logins zugeordnet werden. Auch hierfür wird eine eindeutige Zeichenfolge generiert. Sobald eine Testperson in einem Testmodus angelegt wurde, wird aber nicht nur die **Testtaker-Xml** erzeugt, sondern auch eine **Bookelt-Xml**. Dieser fügt das **Studio** dann gleich die gewählte Aufgabe unter `Units` hinzu. Es können noch weitere Werte im Formular angegeben werden, die sich hauptsächlich auf die Seitennavigation im Testverlauf beziehen. Eine Auswahl finden Sie im Formular unter "Button für Unit-Navigation" und "Unit Seitenwechsel". Die hier gewählten Werte werden dann in der **Booklet-Xml** unter `BookletConfig` angelegt. 

Außerdem wird in diesem Beispiel die Player-Ressource zur Aufgabe ausgegeben. 

Nach dem erfolgreichen Export finden Sie nun die folgenden Dateien am Speicherort: 

* die beiden Steuerdateien: **Testtaker1.xml**, **Booklet1.xml**
* die beiden Dateien zur Aufgabe "MEA": **MEA.xml**, **MEA.voud**
* die Playerressource: **iqb-player-aspect@1.25-Html**

:information_source: Hiermit ist der Aufgabenentwurf mit dem **Studio** abgeschlossen! Im nächsten Kapitel erfahren Sie mehr zu den Testdateien und deren Inhalten.

</td></tr>
</table>

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Testdateien">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

!<--###################################################################################################################### -->
## Schnelleinstieg: Die Testdateien
!<--###################################################################################################################### -->

<table border=1>
<tr>
<th align=center>

### Passen Sie die Testung Ihren Bedürfnissen an

</th></tr>
<tr>
<td>

### :heavy_check_mark: Vorweg

</td></tr>
<tr>
<td>

Um eine Testung mit dem **Testcenter** durchführen zu können, müssen vorab die Testdateien für die Testung in das **Testcenter** geladen werden. Wie im Schnelleinstieg zum **Studio** bereits beschrieben wurde, gibt das **Studio** nach dem Aufgabenentwurf die zugehörigen Testdateien aus. Werden vom **Studio** nicht nur die Dateien zur Aufgabe ausgegeben, sondern auch noch die optionalen Dateien **Booklet-Xml** und **Testtakers-Xml**, werden automatisch Abhängigkeiten zwischen den Testdateien beim Export hergestellt.

Nachfolgend sind die Abhängigkeiten der Testdateien und die Einbindungspunkte dargestellt.

![Abhängigkeiten Testdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Abhängigkeiten_Testdateien_05.png)

Mithilfe von spezifischen Werte in den beiden Dateien: **Testtaker-Xml** und **Booklet-Xml** können Aussehen und Ablauf der Testung festgelegt werden. Einige dieser Werte werden bereits beim Export durch das **Studio** diesen beiden Dateien hinzugefügt. Bspw. wurden in der **Testtaker-Xml** 6 Logins mit einem Passwort und einem Review-Modus angelegt. Die Anpassung der Dateien durch das **Studio** kann eventuell nicht ausreichend sein, um eine Testung den individuellen Bedürfnissen anzupassen. Es gibt da einfach zu viele mögliche Werte und Kombinationen. Daher gibt es die Möglichkeit die Dateien manuell anzupassen und um entsprechende Werte zu erweitern. Nachfolgend wird anhand von kurzen Beispiele aufgezeigt, wie die Dateien angepasst werden können, aber auch wie die Inhalte zu verstehen sind.

:information_source: Wollen Sie noch etwas mehr zu den Funktionen der Testdateien erfahren? Schauen Sie sich gerne das [**Video**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Die-Testdateien) zu diesem Thema an,

:information_source: Mehr Informationen zu den einzelnen Testdateien finden Sie auch im Abschnitt "Direkt zu anderen Seiten". 

</td></tr>
<tr>
<td>

### :heavy_check_mark: XML und die Schema Definition

</td></tr>
<tr>
<td>

**Studio** und **Testcenter** tauschen Informationen mittels der Testdateien aus. Damit dieser Austausch funktioniert, müssen beide Anwendung eine gemeinsame Sprache sprechen. In diesem Fall ist die gemeinsame Sprache **XML**. **XML** ist eine Möglichkeit textbasiert Daten und Werte zu transportieren. Das heißt: Sie können eine **XML** mit einem einfachen Texteditor öffnen und sehen die enthalten **Werte** und **Daten** und können diese manipulieren. Die **Daten** und **Werte** werden dabei in **Elementen** (tags) in Form von **Attributen** hinterlegt. Hier mal ein kurzes Beispiel:

Beim Export wurden 6 Logins in der **Testtaker.xml** angelegt. Ein Login ist dabei ein **Element**. Dieses **Element** verfügt über definierte **Attribute** mit entsprechenden **Werten**. **Attribute** sind in diesem Fall **mode** und **pw**. Die zugehörigen **Werte** werden mittels Gleichheitszeichen zugewiesen. Pure **Daten** gibt es innerhalb dieses **Elements** hier nicht. Aber im **Element: Booklet** sind nur **Daten** zu finden, nämlich der Name des Booklets.

```xml
<Login mode="run-hot-return" name="q2d6b" pw="e4y7">
      <Booklet>booklet1</Booklet>
</Login>
```

Damit das **Testcenter** alle Werte und Daten auch finden kann, dürfen nur festgelegte Elemente mit zulässigen Werten in der XML angelegt sein. Es ist also nicht möglich ein frei erfundenes Element der **XML** hinzuzufügen. Das **Testcenter** kennt dieses Element nicht und wird daher auch keine Werte und Daten dieses Elements auswerten können. Um nicht erlaubte Elemente einer XML bereits beim Laden in das **Testcenter** zu erkennen, muss eine Vorabprüfung stattfinden. Die Vorabprüfung kann mittels so genannter **Schema-Definition** erfolgen.Hierbei handelt es sich grob gesagt um eine Vorlage, wie die entsprechende XML auszusehen hat und welche Elemente enthalten sein dürfen. Spezielle Editoren gleichen bereits bei der manuellen Bearbeitung einer XML auf Wunsch den aktuellen Inhalt mit der **Schema-Definition** ab und melden eventuelle fehlerhafte Inhalte. Diese können dann bereits vor dem Laden in das **Testcenter** korrigiert werden. Spätestens beim Laden in das **Testcenter** erfolgt ein Abgleich der zu ladenden XML mit der deklarierten Vorlage der **Schema-Definition**. Wo diese Definition zu finden ist, wird in der jeweiligen Xml-Datei direkt am Anfang angegeben. Der Verweis auf diese **Schema-Definition** beginnt dann mit `xmlns:xsi`.


</td></tr>
<tr>
<td>

### :heavy_check_mark: Ressourcendatei für den Player

</td></tr>
<tr>
<td>

Während der Aufgabenerstellung im **Studio** wird festgelegt mit welchem Editor die Aufgaben erstellt werden soll. Außerdem wird angegeben mit welchem Player die Aufgabeninhalte später wiedergegeben werden. Dabei ist zu beachten, dass Editor und Player immer zueinander passen müssen. Wird bspw. der Aspect-Editor verwendet, muss auch der Aspect-Player verwendet werden. Gewählter Player und Editor werden beim Export durch das  **Studio** in der Aufgaben-Xml hinterlegt. Sobald Aufgaben in das **Testcenter** geladen werden, prüft das **Testcenter**, ob der in der Aufgaben-Xml angegebene Player in das **Testcenter** geladen wurde. Das **Testcenter** hat nicht jeden Programmcode zu jedem Player hinterlegt, daher muss der Programmcode des jeweiligen Players mit in das **Testcenter** geladen werden. Dies geschieht mittels der Ressourcendatei zum Player. In diesem Fall trägt diese Datei den Namen: **iqb-player-aspect@1.24.html**. 

</td></tr>
<tr>
<td>

### :heavy_check_mark: Aufgaben XML-/ und VOUD-Datei

</td></tr>
<tr>
<td>

Zu jeder im **Studio** erzeugten Aufgabe werden je 2 Dateien erstellt. Eine Datei mit der Endung **XML** und eine weitere mit der Endung **VOUD**. Beiden Dateien wird der Aufgabenname vorangestellt. In der Voud-Datei befinden sich alle Aufgabeninhalte, sprich alle über den Editor angelegten Aufgabenelemente. In der Xml-Datei sind zugehörige Metadaten wie bspw. der Aufgabenname und Kurzbeschreibung der Aufgabe angelegt. Außerdem wird hier angegeben, welcher Editor und Player bei der Aufgabenerstellung verwendet wurde. Es findet weiterhin ein Verweis auf die zugehörige VOUD statt. Prinzipiell können beide Dateien manuell nachträglich bearbeitet werden bevor sie in das **Testcenter** geladen werden. In der Voud-Datei sind manuelle Änderungen allerdings schwierig, da die Struktur unübersichtlich erscheint. In der Xml-Datei sind Änderungen hingegen mittels eines Editors einfach umzusetzen. Nachfolgend ist einmal die zur Aufgabe: **MEA** erzeugte Xml-Datei dargestellt.

![Unit-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Unit_Xml_01.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Unit_Xml_02.md) können Sie den Code kopieren.

:information_source: Übrigens wird eine **Aufgabe** am IQB auch gerne als **Unit** bezeichnet.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Booklet.xml

</td></tr>
<tr>
<td>

In einem **Booklet** können Aufgaben zusammengefasst und sortiert werden. 

:information_source: Ein **Booklet** wird auch als **Testheft** bezeichnet. 

Die Aufgaben können hier zu so genannten **Testlets** zusammengefasst werden. **Testlets** können mit bestimmten Beschränkungen versehen werden. Hierzu gehören bspw. eine zeitliche Beschränkung für die Bearbeitung des **Testlets** und eine Zugangsbeschränkung mittels Freigabewort.

:information_source: Ein **Testlet** wird übrigens auch als **Block** bezeichnet. 

Aufgaben können auch "lose" im Booklet vorliegen und werden dann von oben nach unten bei der Testdurchführung im **Testcenter** angezeigt.

Weiterhin kann in der **Booklet-Xml** mittels spezifischer Elemente, Attribute und Werte eine Booklet-Konfiguration (`BookletConfig`)angelegt sein. Aussehen und Verhalten der Testung können dann mittels dieser festgelegt werden. Hierfür stehen eine Vielzahl möglicher Elemente, Attribute und Werte zur Verfügung. Mehr Informationen zur **Booklet-Konfiguration** sind [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Booklet%E2%80%90Xml) zu finden. 

Nachfolgend werden die Strukturen der **Booklet-xml** einmal kurz aufgezeigt.

:information_source: Die hier gezeigte **Booklet-Xml** ist beim Export durch das **Studio** automatisch erzeugt wurden. Hier werden nur grundsätzliche Strukturen erzeugt. Es fehlen bspw. **Testlets** und spezifische **Booklet Konfigurationen**.

![Booklet-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Booklet_Xml_02.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Booklet_Xml_01.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Booklet.xml: Testlet hinzufügen

</td></tr>
<tr>
<td>

Bei der automatischen Generierung durch das **Studio** ist in der **Booklet-Xml** noch kein **Testlet** angelegt, sondern nur die erstellte Aufgabe "MEA". Fügen Sie nun einmal zum besseren Verständnis ein **Testlet** hinzu. Anschließend verschieben Sie die Aufgabe "MEA" in dieses **Testlet**. Das **Testlet** soll dann noch eine Zeitbeschränkung `TimeMax` und eine Zugangsbeschränkung `CodeToEnter` erhalten. Testpersonen können dann bei einer finalen Testung erst nach Eingabe des Freigabewortes die Aufgabe innerhalb des **Testlets** bearbeiten. Die Testperson hat dann für die eingestellte Zeit die Möglichkeit die enthaltenen Aufgaben zu bearbeiten.

![Booklet Testlet hinzufügen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Booklet_Testlet_02.gif)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Booklet_Testheft_Xml_01.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Testtaker.xml

</td></tr>
<tr>
<td>

In der Testtakers können Logins (`Login`) für die Testpersonen angelegt werden. Dabei stehen verschiedene Anmeldemöglichkeiten zur Verfügung. Mit Passwort, ohne Passwort, als Link usw.. Mehr dazu finden Sie auch [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren).

Die Logins mit den Anmeldedaten werden dabei immer einer entsprechenden Gruppe (`Group`) mit eindeutiger ID zugewiesen. Zusätzlich zu den Anmeldedaten wird angegeben, welches Booklet der jeweiligen Testperson nach Anmeldung präsentiert werden soll. Außerdem wird hier der **Modus** (`mode`) der Testung festgelegt. Mit diesem **Modus** wird festgelegt wie der Test ablaufen soll (Probelauf, finale Testung). Mehr Informationen finden Sie dazu auch [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung).

Es ist auch möglich einzelne Texte individuell für die Anwendung **Testcenter** anzupassen. Die Texte können dann in der **Custom-Text-Konfiguration** geändert werden. In der automatisch erzeugten **Testtaker-Xml** durch das **Studio** sind nur einzelne Elemente, Attribute und Werte von vielen in der **Custom-Text-Konfiguration** angegeben. Welche es noch gibt finden Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml) unter **Custom-Text-Konfiguration**. 

Nachfolgend ist die generierte **Testtaker-Xml** durch das **Studio** zu sehen.

![Testtaker-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testtaker_Xml_03.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Testtaker_Xml_01.md) können Sie den Code kopieren.

:heavy_exclamation_mark: **Gruppen-ID und Name der Testperson dürfen im Testcenter nur einmal vorkommen. Befindet sich in einem anderen Arbeitsbereich ein Duplikat, ist das Laden der Testtaker-Xml in das Testcenter nicht möglich und wird mit einer entsprechenden Fehlermeldung abgelehnt. Daher sollten auch keine "Klarbezeichner" gewählt werden, sondern immer eine Kombination aus Buchstaben und Zahlen. Dies verringert die Wahrscheinlichkeit von Duplikaten.**


</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Testtaker.xml: Testmodus ändern

</td></tr>
<tr>
<td>

Jeder Testmodus weist spezifische Eigenschaften auf. So werden bspw. Anworten einer Testung im Modus: `run-review` nicht gespeichert, im Modus: `run-hot-return` oder `run-hot-restart` aber schon. Eine Übersicht der verfügbaren Modi und deren Funktionen finden Sie [**hier**](https://github.com/iqb-berlin/testcenter-frontend/blob/master/docs/test-mode.md). 

Da mit den hier verwendeten Dateien später im **Testcenter** eine Testung gestartet werden soll und abschließend auch eine Auswertung der gegebenen Antworten erfolgen soll, sollten Sie für eine der Testpersonen den Modus: von `run-review` auf `run-hot-return` ändern und die Änderung anschließend speichern. Zur Erinnerung: Im Review-Modus werden keine Antworten gespeichert und es könnte daher auch keine Auswertung erfolgen.

![Testmodus ändern](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testmodus_aendern_02.png)

:information_source: An dieser Stelle werden erst einmal die Änderungen an den Testdateien beendet. Führen Sie gerne einmal weitere Änderungen an den Dateien durch und schauen Sie sich im **Testcenter** die Auswirkungen auf die Testdurchführung an.

</td></tr>
</table>

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Testcenter">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Studio">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

!<--###################################################################################################################### -->
## Schnelleinstieg: Das Testcenter
!<--###################################################################################################################### -->

<table border=1>
<tr>
<th align=center>

### Führen Sie die erste Testung durch!

</th></tr>
<tr>
<td>

### :heavy_check_mark: Vorweg

</td></tr>
<tr>
<td>

#### Anforderungen an die IT-Systeme

Das Testcenter stellt bestimmte Anforderungen an die Computer auf denen eine Testung durchgeführt wird. Diese Anforderungen können mit der im Testcenter intergrierten Funktion **System-Check** überprüft werden.  [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.7-System-Check) finden Sie mehr Informationen zum **System-Check**. Welche Anforderungen das Testcenter stellt, finden Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2-Testcenter) unter der Überschrift "Anforderungen".

#### Zugang für die Testpersonen

Im Vorfeld sollte sich die Testleitung Gedanken darüber machen, welcher Personenkreis getestet werden soll und wie die Testpersonen die Zugangsdaten erhalten. Mehr Informationen dazu erhalten Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren). 

Das IQB stellt eine weitere Anwendung mit dem Namen: **itc-Toolbox** zur Verfügung mit welcher Logins und bspw. QR-Codes für die Testpersonen erzeugt werden können. Mehr dazu finden Sie [**hier**](https://github.com/iqb-berlin/itc-toolbox).

#### Teststeuerung

Die Testleitung kann mittels einer weiteren integrierten Funktion des Testcenters den Ablauf einer Testung steuern. Diese Funktion trägt den Namen **Testleitungskonsole**. Mehr Informationen dazu finden Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.8-Testleitungskonsole).

:information_source: Detaillierte Informationen zum **Testcenter** finden Sie im gleichnamigen Kapitel.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Testcenter öffnen

</td></tr>
<tr>
<td>

Eingabe der Adresse des Testcenters in einen Browser: **www.iqb-testcenter.de**
 
:information_source: **Das Testcenter muss auf einem Server installiert sein.**

Melden Sie sich anschließend mit Ihren Zugangsdaten am Testcenter an. Betätigen Sie nach Eingabe Ihrer Zugangsdaten die Schaltfläche: **Weiter als Admin**. Die Schaltfläche **Weiter** ist für die Anmeldung der Testpersonen gedacht.

:information_source: Die Zugangsdaten erhalten Sie von Ihren Adminstrator\*innen.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Arbeitsbereich wählen

</td></tr>
<tr>
<td>

Wählen Sie Ihren Arbeitsbereich aus. In diesem Beispiel wird der Arbeitsbereich "Sandbox Tobias" geöffnet.

![TS_AB_Auswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_AB_Auswahl_01.png)

:information_source: Die Administrator\*innen geben die Bereiche für Sie frei.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Laden der Testdateien

</td></tr>
<tr>
<td>

Nun ist es an der Zeit die Testdateien: **Testtakers-xml**, **Booklet-xml**, **MEA-xml** und die zugehörigen Ressourcen: **MEA-voud** und **Player-html** in das **Testcenter** zu laden. Auf diese Weise wird dem **Testcenter** bekannt gegeben wie der Test ablaufen soll, welche Booklets angezeigt werden sollen und welche Testpersonen an der Testung teilnehmen. Das Laden der Dateien findet im Arbeitsbereich unter dem Reiter: **Dateien** statt.

:heavy_exclamation_mark: **Da alle Testdateien in Abhängigkeit zueinander stehen, beachten Sie beim Laden der Testdateien die Reihenfolge in welcher Sie die Dateien in das Testcenter laden. Wird dies nicht beachtet, lehnt das Testcenter die Datei mit einem entsprechendem Hinweis ab.** 

Wurden alle Dateien in das Testcenter geladen, befinden sich abschließend alle für den Test benötigten Dateien gruppiert im Arbeitsbereich:

![TC_Laden_Testdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_Laden_Testdateien_01.png)

:information_source: Möchten Sie die Dateien nicht einzeln in das **Testcenter** laden, ist es auch möglich diese in einem Zip-Format zu verpacken und die gesamte Zip-Datei zu laden.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Starten der Testdurchführung

</td></tr>
<tr>
<td>

In der **Testtaker-Xml** sind Zugangsdaten für 6 Testpersonen angelegt. Um die Testung durchzuführen, müssen Sie sich mit den Zugangsdaten einer dieser Testpersonen am **Testcenter** anmelden. Die Testung wird dann in dem festgelegten Modus für diese Person abgespielt. Wie im Schnelleinstieg "Testdateien" aufgezeigt, wurde der Testmodus für die erste Person von `run-review` in `run-hot-return` geändert. In diesem Modus können Sie nach der Testdurchführung auch die gespeicherten Antworten herunterladen. Melden Sie sich nun einmal mit den Zugangsdaten dieser ersten Person an. Dazu öffnen Sie noch einmal die **Testtaker-Xml** und kopieren oder notieren sich die Zugangsdaten für diese Person.

![Testtaker_Login_kopieren](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testtaker_Login_kopieren_02.png)

Melden Sie sich anschließend vom **Testcenter** ab. Klicken Sie dazu auf das IQB-Logo oben links und melden Sie sich mit den notierten Zugangsdaten erneut an. 

:information_source: Testpersonen melden sich über die Schaltfläche "Weiter" am **Testcenter** an. Die Testleitung verwendet für die Anmeldung die Schaltfläche "Weiter als Admin"!

Nach der Anmeldung wird das zu dieser Person angegebene Booklet in der **Testtaker-Xml** mithilfe der eindeutigen Booklet-ID eingebunden und im **Testcenter** zur Auswahl angezeigt. Das Booklet trägt dann den Namen der unter `Label` in der **Booklet-Xml** eingetragen ist.

![Bookletaufruf](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bookletaufruf_02.png)

Nach Auswahl des Booklets muss zuerst das Freigabewort für das Testlet eingegeben werden. Sobald dieses eingegeben wurde, beginnt die Zeit von 10 Minuten abzulaufen und es wird die im Testlet befindliche Aufgabe: **MEA** angezeigt. Nach Ablauf dieser Zeit wird das Testlet gesperrt.

Nachdem das Freigabewort erfolgreich eingegeben wurde, wird Ihnen die erste und einzige Aufgabe in diesem Testlet angezeigt, nämlich unsere Aufgabe "MEA". Der im **Testcenter** angezeigte Name entspricht dem Attribut `label`, welches in der **Booklet-Xml** zur Aufgabe vergeben werden kann.

```xml
<Testlet id="MET" label="Mein erstes Testheft">
      
   <Restrictions>
      <CodeToEnter code="Hase">Bitte gib das Freigabewort ein.</CodeToEnter>
      <TimeMax minutes="10"/>
   </Restrictions>
    
   <Unit id="MEA" label="Aufgabe 1" labelshort="1"/>
            
</Testlet>
```

Wählen Sie nun in der angezeigten Aufgabe "Aufgabe 1" ein Optionsfeld aus und merken Sie sich dieses. Anschließend kann der Test beendet werden. Dies kann auf verschiedenen Wege erfolgen. Entweder betätigen Sie einen der beiden Pfeile (rechts/ links) im Navigationsmenu oben rechts und verlassen damit das zeitbeschränkte Testlet. Oder Sie klicken einmal auf das IQB-Logo oben links. In beiden Fällen erscheint ein Hinweis, dass ein zeitbeschränkter Bereich verlassen werden soll und das Testlet anschließend gesperrt wird. Bestätigen Sie diesen Hinweis mit "Test beenden". 

Es handelt sich an dieser Stelle um ein sehr vereinfachtest Beispiel mit nur einer Aufgabe. Würden sich weitere Aufgaben im Testlet befinden, könnten Sie über das Navigationsmenu oben rechts zur nächsten Aufgabe wechseln und müssten den Test noch nicht an dieser Stelle beenden. Probieren Sie es aus und legen Sie weitere Aufgaben in Ihrem Testlet an.

:information_source: Kleiner Tipp: Im Navigationsmenu oben rechts sind zwei Pfeile und eine Aufgabe mit der Bezeichnung "1" zu sehen. Die "1" kommt aus der **Booklet-Xml** und ist der Unit über das Attribut `Labelshort` zugewiesen. An dieser Stelle haben Sie also die Möglichkeit den Bezeichner anzupassen.

```xml
<Unit id="MEA" label="Aufgabe 1" labelshort="1"/>
```

</td></tr>
<tr>
<td>

### :heavy_check_mark: Auswertung der Testung

</td></tr>
<tr>
<td>

Wurde eine Testung in einem entsprechenden Modus (nicht jeder Modus speichert Antworten) durchgeführt, werden alle gegebenen Antworten personenspezifisch gespeichert. Sie finden die gegebenen Antworten dann in dem Arbeitsbereich in welchem sich auch die Testdateien befinden. Melden Sie sich dazu wieder als Testleitung (Schaltfläche "Weiter als Admin") an und wechseln Sie in Ihren Arbeitsbereich. Dort gehen Sie zum Reiter "Ergebnisse/Antworten". Dort sollten Sie nun den Namen Ihrer Login-Gruppe finden. Vielleicht erinnern Sie sich noch? Der Name der Login-Gruppe wurde in der **Testtakers-Xml** angegeben. In diesem Beispiel wurde der vom **Studio** automatisch erzeugte Name in **MEG** umbenannt.

![Testtakers Group-ID](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testtakers_Group-ID.png)

Um die Datei der gespeicherten Antworten zu öffnen, setzen Sie den Haken vor der Login-Gruppe **MEG** und betätigen Sie die Schaltfläche: "Antworten". Die Datei wird dann im angegebenen Verzeichnis gespeichert. Anschließend kann diese Datei mit Excel geöffnet werden.

![gespeicherte Anworten](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/gespeicherte_Antworten.png)

In der Spalte "Responses" befinden sich nun die gespeicherten Zustände der Aufgabenelemente, in diesem Fall des Optionsfelds. Da das Optionsfeld aus mehreren Teilen besteht, wie bspw. einer Überschrift, mehreren Zeilen für die Optionen, sind auch all diese Teile in dieser Spalte aufgeführt. Damit es nun etwas übersichtlicher wird und nur die Teile des Aufgabenelements angezeigt werden die in diesem Fall interessant sind, nämlich die eigentlichen Optionsfelder, ist es möglich diese Datei nachträglich zu bearbeiten. Hierfür kann die eingangs schon erwähnte Anwendung **itc-Toolbox** verwendet werden. Wird die Datei mittels dieser Anwednung gewandelt, sieht das Ergebnis wie folgt aus:

![gespeicherte Anworten Wandlung itc](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/gespeicherte_Antworten_itc.png)

Hier ist nun eindeutig zu sehen, dass dieser Testung die Option 1 gewählt wurde. Damit ist nun auch die Auswertung abgeschlossen.

:information_source: Jedes Aufgabenelement in einer Aufgabe wird über die Aufgabenelement-ID eindeutig identifiziert. In der Auswertung kann dann über diese ID die Auswertung des entsprechenden Aufgabenelements erfolgen.

Sie haben nun Ihre erste eigene Testung durchgeführt. Da hier nur ein sehr einfaches Bsp. zum Einsatz kam, probieren Sie gerne einmal mehr aus und binden Sie weitere Aufgaben zu Testheften und Booklets zusammen und führen Sie größere Testungen durch.

</td></tr>

</table>

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Testdateien">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---