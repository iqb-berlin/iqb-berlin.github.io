```yaml
Dokumentstatus: Review (THuste)
Stand: 20.07.2021
todo: - Weiter mit Inhalten füllen      
```

<table border=1>
  <tr>
    <td><a href="#Allgemein">Allgemein</a></td>    
	<td><a href="#Testcenter">Testcenter</a></td>
	<td><a href="#Teststudio">Teststudio</a></td>
	<td><a href="#itc">ITC-Toolbox</a></td>
  </tr>
</table>

---


<!--############################## Tabelle Allgemein ######################################-->
<table border=1>
<tr>
<th align=left>

### <a name="Allgemein"></a>A L L G E M E I N

</th>    
</tr>
<tr>
<td>

#### Wo finde ich Ansprechpartner zum Thema TBA?
> Sie finden die entsprechenden Ansprechpartner auf der Startseite des [IQB GitHub Wikis](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki). Hier finden Sie auch Kontaktdaten zu unserem Support Team. Weitere Informationen finden Sie auch auf der [IQB Webseite](https://www.iqb.hu-berlin.de/institut/staff/).

</td></tr>
<tr>
<td>

#### Welche Testsysteme bietet das IBQ zur Umsetzung einer digitalisierten Testung an?
> Das IQB bietet die beiden Webanwendungen **Teststudio** (Aufgabenentwurf) und **Testcenter** (Testdurchführung) an.

</td></tr>
<tr>
<td>

#### Gibt es einführende Videos zu den IQB Testsystemen?
> Ja. Ein Video ist [hier](https://box.hu-berlin.de/f/2530ebf557404b1bac8b/) zu finden.

</td>
</tr>

</table>

<!--############################## Tabelle Testcenter ######################################-->
<table border=1>
<tr>
<th align=left>

### <a name="Testcenter"></a>T E S T C E N T E R

</th>    
</tr>
<tr>
<td>

#### Wie kann ich auf das Testcenter zugreifen?
> Der Zugriff erfolgt mittels Adresseingabe in Ihrem Webbrowser. Beachten Sie bitte: Das **Testcenter** muss zuvor in Ihrer IT-Netzstruktur auf einem dafür geeignetem Server installiert werden. Die Serveradresse erhalten Sie dann von Ihrem IT-Dienstleister oder den internen Administrator\*innen.

</td></tr>
<tr>
<td>

#### Welchen Browser sollte ich verwenden?
> Es gibt da derzeitg keine Vorgaben seitens des IQB. Empfohlen werden die gängigen Browser, wie Google Chrome oder Firefox.

</td></tr>
<tr>
<td>

#### Wie wird das Testcenter installiert?
> Bachten Sie dazu bitte die Informationen auf GitHub zum [Frontend](https://github.com/iqb-berlin/testcenter-frontend) und zum [Backend](https://github.com/iqb-berlin/testcenter-backend). Eventuell benötigen Sie oder Ihr IT-Dienstleister dabei Unterstützung. Melden Sie sich dazu gerne bei unserem Support-Team.

</td></tr>
<tr>
<td>

#### Ist es möglich jeden PC vor einer Testdurchführung auf Eignung bzgl. der Performance zu prüfen?
> Das Testcenter bietet einen sogenannten **System-Check** an. Dieser kann auf jedem, während einer Testung zum Einsatz kommenden PC, ausgeführt werden. Er liefert die entsprechenden Eckdaten die eine Aussage über eine ausreichende Performance zulassen. Mehr dazu finden Sie auch im gleichnamigen [Kapitel](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.7-System-Check).

</td></tr>
<tr>
<td>

#### Wie melde ich mich am Testcenter an?
> Gebe Sie die Adresse Ihres **Testcenters** in den Webbrowser ein. Die Anmeldung erfolgt dann via Benutzernamen und Passwort. Beides erhalten Sie von den IT-Administrator\*innen bzw. Ihrem IT-Dienstleister.

</td></tr>
<tr>
<td>

#### Nach der Anmeldung sehe ich keine Inhalte im Testcenter. Was mache ich falsch?
> Eventuell sind keine Inhalte zu sehen, weil die IT keine Arbeitsbereiche für Sie freigegeben hat. Wenden Sie sich dazu bitte an die Administrator\*innen.

</td></tr>
<tr>
<td>

#### Wie lade ich Inhalte in meinen Arbeistbereich?
> Öffne Sie Ihren Bereich, wechseln Sie zum Tab: **Dateien** und klicken Sie auf die kleine **Wolke** im rechten Bereich des Fensters.

</td></tr>
<tr>
<td>

#### Meine Testdateien werden beim Laden in das Testcenter abgelehnt. Was kann ich tun?
> **Testdateien können aus verschiedenen Gründen abgelehnt werden:**
>
> Es erscheint ein rotes Ausrufezeichen und der Vermerk eines nicht gefundenen Bestandteils.
> * Beachten Sie: Alle Dateien stehen zueinander in Abhängigkeiten. Wenn Sie eine Datei laden in welcher auf eine andere Datei verwiesen wird, diese aber noch nicht im Testcenter ist, wird eine entsprechende Fehlermeldung erzeugt. Beachten Sie dazu auch das folgende [Kapitel](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Testinhalte-hochladen).<br>
>
> Es erscheint ein rotes Ausrufezeichen mit dem Vermerk: Error [xxx].
> * Es wurde ein Syntaxfehler (Validierung) in Ihrer Datei gefunden. Es ist nicht möglich wahllos Daten und Attribute in Ihrer Testdatei zu verwenden! Jede Testdatei muss sich nach bestimmten Vorgaben richten. Diese Vorgaben werden in der sogenannten **Schema-Definitionen** festgelegt. Mehr zu diesem Thema finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Arbeiten-mit-Xml%E2%80%90Dateien).
>

</td></tr>
<tr>
<td>

#### Testdatei werden in das Testcenter geladen, aber mit einem orangefarbenen Dreieck versehen. Was bedeutet das?
> **Es gibt mehrere Ursachen für eine solche Kennzeichnung einer Datei:**
>
> Es erscheint ein orangefarbenes Dreieck mit dem Vermerk: File has no link to XSD-Schema.
> * In Ihrer Testdatei ist kein Verweis auf die zugehörige Schema-Definition gesetzt.
>
> Es erscheint ein orangefarbenes Dreieck mit dem Vermerk: .....never used
> * Ihre Testdatei wird noch von keiner anderen Testdatei aufgerufen bzw. eingebunden.

</td></tr>
<tr>
<td>

#### Wie bearbeite ich meine Testdateien?
> Da es sich bei den Testdateien um Xml-Dateien handelt, empfiehlt sich ein Editor der eine Hervorhebung der Xml-Syntax ermöglicht. Generell ist eine Bearbeitung mit jedem Texteditor möglich. Editoren, die die Xml-Syntax kennen, haben aber den Vorteil einer Syntaxprüfung und einer besseren Übersichtlichkeit durch farbliche Kennzeichnung. Mehr Informatonen zur Bearbeitung finden Sie auch im gleichnamigen [Einzeldokument](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Arbeiten-mit-Xml%E2%80%90Dateien).

</td></tr>
<tr>
<td>

#### Muss ich die Testdateien zwingend direkt bearbeiten oder kann ich diese auch indirekt bearbeiten?
> Es ist möglich einzelne Testdateien auch indirekt und ohne Vorkenntnisse der Xml-Syntax zu bearbeiten. Derzeitig ist dies aber nur für die **Booklet.xml** möglich. Da die **Booklet.xml** den Aufbau eines Tests festlegt, kann diese abhängig von den Testanforderungen komplex und unübersichtlich werden. Daher ist insbesondere bei dieser Testdatei eine indirekte Bearbeitungsmöglichkeit hinsichtlich Übersichtlichkeit und Fehleranfälligkeit günstig. Zur indirekten Bearbeitung dieser Testdatei wird ein weiteres IQB-Tool mit dem Namen **Itc-Toolbox** benötigt. Die indirekte Bearbeitung erfolgt dann mittels Excel. **Itc-Toolbox** generiert aus der fertigen Excel-Datei dann eine **Booklet.xml**. Mehr zu diesem Thema entnehmen Sie bitte dem folgenden [Kapitel](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/itc%E2%80%90ToolBox:-Booklets).

</td></tr>
<tr>
<td>

#### Was muss ich beachten nachdem ich eine Testdatei bearbeitet habe?
> Nach Speicherung der Änderungen, muss die geänderte Datei erneut in das **Testcenter** geladen werden.

</td></tr>
<tr>
<td>

#### Wie starte ich meinen angelegten Test und gibt es eine Art Voransicht?
> Sie selbst können mithilfe der **Testtakers.xml** festlegen wie ein Test ablaufen soll und mit welchen Zugangsdaten sich die gewählte Testperson anmelden soll. Der Ablauf eines Tests wird mit dem gewählten Testmodus bestimmt. Sie können zwischen verschieden Modi wählen. Der gewählte Modus bestimmt dann, ob es sich um einen finalen Lauf handelt oder nur um einen Probelauf. Mehr Informationen zur Bearbeitung der **Testtakers.xml** erhalten Sie im gleichnamigen [Einzeldokument](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml).

</td></tr>
<tr>
<td>

#### Wie sollte die Einteilung der Testpersonen in der Testtakers.xml erfolgen? Gibt es da Vorgaben?
> Es ist Ihnen überlassen wie Sie die Personen anlegen. Gerne aber berät Sie das IQB hinsichtlich eigener Erfahrungen diesbezüglich. Es ist möglich Personen einzeln mit Namen und Passwort anzulegen. Sie können aber auch Gruppen anlegen und einzelne Personen dieser Gruppe zuordnen. Mehr zum Thema Anmeldung der Testperson finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren).

</td></tr>
<tr>
<td>

#### Kann ich betimmte Restriktionen/ Beschränkungen für einen Test festlegen?
> Ja dies ist möglich. Die Restriktionen können in der **Booklet.xml** festgelegt werden. Dort können Sie zeitliche Begrenzungen für die Testhefte und Codeabfragen zum Weiterblättern festlegen. Mehr dazu finden Sie auch im gleichnamigen [Einzeldokument](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Booklet%E2%80%90Xml).

</td></tr>
<tr>
<td>

#### Kann ich den Test überwachen oder steuern?
> Ja. Das **Testcenter** stellt die sogenannte **Testleitungskonsole** zur Verfügung. Diese wird mittels Festlegung eines entsprechenden **Testmodi** in der **Testtakers.xml** getartet. Mehr dazu erfahren Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.8-Testleitungskonsole).

