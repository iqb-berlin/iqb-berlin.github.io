# 2 Testcenter

Das IQB-Testcenter ist eine Web-Anwendung für die Durchführung von Kompetenztests oder Befragungen. 
Nach der Installation auf einem Webserver wählt man diesen Server über seine Adresse an, d. h. man schreibt 
dessen Internet-Adresse in die Adresszeile eines Internet-Browsers. Dadurch werden die Programmierungen geladen 
und man sieht ein Formular zum Anmelden. Alle Daten für einen Test sind vorher auf dem Server zu speichern. 
Das kann über ein integriertes Verwaltungsportal erfolgen oder über andere Webanwendungen, die auf den Server zugreifen.

Eine grobe Einführung in das Testcenter geben auch die nachfolgenden Verlinkungen.                        
Das IQB bietet folgende Video-Präsentationen bzgl. des Testcenters an:

* [Einführung in das IQB-Testcenter](https://box.hu-berlin.de/f/a8f7aea9c751493c8d35/)
* [Diskussion der Optionen Testcenter-Einsatz oder Implementation der Verona-Schnittstelle](https://box.hu-berlin.de/f/d23af87168fa4e9f9bb0/)

Des Weiteren besteht das folgende Forum: [Testcenter-Forum](https://github.com/iqb-berlin/testcenter-frontend/discussions)<br> 
Hier finden Sie häufig gestellte Fragen und Antworten sowie Berichte über Einsätze des IQB-Testcenters.

**Installation**

Das IQB hat alle Programmierungen unter einer Open Source veröffentlicht und erleichtert die Installation durch ein sog. 
Docker-Setup. Für die Installation muss man einen Server bereitstellen (Linux oder Windows), und dieser Server muss dann über 
eine Internet-Adresse erreichbar sein. Die Installation sollte erfahrenes IT-Fachpersonal durchführen. 
Die Dokumentation hierzu setzt Wissen vor allem zur Virtualisierungssoftware Docker voraus. 
Es ist weiterhin Wissen zu Datensicherheit nötig, denn sobald ein Server öffentlich verfügbar ist, müssen Maßnahmen 
gegen Angriffe durch Schadsoftware ergriffen werden. Das IQB ist bemüht, die Installationspakete gut abzusichern, 
übernimmt aber im Schadensfall keine Verantwortung.

**Verwaltung der Tests**

Nach der Installation ist zunächst ein Standard-Konto für die Verwaltung von Tests angelegt. 
Außerdem ist ein Arbeitsbereich angelegt mit einem Beispieltest. Als erste Schritte sind über ein Verwaltungsportal die Testinhalte 
(Aufgaben, Testabläufe usw., z. B. als XML-Dateien) in das Testcenter zu laden. Nach der Durchführung des Tests kann man über 
dieses Verwaltungsportal die Ergebnisse herunterladen (Csv-Dateien). Die Texte dieses Wikis sind vor allem für Personen gedacht, 
die diese Verwaltungsaufgaben ausführen.

Man kann eine Installation des IQB-Testcenters weitgehend anpassen. Begrüßungsnachrichten, Logo auf der Startseite und selbst der Name 
kann an eigene Wünsche angepasst werden.

**Durchführung von Tests oder Befragungen**

Durch Anwählen der Internet-Adresse des Testcenter-Servers erhält man ein Anmeldeformular. 
Eine Testperson muss über Zugangsdaten verfügen, und es startet dann das für diese Person vorbereitete Testheft 
(d. h. die Abfolge von Aufgaben bzw. Fragen). Folgende besonderen Funktionen sind im IQB-Testcenter derzeit umgesetzt:

* Verschiedene Varianten der Anmeldung: Anmeldung über einen Link, zweistufige Anmeldung zur Vereinfachung der Durchführung, 
spezieller Modus für das Ausprobieren eines Tests (Review) usw.
* Mehrere Testhefte: Eine Testperson kann auch mehrere Testhefte nacheinander bearbeiten mit denselben Anmeldedaten
* zeitliche Beschränkung von Testteilen: Für eine bestimmte Anzahl Aufgaben steht der Testperson eine begrenzte Zeit zur Verfügung
* Fortsetzung erst mit Freigabewort: Die Testdurchführung z. B. in einer Klasse kann synchronisiert werden, indem die Testleitung 
ein Wort ansagt, mit dem dann der Test fortgesetzt werden kann
* Fortsetzung erst nach vollständiger Anzeige: Um zu vermeiden, dass Teile einer Aufgabe übersehen werden, 
kann das Weiterblättern solange unterbunden werden, bis alle Audio-Sequenzen abgespielt wurden und alle Seiten vollständig angezeigt wurden
* Fortsetzung erst nach vollständiger Beantwortung
* sofortige Speicherung: Alle Antworten werden sofort zum Testcenter-Server gesendet; 
nach Abbruch oder Absturz eines Computers oder des Browsers kann daher der vorherige Stand wiederhergestellt werden

Es können mehrere Tests oder Befragungen gleichzeitig laufen.

**System-Check**

Da die Programmierungen des Testcenters online in einem Browser ablaufen, ist keine vorherige Installation von Software auf einem Computer nötig, 
mit dem der Test oder die Befragung durchgeführt werden soll. Es ist nur ein Internet-Zugriff und ein Browser nötig. Allerdings kann man bei der 
enormen Vielfalt der Hardware (Tablet, Smartphone usw.) und Software (Apple, Linux, Android usw.) nicht garantieren, dass ein Test oder eine 
Befragung so wie beabsichtigt funktioniert. Je nach Anforderung an den Test wird das auch nicht sinnvoll sein, z. B. wenn eine Mindestbreite 
für den Bildschirm erforderlich ist.

Das IQB bemüht sich, hier eine möglichst breite Palette an Systemen abzudecken. 
Wenn man jedoch erfahren möchte, ob die Zielsysteme geeignet sind, kann man im IQB-Testcenter einen System-Check konfigurieren. 
Dann können z. B. die verantwortlichen Lehrkräfte in der Vorbereitungsphase im Testcenter einen auf die speziellen Anforderungen des 
Tests abgestimmten Check durchführen. Auch die Internetverbindung kann hierüber bewertet werden.

**Testleitungskonsole**

Soll ein Test für eine bestimmte Personengruppe (z. B. Klasse) gleichzeitig stattfinden, kann ein Monitor dafür eingerichtet werden. 
Die Testleitung kann dann für jede Testperson den Fortschritt beobachten, ggf. das Weiterblättern erzwingen, Personen ausschließen oder eine 
Sperre wieder aufheben.

<!--++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.1-Daten-und-Prozesse">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++home+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.1 Daten und Prozesse

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Umgebungsmodule_final.png)

## Daten-Input für das Testcenter

### Logins

Jede Person, die an einem Test bzw. einer Befragung beteiligt ist, muss Zugangsdaten erhalten. Diese Informationen sind in einer [XML-Datei](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml) festgelegt. Folgende Arten des Zugriffs (Rollen) werden unterschieden:
* Testpersonen: Die Personen, die den Test bzw. die Befragung absolvieren. Deren Antworten bilden mit dem Rohdatensatz die Grundlage der Auswertung.
* Testleitung: Ein spezieller Login sorgt dafür, dass die angemeldete Person den Monitor für eine Testgruppe startet. Damit kann der Fortschritt der Beantwortung beobachtet werden. Außerdem können Testpersonen ausgeschlossen, ein Test angehalten oder eine Navigation zu einem Testblock erzwungen werden.
* Review: Zum Ausprobieren eines Tests können spezielle Logins vorbereitet werden. Man kann dann Kommentare zu den Aufgaben und dem Test vergeben und es sind einige Navigationsbeschränkungen unwirksam, wie z. B. Zeitlimits.
* Demo: Man kann den Test aufrufen, aber die Antworten werden nicht dauerhaft gespeichert. Ruft eine andere Person mit denselben Login-Daten den Test auf, werden keine älteren Antworten geladen.

Das Erstellen von Logins wird unterstützt über das Windows-Programm [itc-ToolBox](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/itc%E2%80%90ToolBox:-Logins).

### Test-Definition

Diese [Xml-Datei](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Booklet%E2%80%90Xml) legt die Reihenfolge der Aufgaben (Units) fest. Man kann die Aufgaben bzw. Zwischenseiten auch in Blöcke (Testlets) gruppieren. Dann kann man festlegen, dass ein Block nur nach Eingabe eines Code-Wortes betreten werden kann oder dass es ein Zeitlimit für die Bearntwortung gibt. Außerdem kann über die Test-Definition festgelegt werden, dass eine navigation zur nächsten Aufgabe/Seite erst erlaubt ist, wenn alle Teile der Aufgabe angezeigt/präsentiert wurden (auch z. B. eine Audio-Sequenz) oder wenn alle erforderlichen Antworten gegeben wurden.

> **In der Grafik ist dargestellt, dass die Definition von Tests über das IQB-Teststudio erfolge. Das wird in zukünftigen Versionen der Fall sein. Die aktuelle Version IQB-Teststudio-Lite unterstützt dies nicht, sondern man muss die Xml-Datei für die Test-Definition manuell erzeugen.**

### Unit-Definition

Eine Unit-Definition besteht aus einer [Xml-Datei](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Unit%E2%80%90Xml) und einer Voud-Datei. Erstere enthält Metadaten wie die interne ID und den Datentyp der Unit, letztere ist ein internes Format, das manuell kaum editierbar ist. Es muss statt dessen über einen Editor erzeugt werden. Das IQB-Teststudio bietet derartige Editoren.

### Player

In der Grafik ist dargestellt, dass das Testcenter intern eine Komponente "Player" enthält. Grundidee dieser Teilung ist, dass das interne Format einer Unit-Definition nicht direkt vom Testcenter selbst verarbeitet wird, sondern von einem Plug-In, das je nach Unit-Datentyp hinzugeladen wird. Durch diese Technik wird eine hohe Flexibilität erreicht: Änderungen der unitbezogenen Programmierung führen nicht zu einem neuen Testcenter, sondern nur der Plug-In-Code des Players wird ausgetauscht. Näheres hierzu im Abschnitt [2.5 Player (Verona)](2.5-Player-(Verona)).

Für die Vorbereitung eines Tests bedeutet dies, dass
1. jede Unit-Definition einen Verweis auf das Datenformat und damit auf den erforderlichen Player enthalten muss und
2. alle Player, die von Units benötigt werden, müssen vorab als Ressourcendatei in das Testcenter geladen werden

## Daten-Output des Testcenters

### Logs

Ereignisse sowohl innerhalb einer Unit als auch insgesamt eines Tests werden in ein Protokoll geschrieben. Dieses sog. "Logging" kann reduziert und auch ganz abgestellt werden, um die Datenmenge zu reduzieren. Welche Ereignisse genau gespeichert werden, ist auch vom Player abhängig. Folgende Erkenntnisse lassen sich beispielsweise aus den Log-Daten ablesen:
* Version des Betriebssystems und des Browsers
* Verweildauer auf einer Seite
* Zeitpunkt des Beendens der Beantwortung

### Antworten

Als Antworten werden Zustandsänderungen der Eingabe-Elemente der Units verstanden. Wenn die Testperson ein Ankreuzkästchen wählt, eine Linie mit der Maus verschiebt oder mehrere Sätze in ein Eingabefeld schreibt - all diese Eingaben werden mit dem jeweils letzten Stand gespeichert.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.2-Die-Sicht-der-Testperson">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2-Testcenter">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.2 Die Sicht der Testperson

## Computer starten

Zunächst muss man sich am Computer, an dem der Test durchgeführt werden soll, anmelden. Sollte man die Account-Daten nicht parat haben, braucht's erstmal etwas Zeit, dass neue beschafft werden (ist die ITG-Lehrerin da?). Der Computer ist dann hochgefahren und ein einigermaßen moderner Browser ist installiert. Hoffentlich fängt der jetzt nicht an, Updates zu laden und zu installieren, dann sollte man lieber einen anderen nehmen.

## Am Testsystem anmelden

Nun kommt es auf die richtige Internet-Adresse an. Die soll bitte nicht in das Suchfeld von Google oder einer anderen Suchmaschine eingegeben werden, denn dann gibt es eine Trefferliste mit ungewissem Ausgang. Also besser oben in die Adressleiste eintragen, genau wie auf dem Zettel steht.

Das Startbild ist sehr reduziert. Rechts ein paar allgemeine Informationen, so wie Datenschutz und so etwas, aber links nur Eingabefelder für Name und Kennwort. Nach der Eingabe wird ein großer Schalter präsentiert, der das Testheft symbolisiert, das gestartet werden soll. Daran erkennt man, dass die Anmeldung erfolgreich war.

> Weitere Informationen zur Anmeldung dazu finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren)

Mögliche Probleme:
* Wenn das Startbild zu sehen ist, dann ist schonmal klar, dass die Internet-Verbindung funktioniert. Ansonsten sollte man mal die Kabel prüfen.
* Wenn das Startbild einigermaßen gut aussieht (nichts verrutscht, nichts überlagert), dann ist auch der Browser nicht zu alt. 
* Wenn gleich zu Anfang vor der Anmeldung ein roter Balken oben zu sehen ist, dann stimmt etwas nicht mit der Programmierung. Das sollten dann alle in der Klasse auch haben. Die Hotline muss unbedingt kontaktiert werden.
* Wenn für die Anmeldedaten kein Testheft gefunden wurde, dann gibt es eine rote Ausschrift, die genau das meldet. Dann sollte man nochmal prüfen, ob die Eingabe richtig war.
* Wenn der Schalter für das Testheft ausgegraut ist, dann ist dieser Test gesperrt oder noch nicht freigegeben. Für Tests könnte ein Zeitfenster definiert sein. Dann nochmal die Anweisungen studieren und ggf. bei der Hotline nachfragen.

## Durchführen des Testheftes bzw. der Befragung

Mit Klick auf den Schalter des Testheftes werden alle Testinhalte geladen. Sobald möglich, wird auch die erste Seite schon gezeigt und das Laden wird im Hintergrund fortgesetzt. Jeder Computer im Raum lädt immer nur die Daten für eine Aufgabe. Obwohl theoretisch ein Browser mehrere Aufgaben gleichzeitig laden könnte, wird das unterbunden, damit sich einzelne Computer nicht vordrängeln und die anderen ausbremsen. Ein Computer, der später mit dem Herunterladen startet, wäre sonst erstmal blockiert bis die anderen fertig sind.

Während des Tests werden keine weiteren Inhalte vom Server geladen, sondern nur die Antworten gespeichert.

Die Navigation erfolgt rechts oben für die Aufgaben, und sollte eine Aufgabe aus mehreren Seiten bestehen, dann kann man rechts unten mit entsprechenden Schaltern blättern.

Sollte es mal technische Probleme mit dem Computer geben (z. B. Audio-Buchse defekt), dann kann man jederzeit den Browser schließen und den Test auf einem anderen Computer neu starten. Die schon gegebenen Antworten werden geladen.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Portal-zur-Verwaltung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.1-Daten-und-Prozesse">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.3 Portal zur Verwaltung

Auf einem Testcenter müssen die Inhalte für Tests geladen werden und es muss einen Weg geben, die Antworten zu erhalten. Für diese Aufgaben ist ein Verwaltungsportal eingerichtet. Die Verantwortlichen für eine Studie melden sich am Testsystem an derselben Stelle an, wo auch eine Testperson sich anmelden würde. Das System erkennt, dass die Anmeldedaten zu einem Konto für die Verwaltung gehören und lädt entsprechend die Funktionen dafür.

## Arbeitsbereich

Damit mehrere Studien gleichzeitig auf einem Testsystem durchgeführt bzw. vorbereitet werden können, sind sog. Arbeitsbereiche vorbereitet. Die Benennung richtet sich günstigerweise nach dem Zweck, also z. B. "Demo Deutsch Sek1" oder "Review Abi" oder "VERA Englisch". Für jedes Verwaltungskonto ist festgelegt, welche Arbeitsbereiche eingesehen (Nur-Lese-Modus) bzw. geändert werden können (Lesen-Und-Schreiben-Modus).

Nach der Anmeldung präsentiert das System eine Liste aller Arbeitsbereiche, auf die die Person mit den Anmeldedaten Zugriff hat. Mit Klick auf einen Schalter wird der Arbeitsbereich geöffnet. Zur Liste der Arbeitsbereiche kehrt man zurück, indem man auf das IQB-Logo links oben in der Ecke klickt.

Der Arbeitsbereich hat drei Grundfunktionen, die man mit Klick oben auf den entsprechenden Tab auswählt: Dateien, System-Check Berichte und Ergebnisse/Antworten.

### Tab Dateien

Alle Testinhalte und Definitionen eines Tests bzw. einer Befragung werden über Dateien in das System hochgeladen. Sie müssen also ersteinmal auf dem eigenen Computer vorbereitet werden, z. B. über einen Download aus einer anderen Webanwendung (Units). Meist handelt es sich um XML-Dateien, die einer fest vorgeschriebenen Syntax folgen und aus denen das Testsystem alle notwendigen Informationen liest. Die Bedeutung der Dateien entnehmen Sie bitte den anderen Kapiteln dieses Wikis.

Sobald eine Datei hochgeladen ist, ist sie wirksam. D. h. unmittelbar nachdem eine Datei mit Login-Daten hochgeladen wurde, kann sich eine Testperson mit diesen Daten anmelden. Sollte man feststellen, dass eine Unit Fehler enthält, kann man die Unit-Datei neu hochladen. Durch das Überschreiben wird sofort jeder danach gestartete Test die neue Unit verwenden.

Beim Hochladen werden die XML-Dateien geprüft. Eine Datei kann abgewiesen werden, wenn sie syntaktisch oder inhaltlich fehlerhaft ist. Z. B. wird eine Testtaker-Datei abgewiesen, wenn sie Anmeldedaten enthält, die bereits in einem anderen Arbeitsbereich verwendet wurden. Es wird auch eine Booklet-Datei abgewiesen, wenn sie auf Units verweist, die nicht im Arbeitsbereich gefunden wurden. Daher spielt die Reihenfolge des Hochladens eine Rolle.

### Tab System-Check Berichte

Hier können die Berichte, die über einen System-Check dieses Arbeitsbereiches abgeschickt wurden, heruntergeladen werden.

### Tab Ergebnisse/Antworten

Hier können Antworten und Logs, die über die Tests bzw. Befragungen dieses Arbeitsbereiches abgeschickt wurden, heruntergeladen werden.

## System-Admin

Wenn das eigene Verwaltungskonto die Markierung "System-Administration" hat, dann wird am Ende der Liste der Arbeitsbereiche ein Schalter eingeblendet, mit dem man in die Systemverwaltung kommt. Hierüber werden die Nutzerkonten angelegt (Benutzername und Kennwort), die Arbeitsbereiche angelegt sowie die Rechte vergeben, wer auf welchen Arbeitsbereich zugreifen kann.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Testinhalte-hochladen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.2-Die-Sicht-der-Testperson">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.4 Testinhalte hochladen

Wie in der [Einführung](2.1-Daten-und-Prozesse) erläutert, besteht die Definition eines Tests oder einer Befragung aus dem Hochladen spezieller Dateien. Die Verwaltung der Dateien erfolgt im [Verwaltungsportal](2.3-Portal-zur-Verwaltung). Die folgende Darstellung zeigt die Zusammenhänge der Dateien untereinander: Units definieren jeweils eine Aufgabe bzw. eine Seite, Booklets definieren die Aneinanderreihung der Aufgaben und Logins definieren den Zugriff einer Testperson auf ein Booklet.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Upload_Ablauf_final.png)

