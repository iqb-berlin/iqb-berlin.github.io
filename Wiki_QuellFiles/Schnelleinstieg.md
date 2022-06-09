# TBA Schnelleinstieg

Im Rahmen der digitalisierten Testung hat das **IQB** zwei webbasierte Anwendungen entwickelt.

Eine Anwendung wird für das Aufgabenmanagement und die Aufgabenentwicklung verwendet und trägt den Namen **Teststudio**. Ein integrierter **Editor** übernimmt dabei den eigentlichen Aufgabenentwurf. 

Eine weitere Anwendung trägt den Namen **Testcenter** und wird für die Testdurchführung und Auswertung einer Testung verwendet.

Sind Aufgaben mit dem **Teststudio** final entworfen, können diese abschließend in einem bestimmten Dateiformat vom **Teststudio** ausgegeben werden. Die so ausgegebenen Dateien können bei Bedarf nachträglich verändert werden. Zur Testdurchführung werden diese Dateien dann in das **Testcenter** geladen und wiedergegeben.


Lernen Sie beiden Anwendung **Teststudio** und **Testcenter** und die Bearbeitung der **Testdateien** doch einmal kurz kennen:

<table border=0 >
    <tr>
        <th align=center>
            <img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Symbol_004.png" alt="Alt-Text" title="Teststudio Symbol" />
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
            <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Das-Teststudio">Teststudio</a>
        </th>
        <th align=center>
           <a href=""></a>
        </th>
        <th align=center>
           <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Die-Testdateien">Testdateien</a>
        </th>
        <th align=center>
           <a href=""></a>
        </th>
        <th align=center>
           <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Das-Testcenter">Testcenter</a>
        </th>
    </tr>
</table>

:information_source: Detailiertere Informationen zu den Anwendungen finden Sie in den gleichnamigen Kapiteln dieser Wiki.

<!--###################################################################################################################### -->
## Schnelleinstieg: Das Teststudio
<!--###################################################################################################################### -->

<table border=1>
<tr>
<th align=center>

### Entwerfen Sie Ihre erste Aufgabe mit dem Teststudio

</th>

</tr>
<tr>
<td>

### :heavy_check_mark: Teststudio öffnen

</td></tr>
<tr>
<td>

Eingabe der Adresse des Teststudios in einem Browser: **www.iqb-teststudio.de**
 
:heavy_exclamation_mark: Das Teststudio muss dazu auf Ihrem Server installiert sein.

Melden Sie sich anschließend mit Ihren Zugangsdaten am Teststudio an.

:heavy_exclamation_mark: Die Zugangsdaten erhalten Sie von Ihren Adminstrator\*innen.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Arbeitsbereich wählen

</td></tr>
<tr>
<td>

Wählen Sie Ihren Arbeitsbereich aus. In diesem Beispiel werde ich meinen Arbeitsbreich: *Tobias* öffnen.

:heavy_exclamation_mark: Die Administrator\*innen geben die Bereiche für Sie frei.

![TS_AB_Auswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_AB_Auswahl_03.png)


</td></tr>
<tr>
<td>

### :heavy_check_mark: Aufgabe anlegen

</td></tr>
<tr>
<td>

Legen Sie eine neue Aufgabe an oder bearbeiten Sie eine bestehende Aufgabe durch Markierung der Aufgabe.

Es besteht bereits eine Aufgabe mit dem Namen: *UEA01* in meinem Arbeitsbereich und ich füge eine weiterer Aufgabe mit dem Namen: *MEA* hinzu.

:information_source: Eine Aufgabe wird auch Unit genannt!

![TS_Aufgabe_anlegen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Aufgabe_anlegen_01.gif)

:heavy_exclamation_mark: Wählen Sie kurze ID-fähige Namen, die Ihre Aufgabe eindeutig identifizieren und diese von anderen Aufgaben sehr wahrscheinlich unterscheiden.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Auswahl Editor und Player

