# 2 Testcenter

Das IQB-Testcenter ist eine Webanwendung für die Durchführung von Kompetenztests oder Befragungen. 
Nach der Installation auf einem Webserver wählt man diesen Server über seine Adresse an, d. h. man schreibt 
dessen Internet-Adresse in die Adresszeile eines Internet-Browsers. Dadurch werden die Programmierungen geladen 
und man sieht ein Formular zum Anmelden. Alle Daten für einen Test sind vorher auf dem Server zu speichern. 
Das kann über ein integriertes Verwaltungsportal erfolgen oder über andere Webanwendungen, die auf den Server zugreifen.

Eine grobe Einführung in das Testcenter geben auch die nachfolgenden Verlinkungen.                        
Das IQB bietet folgende [Video-Präsentationen](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Testcenter) bzgl. des Testcenters an.

**Installation**

Das IQB hat alle Programmierungen unter der Open Source-Lizenz [MIT](https://opensource.org/licenses/MIT) veröffentlicht und erleichtert die Installation durch ein sog. 
Docker-Setup. Für die Installation muss man einen Server bereitstellen (Linux oder Windows) und dieser Server muss dann über 
eine Internet-Adresse erreichbar sein. Die Installation sollte erfahrenes IT-Fachpersonal durchführen. 
Die Dokumentation hierzu setzt Wissen vor allem zur Virtualisierungssoftware Docker voraus. 
Es ist weiterhin Wissen zu Datensicherheit nötig, denn sobald ein Server öffentlich verfügbar ist, müssen Maßnahmen 
gegen Angriffe durch Schadsoftware ergriffen werden. Das IQB ist bemüht, die Installationspakete gut abzusichern, 
übernimmt aber im Schadensfall keine Verantwortung.

**Verwaltung der Tests**

Nach der Installation ist zunächst ein Standard-Konto für die Verwaltung von Tests angelegt. 
Außerdem ist ein Arbeitsbereich angelegt mit einem Beispieltest. Im ersten Schritt sind über ein Verwaltungsportal die Testinhalte 
(Aufgaben, Testabläufe usw., z. B. als XML-Dateien) in das Testcenter zu laden. Nach der Durchführung des Tests, können über
dieses Verwaltungsportal die Ergebnisse heruntergeladen werden (Csv-Dateien). Die Texte dieser Wiki sind vor allem für Personen gedacht, 
die diese Verwaltungsaufgaben ausführen.

Man kann eine Installation des IQB-Testcenters weitgehend anpassen. Begrüßungsnachrichten, Hintergrundfarbe, Logo auf der Startseite und selbst der Name der Anwendung kann an eigene Wünsche angepasst werden.

**Durchführung von Tests oder Befragungen**

Durch Anwählen der Internet-Adresse des Testcenter-Servers erhält man ein Anmeldeformular. 
Eine Testperson muss über Zugangsdaten verfügen und es startet dann das für diese Person vorbereitete Testheft 
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

Man kann bei der enormen Vielfalt der Hardware (Tablet, Smartphone usw.) und Software (Apple, Linux, Android usw.) nicht garantieren, dass ein Test oder eine Befragung so wie beabsichtigt funktioniert. Je nach Anforderung an den Test wird das auch nicht sinnvoll sein, z. B. wenn eine Mindestbreite 
für den Bildschirm erforderlich ist.

Wenn man erfahren möchte, ob die Zielsysteme geeignet sind, kann man im IQB-Testcenter einen System-Check konfigurieren. 
Dann können z. B. die verantwortlichen Lehrkräfte in der Vorbereitungsphase im Testcenter einen auf die speziellen Anforderungen des 
Tests abgestimmten Check durchführen. Auch die Internetverbindung kann hierüber bewertet werden.

Ein System-Check sollte aber auch nicht überbewertet werden. Ein positiver Befund ist keine Garantie dafür, dass am Tag der Durchführung alles glatt läuft. Die Leistungsfähigkeit der Internetverbindung beispielsweise hängt davon ab, was parallel in der Schule gerade an Bandbreite für andere Zwecke (z. B. automatische System-Updates) belegt ist. Außerdem erhöht ein System-Check den ohnehin hohen Aufwand einer Testung und könnte die Teilnahmemotivation weiter senken.

**Testleitungskonsole**

Soll ein Test für eine bestimmte Personengruppe (z. B. Klasse) gleichzeitig stattfinden, kann ein Monitor dafür eingerichtet werden. 
Die Testleitung kann dann für jede Testperson den Fortschritt beobachten, ggf. das Weiterblättern erzwingen, Personen ausschließen oder eine 
Sperre wieder aufheben.

**<a name="system-requirements"></a>Systemanforderungen**

Da die Programmierungen des Testcenters online in einem Browser ablaufen, ist keine vorherige Installation von Software auf einem Computer nötig, 
mit dem der Test oder die Befragung durchgeführt werden soll. Es ist nur ein Internet-Zugriff und ein Browser nötig.

Es gibt immer wieder die Diskussion darüber, ob bzw. in welchem Maße ältere Browser bzw. Browserversionen unterstützt werden sollen. Hier wird argumentiert, dass Schulen bzw. deren Träger oft nicht in der Lage seien, die Verwendung aktueller Browser sicherzustellen. Aus dieser Realität ergebe sich, dass die Programmierungen für TBA stets ein Maximum an Abdeckung auch für alte Browser leisten müssten.

Das IQB folgt hier jedoch den Anforderungen an die Datensicherheit, so wie es z. B. das [Bundesamt für Sicherheit in der Informationstechnik](https://www.bsi.bund.de/) formuliert:

> "Der Internet-Browser ist die zentrale Komponente für die Nutzung von Online-Angeboten und stellt somit eins der beliebtesten Ziele für Cyber-Angriffe dar. Hieraus ergibt sich ein besonders hohes Gefahrenpotenzial." [Quelle](https://www.bsi.bund.de/DE/Themen/Verbraucherinnen-und-Verbraucher/Informationen-und-Empfehlungen/Cyber-Sicherheitsempfehlungen/Updates-Browser-Open-Source-Software/Der-Browser/der-browser_node.html)

> "Installieren Sie alle Updates sofort oder zeitnah nach ihrer Veröffentlichung, sowohl die für Ihren Browser, als auch für alle Erweiterungen und natürlich Ihr Betriebssystem. Verwenden Sie stets die neuste Version Ihres Browsers." [Quelle](https://www.bsi.bund.de/DE/Themen/Verbraucherinnen-und-Verbraucher/Informationen-und-Empfehlungen/Cyber-Sicherheitsempfehlungen/Updates-Browser-Open-Source-Software/updates-browser-open-source-software_node.html)

Das IQB unterstützt daher nur die jeweils letzten beiden Hauptversionen eines Browsers bzw. - bei Chrome und Firefox - die Versionen der letzten 12 Monate. Beispielsweise werden derzeit (Stand April 2022) bei Safari nur die Versionen 14 (Veröffentlichung September 2020) und 15 unterstützt. 

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

Das **Teststudio** gibt nach dem Aufgabenentwurf Dateien aus. Diese Dateien müssen zur Testdurchführung in das **Testcenter** geladen werden. Nachfolgend werden die Funktionen dieser Dateien beschrieben. Zum besseren Verständnis schauen Sie sich auch gerne die [**Videos**](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Die-Testdateien) zum Thema Testdateien an .

### Logins

Jede Person, die an einem Test bzw. einer Befragung beteiligt ist, muss Zugangsdaten erhalten. Diese Informationen sind in einer [XML-Datei](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml) festgelegt. Folgende Arten des Zugriffs (Rollen) werden unterschieden:
* Testpersonen: Die Personen, die den Test bzw. die Befragung absolvieren. Deren Antworten bilden mit dem Rohdatensatz die Grundlage der Auswertung.
* Testleitung: Ein spezieller Login sorgt dafür, dass die angemeldete Person den Monitor für eine Testgruppe startet. Damit kann der Fortschritt der Beantwortung beobachtet werden. Außerdem können Testpersonen ausgeschlossen, ein Test angehalten oder eine Navigation zu einem Testblock erzwungen werden.
* Review: Zum Ausprobieren eines Tests können spezielle Logins vorbereitet werden. Man kann dann Kommentare zu den Aufgaben und dem Test vergeben und es sind einige Navigationsbeschränkungen unwirksam, wie z. B. Zeitlimits.
* Demo: Man kann den Test aufrufen, aber die Antworten werden nicht dauerhaft gespeichert. Ruft eine andere Person mit denselben Login-Daten den Test auf, werden keine älteren Antworten geladen.

Das Erstellen von Logins wird unterstützt über das Windows-Programm [itc-ToolBox](https://github.com/iqb-berlin/itc-toolbox#readme).

### Test-Definition

Diese [XML-Datei](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Booklet%E2%80%90Xml) legt die Reihenfolge der Aufgaben (Units) fest. Man kann die Aufgaben bzw. Zwischenseiten auch in Blöcke (Testlets) gruppieren. Innerhalb dieser Blöcke (Testlets) können dann Beschränkungen festgelegt werden. Bspw. kann ein Block dann nur nach Eingabe eines Code-Wortes betreten werden oder es gilt eine zeitliche Beschränkung für einen Block. Außerdem kann über die Test-Definition das Weiterblättern auf Folgeseiten mit Bedingungen verknüpft werden. Das Springen (scrollen) an das Seitenende könnte bspw. eine solche Bedingung darstellen. Diese Bedingung würde sicherstellen, dass die Testperson den gesamten Inhalt der Seite wahrgenommen hat. Auch das Beendigen von Audio-Sequenzen oder die Beantwortung aller Fragen, könnte eine solche Bedingung sein.

> **In der Grafik ist dargestellt, dass die Definition von Tests über das IQB-Teststudio erfolgt. Das wird in zukünftigen Versionen der Fall sein. Die aktuelle Version IQB-Teststudio-Lite unterstützt dies nicht, sondern man muss die XML-Datei für die Test-Definition manuell erzeugen.**

### Unit-Definition

Eine Unit-Definition besteht aus einer [XML-Datei](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Unit%E2%80%90Xml) und einer Voud-Datei. Erstere enthält Metadaten, wie die interne ID und den Datentyp der Unit. Bei der Voud-Datei handelt es sich um ein internes Format, welches manuell kaum editierbar ist. Es muss stattdessen über einen Editor erzeugt werden. Das IQB-Teststudio bietet derartige Editoren.

### Player

In der Grafik ist dargestellt, dass das Testcenter intern eine Komponente "Player" enthält. Grundidee dieser Teilung ist, dass das interne Format einer Unit-Definition nicht direkt vom Testcenter selbst verarbeitet wird, sondern von einem Plug-In, welches je nach Unit-Datentyp hinzugeladen wird. Durch diese Technik wird eine hohe Flexibilität erreicht: Änderungen der unitbezogenen Programmierung führen nicht zu einem neuen Testcenter, sondern nur der Plug-In-Code des Players wird ausgetauscht. Näheres hierzu im Abschnitt [2.5 Player (Verona)](2.5-Player-(Verona)).

Für die Vorbereitung eines Tests bedeutet dies:

1. jede Unit-Definition einen Verweis auf das Datenformat und damit auf den erforderlichen Player enthalten muss und
2. alle Player, die von Units benötigt werden, müssen vorab als Ressourcendatei in das Testcenter geladen werden

## Daten-Output des Testcenters

### Logs

Ereignisse innerhalb einer Unit und auch insgesamt innerhalb eines Tests, werden in ein Protokoll geschrieben. Dieses sog. "Logging" kann reduziert und auch ganz abgestellt werden, um die Datenmenge zu reduzieren. Welche Ereignisse genau gespeichert werden, ist auch vom Player abhängig. Folgende Erkenntnisse lassen sich beispielsweise aus den Log-Daten ablesen:
* Version des Betriebssystems und des Browsers
* Verweildauer auf einer Seite
* Zeitpunkt des Beendens der Beantwortung

### Antworten

Als Antworten werden Zustandsänderungen der Eingabe-Elemente der Units verstanden. Wenn die Testperson ein Ankreuzkästchen wählt, eine Linie mit der Maus verschiebt oder mehrere Sätze in ein Eingabefeld schreibt - all diese Eingaben werden mit dem jeweils letzten Stand gespeichert.

### Weitere Daten

* **Kommentare, Review**: Wenn ein Test im Review-Modus durchgeführt wird, können zu Aufgaben oder zum gesamten Test Kommentare gegeben werden. Auch diese Kommentare sind über den Management-Bereich abrufbar.
* **System-Check Berichte**: Nach der Durchführung eines System-Checks werden bei Bedarf die Daten in der Datenbank gespeichert und sind ebenfalls abrufbar.

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

Zunächst muss man sich am Computer, an dem der Test durchgeführt werden soll, anmelden. Sollte man die Account-Daten nicht parat haben, braucht es erstmal etwas Zeit, um neue Daten zu beschaffen (Ist die ITG-Lehrerin da?). Der Computer ist dann hochgefahren und ein einigermaßen moderner Browser ist installiert.

## Am Testsystem anmelden

Nun kommt es auf die richtige Internet-Adresse an. Diese sollte bitte nicht in das Suchfeld von Google oder einer anderen Suchmaschine eingegeben werden, denn dann gibt es eine Trefferliste mit ungewissem Ausgang. Die Adresse ist also besser oben in die Adressleiste des Browsers einzutragen.

Das Startbild ist sehr reduziert. Rechts ein paar allgemeine Informationen (Version, Datenschutz etc.), links nur Eingabefelder für Name und Kennwort. Nach der Eingabe wird ein großer Schalter präsentiert, der das Testheft symbolisiert, das gestartet werden soll. Die Anzeige des Testheftes signalisiert auch eine erfolgreiche Anmeldung.

> Weitere Informationen zur Anmeldung finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Login:-Anmeldeverfahren)

Mögliche Probleme:

* Wenn das Startbild zu sehen ist, ist schonmal eine funktionierende Internet-Verbindung anzunehmen. Ist dies nicht der Fall, sollten entsprechende Routinen zur Fehlerbehebung beginnen (lose Kabel etc.).
* Wenn das Startbild einigermaßen gut aussieht (nichts verrutscht, nichts überlagert), dann ist auch der Browser nicht zu alt. 
* Wenn gleich zu Anfang vor der Anmeldung ein roter Balken oben zu sehen ist, dann stimmt etwas nicht mit der Programmierung. Diese Erscheinung sollte dann an allen Arbeitsplätze auftreten. In diesem Fall sollte unbedingt die Hotline kontaktiert werden.
* Wenn für die Anmeldedaten kein Testheft gefunden wurde, dann gibt es eine rote Ausschrift, die genau das meldet. Es ist dann zu prüfen, ob die Eingabe richtig war.
* Wenn der Schalter für das Testheft ausgegraut ist, dann ist dieser Test gesperrt oder noch nicht freigegeben. Für Tests könnte ein Zeitfenster definiert sein. Es sollte dann nochmal einmal die Anweisungen studiert und ggf. bei der Hotline nachgefragt werden.

## Durchführen des Testheftes bzw. der Befragung

Mit Klick auf die Schaltfläche des Testheftes werden alle Testinhalte geladen. Sobald möglich wird auch die erste Seite schon gezeigt und das Laden wird im Hintergrund fortgesetzt. Jeder Computer im Raum lädt immer nur die Daten für eine Aufgabe. Obwohl theoretisch ein Browser mehrere Aufgaben gleichzeitig laden könnte, wird dies unterbunden, damit sich einzelne Computer nicht vordrängeln und andere ausbremsen. Ein Computer, der später mit dem Herunterladen startet, wäre sonst erstmal blockiert bis andere fertig sind.

Während des Tests werden keine weiteren Inhalte vom Server geladen, sondern nur die Antworten gespeichert.

Die Aufgabennavigation erfolgt rechts oben. Sollte eine Aufgabe aus mehreren Seiten bestehen, dann kann man rechts unten mit entsprechenden Schaltern blättern. Manchmal ist die Bearbeitungszeit begrenzt, dann werden rechtzeitig (5 min und 1 min vor Ende) Hinweise eingeblendet.

Sollten technische Probleme mit dem Computer auftreten (z. B. Audio-Buchse defekt), dann kann jederzeit der Browser geschlossen und der Test auf einem anderen Computer neu gestartet werden. Die schon gegebenen Antworten werden geladen.

## Steuerung durch Testleitungskonsole

Die Testleitung hat eventuell mittels separater Anmeldung die sog. Testleitungskonsole gestartet. Das kann dazu führen, dass bswp. für eine Ansage die Bearbeitung für alle gestoppt wird und erst einmal nichts mehr beantwortet werden kann. Später wird eventuell eine Fortsetzung mit einer ganz anderen Aufgabe erzwungen. Es wird dann bspw. auch bemerkt, wenn ein anderes Browserfenster geöffnet wird.

## Test oder Befragung beenden

Die Beantwortung kann jederzeit beendet werden. Die Antworten werden stets sofort gespeichert und es ist hierfür kein Kommando erforderlich. Manchmal gibt es am Ende einen Schalter "Test beenden" oder "Befragung verlassen". Dann kehrt man zur Auswahl des Testheftes zurück.

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

In das **Testcenter** müssen die Inhalte für Tests geladen werden und es muss einen Weg geben, die Antworten zu erhalten. Für diese Aufgaben ist ein Verwaltungsportal eingerichtet. Die Verantwortlichen für eine Studie melden sich am Testsystem an derselben Stelle an, an welcher sich auch die Testperson anmelden würde. Das System erkennt, dass die Anmeldedaten zu einem Konto für die Verwaltung gehören und lädt entsprechend die Funktionen dafür.

## Arbeitsbereich

Damit mehrere Studien gleichzeitig auf einem Testsystem durchgeführt bzw. vorbereitet werden können, sind sog. Arbeitsbereiche vorbereitet. Die Benennung richtet sich günstigerweise nach dem Zweck, also z. B. "Demo Deutsch Sek1" oder "Review Abi" oder "VERA Englisch". Für jedes Verwaltungskonto ist festgelegt, welche Arbeitsbereiche eingesehen (Nur-Lese-Modus) bzw. geändert werden können (Lesen-Und-Schreiben-Modus).

Nach der Anmeldung präsentiert das System eine Liste aller Arbeitsbereiche, die für diese Person freigegeben sind. Mit einem Klick auf den jeweiligen Arbeitsbereich wird dieser geöffnet. Zur Liste der Arbeitsbereiche kehrt man zurück, indem man auf das IQB-Logo links oben in der Ecke klickt.

Der Arbeitsbereich hat drei Grundfunktionen. Diese können mit einem Klick auf den entsprechenden Tab ausgewählt werden:
* Dateien
* System-Check Berichte
* Ergebnisse/Antworten

### Tab Dateien

Alle Testinhalte und Definitionen eines Tests bzw. einer Befragung, werden über Dateien in das System hochgeladen. Sie müssen also erst einmal auf dem eigenen Computer vorbereitet werden (bspw. über einen Download aus einer anderen Webanwendung (Units)). Meist handelt es sich um XML-Dateien, die einer fest vorgeschriebenen Syntax folgen und aus denen das Testsystem alle notwendigen Informationen liest. Die Bedeutung der Dateien sind den Einzeldokumenten in dieser Wiki zu entnehmen.

Sobald eine Datei hochgeladen ist, ist sie wirksam. D. h. unmittelbar nachdem eine Datei mit Login-Daten hochgeladen wurde, kann sich eine Testperson mit diesen Daten anmelden. Sollte man feststellen, dass eine Unit Fehler enthält, kann man die Unit-Datei überarbeiten und erneut in das **Testcenter** laden. Jeder danach gestartete Test, wird dann die neue Unit verwenden.

Beim Laden in das **Testcenter** werden die XML-Dateien geprüft. Eine Datei kann abgewiesen werden, wenn sie syntaktisch oder inhaltlich fehlerhaft ist. Z. B. wird eine Testtaker-Datei abgewiesen, wenn sie Anmeldedaten enthält, die bereits in einem anderen Arbeitsbereich verwendet wurden. Es wird auch eine Booklet-Datei abgewiesen, wenn sie bspw. auf Units verweist, die nicht im Arbeitsbereich gefunden wurden. Daher spielt die Reihenfolge des Hochladens eine wichtige Rolle.

Probleme kann es geben, wenn ein Test gestartet wurde (also ein Login verwendet wurde), und dann durch Hochladen einer neuen Testtaker-Datei die Testheftzuweisung oder der Durchführungsmodus geändert wird. In diesem Fall sollten statt dessen neue Logins angelegt werden.

### Tab System-Check Berichte

Hier können die Berichte, die über einen System-Check abgeschickt wurden, heruntergeladen werden. Es handelt sich um CSV-Dateien, die man sich gleich z. B. in Microsoft Excel anschauen kann.

### Tab Ergebnisse/Antworten

Hier können Antworten und Logs, die über die Tests bzw. Befragungen innerhalb dieses Arbeitsbereiches abgeschickt wurden, heruntergeladen werden. Auch hier ist das Dateiformat CSV. Sollte das Testcenter über ein Länderportal verwaltet werden, dann steht hier auch ein Download im JSON-Format zur Verfügung.

## System-Admin (Super-Admin)

Wurden Ihnen Rechte für die Verwaltung des Gesamtsystems zugewiesen (sog. Super-Admin), wird am Ende der Liste der Arbeitsbereiche ein System-Admin-Schalter eingeblendet. Über diesen Schalter gelangen Sie zur Systemverwaltung. Dort können Nutzerkonten (Benutzername und Kennwort) und Arbeitsbereiche angelegt werden. Auch der Zugriff auf diese Arbeitsbereiche kann für die jeweiligen Personenkreise festgelegt und grundsätzliche Systemeinstellungen (Hintergrundfarbe, Logo) vorgenommen werden.

Der System-Admin-Bereich wird in **3 Reiter** unterteilt:

* **Users:**<br>
Hier können bestehende Benutzer\*innen verwaltet werden. Es können mittels Pluszeichen-Schaltfläche neue Benutzer\*innen hinzugefügt werden oder mit der Löschen-Schaltfläche gelöscht werden. Weiterhin stehen zwei Schaltflächen zur Änderungen von Kennwort und Zugriffebene bereit. Diese beide Schaltflächen sind mit einem Stift-Symbol gekennzeichnet. Ist eine Person als Super-Adminn angelegt, wird diese mit einem Stern gekennzeichnet. Wird in der Liste der angelegten Personen eine Person markiert, werden auf der rechten Seite alle Arbeitsbereiche angezeigt, auf die diese Person Zugriff hat. Die Berechtigung für einen Arbeitsbereich sind dabei noch einmal unterteilt in "read only" (RO) und "read and write" (RW).

* **Arbeitsbereiche:**<br>
Hier werden alle angelegten Bereiche aufgelistet. Es können neue Bereiche angelegt, gelöscht oder nachträglich bearbeitet werden. Durch Markierung eines Bereichs werden rechts alle Personen aufgelistet, die auf diesen Bereich Zugriff haben. Dabei wird noch einmal unterschieden, ob die Personen nur lesend (RO) oder lesend und schreibend (RW) auf den Bereich zugreifen darf. Sollen Personen einen Zugriff auf einen Bereich erhalten, ist der jeweilige Bereich zu markieren und die Person mit RO- oder RW-Zugriff auszuwählen. Anschließend muss zwingend das Speicher-Symbol oben rechts aktiviert werden, ansonsten werden die Änderungen nicht gespeichert.

* **Einstellungen:**<br>
Hier können einige Bereiche des Testcenters an individuelle Bedürfnisse angepasst werden. Es ist bspw. möglich ein Logo einzufügen, Hintergrundfarben der Anwendung und verschiedener Anzeigebereiche anzupassen und Texte zu verändern. Es können weiterhin Textersetzungen für die Bereiche: Testheft, Gruppenmonitor, Login und System-Check erfolgen. Sollen Texte ersetzt werden, ist nach Änderungen zwingend die Speichern-Schaltfläche zu betätigen um die Änderungen zu übernehmen.

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

Wie im Abschnitt [Daten und Prozesse](2.1-Daten-und-Prozesse) beschrieben, besteht die Definition eines Tests oder einer Befragung aus speziellen Dateien, welche in das **Testcenter** geladen werden müssen. Die Verwaltung der Dateien erfolgt dabei im [Verwaltungsportal](2.3-Portal-zur-Verwaltung). Die Dateien weisen dabei untereinander Abhängigkeiten auf. Diese sind grob:

* Units definieren jeweils eine Aufgabe bzw. eine Seite
* Booklets definieren die Anordnung der Units
* Logins definieren den Zugriff einer Testperson auf ein Booklet.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Upload_Ablauf_final.png)

Folgende Texte geben Erläuterungen für diese zentralen Funktionen:

* [Allgemeine Hinweise für die Bearbeitung von XML-Dateien](Arbeiten-mit-Xml%E2%80%90Dateien)
* Units: 
  * [Bearbeiten der XML-Datei](Unit%E2%80%90Xml)
* Booklets:
  * [Bearbeiten der XML-Datei](Booklet%E2%80%90Xml)
  * [Unterstützung durch itc-ToolBox](https://github.com/iqb-berlin/itc-toolbox#readme)
* Logins:
  * [Bearbeiten der XML-Datei](Testtaker%E2%80%90Xml)
  * [Unterstützung durch itc-ToolBox](https://github.com/iqb-berlin/itc-toolbox#readme)
  * [Anmeldeverfahren](Login%3A-Anmeldeverfahren)
  * [Modi der Testdurchführung](Login%3A-Modi-der-Testdurchf%C3%BChrung)

**Empfehlung: Verweis zur Validierung**

Eventuell wird nach dem Hochladen in das Testcenter eine Warnung "File has no link to XSD-Schema..." angezeigt. Diese Warnung bedeutet, dass die XML-Datei keinen expliziten Verweis auf eine XSD-Datei enthält. Eine solche XSD-Datei definiert die möglichen Elemente und Attribute einer XML-Datei und kann daher zur Prüfung der XML-Datei verwendet werden. Das IQB stellt solche XSD-Dateien bereit. 

Die Deklaration der XSD-Datei erfolgt im Haupt-Element einer XML-Datei. Für die Unit-XML heißt das Hauptelement `Unit` und muss folgendermaßen geändert werden:

```
<Unit 
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:noNamespaceSchemaLocation="https://raw.githubusercontent.com/iqb-berlin/testcenter-backend/9.1.1/definitions/vo_Unit.xsd">
```

Ein nützlicher Nebeneffekt hierbei ist, dass auch Editoren zur Bearbeitung von XML-Dateien (z. B. Notepad++, Sublime) nun eine Validierung vornehmen können. Man kann also bereits vor dem Hochladen eine Validierung bereits beim Schreiben einer XML-Datei vornehmen lassen.

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

Es können Antwort- und Logdateien heruntergeladen werden. Diese werden im **Testcenter** in dem Arbeitsbereich gespeichert, in den auch die Testdateien für den Test geladen wurden.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Ergebnisse_final.png)

> **Es werden nicht in jedem Testmodus Ergebnisse gespeichert. Die Speicherung findet nur in den beiden Modi: 'run-hot-return' und 'run-hot-restart' statt!**

Die Ergebnisse können mittels der üblichen Browserfunktionalitäten heruntergeladen werden. Die Dateien werden dann als CSV-Dateien gespeichert und können im Sinne einer besseren Übersichtlichkeit mit dem IQB Tool **itc-Toolbox** in eine XLSX-Datei gewandelt werden. Mehr dazu erfahren Sie auch in dem folgenden [Einzeldokument](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/itc%E2%80%90ToolBox:-Antworten-und-Logs).

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

Das Testcenter ist modular aufgebaut. Es besteht aus der eigentlichen Webanwendung und einem Player. Letzterer ist dabei in die Webanwendung eingebettet. Der Player ist ein Stück Software und übernimmt die Wiedergabe der Aufgaben. Er verfügt des Weiteren über entsprechende Schnittstellen, die ihn mit dem **Testcenter** verbinden. So kann der Player bspw. Aktionen innerhalb einer Aufgabe aufzeichnen. Zu diesen Aktionen gehören bspw. das Setzen von Anwortoptionen, das Scrollen zum Seitenende, die Verweildauer auf einer Testseite und einige mehr. Der Player trägt mit seinen Schnittstellen also auch erheblich zur Auswertungsmöglichkeit eines Tests bei. 

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Bereich_Player_final.png)

**Rot markiert:**<br>
Bereich der Webanwendung zur Steuerung eines Tests mittels Funktionsschaltknöpfen und Informationen zum Test.

**Blau markiert:**<br>
Bereich des Players zum Abspielen einer Aufgabe.

Welche Vorteile bietet diese Aufteilung?<br>
Werden Aufgaben erstellt und dabei neue Elemente verwendet, die dem Testcenter noch unbekannt sind, muss nicht der Programmcode des gesamten **Testcenter** angepasst werden, sondern nur der Programmcode des verwendeten Players. Bei der Aufgabenerstellung im **Teststudio** kommen unterschiedliche Editoren zum Einsatz. Diese Editoren bieten unterschiedliche Funktionen und Aufgabenelemente. Zu jedem Editor gehört ein entsprechender Player, welcher die Funktionen und Elemente des verwendeten Editors kennt und diese daher später auch wiedergeben kann. 

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
Online-Test nicht geeignet ist. Der **System-Check** ist ein Weg vorab diese Eignung zu prüfen. Man kann natürlich nicht alle Probleme erkennen 
und vielleicht hat man für bestimmte Probleme auch keine Lösung parat, aber man kann die Ausfall-/ und damit die Frustrate deutlich senken.

## Planung

Bzgl. Personen-, Aufgaben- und Bookletanzahl ist jede Testung anders und stellt daher auch unterschiedliche Anforderungen an die testdurchführenden IT-Systeme. Die Testleitung muss daher die Anforderungen an das testdurchführende IT-System individuell für ihre Testung ermitteln. Ist bspw. eine Testung mit 10 Schüler\*innen und einem Booklet mit jeweils 10 Units geplant, stellt dies sicherlich eine geringere Anforderung an die IT-Systeme dar, als eine Testung mit 100 Schüler\*innen und mehreren Booklets. In diesem Zusammenhang dürfte die Bandbreite der Internetverbindung eine der wichtigsten Kriterien bzgl. Durchführbarkeit einer Testung sein. Aber auch Betriebssystem, Browserversion und Bildschirmauflösung stellen wichtige Kriterien dar.

:heavy_exclamation_mark: Der **System-Check** kann keine Aussage darüber machen ob das gewählte IT-System geeignet ist oder nicht. Der **System-Check** ermittelt nur den Ist-Zustand des Systems. Mithilfe dieser Daten müssen Sie entscheiden ob eine Eignung vorliegt oder nicht.

Es sollten also seitens der Testleitung vor der Testdurchführungen Überlegungen bzgl. der Anforderungen an die eigene Testung angestellt werden.

### Welche Fragen sollte sie sich in diesem Zusammenhang stellen und wo erhalten Sie Antworten?

**Ist das Betriebssystem und der Browser für die Testung geeignet?**

Diese Frage hängt weniger von Ihrem Test, als vielmehr von der eigentlichen Anwendung: **Testcenter** ab. Daher finden Sie diese Informationen auch in diesem [Wiki](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/2-Testcenter) unter "Anforderungen".

**Handelt es sich um einen PC oder vielleicht ein Tablet?**

Diese Frage ist eigentlich nur dann interessant, wenn die Aufgaben zuvor im **Teststudio** nicht dynamisch entworfen wurden. Dann verhalten sich die Aufgabeninhalte nicht responsiv und werden bspw. auf einem Tablet eventuell nicht so dargestellt wie ursprünglich angedacht.

**Wie hoch ist die Auflösung des Wiedergabebildschirms?**

Diese Frage spielt eine wichtige Rolle bzgl. der Darstellung und Lesbarkeit Ihrer Aufgaben. Mittels **System-Check** ist es möglich, als kritisch eingestufte Aufgabe hinsichtlich der Lesbarkeit, während des **System-Checks** abzuspielen. Dazu können dann noch Fragen während des "System-Checks" gestellt werden. Bspw.: Konnte alles gelesen und abgespielt werden? Die Antworten werden dann im Rahmen des **System-Checks** gespeichert und können dann ausgewertet werden.

**Welche Internet-Bandbreite wird für die Testung mindestens benötigt?**

Das ist wohl eine der wichtigsten Fragen, die Sie sich stellen sollten. Ist die Bandbreite zu gering, kann im schlimmsten Fall die Testung am jeweiligen PC nicht durchgeführt werden. Um die benötigte Bandbreite aus Ihrer Testung abzuleiten bedarf es weiterer Überlegungen. Entscheidend sind dabei die folgenden Punkte:

* Wie viele Booklets werden während der Testung voraussichtlich gleichzeitig gestartet?
* Wie groß sind diese Booklets?
* Wie viele Testpersonen werden an der Testung gleichzeitig teilnehmen?
* Wie lang sollen die Ladezeiten für jede Testperson maximal sein?

Aus all diesen Fragen eine benötigte Bandbreite abzuleiten kann immer nur ein grober Richtwert sein. Zu viele Faktoren spielen dabei eine große Rolle. Bspw. kann am Tag der Testdurchführung die schulische Internetanbindung ganz anders ausgelastet sein als am Tag des **System-Checks**. Daher sollten immer entsprechende Reserven eingeplant werden. Die so ermittelten Anforderungen an die Bandbreite können dann als Grenzwerte im **System-Check** hinterlegt werden. Auf dieser Grenzwerte gibt der **System-Check** abschließend aus ob die Bandbreite ausreichend ist oder nicht.

Nachfolgend finden Sie ein kleines Beispiel wie eine Berechnung angestellt werden könnten.

---

Testszenario:<br> 
* 10 Testpersonen, 1 Booklet, Bookletgröße = 6 MByte, max. Ladezeiten = 30s
* alle Testpersonen sollen den Test zeitgleich starten

:information_source: Haben Sie das/ die verwendet_en Booklets in das **Testcenter** geladen, sehen sie rechts daneben die Größe in MByte.

---

Berechnungen:<br>
Die Grenzwertangaben im **System-Check** müssen in Bytes pro Sekunde angegeben werden. Daher müssen wir erst einmal alle Einheiten in diese Einheit überführen.

Die Bookletgröße beträgt: 6 MByte <br>
Umgerechnet entspricht dies: 6.291.456 Bytes (1024 Byte = 1 kByte)

10 Testpersonen nutzen das Booklet zeitgleich <br>
Das ergibt eine Gesamtdatenlast für den Test von: 10 x 6.291.456 Bytes = 62.914.560 Bytes

Diese Datenmenge muss nun innerhalb der max. Ladezeit von 30 s übertragen werden <br>
62.914.560 Bytes / 30s = 2.097.152 Bytes/ s



Im **System-Check** könnten anschließend diese Grenzwerte als Mindestanforderung an die Bandbreite hinterlegt werden. Nach dem Start des **System-Checks** würden dann ermittelte Geschwindigkeitswerte über dem Grenzwert als "Gut" bezeichnet werden. 

Nach dem Einrichten eines System-Check erscheint auf der Seite der Webanwendung (hier: IQB-Testcenter) ein neuer Schalter `System-Check`. 
Man kann alle Interessierten einladen darüber zumindest eine Prüfung der Internetanbindung vorzunehmen (Bandbreite) und eine Anzahl von 
Hardware- und Softwareinformationen anzuzeigen. Außerdem stehen die folgenden Optionen zur Verfügung:

* Probeweises Aufrufen einer Testaufgabe: Eine speziell dafür entwickelte Testaufgabe wird gezeigt und man kann die Bearbeitungselemente auswählen,
  ändern und so prüfen, ob die Aufgabenelemente wie erwartet funktionieren.
* Fragebogen beantworten: Die Person, die den System-Check durchführt, kann eine Liste von Fragen beantworten. 
  Die Fragen können sich zunächst auf die vorherige Testaufgabe beziehen (Wurde die Audio-Datei abgespielt?;
  Passte alles auf den Bildschirm? usw.), aber auch weitere Informationen zur Ausstattung vor Ort können erfragt werden 
  (Wieviele Plätze sind im PC-Lab?; Können die Testpersonen sich gegenseitig auf den Bildschirm schauen?; Gibt es ein Whiteboard? usw.)
* Bericht abschicken: Es kann festgelegt sein, dass die Daten gespeichert werden zur späteren Auswertung. 
  Dazu sollte ein Kennwort vergeben werden und eine weitere Kennung anhand derer die Zuordnung der Daten z. B. 
  zu einer bestimmten Schule möglich wird.

### Einrichten des System-Checks: XML-Definition schreiben




Ein System-Check wird über eine XML-Datei gesteuert. Hier kann die Testleitung einige Eckdaten angeben, die nach Auswertung des System-Checks angeben, ob das System auf dem die Testung durchgeführt werden soll, geeignet ist oder nicht.  




  Außerdem kann eine Unit-Definition hinzugelegt werden (XML-Datei, 
VOUD-Datei und zugehöriger Player).  in All diese Dateien sind über einen beliebigen Arbeitsbereich in das **Testcenter** zu laden. 
Nach Abmeldung am **Testcenter** ist dann ein Schalter auf der rechte Seite des Testcenters mit dem Namen: System-Check zu finden. Die Berichte des System-Checks können nach Abschluss in diesem Arbeitsbereich gespeichert werden.

Nachfolgend ist eine System-Check-XML einmal bspw. aufgeführt. Texte und Parameter können den Bedürfnissen entsprechend angepasst werden.

> **Für diese XML-Datei ist eine Schema-Definition angelegt. Das heißt: Es können nur erlaubte Attribute und Daten in dieser Datei verwendet werden. Was erlaubt ist und was nicht entnehmen Sie bitte dieser [Schema-Definition](https://github.com/iqb-berlin/testcenter-backend/blob/master/definitions/vo_SysCheck.xsd)!**

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

Die XML-Datei sollte mit einem Editor bearbeitet werden, der zumindest eine Validierung vornehmen kann. 
Dies bedeutet: Es wird nicht nur die XML-Syntax geprüft (beginnende und schließende Tags, keine Leerzeichen 
vor/hinter einem Attribut usw.), sondern auch ob die verwendeten Elemente und Attribute in dieser System-Check-XML erlaubt sind. 
Dazu muss im Editor der Pfad zur jeweiligen Schemadatei angegeben werden. Dies erfolgt üblicherweise über die Deklaration `noNamespaceSchemaLocation` wie im Beispiel gezeigt.
Gute Editoren unterstützen die Bearbeitung dann außerdem mit automatischer Vervollständigung. Weitere Informationen dazu finden Sie auch in den Einzeldokumenten [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Arbeiten-mit-Xml%E2%80%90Dateien)

#### Metadaten

Zur Kennzeichnung und Beschreibung der Datei, sollen eine ID und ein Label vergeben werden. Ersteres dient der internen Zuordnung, auch der 
Berichte. Letzteres wird bei der Beschriftung des Start-Schalters verwendet. Eine Beschriftung kann helfen verschiedene Versionen eines 
System-Check zu unterscheiden.

#### Netzwerkverbindung

Die Angaben in den Bereichen `UploadSpeed` und `DownloadSpeed` sind rein technischer Natur und sollten nur angepasst werden, 
wenn die Ergebnisse überwiegend unerwartet sind. Bitte fragen Sie die Spezifikation beim Entwickler-Team ab!

#### Unit

Wenn im Element `Config` ein Attribut `unit` gefunden wird, dann erfolgt nach dem Test der Verbindungsqualität die Anzeige einer Unit. 
Diese Befragungsseite bzw. Testaufgabe soll möglichst alle Element-Typen enthalten, die später auch im Test bzw. der Befragung benutzt werden. 
Es ist also z. B. hier unnötig, eine Audio-Datei einzubauen, wenn im Test keine Hörverstehensaufgabe vorkommt.

Es muss natürlich in den Arbeitsbeich auch eine Unit mit dieser ID hochgeladen werden. Der in der Unit-Definition genannte 
Player, muss dann auch im Arbeitsbereich zur Verfügung gestellt werden.

## Bericht speichern

Wenn im Element `Config` ein Attribut `savekey` gefunden wird, dann können die Ergebnisse des System-Checks abschließend mithilfe dieses Savekeys gespeichert werden. Die letzte Seite enthält dann einen Schalter `Bericht senden` und es wird der Savekey abgefragt.

## Ergebnisse herunterladen

Werden am Ende eines System-Checks die Ergebnisse gesendet (gespeichert), landen diese Ergebnisse in Form einer CSV-Datei in dem Arbeitsbereich in den die System-Check Xml-Definition geladen wurde. Die CSV-Datei ist dann im jeweiligen Arbeitsbereich unter dem Tab: System-Check Berichte zu finden und kann dort mittels der üblichen Browserfunktionalitäten heruntergeladen werden. Da eine CSV-Datei nicht sehr gut lesbar ist, kann diese Datei auch in eine XLSX-Datei gewandelt werden. Dies kann mit dem IQB Tool **Itc-Toolbox** erfolgen. Mehr dazu finden Sie [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/itc-Toolbox:-SysCheck).

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

# 2.8 Testleitungskonsole (TLK)

Soll ein Test für eine bestimmte Personengruppe (z. B. Klasse) gleichzeitig stattfinden, kann ein Monitor dafür eingerichtet werden. 
Die Testleitung kann dann für jede Testperson den Fortschritt beobachten, ggf. das Weiterblättern erzwingen, Personen ausschließen oder Testhefte sperren bzw. freigeben.

Hier finden Sie [Videos](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Videos:-Testleitungskonsole) zur Testleitungskonsole.


## Einrichten der Testleitungskonsole (TLK)

Die Testleitungskonsole wird mittels **Testtakers.xml** eingerichtet. Diese gehört neben der **Booklet.xml**, der **Unit.xml** und weiteren Ressourcen zu den Testdateien. Nachfolgend ist eine Beispielkonfiguration der **Testtakers.xml** zu sehen.

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

Zum Einrichten der Testleitungskonsole (TLK) wird ein entsprechender Login:`monitor-group` in der zu beobachtenden Gruppe angelegt. In diesem Fall befindet sich der TLK-Login in der Gruppe: Testgruppe_1. Daraus folgt:<br> Die TLK überwacht alle Testpersonen, die sich in dieser Testgruppe befinden. Der auf diese Weise angelegte TLK-Login in der **Testtakers.xml** muss anschließend in das **Testcenter** geladen werden. 

> Der oben gezeigte Code ist nur ein Bsp.! Es können weitere Gruppen, Testpersonen etc. angelegt werden und für jede dieser Gruppen kann ein eigener Testmonitor angelegt werden!

Weitere Informationen zur Konfiguration der **Testtakers.xml** finden Sie auch [hier](https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/Testtaker%E2%80%90Xml).

## Starten der Testleitungskonsole

Um die TLK zu starten, muss eine Neuanmeldung am **Testcenter** erfolgen. Anschließend sind die Zugangsdaten zu verwenden, die für den Login der Testleitungskonsole (`monitor-group`) festgelegt wurden. In diesem Fall muss zur Anmeldung der Name: *group-monitor_1* und das Passwort: *567* verwendet werden. 

Nach der Anmeldung kann die Gruppe, der die TLK zugeordnet wurde, ausgewählt werden.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Anmeldung.png)

Anschließend ist die Oberfläche der TLK zu sehen:

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Ansicht1.png)

### Ansicht der TLK

Schauen wir uns an was in der TLK zu sehen ist:

* die beobachtete Gruppe -> Dieser Name wurde über das Group Label gesetzt. In diesem Fall Gruppe 1.
* Benutzername der Testleitungskonsole -> Dieser Name wurde über den Login Namen der `monitor-group` gesetzt.
* die Testpersonen -> Diese Namen wurden über die Login Namen innerhalb der zu überwachenden Gruppe gesetzt.

Zu Erklärung weiterer Symbole innerhalb der Testleitungskonsole muss ein Einblick  in die zugehörige **Booklet.xml** genommen werden. 

> Es wird nur der Code innerhalb der **Booklet.xml** aufgezeigt der für diese Beschreibung notwendig ist!

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

Die im Bild rot markierten Symbole der *Testperson_a* entsprechen einer einzelnen Unit. In diesem Fall der Start- und Endunit.

Das gelb markierte Symbol entspricht dem Testlet: Examples. Die enthaltende Zahl in der gelben Markierung entspricht der Unit innerhalb des Testlets. In diesem Fall gibt es nur die Unit 1.


## Arbeiten mit der Testleitungskonsole

Nachdem die Konsole gestartet wurde, können die Zugangsdaten für die Testpersonen vergeben werden. Nach Anmeldung ist der Bearbeitungsstand des Tests durch die Testperson ersichtlich. Über das kleine Zahnradsymbol oben rechts kann die Ansicht individuell angepasst werden. Es können weitere Informationen ein- oder ausgeblendet werden. 

> **Ablauf, Struktur und Kontrolle eines Tests können von den Verantwortlichen individuell gestaltet werden.<br> 
An dieser Stelle können nur Empfehlungen auf Erfahrungsgrundlage gegeben werden! Die Durchführung sollte genauestens geplant und überdacht sein, um einen reibungslosen Ablauf und repräsentative Ergebnisse zu gewährleisten.**

In diesem Bsp. hat sich nur  *Testperson_c* angemeldet und befindet sich in der Unit 1 innerhalb des *Testlets*.<br>
*Testperson_a* hat den Test schon abgeschlossen. Da der Modus: `run-hot-return` verwendet wurde, ist der Test nach Abschluss gesperrt. Dies ist auch zu sehen an dem Schlosssymbol.
Durch Markierung einer Testperson kann der Ablauf für diese Testperson mithilfe der Steuersymbole auf der linken Seite gesteuert werden.

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Ansicht2.png)

> **Werden mehrere Testhefte mit ähnlicher Struktur verwendet, ist es eventuell nicht möglich alle Testpersonen gleichzeitig zu steuern. In diesem Fall müssen die zu steuernden Testpersonen einzeln markiert (Haken setzen vor der Testperson) und dann die Steuerbefehle (Pause, springe zu etc.) abgesetzt werden.**

Nachfolgend sind die möglichen Symbole für den Teststatus zu sehen:

![iqb online assessment applications with relations: testcenter](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TC_FE_Testleitkonsole_Ansicht3.png)

Weitere Informationen zum Teststatus finden Sie auch [hier](https://iqb-berlin.github.io/testcenter-frontend/super-states).

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