Folgende Texte geben Erläuterungen für diese zentralen Funktionen:
* [Allgemeine Hinweise für die Bearbeitung von XML-Dateien](Arbeiten-mit-Xml%E2%80%90Dateien)
* Units: 
  * [Bearbeiten der XML-Datei](Unit%E2%80%90Xml)
* Booklets:
  * [Bearbeiten der XML-Datei](Booklet%E2%80%90Xml)
  * [Unterstützung durch itc-ToolBox](itc%E2%80%90ToolBox%3A-Booklets)
* Logins:
  * [Bearbeiten der XML-Datei](Testtaker%E2%80%90Xml)
  * [Unterstützung durch itc-ToolBox](itc%E2%80%90ToolBox%3A-Logins)
  * [Anmeldeverfahren](Login%3A-Anmeldeverfahren)
  * [Modi der Testdurchführung](Login%3A-Modi-der-Testdurchf%C3%BChrung)

**Empfehlung: Verweis zur Validierung**

Eventuell wird nach dem Hochladen in das Testcenter eine Warnung "File has no link to XSD-Schema..." angezeigt. Diese Warnung bedeutet, dass die Xml-Datei keinen expliziten Verweis auf eine Xsd-Datei enthält. Eine solche Xsd-Datei definiert die möglichen Elemente und Attribute einer Xml-Datei und kann daher zur Prüfung der Xml-Datei auf Korrektheit verwendet werden. Das IQB stellt solche Xsd-Dateien bereit. 