</td></tr>
<tr>
<td>

Bevor Sie mit dem Aufgabentwurf starten, müssen Sie festlegen mit welchem Editor Sie die Aufgabe entwerfen möchten. Jeder vom IQB angebotene Editor verfügt über eigene Eigenschaften und Funktionen. Wählen Sie den Aspect-Editor, wenn Sie Ihre Aufgabe mittels vorgefertigter Elemente entwerfen wollen und wenn sich die Aufagebansicht dynamisch an andere Bildschirmgrößen anpassen soll. Wählen Sie den Editor für Text, wenn Sie Ihre Aufgabe mittels einer Scriptsprache entwerfen möchten und auf eine dynamische Ansicht verzichten können.

Ist der Editor ausgewählt, muss auch ein zum Editor passender Player gewählt werden. Der Player gibt die Aufgabe mit Ihren Aufgabenelementen dann sowohl in der Vorschau als auch später bei der Testdurchführung im **Testcenter** wieder.

![TS_Editorwahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Editorwahl_02.gif)


 Player und Editor werden in verschieden Versionständen angeboten. Wählen Sie immer die aktuellste Version.

:heavy_exclamation_mark: An dieser Stelle können Sie die Aufgabe auch schon einmal speichern.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Der Editor

</td></tr>
<tr>
<td>

Jetzt gehts los! Starten Sie den zuvor ausgewählten Editor mithilfe des gleichnamigen Reiters.

![TS_Editorreiter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Editor_Reiter_01.png)

Soll sich Ihre Aufgabe dynamisch an entsprechende Bildschirmgrößen anpassen, wählen Sie zuvor einen dynamischen Abschnitt aus.

![TS_Editor_dynamisch](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Editor_dynamisch.gif)

Legen Sie ihr erstes Aufgabenelement in Ihrer Aufgabe an und speichern Sie die Aufgabe. Ich wähle einmal ein Optionsfeld.

![TS_Elementenauswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Elementenauswahl_02.gif)

Vielleicht möchten Sie die Aufgabe vorher betrachten bevor sie ausgegeben wird? Klicken Sie dazu auf den Reiter: *Vorschau*. Dort wird Ihre Aufgabe genau so angezeigt wie sie auch im **Testcenter** angezeigt werden würde.

![TS_Vorschau](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Vorschau_04.gif)

</td></tr>
<tr>
<td>

### :heavy_check_mark: Ausgabe der Aufgabe

</td></tr>
<td>

Jetzt können Sie Ihre Aufgabe mit dem **Teststudio** ausgeben lassen.

![TS_Output](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Output_01.gif)

Was hat das **Teststudio** erzeugt?

Es wird zu jeder Aufgabe jeweils eine Voud-Datei und eine Xml-Datei erzeugt. Alle Inhalte einer Aufgabe befinden sich nun in diesen beiden Dateien. Wird der Haken bei: "Als Paket ausgeben" gesetzt, werden außerdem noch 3 andere Dateien erzeugt, eine `Testtakers.xml`, eine `Booklet.xml` und eine `iqb-player-aspect@1.24.html`. Alles zusammen wird in einer Zip-Datei verpackt ausgegeben.

![TS_Outputdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Outputdateien_03.gif)

**Wollen Sie noch etwas mehr zu den Testdateien erfahren? Schauen Sie sich gerne die [Videos](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Die-Testdateien) zu diesem Thema an.**

:information_source: Hiermit ist der Aufgabenentwurf mit dem **Teststudio** abgeschlossen!

</td></tr>


</table>

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>

!<--###################################################################################################################### -->
## Schnelleinstieg: Die Testdateien
!<--###################################################################################################################### -->

```yaml
Dokumentstatus: In Bearbeitung (THuste)
Stand: 27.05.22
todo: - weitere Inhalte
      
```

<table border=1>
<tr>
<th align=center>

### Passen Sie die Testung Ihren Bedürfnissen an

</th></tr>
<tr>
<td>

