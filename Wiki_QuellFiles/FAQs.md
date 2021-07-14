<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
# FAQs (Abschnittsmarker)
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->

<table>
  <tr>
    <td><a href="#Allgemein">Attribute und Daten</a></td>    
	<td><a href="#Testcenter">Testcenter</a></td>
	<td><a href="#Teststudio">Teststudio</a></td>
	<td><a href="#itc">ITC-Toolbox</a></td>
  </tr>
</table>

---

### <a name="Allgemein"></a>ALLGEMEIN

**Wo finde ich Ansprechpartner zum Thema TBA?**
> Sie finden die entsprechenden Ansprechpartner auf der Startseite des [IQB GitHub Wikis](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki). Hier finden Sie auch Kontaktdaten zu unserem Support Team. Weitere Informationen finden Sie auch auf der [IQB Webseite](https://www.iqb.hu-berlin.de/institut/staff/). 

**Welche Testsysteme bietet das IBQ zur Umsetzung einer digitalisierten Testung an?**
> Das IQB bietet die beiden Webanwendungen **Teststudio** (Aufgabenentwurf) und **Testcenter** (Testdurchführung) an.

---

### <a name="Testcenter"></a>TESTCENTER

**Wie kann ich auf das Testcenter zugreifen?**
> Der Zugriff erfolgt mittels Adresseingabe in Ihrem Webbrowser. Beachten Sie bitte: Das **Testcenter** muss zuvor in Ihrer IT-Netzstruktur auf einem dafür geeignetem Server installiert werden. Die Serveradresse erhalten Sie dann von Ihrem IT-Dienstleister oder den internen Administrator\*innen.

**Wie wird das Testcenter installiert?**
> Bachten Sie dazu bitte die Informationen auf GitHub zum [Frontend](https://github.com/iqb-berlin/testcenter-frontend) und zum [Backend](https://github.com/iqb-berlin/testcenter-backend). Eventuell benötigen Sie oder Ihr IT-Dienstleister dabei Unterstützung. Melden Sie sich dazu gerne bei unserem Support-Team.

**Wie melde ich mich am Testcenter an?**
> Gebe Sie die Adresse Ihres **Testcenters** in den Webbrowser ein. Die Anmeldung erfolgt dann via Benutzernamen und Passwort. Beides erhalten Sie von den IT-Administrator\*innen bzw. Ihrem IT-Dienstleister.

**Nach der Anmeldung sehe ich keine Inhalte im Testcenter. Was mache ich falsch?**
> Eventuell sind keine Inhalte zu sehen wenn für Sie seitens der IT-Administration keine Arbeitsbereiche freigegeben wurden. Wenden Sie sich dazu bitte an die Administrator\*innen.

**Wie lade ich Inhalte in meinen Arbeistbereich?**
> Öffne Sie Ihren Bereich, wechseln Sie zum Tab: **Dateien** und klicken Sie auf die kleine "Wolke" im rechten Bereich des Fensters.

**Meine Testdateien werden beim Laden in das Testcenter abgelehnt. Was kann ich tun?**
> **Testdateien können aus verschiedenen Gründen abgelehnt werden:**
>
> Es erscheint ein rotes Ausrufezeichen und der Vermerk eines nicht gefundenen Bestandteils.
> * Beachten Sie: Alle Dateien stehen zueinander in Abhängigkeiten. Wenn Sie eine Datei laden in welcher auf eine andere Datei verwiesen wird, diese aber noch nicht im Testcenter ist, wird eine entsprechende Fehlermeldung erzeugt. Beachten Sie dazu auch das folgende [Kapitel](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Testinhalte-hochladen).<br>
>
> Es erscheint ein rotes Ausrufezeichen mit dem Vermerk: Error [xxx].
> * Es wurde ein Syntaxfehler (Validierung) in Ihrer Datei gefunden. Es ist nicht möglich wahllos Daten und Attribute in Ihrer Testdatei zu verwenden! Jede Testdatei muss sich nach bestimmten Vorgaben richten. Diese Vorgaben werden in der sogenannten **Schema-Definitionen** festgelegt. Mehr zu diesem Thema finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Arbeiten-mit-Xml%E2%80%90Dateien).
>

**Testdatei werden in das Testcenter geladen, aber mit einem orangefarbenen Ausrufezeichen versehen. Was bedeutet das?**
> **Es gibt mehrere Ursachen für eine solche Kennzeichnung einer Datei:**
>
> Es erscheint ein orangefarbenes Ausrufezeichen mit dem Vermerk: File has no link to XSD-Schema.
> * In Ihrer Testdatei ist kein Verweis auf die zugehörige Schema-Definition gesetzt.
>
> Es erscheint ein orangefarbenes Ausrufezeichen mit dem Vermerk: .....never used
> * Ihre Testdatei wird noch von keiner anderen Testdatei aufgerufen bzw. eingebunden.

---

### <a name="Teststudio"></a>TESTSTUDIO








---

### <a name="itc"></a>ITC-Toolbox