Die Deklaration der Xsd-Datei erfolgt im Haupt-Element einer Xml-Datei. Für die Unit-Xml heißt das Hauptelement `Unit` und muss folgendermaßen geändert werden:
```
<Unit 
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Unit.xsd">
```
Ein nützlicher Nebeneffekt hierbei ist, dass auch Editoren zur Bearbeitung von Xml-Dateien (z. B. Notepad++, Sublime) nun eine Validierung vornehmen können. Man kann also vor dem Hochladen eine Validierung bereits beim Schreiben einer Xml-Datei vornehmen lassen.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Ergebnisse-herunterladen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.3-Portal-zur-Verwaltung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.5 Ergebnisse herunterladen


```yaml
Dokumentstatus: Review (THuste)
Stand: 29.06.2021
todo: - Weiter mit Inhalt füllen      
```

Es können Antwort- und Logdateien heruntergeladen werden. Es handelt sich um CSV-Dateien. Für die Aufbereitung der Daten steht eine Windows-Software zur Verfügung: [itc-ToolBox](itc%E2%80%90ToolBox%3A-Antworten-und-Logs).


---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.6-Player-Testwiedergabe-(Verona)">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.4-Testinhalte-hochladen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.6 Player Testwiedergabe (Verona)

```yaml

Dokumentstatus: Entwurf
Stand: 6.4.2021
todo:

```

