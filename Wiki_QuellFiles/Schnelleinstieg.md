# TBA Schnelleinstieg

```yaml
Dkumentstatus: in Bearbeitung (THuste)
Stand: 13.05.22
todo: - weitere Inhalte
      
```
Im Rahmen der digitalisierten Testung hat das **IQB** zwei webbasierte Anwendungen entwickelt.

Eine Anwendung wird für das Aufgabenmanagement und die Aufgabenentwicklung verwendet und trägt den Namen **Teststudio**. Ein integrierter **Editor** übernimmt dabei den eigentlichen Aufgabenentwurf. 

Eine weitere Anwendung trägt den Namen **Testcenter** und wird für die Testdurchführung und Auswertung einer Testung verwendet.

Sind Aufgaben mit dem **Teststudio** final entworfen, können diese abschließend in einem bestimmten Dateiformat vom **Teststudio** ausgegeben werden. Die so ausgegebenen Dateien können bei Bedarf nachträglich verändert werden. Zur Testdurchführung werden diese Dateien dann in das **Testcenter** geladen und wiedergegeben.


Lernen Sie beiden Anwendung **Teststudio** und **Testcenter** doch einmal kurz kennen:

<table border=0 >
    <tr>
        <th align=center width=500>
            <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Das-Teststudio">Das Teststudio</a>
        </th>
        <th align=center width=500>
             <a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg:-Das-Testcenter">Das Testcenter</a>
        </th>
    </tr>
</table>


:information_source: Detailiertere Informationen zu den Anwendungen finden Sie in den gleichnamigen Kapiteln dieser Wiki.

!<--###################################################################################################################### -->
## Schnelleinstieg: Das Teststudio
!<--###################################################################################################################### -->

<table border=1>
<tr>
<th align=center width=1000>

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


:heavy_exclamation_mark: Player und Editor werden in verschieden Versionständen angeboten. Wählen Sie immer die aktuellste Version.

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
## Schnelleinstieg: Das Testcenter
!<--###################################################################################################################### -->

```yaml
Dokumentstatus: In Bearbeitung (THuste)
Stand: 16.05.22
todo: - warte auf Feedback
      
```
<table border=1>
<tr>
<th align=center width=1000>

### Führen Sie die erste Testung durch

</th>

</tr>
<tr>
<td>

### :heavy_check_mark: Die Testdateien

</td></tr>
<tr>
<td>

Um eine Testung mit dem **Testcenter** durchführen zu können, müssen vorab die gewünschten Dateien für die Testung in das **Testcenter** geladen werden. Wie im Schnelleinstieg zum **Teststudio** bereits beschrieben wurde, gibt das **Teststudio** nach dem Aufgabenentwurf die zugehörigen Testdateien aus. Um nun eine Testung den spezifischen Anforderungen entsprechend durchführen zu können, können die Testdateien vor dem Laden in das **Testcenter** angepasst werden. Zum besseren Verständnis folgt nun eine kurze Beschreibung der Dateien. Wir orientieren uns hierfür an den zuvor durch das **Teststudio** ausgegebenen Dateien.

![TS_Outputdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Outputdateien_03.gif)















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


:heavy_exclamation_mark: Player und Editor werden in verschieden Versionständen angeboten. Wählen Sie immer die aktuellste Version.

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

Es wird zu jeder Aufgabe jeweils eine Voud-Datei und eine Xml-Datei erzeugt. Alle Inhalte einer Aufgabe befinden sich nun in diesen beiden Dateien. Wird der Haken bei: "Als Paket ausgeben" gesetzt, werden außerdem noch 3 andere Dateien erzeugt, eine `Testtakers.xml`, eine `Booklet.xml` und eine `iqb-player-aspect@1.24.html` . Im Schnelleinstieg zum **Testcenter** werden wir uns diese Dateien noch einmal näher anschauen. Alles zusammen wird in einer Zip-Datei verpackt ausgegeben.

![TS_Outputdateien](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Outputdateien_03.gif)

:information_source: Hiermit ist der Aufgabenentwurf mit dem **Teststudio** abgeschlossen!

</td></tr>


</table>

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