### :heavy_check_mark: Kurze Einführung zu den Testdateien

</td></tr>
<tr>
<td>

Um eine Testung mit dem **Testcenter** durchführen zu können, müssen vorab die gewünschten Dateien für die Testung in das **Testcenter** geladen werden. Wie im Schnelleinstieg zum **Teststudio** bereits beschrieben wurde, gibt das **Teststudio** nach dem Aufgabenentwurf die zugehörigen Testdateien aus. Um nun eine Testung den spezifischen Anforderungen entsprechend durchführen zu können, können die Testdateien vor dem Laden in das **Testcenter** angepasst werden. 

:information_source: Wollen Sie noch etwas mehr zu den Funktionen der Testdateien erfahren? Schauen Sie sich gerne die [Videos](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Die-Testdateien) zu diesem Thema an.

</td></tr>
<tr>
<td>

### :heavy_check_mark: XML-Schema Definition

</td></tr>
<tr>
<td>

Die verwendeten Testdateien sind XML-Dateien. Damit diese XML-Dateien auch vom **Testcenter** gelesen werden können, dürfen diese nur definierte Inhalte aufweisen. Welche Inhalte erlaubt sind, legt eine so genannte Schema-Definition fest. Hierbei handelt es sich grob gesagt um eine Vorlage, wie die entsprechende Xml-Datei auszusehen hat. Spezielle Editoren gleichen bereits bei der manuellen Bearbeitung auf Wunsch den aktuellen Inhalt mit der Schema-Definition ab und melden eventuelle fehlerhafte Inhalte. Diese können dann bereits vor dem Laden in das **Testcenter** korrigiert werden. Spätestens bei Laden in das **Testcenter** erfolgt ein Abgleich der zu ladenden Xml-Datei mit der deklarierten Schema-Definition. Wo diese Definition zu finden ist, wird in der jeweiligen Xml-Datei direkt am Anfang angegeben. Der Verweis auf diese Schema-Definition beginnt dann mit `xmlns:xsi`.


</td></tr>
<tr>
<td>

### :heavy_check_mark: Ressourcendatei für den Player

</td></tr>
<tr>
<td>

Während der Aufgabenerstellung im **Teststudio** wird festgelegt mit welchem Editor die Aufgaben erstellt werden soll. Außerdem wird angegeben mit welchem Player die Aufgabeninhalte später wiedergegeben werden. Dabei ist zu beachten, dass Editor und Player immer zueinander passen müssen. Wird bspw. der Aspect-Editor verwendet, muss auch der Aspect-Player verwendet werden. Gewählter Player und Editor werden beim Export durch das  **Teststudio** in den Metadaten zur Aufgabe hinterlegt. Sobald Aufgaben in das **Testcenter** geladen werden, prüft das **Testcenter**, ob der in der Aufgaben-Xml angegebene Player in das **Testcenter** geladen wurde. Das **Testcenter** hat nicht jeden Programmcode zu jedem Player hinterlegt, daher muss der Programmcode des jeweiligen Players mit in das **Testcenter** geladen werden. Dies geschieht mittels Ressourcendatei zum Player. In unserem Fall trägt diese Datei den Namen: **iqb-player-aspect@1.24.html**. 

:heavy_exclamation_mark: Werden Aufgaben in das **Testcenter** geladen, muss auch immer die zugehörige Ressourcendatei für den Player mit das **Testcenter** geladen werden. 


</td></tr>
<tr>
<td>

### :heavy_check_mark: Aufgaben XML-/ und VOUD-Datei

</td></tr>
<tr>
<td>