Das Testcenter ist modular aufgebaut. Es besteht zum einen aus der eigentlichen Webanwendung und einem Player, welcher in die Webanwendung integriert ist. Der Player übernimmt die Wiedergabe der Aufgaben und visualisiert diese. Stellen Sie sich das Testcenter als einen CD-Player vor. Das Gehäuse mit allen Funktionstasten (Pause, Play etc.) ist die eigentliche Webanwendung Testcenter. Hierüber kann die Wiedergabe einer CD gesteuert werden. Das Gehäuse ermöglicht den Einbau eines CD-Laufwerkes, welches die CDs wiedergeben kann. Die eingelegte CD entspricht dann einer in das Testcenter hochgeladenen Unit. Die CD kann über die Tasten am Gehäuse, also die Webanwendung gestartet werden. Die Wiedergabe kann nur erfolgen, wenn Laufwerk und CD zueinander passen. Nachfolgend sind die Bereiche der Webanwendung und der Bereich des Players zu sehen:

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Bereich_Player_final.png)

**Rot markiert:**<br>
Bereich der Webanwendung zur Steuerung des Tests mittels Funktionsschaltknöpfen und Informationen zum Test.

**Blau markiert:**<br>
Bereich des Players zur Wiedergabe der Aufgabe.

Der Vorteil dieser Aufteilung besteht hauptsächlich darin:<br>
Werden Aufgaben erstellt und dabei neue Elemente verwendet, die dem Testcenter noch unbekannt sind, muss nicht der Programmcode des gesamten Testcenter angepasst werden, sondern nur der Programmcode des verwendeten Players. Bei der Aufgabenerstellung im **Teststudio** kommen unterschiedliche Editoren zum Einsatz. Diese Editoren bieten unterschiedliche Funktionen und Aufgabenelemente. Zu jedem Editor gehört ein entsprechender Player, welcher die Funktionen und Elemente des verwendeten Editors kennt und diese daher später auch wiedergeben kann. 

