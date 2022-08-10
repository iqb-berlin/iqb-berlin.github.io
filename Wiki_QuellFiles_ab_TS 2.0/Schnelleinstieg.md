# TBA Schnelleinstieg

Im Rahmen der digitalisierten Testung hat das **IQB** zwei webbasierte Anwendungen entwickelt.

Eine Anwendung wird für das Aufgabenmanagement und die Aufgabenentwicklung verwendet und trägt den Namen **Studio**. Ein integrierter **Editor** übernimmt dabei den eigentlichen Aufgabenentwurf. 

Eine weitere Anwendung trägt den Namen **Testcenter** und wird für die Testdurchführung und Auswertung einer Testung verwendet.

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

In diesem Beispiel befinden sich bereits einige Aufgaben im geöffneten Arbeitsbereich. Fügen Sie nun eine neue Aufgabe hinzu. Wählen Sie anschließend einen eindeutigen Namen für die Aufgabe. In diesem Beispiel wird er Name "MEA" vergeben. "MEA" soll für "Meine erste Aufgabe" stehen. Sie können diese Aufgabe dann noch zur besseren Übersicht einer Gruppe hinzufügen. 

:information_source: Eine Aufgabe wird übrigens auch Unit genannt!

![TS_Aufgabe_anlegen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Aufgabe_anlegen_01.gif)

:heavy_exclamation_mark: **Wählen Sie kurze ID-fähige Namen, die Ihre Aufgabe eindeutig identifizieren und diese von anderen Aufgaben sehr wahrscheinlich unterscheiden.**

</td></tr>
<tr>
<td>

### :heavy_check_mark: Auswahl Editor und Player

</td></tr>
<tr>
<td>

Bevor Sie mit dem Aufgabentwurf starten, müssen Sie festlegen mit welchem Editor Sie die Aufgabe entwerfen möchten. Jeder vom IQB angebotene Editor verfügt über spezifische Eigenschaften und Funktionen. Wählen Sie den Aspect-Editor, wenn Sie Ihre Aufgabe mittels vorgefertigter Elemente entwerfen wollen und wenn sich die Aufagebansicht dynamisch an andere Bildschirmgrößen anpassen soll. Wählen Sie den Editor für Text, wenn Sie Ihre Aufgabe mittels einer Scriptsprache entwerfen möchten und auf eine dynamische Ansicht verzichten können.

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

Sie können die Aufgabe vor der finalen Ausgaben durch das **Studio** in einer Vorschau betrachten. Klicken Sie dazu auf den Reiter: "Vorschau". Dort wird Ihre Aufgabe genau so angezeigt, wie sie auch im **Testcenter** angezeigt werden würde. So erkennen Sie schon vor der Ausgabe Fehler und können diese beheben!

![TS_Vorschau](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Vorschau_03.gif)

</td></tr>
<tr>
<td>

### :heavy_check_mark: Ausgabe der Aufgabe

</td></tr>
<td>

Im nächsten Schritt lassen Sie Ihre Aufgabe mit dem **Studio** ausgeben.

![Studio Output Formular](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Output_Formular_01.png)

Es können entweder nur die Dateien zu einer Aufgabe ausgeben werden oder weitere Dateien, die den späteren Testablauf im **Testcenter** steuern können. Nachfolgend werden diese zusätzlichen Dateien aufgeführt und deren Verwendung wird kurz beschrieben. Genauere Informationen zu diesen Dateien finden Sie im Kapitel: "Die Testdateien".

**Player-Html**<br>
Wiedergabe der Aufgaben im **Testcenter**. Diese Datei wird auch als **Player-Ressource** bezeichnet.

**Booklet-Xml**<br>
Bündelung ausgewählter Aufgaben zu Testheften.

**Testtaker-Xml**<br>
Festlegungen in welchem Modus die Testung ablaufen soll und anlegen der Zugangsdaten für die Testpersonen.

Schauen wir uns an was das **Studio** nun erzeugt hat.

![Studio_Outputdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Studio_Outputdateien_01.png)

Es wird zu jeder Aufgabe jeweils eine **VOUD-Datei** und eine **XML-Datei** erzeugt. Alle Inhalte einer Aufgabe befinden sich nun in diesen beiden Dateien. In diesem Beispiel wurde auch die Ausgabe der Player-Ressource und die Ausgabe der beiden Dateien zur Teststeuerung gewünscht. Diese 3 Dateien: **Booklet-Xml**, **Testtakers-Xml** und **iqb-player-aspect@1.25-Html** befinden sich nun zusätzlich zu den Dateien der Aufgabe im Ausgabeordner.

