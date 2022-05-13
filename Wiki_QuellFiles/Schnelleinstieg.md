# TBA Schnelleinstieg

```yaml
Dokumentstatus: in Bearbeitung (THuste)
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

```yaml
Dokumentstatus: in Bearbeitung (THuste)
Stand: 13.05.22
todo: - weitere Inhalte
      
```
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
test
</td></tr>
<tr>
<td>

Eingabe der Adresse des Teststudios in einem Browser: **www.iqb-teststudio.de**
 
:heavy_exclamation_mark: Das Teststudio muss dazu auf Ihrem Server installiert sein.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Anmeldung

</td></tr>
<tr>
<td>

Melden Sie sich mit Ihren Zugangsdaten am Teststudio an.

:heavy_exclamation_mark: Die Zugangsdaten erhalten Sie von Ihren Adminstrator\*innen.

![TS_Anmeldung](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Anmeldung.gif)


</td></tr>
<tr>
<td>

### :heavy_check_mark: Arbeitsbereich wählen

</td></tr>
<tr>
<td>

Wählen Sie Ihren Arbeitsbereich aus.

:heavy_exclamation_mark: Die Administrator\*innen geben Bereiche für Sie frei.

![TS_AB_Auswahl](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_AB_Auswahl_01.png)


</td></tr>
<tr>
<td>

### :heavy_check_mark: Aufgabe anlegen

</td></tr>
<tr>
<td>

Legen Sie eine neue Aufgabe an oder bearbeiten Sie eine bestehende Aufgabe durch Markierung der Aufgabe.

:information_source: Eine Aufgabe wird auch Unit genannt!

![TS_Aufgabe_anlegen](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_Aufgabe_anlegen.gif)

:heavy_exclamation_mark: Vergeben Sie für den Kurznamen eindeutige ID-fähige Namen. Der hier aufgezeigte Name soll nur als Beispiel dienen und wäre eigentlich nicht günstig.

</td></tr>
<tr>
<td>

### :heavy_check_mark: Auswahl Editor und Player

</td></tr>
<tr>
<td>

Bevor Sie mit dem Aufgabentwurf starten, müssen Sie festlegen mit welchem Editor Sie die Aufgabe entwerfen möchten. Jeder vom IQB angebotene Editor verfügt über eigene Eigenschaften und Funktionen. Wählen Sie den Aspect-Editor, wenn Sie Ihre Aufgabe mittels vorgefertigter Elemente entwerfen wollen und Sie responsives Verhalten wünschen . Wählen Sie den Editor für Text, wenn Sie Ihre Aufgabe mittels einer Scriptsprache entwerfen möchten und auf responsives Verhalten verzichten können.

Ist der Editor ausgewählt muss auch ein zum Editor passender Player gewählt werden. Der Player gibt die Aufgabe mit Ihren Aufgabenelementen dann in der Vorschau, aber auch später bei der Testdurchführung im **Testcenter** wieder.


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


Legen Sie ihr erstes Aufgabenelement in Ihrer Aufgabe an. Ich wähle einmal ein Textelement.



:heavy_exclamation_mark: Speichern Sie die Aufgabe mal wieder!

</td></tr>
<tr>
<td>

### :heavy_check_mark: Ausgabe der Aufgabe

</td></tr>
<td>

Jetzt können Sie Ihre Aufgabe mit dem **Teststudio** ausgeben lassen.



Was hat das **Teststudio** erzeugt?

Es wird zu jeder Aufgabe jeweils eine Voud-Datei und eine Xml-Datei erzeugt. Außerdem werden noch 2 andere Dateien erzeugt, eine `Testtakers.xml` und eine `Booklet.xml`. Im Schnelleinstieg zum **Testcenter** werden wir uns diese beiden Dateien noch einmal näher anschauen. Alles wird in einer Zip-Datei verpackt ausgegeben.

:information_source: Hiermit ist der Aufgabenentwurf mit dem **Teststudio** abgeschlossen!

</td></tr>


</table>

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Schnelleinstieg">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