> **Weitere Informationen zu den angebotenen Playern finden Sie auch in den gleichnamigen Einzeldokumenten unter "Direkt zu anderen Seiten".**

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.7-System-Check">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.5-Ergebnisse-herunterladen">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.7 System Check

## Was ist ein System-Check?

Es ist bitter, wenn man erst während der Studiendurchführung bemerkt, dass die Hardware oder die Software-Ausstattung für einen 
Online-Test nicht geeignet ist. Der System-Check ist ein Weg, vorab diese Eignung zu prüfen. Man kann natürlich nicht alle Probleme erkennen 
und vielleicht hat man für bestimmte Probleme auch keine Lösung parat, aber man kann die Ausfall- und damit die Frustrate deutlich senken.

## Planung

Nach dem Einrichten eines Systemchecks erscheint auf der Seite der Webanwendung (hier: IQB-Testcenter) ein neuer Schalter `System-Check`. 
Man kann alle Interessierten einladen, darüber zumindest eine Prüfung der Internetanbindung vorzunehmen (Bandbreite) und eine Anzahl von 
Hardware- und Softwareinformationen anzuzeigen. Außerdem stehen folgende Optionen zur Verfügung:

* Probeweises Aufrufen einer Testaufgabe: Eine speziell dafür entwickelte Testaufgabe wird gezeigt und man kann die Bearbeitungselemente auswählen,
  ändern und so prüfen, ob die Aufgabenelemente wie erwartet funktionieren.