:information_source: Hiermit ist der Aufgabenentwurf mit dem **Studio** abgeschlossen!

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

Um eine Testung mit dem **Testcenter** durchführen zu können, müssen vorab die gewünschten Dateien für die Testung in das **Testcenter** geladen werden. Wie im Schnelleinstieg zum **Studio** bereits beschrieben wurde, gibt das **Studio** nach dem Aufgabenentwurf die zugehörigen Testdateien aus. Werden vom **Studio** nicht nur die Aufgaben-Xml`s ausgegeben, sondern auch noch die Steuerdateien **Booklet-Xml** und **Testtakers-Xml**, werden automatisch Abhängigkeiten zwischen den Testdateien hergestellt.

Folgende Abhängigkeiten werden zwischen den Testdateien erzeugt: 

![Abhängigkeiten Testdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Abhängigkeiten_Testdateien_02.png)

Die **Testtaker-Xml** bindet die **Booklet-Xml** ein. Die **Booklet-Xml** bindet die **Aufgaben-Xml** ein. Die **Aufgaben-Xml** wiederum bindet die Ressourcen-Dateien **Aufgaben-Voud** und **Player.html** ein.

Einige Abhängigkeiten und Werte wurde bereits automatisch in den beiden Steuerdateien **Testtaker-Xml** und **Booklet-Xml** bei der Ausgabe durch das **Studio** gesetzt. Bspw. wurden in der **Testtaker-Xml** 6 Logins mit einem Passwort und einem Review-Modus angelegt. Manchmal reichen diese Automatismen des **Studios** aber nicht aus um eine Testung den spezifischen Anforderungen entsprechend anzupassen. In diesem Fall sind die Testdateien manuell anzupassen. Nachfolgend wird noch einmal die Funktion der Testdateien beschrieben und wie diese manuell an die spezifischen Testanforderungen angepasst werden können.

:information_source: Wollen Sie noch etwas mehr zu den Funktionen der Testdateien erfahren? Schauen Sie sich gerne das [**Video**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Die-Testdateien) zu diesem Thema an,

:information_source: Mehr Informationen zu den einzelnen Testdateien finden Sie auch im Abschnitt: "Direkt zu anderen Seiten". 

</td></tr>
<tr>
<td>

### :heavy_check_mark: XML-Schema Definition

</td></tr>
<tr>
<td>

Die verwendeten Testdateien sind XML-Dateien. Damit diese XML-Dateien auch vom **Testcenter** gelesen werden können, dürfen diese nur definierte Inhalte aufweisen. Welche Inhalte erlaubt sind, legt eine so genannte Schema-Definition fest. Hierbei handelt es sich grob gesagt um eine Vorlage, wie die entsprechende Xml-Datei auszusehen hat. Spezielle Editoren gleichen bereits bei der manuellen Bearbeitung auf Wunsch den aktuellen Inhalt mit der Schema-Definition ab und melden eventuelle fehlerhafte Inhalte. Diese können dann bereits vor dem Laden in das **Testcenter** korrigiert werden. Spätestens beim Laden in das **Testcenter** erfolgt ein Abgleich der zu ladenden Xml-Datei mit der deklarierten Schema-Definition. Wo diese Definition zu finden ist, wird in der jeweiligen Xml-Datei direkt am Anfang angegeben. Der Verweis auf diese Schema-Definition beginnt dann mit `xmlns:xsi`.


</td></tr>
<tr>
<td>

### :heavy_check_mark: Ressourcendatei für den Player

</td></tr>
<tr>
<td>

Während der Aufgabenerstellung im **Studio** wird festgelegt mit welchem Editor die Aufgaben erstellt werden soll. Außerdem wird angegeben mit welchem Player die Aufgabeninhalte später wiedergegeben werden. Dabei ist zu beachten, dass Editor und Player immer zueinander passen müssen. Wird bspw. der Aspect-Editor verwendet, muss auch der Aspect-Player verwendet werden. Gewählter Player und Editor werden beim Export durch das  **Studio** in der Aufgabe-Xml hinterlegt. Sobald Aufgaben in das **Testcenter** geladen werden, prüft das **Testcenter**, ob der in der Aufgaben-Xml angegebene Player in das **Testcenter** geladen wurde. Das **Testcenter** hat nicht jeden Programmcode zu jedem Player hinterlegt, daher muss der Programmcode des jeweiligen Players mit in das **Testcenter** geladen werden. Dies geschieht mittels der Ressourcendatei zum Player. In unserem Fall trägt diese Datei den Namen: **iqb-player-aspect@1.24.html**. 

:heavy_exclamation_mark: **Werden Aufgaben in das Testcenter geladen, muss auch immer die zugehörige Ressourcendatei für den Player mit das Testcenter geladen werden.**


</td></tr>
<tr>
<td>

### :heavy_check_mark: Aufgaben XML-/ und VOUD-Datei

</td></tr>
<tr>
<td>

Zu jeder im **Studio** erzeugten Aufgabe werden je 2 Dateien erstellt. Eine Datei mit der Endung **XML** und eine weitere mit der Endung **VOUD**. Beiden Dateien wird der Aufgabenname vorangestellt. In der Voud-Datei befinden sich alle Aufgabeninhalte, sprich alle Aufgabenelemente. In der Xml-Datei sind zugehörige Metadaten wie bspw. der Aufgabenname und Kurzbeschreibung der Aufgabe angelegt. Außerdem wird hier angegeben welcher Editor und Player bei der Aufgabenerstellung verwendet wurde. Es findet weiterhin ein Verweis auf die zugehörige VOUD statt. Prinzipiell können beide Dateien manuell nachträglich bearbeitet werden, bevor sie in das **Testcenter** geladen werden. In der Voud-Datei sind manuelle Änderungen allerdings schwierig, da die Struktur unübersichtlich erscheint. In der Xml-Datei sind Änderungen hingegen mittels eines Editors einfach umzusetzen. Nachfolgend ist einmal die zur Aufgabe: **MEA01.xml** erzeugte Xml-Datei dargestellt.

![Unit-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Unit_Xml_01.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Unit_Xml_01.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Booklet.xml

</td></tr>
<tr>
<td>

Mittels **Booklet.xml** wird festgelegt in welcher Reihenfolge Aufgaben der Testperson präsentiert werden. Werden Aufgaben in Testheften zusammengefasst, ist es weiterhin möglich Zugangsbeschränkungen und zeitliche Limits festzulegen. Außerdem kann in der **Booklet-Xxml** mittels spezifischer Parameter (Booklet Konfiguration) festgelegt werden, wie zwischen den Aufgaben navigiert werden kann. Bspw. kann das Weiterblättern zur nächsten Aufgabe von bestimmten Bedingungen abhängig gemacht werden. Nachfolgend werden die Strukturen der **Booklet-xml** einmal kurz aufgezeigt.

:information_source: Die hier gezeigte **Booklet-Xml** ist beim Export durch das **Studio** automatisch erzeugt wurden. Hier werden nur grundsätzliche Strukturen erzeugt. Es fehlen bspw. Testhefte und spezifische Booklet Konfigurationen.

![Booklet-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Booklet_Xml_02.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Booklet_Xml.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Booklet.xml: Testheft hinzufügen

</td></tr>
<tr>
<td>

Bei der automatischen Generierung durch das **Studio** ist in der **Booklet-Xml** noch kein Testheft angelegt, sondern nur die erstelle Aufgabe: "MEA". Fügen Sie nun einmal zum besseren Verständnis ein Testheft (Testlet) hinzu. Anschließend verschieben Sie die Aufgabe: "MEA" in dieses Testheft. Das Testheft soll dann noch eine Zeitbeschränkung `TimeMax` und eine Zugangsbeschränkung `CodeToEnter` erhalten. Testpersonen können dann bei einer finalen Testung erst nach Eingabe des Freigabewortes die Aufgabe bearbeiten. Die Aufgabe muss dann innerhalb der angegeben Zeit bearbeitet werden.

![Booklet:Testheft](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Booklet_Testlet_04.gif)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Booklet_Testheft_Xml.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Testtaker.xml

</td></tr>
<tr>
<td>

In der Testtakers können Logins für die Testpersonen angelegt werden. Dabei stehen verschiedene Anmeldemöglichkeiten zur Verfügung. Mit Passwort, ohne Passwort, als Link usw.. Mehr dazu finden Sie auch [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren).

Es wird angegeben welches Booklet die jeweilige Testperson bearbeiten soll. Außerdem wird hier der Modus der Testung festgelegt. Mit diesem Modus wird festgelegt wie der Test ablaufen soll (Probelauf, finale Testung). Mehr Informationen finden Sie dazu auch [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung).

Es ist auch möglich einzelne Texte in der Anwendung **Testcenter** zu verändert. Die Texte können dann in der **Custom-Text-Konfiguration** geändert werden. In der automatisch erzeugten **Testtaker-Xml** durch das **Studio** ist noch keine **Custom-Text-Konfiguration** enthalten. Diese muss der **Testtaker-Xml** hinzugefügt werden. Mehr dazu finden Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml) unter **Custom-Text-Konfiguration**. 

![Testtaker-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testtaker_Xml_03.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Testtaker_Xml.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Testtaker.xml: Testmodus ändern

</td></tr>
<tr>
<td>

Jeder Testmodus weist spezifische Eigenschaften auf. So werden bspw. Anworten einer Testung im Modus: `run-review` nicht gespeichert, im Modus: `run-hot-return` oder `run-hot-restart` aber schon. Eine Übersicht welcher Modus welche Funktionen bietet finden Sie [**hier**](https://github.com/iqb-berlin/testcenter-frontend/blob/master/docs/test-mode.md). 

Da mit den hier verwendeten Dateien später im **Testcenter** eine Testung gestartet werden soll und abschließend auch eine Auswertung der gegebenen Antworten erfolgen soll, sollten Sie für eine Testperson den Modus: von `run-review` auf `run-hot-return` ändern und die Änderung anschließend speichern.

![Testmodus ändern](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testmodus_aendern_02.png)

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

Das Testcenter stellt bestimmte Anforderungen an die Computer auf denen eine Testung durchgeführt wird. Diese Anforderungen können mit der im Testcenter intergrierten Funktion **System-Check** überprüft werden.  [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.7-System-Check) finden Sie mehr Informationen zum **System-Check**. Welche Anforderungen das Testcenter stellt, finden Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2-Testcenter) unter der Überschrift: "Anforderungen".

#### Zugang für die Testpersonen

Im Vorfeld sollte sich die Testleitung Gedanken darüber machen welcher Personenkreis getestet werden soll und wie die Testpersonen die Zugangsdaten erhalten. Mehr Informationen dazu erhalten Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren). 

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
 
:heavy_exclamation_mark: **Das Testcenter muss dazu auf Ihrem Server installiert sein.**

Melden Sie sich anschließend mit Ihren Zugangsdaten am Testcenter an. Betätigen Sie nach Eingabe Ihrer Zugangsdaten die Schaltfläche: **Weiter als Admin**. Die Schaltfläche **Weiter** ist für die Anmeldung der Testpersonen gedacht.

:information_source: Die Zugangsdaten erhalten Sie von Ihren Adminstrator\*innen.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Arbeitsbereich wählen

</td></tr>
<tr>
<td>

Wählen Sie Ihren Arbeitsbereich aus. In diesem Beispiel wird der Arbeitsbereich: "Sandbox Tobias" geöffnet.

![TS_AB_Auswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_AB_Auswahl_01.png)

:information_source: Die Administrator\*innen geben die Bereiche für Sie frei.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Laden der Testdateien

</td></tr>
<tr>
<td>

Nun ist es an der Zeit die Testdateien: **Testtakers-xml**, **Booklet-xml**, **MEA01-xml** und die zugehörigen Ressourcen: **MEA01-voud** und **Player-html** in das **Testcenter** zu laden. Auf diese Weise geben wir dem **Testcenter** bekannt, wie der Test ablaufen soll, welche Booklets angezeigt werden sollen und welche Testpersonen an der Testung teilnehmen. Das Laden der Dateien findet im Arbeitsbereich unter dem Reiter: **Dateien** statt.

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

In der **Testtaker-Xml** sind Zugangsdaten für 6 Testpersonen angelegt. Um die Testung durchzuführen, müssen Sie sich mit den Zugangsdaten einer dieser Testpersonen am **Testcenter** anmelden. Die Testung wird dann in dem festgelegten Modus für diese Person abgespielt. Wie im Schnelleinstieg: "Testdateien" aufgezeigt, haben wir den Testmodus für die erste Person von `run-review` in `run-hot-return` geändert. In diesem Modus können Sie nach der Testdurchführung auch die gespeicherten Antworten herunterladen. Melden Sie sich nun einmal mit den Zugangsdaten dieser ersten Person an. Dazu öffnen Sie noch einmal die **Testtaker-Xml** und kopieren oder notieren sich die Zugangsdaten für diese Person.

![Testtaker_Login_kopieren](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testtaker_Login_kopieren.gif)

Melden Sie sich anschließend vom **Testcenter** ab. Klicken Sie dazu auf das IQB-Logo oben links und melden Sie sich mit den notierten Zugangsdaten erneut an. 

:information_source: Testpersonen melden sich über die Schaltfläche: "Weiter" am **Testcenter** an. Die Testleitung verwendet für die Anmeldung die Schaltfläche: "Weiter als Admin"!

Nach der Anmeldung wird Ihnen das zu dieser Person angegebene Booklet angeboten. Das Booklet trägt dann den Namen der unter `Label` in der **Booklet-Xml** eingetragen ist.

![Bookletanzeige](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bookletanzeige_06.png)

Nach Auswahl des Booklets, müssen Sie wie in der **Booklet-Xml** angegeben, ein Freigabewort eingeben. Erst dann wird Ihnen die in der **Booklet-Xml** angelegte Aufgabe (MEA-Xml) angezeigt. Nun haben Sie 10 Minuten Zeit die Aufgabe zu beantworten. Beantworten Sie die Aufgabe in dieser Zeit nicht, wird das Testheft gesperrt. 

![Booklet Beschraenkungen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Booklet_Beschraenkungen_01.png)

Sobald Sie die Aufgabe beantwortet haben, klicken Sie im Menu oben rechts auf "Test beenden". Sie werden darauf hingewiesen, dass Sie einen zeitbeschränkten Bereich verlassen und nicht zurückkehren können. Bestätigen Sie diese Meldung um den Test zu beenden.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Auswertung der Testung

</td></tr>
<tr>
<td>

Wurde eine Testung in einem entsprechenden Modus (nicht jeder Modus speichert Antworten) durchgeführt, werden alle gegebenen Antworten personenspezifisch gespeichert. Sie finden die gegebenen Antworten dann in dem Arbeitsbereich in welchem sich auch die Testdateien befinden. Melden Sie sich dazu wieder als Testleitung (Schaltfläche: "Weiter als Admin") an und wechseln Sie in Ihren Arbeitsbereich. Dort gehen Sie zum Reiter: "Ergebnisse/Antworten". Dort sollten Sie nun den Namen Ihrer Login-Gruppe finden. Vielleicht erinnern Sie sich noch? Der Name der Login-Gruppe wurde in der **Testtakers-Xml** angegeben. In diesem Beispiel wurde der vom **Studio** automatisch erzeugte Name in **MEG** umbenannt.

![Testtakers Group-ID](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testtakers_Group-ID.png)

Um die Datei der gespeicherten Antworten zu öffnen, setzen Sie den Haken vor der Login-Gruppe **MEG** und betätigen Sie die Schaltfläche: "Antworten". Die Datei wird dann im angegebenen Verzeichnis gespeichert. Anschließend kann diese Datei mit Excel geöffnet werden.

![gespeicherte Anworten](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/gespeicherte_Antworten.png)

In der Spalte: "Responses" befinden sich nun die gespeicherten Zustände unserer Aufgabenelemente, in unserem Fall des Optionsfelds. Da das Optionsfeld aus mehreren Teilen besteht, wie bspw. einer Überschrift, mehreren Zeilen für die Optionen, sind auch all diese Teile in dieser Spalte aufgeführt. Damit es nun etwas übersichtlicher wird und nur die Teile des Aufgabenelements angezeigt werden die für uns interessant sind, nämlich die eigentlichen Optionsfelder, ist es möglich diese Datei nachträglich zu bearbeiten. Hierfür kann die eingangs schon erwähnte Anwendung **itc-Toolbox** verwendet werden. Wird die Datei mittels dieser Anwednung gewandelt, sieht das Ergebnis wie folgt aus:

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