Zu jeder im **Teststudio** erzeugten Aufgabe werden je 2 Dateien erstellt. Eine Datei mit der Endung XML und eine weitere mit der Endung VOUD. Beiden Dateien wird der Aufgabenname vorangestellt. In der Voud-Datei befinden sich alle Aufgabeninhalte, sprich alle Aufgabenelemente. In der Xml-Datei sind zugehörige Metadaten wie bspw. der Aufgabenname und Kurzbeschreibung der Aufgabe angelegt. Außerdem wird hier angegeben welcher Editor und Player bei der Aufgabenerstellung verwendet wurde. Es findet weiterhin ein Verweis auf die zugehörige VOUD statt. Prinzipiell können beide Dateien manuell nachträglich bearbeitet werden bevor sie in das **Testcenter** geladen werden. In der Voud-Datei sind manuelle Änderungen allerdings schwierig, da die Struktur unübersichtlich erscheint. In der Xml-Datei sind Änderungen hingegen mittels eines Editors einfach umzusetzen. Nachfolgend ist einmal die zu unserer Aufgabe: **MEA01.xml** erzeugte Xml-Datei dargestellt.

![Unit-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Unit_Xml_01.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Unit_Xml_01.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Booklet.xml

</td></tr>
<tr>
<td>

Mittels **Booklet.xml** wird festgelegt in welcher Reihenfolge Aufgaben der Testperson präsentiert werden. Werden Aufgaben in Testheften zusammengefasst ist es weiterhin möglich Zugangsbeschränkungen und zeitliche Limits festzulegen. Außerdem kann in der **Booklet.xml** mittels spezifischer Parameter (Booklet Konfiguration) festgelegt werden, wie zwischen den Aufgaben navigiert werden kann. Bspw. kann das Weiterblättern zur nächsten Aufgabe von bestimmten Bedingungen abhängig gemacht werden. 
Nachfolgend werden die Strukturen der **Booklet.xml** einmal kurz aufgezeigt.

:information_source: Die hier gezeigte **Booklet.xml** ist beim Export durch das **Teststudio** automatisch erzeugt wurden. Hier werden nur grundsätzliche Strukturen erzeugt. Es fehlen bspw. Testhefte und spezifische Booklet Konfigurationen.

![Booklet-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Booklet_Xml.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Booklet_Xml.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Booklet.xml: Testheft hinzufügen

</td></tr>
<tr>
<td>

Bei der automatischen Generierung durch das **Teststudio** ist in der **Booklet.xml** noch kein Testheft angelegt, sondern nur unsere Aufgabe. Wir fügen nun einmal zum besseren Verständnis ein Testheft (Testlet) hinzu. Anschließend verschieben wir unsere Aufgabe in dieses Testheft. Das Testheft soll dann noch eine Zeitbeschränkung `TimeMax` und eine Zugangsbeschränkung `CodeToEnter` erhalten. Testpersonen können dann bei einer finalen Testung erst nach Eingabe des Freigabewortes die Aufgabe bearbeiten. Die Aufgabe muss dann innerhalb der angegeben Zeit bearbeitet werden.

![Booklet:Testheft](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Booklet_Testlet_03.gif)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Booklet_Testheft_Xml.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Die Testtaker.xml

</td></tr>
<tr>
<td>

In der Testtakers können Logins für die Testpersonen angelegt werden. Dabei stehen verschiedene Anmeldemöglichkeiten zur Verfügung. Mit Passwort, ohne Passwort, als Link usw.. Mehr dazu finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren). Es wird angegeben welches Booklet die jeweilige Testperson bearbeiten soll. Außerdem wird hier der Modus der Testung festgelegt. Mit diesem Modus wird festgelegt wie der Test ablaufen soll (Probelauf, finale Testung). Mehr Informationen finden Sie dazu auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung). Es ist auch möglich einzelne Texte in der Anwendung **Testcenter** zu verändert. Die Texte können dann in der CustomText Konfiguration geändert werden. In der automatisch erzeugten **Testtaker.xml** durch das **Teststudio** ist noch keine **Custom Text Konfiguration** enthalten. Diese muss der XML hinzugefügt werden. Mehr dazu finden Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml) unter **Custom Text Konfiguration**. 

![Testtaker-XML](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Testtaker_Xml.png)