* Fragebogen beantworten: Die Person, die den System-Check durchführt, kann eine Liste von Fragen beantworten. 
  Die Fragen können sich zunächst auf die vorherige Testaufgabe beziehen (wurde die Audio-Datei abgespielt? 
  Passte alles auf den Bildschirm? usw.), aber auch weitere Informationen zur Ausstattung vor Ort können erfragt werden 
  (wieviele Plätze sind im PC-Lab?, Können die Testpersonen sich gegenseitig auf den Bildschirm schauen?, Gibt es ein Whiteboard? usw.)
* Bericht abschicken: Es kann festgelegt sein, dass die Daten gespeichert werden zur späteren Auswertung. 
  Dazu sollte ein Kennwort vergeben werden und eine weitere Kennung, anhand der die Zuordnung der Daten z. B. 
  zu einer bestimmten Schule möglich ist.

### XML-Definition schreiben

Ein System-Check wird über eine XML-Datei gesteuert. Außerdem kann eine Unit-Definition hinzugelegt werden (XML-Datei, 
VOUD-Datei und zugehöriger Player). All diese Dateien sind über einen beliebigen Arbeitsbereich in das Testcenter zu laden. 
Die Berichte des System-Checks werden dann auch in diesem Arbeitsbereich gespeichert.

Der genaue Aufbau und die möglichen Parameter der System-Check-XML sind in einer Schema Definition festgelegt.
Anhand einer Beispieldatei sollen nachfolgend die Optionen beschrieben werden:

```xml
<?xml version="1.0" encoding="utf-8"?>
<SysCheck xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_SysCheck.xsd">
	<Metadata>
		<Id>LAL8_2021</Id>
		<Label>System-Check für LAL8 2021</Label>
		<Description>Version 4.2.2021</Description>
	</Metadata>
	<Config unit="SC3" savekey="fichtelgebirge">
		<UploadSpeed min="1024" good="2048" maxDevianceBytesPerSecond="10000" maxErrorsPerSequence="0" maxSequenceRepetitions="15">100000, 200000, 400000, 800000</UploadSpeed>
		<DownloadSpeed min="1024" good="2048" maxDevianceBytesPerSecond="200000" maxErrorsPerSequence="0" maxSequenceRepetitions="15">400000, 800000, 1600000, 3200000</DownloadSpeed>		
		<Q id="1" type="header" prompt="Abschnitt I: Computerübergreifende Fragen – diese müssen nur einmal online eingegeben werden."></Q>
		<Q id="2" type="radio" prompt="1. Wer ist an der Schule die Ansprechperson für technische Fragen?">der Schulkoordinator/die Schulkoordinatorin selbst#eine andere Person (Eingabe nächstes Feld)#es gibt keine Ansprechperson</Q>
		<Q id="2a" type="text" prompt="Weitere Informationen zur Ansprechperson"/>
		<Q id="3" type="string" prompt="2. In welchem Raum wurde die Systemdiagnose durchgeführt? Bitte geben Sie die Raumbezeichnung an."/>
		<Q id="4" type="text" prompt="3. Bitte notieren Sie ggf. Informationen zur Erreichbarkeit des Raumes."/>
		<Q id="5" type="string" prompt="4. Wie viele Computer gibt es im Raum?"/>
		<Q id="6" type="string" prompt="5. Wie viele funktionstüchtige Computer gibt es im Raum?"/>
		<Q id="7" type="text" prompt="6. Wie würden Sie den allgemeinen Zustand der Computer (und Bildschirme, Mäuse, Tastaturen) beschreiben? 
	z. B. modern, veraltet, gut instandgehalten etc."/>

		<Q id="8" type="header" prompt="Abschnitt II: Fragen zum Account für die Systemdiagnose"></Q>
		<Q id="9" type="radio" prompt="1. Ist dies ein allgemeiner Account?">der Account kann für alle PC verwendet werden#der Account ist nur für bestimmte PC zur Anmeldung möglich#konnte Reichweite des Accounts nicht ermitteln</Q>
		<Q id="10" type="radio" prompt="2. Ist dies ein Account mit Zugriff auf USB?">ein mobiler Browser konnte direkt von USB gestartet werden#ein mobiler Browser konnte auf den Desktop kopiert und ausgeführt werden#ein mobiler Browser konnte nicht gestartet werden</Q>
		<Q id="11" type="text" prompt="3. Gibt es Änderungen dieser Situation im Testzeitraum bis Mai? Bitte beschreiben!"/>

		<Q id="12" type="header" prompt="Abschnitt III: Fragen zum Funktionieren der Aufgabe"></Q>
		<Q id="13" type="text" prompt="1. Besonderheiten beim Starten des Browsers und beim Zugriff auf das Testcenter"/>
		<Q id="14" type="text" prompt="2. Allgemeine Auffälligkeiten bei der Darstellung der Aufgabe"/>
		<Q id="15" type="text" prompt="3. Probleme beim Abspielen der Audio-Sequenz"/>
		<Q id="16" type="text" prompt="4. Klarheit der Darstellung der Grafik"/>
		<Q id="17" type="text" prompt="5. Auffälligkeiten beim Scrollen"/>
		<Q id="18" type="text" prompt="6. Auffälligkeiten beim Navigieren zwischen Seiten"/>
		<Q id="19" type="text" prompt="7. Anmerkungen zur Kästchendarstellung der Ankreuzoptionen"/>
		<Q id="20" type="check" prompt="8. Nutzung des mobilen Browsers.">Beim Systemcheck musste der mobile Browser benutzt werden.</Q>
	</Config>
</SysCheck>
```
#### Kopfdeklarationen