</td></tr>
<tr>
<td>

#### Die Reihenfolge meiner Units ist nicht wie sie sein sollte. Was kann ich tun?
> Die Reihenfolge der zu verwendenen Units wird in der **Booklet.xml** festgelegt. Von oben nach unten betrachtet, wird mit der obersten Unit begonnen.

</td></tr>
<tr>
<td>

#### Kann ich einen Test nach Abschluss auswerten? Wo finde ich entsprechende Ergebnisse?
> Das **Testcenter** speichert in bestimmten **Testmodi** die Egebnisse eines Tests in dem Arbeitsbereich ab, in welchem sich auch die Testdateien für den Test befinden. Öffnen Sie den jeweiligen Arbeitsbereich und klicken Sie auf den Tab: **Ergebnisse/Antworten**. Dort können Sie die Ergebnisse herunterladen. Die Dateien werden dann in einem Csv-Format gespeichert.

</td></tr>
</table>


<!--############################## Tabelle Teststudio ######################################-->
<table border=1>
<tr>
<th align=left>

### <a name="Teststudio"></a>T E S T S T U D I O

</th>    
</tr>
<tr>
<td>Hier muss noch was hin.

</td></tr>
</table>


<!--############################## Tabelle Itc-Toolbox ######################################-->
<table border=1>
<tr>
<th align=left>

### <a name="itc"></a>I T C - T o o l b o x

</th>    
</tr>
<tr>
<td>Hier muss noch was hin.                                                                                                                         

</td></tr>
</table>