> [**Hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Ref_Testtaker_Xml.md) können Sie den Code kopieren.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Testtakers: Gruppen anlegen

</td></tr>
<tr>
<td>

Es können für die Testung Gruppen angelegt werden. Diese enthalten dann Logins für entsprechende Personenkreise.

![TC_Testdateien_Testtakers_Group](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_Testtakers_Group.gif)


:heavy_exclamation_mark: Das **Testcenter** prüft ob der Gruppenname bereits in einem anderen Arbeitsbereich besteht. Verwenden Sie daher für den Gruppennamen Bezeichner, die die Wahrscheinlichkeit verringern, dass eine solche Gruppe bereits existiert. Ein schlechter Name wäre bspw. ""Gruppe1".


</td></tr>
<tr>
<td>

### :heavy_check_mark: Testtakers: Testpersonen anlegen

</td></tr>
<tr>
<td>

Durch das **Teststudio** wurden bereits 6 zufällig generierte Logins mit einem Passwort erzeugt. In diesem Fall nutzen wir diese und ändern Sie nicht.

![TC_Testdateien_Testtakers_Login](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_Testtakers_Login.gif)

:heavy_exclamation_mark: Wählen Sie als Loginname möglichst ID-fähige Namen und vermeiden Sie Klarnamen. Das **Testcenter** prüft ob der Login bereits in einem anderen Arbeitsbereich existiert. So verringern Sie die Wahrscheinlichkeit eines Duplikates.


</td></tr>
<tr>
<td>

### :heavy_check_mark: Testtakers: Testmodus festlegen

</td></tr>
<tr>
<td>

Für jede Testung kann mithilfe eines festgelegten Modus bestimmt werden wie die Testung ablaufen soll. Soll es sich bspw. nur um einen Probelauf oder um eine finale Testung handeln. Wir wollen hier einmal einmal einmal eine finale Testung durchführen und wählen hierfür den Modus: run-hot-return



:information_source: Mehr über die Modi und deren Funktionen erfahren Sie [**hier**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Modi-der-Testdurchf%C3%BChrung)

Wir wollen hier einmal einmal einmal eine finale Testung durchführen und wählen hierfür den Modus: run-hot-return


</td></tr>
<tr>
<td>

### :heavy_check_mark: Testtakers: Booklet auswählen

</td></tr>
<tr>
<td>

Jeder angelegten Testperson kann ein entsprechendes Booklet zugewiesen werden. Die Testpersonen sind entsprechenden In diesem Booklet sind dann die Aufgaben für jeweilige Testpersongebündelt 

</td></tr>
</table>

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>


!<--###################################################################################################################### -->
## Schnelleinstieg: Das Testcenter
!<--###################################################################################################################### -->

```yaml
Dokumentstatus: In Bearbeitung (THuste)
Stand: 16.05.22
todo: - weitere Inhalte

```
<table border=1>
<tr>
<th align=center>

### Führen Sie die erste Testung durch

</th>
</tr>
<tr>
<td>

### :heavy_check_mark: Öffnen des Testcenters

</td></tr>
<tr>
<td>

Eingabe der Adresse des Teststudios in einem Browser: **www.iqb-teststudio.de**
 
:heavy_exclamation_mark: Das Teststudio muss dazu auf Ihrem Server installiert sein.

Melden Sie sich anschließend mit Ihren Zugangsdaten am Teststudio an.

:heavy_exclamation_mark: Die Zugangsdaten erhalten Sie von Ihren Adminstrator\*innen.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Arbeitsbereich wählen

</td></tr>
<tr>
<td>

Wählen Sie Ihren Arbeitsbereich aus. In diesem Beispiel werde ich meinen Arbeitsbreich: *Tobias* öffnen.

:heavy_exclamation_mark: Die Administrator\*innen geben die Bereiche für Sie frei.

![TS_AB_Auswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_AB_Auswahl_03.png)


</td></tr>
</table>

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>