Die XML-Datei sollte man mit einem Editor bearbeiten, der zumindest eine Validierung vornehmen kann. 
Das bedeutet, dass nicht nur die allgemeine Syntax geprüft wird (stets schließende Tags, keine Leerzeichen 
vor/hinter einem Attribut usw.), sondern nur Elemente und Attribute akzeptiert werden, die in einer System-Check-XML erlaubt sind. 
Dazu muss der Editor die Schemadatei kennen. Dies erfolgt üblicherweise über die Deklaration `noNamespaceSchemaLocation` wie im Beispiel gezeigt.
Gute Editoren unterstützen die Bearbeitung dann außerdem mit automatischer Vervollständigung.

#### Metadaten

Zur Kennzeichnung und Beschreibung der Datei sollen eine ID und ein Label vergeben werden. Ersteres dient der internen Zuordnung auch der 
Berichte, letzteres wird bei der Beschriftung des Start-Schalters verwendet. Eine Beschriftung kann helfen, verschiedene Versionen eines 
Systemchecks zu unterscheiden.

#### Netzwerkverbindung

Die Angaben in den Bereichen `UploadSpeed` und `DownloadSpeed` sind rein technischer Natur und sollten nur angepasst werden, 
wenn die Ergebnisse überwiegend unerwartet sind. Bitte fragen Sie die Spezifikation beim Entwickler-Team nach!

#### Unit

Wenn im Element `Config` ein Attribut `unit` gefunden wird, dann erfolgt nach dem Test der Verbindungsqualität die Anzeige einer Unit. 
Diese Befragungsseite bzw. Testaufgabe soll möglichst alle Element-Typen enthalten, die später auch im Test bzw. der Befragung benutzt werden. 
Es ist also z. B. hier unnötig, eine Audio-Datei einzubauen, wenn im Test keine Hörverstehensaufgabe vorkommt.

Es muss natürlich in den Arbeitsbeich auch eine Unit mit dieser ID hochgeladen werden. Außerdem ist der in der Unit-Definition genannte 
Player im Arbeitsbereich bereitzustellen.

#### Bericht speichern

Wenn im Element `Config` ein Attribut `savekey` gefunden wird, dann können die Ergebnisse des System-Checks abschließend gespeichert werden. 
Die letzte Seite enthält dann einen Schalter `Bericht senden` und es wird ein Kennwort erfragt.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.8-Testleitungskonsole">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.6-Player-Testwiedergabe-(Verona)">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 2.8 Testleitungskonsole

Soll ein Test für eine bestimmte Personengruppe (z. B. Klasse) gleichzeitig stattfinden, kann ein Monitor dafür eingerichtet werden. 
Die Testleitung kann dann für jede Testperson den Fortschritt beobachten, ggf. das Weiterblättern erzwingen, Personen ausschließen oder eine Sperre wieder aufheben.

Hier finden Sie ein kurzes [Einleitungsvideo](https://box.hu-berlin.de/f/3f23e8a85edb445ebc81/).


## Einrichten der Testleitungskonsole

Die Testleitungskonsole wird mittels **Testtakers.xml** eingerichtet. Diese gehört zu den Testdateien, wie auch die **Booklet.xml** und die **Unit.xml**. Nachfolgend ist eine Beispielkonfiguration bzw. Syntax der **Testtakers.xml** zu sehen, an der eine Orientierung im weiteren Verlauf dieses Kapitels erfolgen wird.

```xml
<Testtakers>
.
.
.
	<Group id="Testgruppe_1" label="Gruppe 1">
			
		<Login mode="run-hot-return" name="Testperson_a" pw="123">
			<Booklet>THETLK</Booklet>
		</Login>
		
		<Login mode="run-hot-return" name="Testperson_c" pw="125">
			<Booklet>THETLK</Booklet>
		</Login>
							
		<Login mode="monitor-group" name="group-monitor_1" pw="567"/>
	
	</Group>
.
.
.	
</Testtakers>
```

Zum Einrichten der Testleitungskonsole wird ein Login mit dem Modus:`monitor-group` in der zu beobachtenden Gruppe angelegt.In diesem Fall befindet sich der Login mit diesem Modus in der Group: Testgruppe_1. Daraus folgt: Die Testleitungskonsole überwacht alle Testpersonen die sich in dieser Testgruppe_1 befinden. Die final bearbeitete **Testtakers.xml** ist anschließend mit den anderen Testdateien in das Testcenter zu laden.

>Der oben gezeigte Code ist nur ein Bsp.! Es können weitere Gruppen, Testpersonen etc. angelegt werden und für jede dieser Gruppen kann ein eigener Testmonitor angelegt werden!

Weitere Informationen zur Konfiguration der **Testtaker.xml** finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml).

## Starten der Testleitungskonsole

Um die Testleitungskonsole zu starten, muss eine Neuanmeldung am Testcenter erfolgen. Anschließend sind die Zugangsdaten zu verwenden, welche als Login für die Testleitungskonsole (`monitor-group`) in der **Testtakers.xml** festgelegt wurden. In diesem Fall muss zur Anmeldung der Name: *group-monitor_1* und das Passwort: *567* verwendet werden. 

Nach der Anmeldung kann die Gruppe, welche dieser Testleitungskonsole zugeordnet ist, ausgewählt werden.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Anmeldung.png)

Nachdem die gewünschte Gruppe gewählt wurde (in diesem Fall gibt es nur eine Gruppe), ist die Testleitungskonsole zu sehen.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Ansicht1.png)

### Was ist nun zu sehen?

Nachfolgend erfolgt eine Auflistung, welche Bestandteile resultierend aus der Konfiguration der **Testtakers.xml** in der Testleitungskonsole zu sehen sind:

* die beobachtete Gruppe -> Dieser Name wurde über das Group Label gesetzt. In diesem Fall Gruppe 1.
* Benutzername der Testleitungskonsole -> Dieser Name wurde über den Login Namen der `monitor-group` gesetzt.
* die Testpersonen -> Diese Namen wurden über die Login Namen innerhalb der zu überwachenden Gruppe gesetzt.

Zu Erklärung weiterer Symbole innerhalb der Testleitungskonsole muss ein Einblick  in die **Booklet.xml** genommen werden, die zusammen mit der **Testtakers.xml** und den **Unit.xml`s** für dieses Bsp. in das Testcenter geladen wurde.

>Es wird nur der Code innerhalb der **Booklet.xml** aufgezeigt der für die Beschreibung notwendig ist!

```xml
<Booklet>
.
.
.
  <Units>
	
    <Unit id="Unit_Start" label="Beispielhafte Startseite" />
		
	<Testlet id="Examples" label="Beispiele">
		<Restrictions>
			<CodeToEnter code="Hase">Bitte 1. Freigabewort eingeben!</CodeToEnter>
		</Restrictions>
		<Unit id="Unit1" label="Postcard" labelshort="1" />
	</Testlet>
	
	<Unit id="Unit_Ende" label="Ende des Reviews" />

  </Units>
.
.
.
</Booklet>
```

Die im Bild rot markierten Symbole der Testperson_a entsprechen einer einzelnen Unit. In diesem Fall der Start- und Endunit.

Das gelb markierte Symbol entspricht dem Testlet: Examples. Die enthaltende Zahl in der gelben Markierung entspricht der Unit innerhalb des Testlets. In diesem Fall gibt es nur die Unit 1.


## Arbeiten mit der Testleitungskonsole

Nachdem die Konsole gestartet wurde, können die Zugangsdaten für die Testpersonen vergeben werden. Nach Anmeldung, ist der Bearbeitungsstand des Tests durch die Testperson ersichtlich. Über das kleine Zahnradsymbol oben rechts, kann die Ansicht individuell angepasst werden. Es können weitere Informationen ein- oder ausgeblendet werden. 

> **Ablauf, Struktur und Kontrolle eines Tests können von den Verantwortlichen individuell gestaltet werden.<br> 
An dieser Stelle können nur Empfehlungen auf Erfahrungsgrundlage gegeben werden! Die Durchführung sollte genauestens geplant und überdacht sein, um einen reibungslosen Ablauf und repräsentative Ergebnisse zu gewährleisten.**

In diesem Bsp. hat sich nur  Testperson c angemeldet und befindet sich in der Unit 1 innerhalb des Testlets.<br>
Testperson_a hat seinen Test schon abgeschlossen. Da der Modus: `run-hot-return` verwendet wurde, ist der Test nach Abschluss gesperrt, auch zu sehen an dem kleinen Schlosssymbol.
Durch markieren einer Testperson, kann der Ablauf für diese Testperson mithilfe der Steuersymbole auf der linken Seite gesteuert werden.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Ansicht2.png)

> **Werden mehrere Testhefte mit ähnlicher Struktur verwendet, ist es eventuell nicht möglich alle Testpersonen gleichzeitig zu steuern. In diesem Fall müssen die zu steuernden Testpersonen einzeln markiert (Haken setzen vor der Testperson) und dann die Steuerbefehle (Pause, springe zu etc.) abgesetzt werden.**

Die folgenden Stati können während eines Testablaufs angezeigt werden (dies ist nur eine bsph. Darstellung, die aufgezeigten Symbole können nicht gemeinsam auftreten!):

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Ansicht3.png)

Weitere detailierte Informationen zu den den Stati finden Sie auch [hier](https://iqb-berlin.github.io/testcenter-frontend/super-states).

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2.7-System-Check">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Bw_Button_final.png" align="left">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---