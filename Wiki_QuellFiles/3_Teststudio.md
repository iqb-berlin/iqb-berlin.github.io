# 3 Teststudio

```yaml
Achtung: Noch nicht aktualisiert auf 1.0
Dokumentstatus: Review (THuste)
Stand: 02.06.2021
todo:
```
Das IQB-Teststudio ist eine Web-Anwendung für den Entwurf von Kompetenztests oder Befragungen. Nach der Installation auf einem Webserver wählt man diesen Server über seine Adresse an, d. h. man schreibt dessen Internet-Adresse in die Adresszeile eines Internet-Browsers. Dadurch werden die Programmierungen geladen und man sieht ein Formular zum Anmelden.

Eine grobe Einführung in das Teststudio geben auch die nachfolgenden Verlinkungen.
Das IQB bietet folgende Video-Präsentationen bzgl. des Testcenters an:

 * [IQB-Teststudio Intro](https://box.hu-berlin.de/f/e29f3e8d8c35480f8531/)
 * [Schulung Teststudio Editor Dan2](https://box.hu-berlin.de/f/edc2409b79954dc3b3a1/)    

Des Weiteren besteht das folgende Forum: [Teststudio-Forum](https://github.com/iqb-berlin/teststudio-lite-frontend/discussions)<br>
Hier finden Sie häufig gestellte Fragen und Antworten sowie Berichte über Einsätze des IQB-Teststudios.

**Installation**

Das IQB hat alle Programmierungen unter einer Open Source veröffentlicht und erleichtert die Installation durch ein sog. Docker-Setup. Für die Installation muss man einen Server bereitstellen (Linux oder Windows), und dieser Server muss dann über eine Internet-Adresse erreichbar sein. Die Installation sollte erfahrenes IT-Fachpersonal durchführen. Die Dokumentation hierzu setzt Wissen vor allem zur Virtualisierungssoftware Docker voraus. Es ist weiterhin Wissen zu Datensicherheit nötig, denn sobald ein Server öffentlich verfügbar ist, müssen Maßnahmen gegen Angriffe durch Schadsoftware ergriffen werden. Das IQB ist bemüht, die Installationspakete gut abzusichern, übernimmt aber im Schadensfall keine Verantwortung.

**Verwaltung der Tests**

Nach der Installation ist zunächst ein Standard-Konto für die Verwaltung von Tests angelegt. Mit diesem Zugang können dann entsprechende Arbeitsbereiche und Personenzugriffe angelegt werden. Meldet sich eine entsprechend freigegebene Person am Teststudio an, kann diese in ihrem Arbeitsbereich erste Aufgabenentwürfe starten. Bereits bestehende Aufgaben können auch in diesen Bereich importiert werden.

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Stand-der-Entwicklung%3A-Teststudio‐Lite">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++home++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<div align='center'>
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Button_Home_final.png">
</a>
</div>

---

# 3.1 Stand der Entwicklung: Teststudio-Lite

```yaml
Dokumentstatus: Entwurf
Stand: 6.4.2021
```

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Portal-zur-Verwaltung">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3-Teststudio">
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

# 3.2 Portal zur Verwaltung

````yaml
Dokumentstatus: Entwurf T.Huste
Stand: 03.06.2021
```
Um mehreren für die Aufgabenentwicklung verantwortlichen Personen die Möglichkeit zu bieten an Aufgabenentwürfen zu arbeiten, ist eine Aufteilung bzw. Organisation sinnvoll. Hierfür ist ein Verwaltungsportal eingerichtet. In diesem sind die Units verschiedener Entwicklerteams in Arbeitsbereiche aufgeteilt. Die Arbeitsbereich können im Sinne einer besseren Übersicht zusätzlich in Gruppen eingeteilt werden. Zugriffsrechte regeln den Zugriff auf diese Bereiche. Nach Eingabe der Adresse des Teststudios in einem Internetbrowser und Anmeldung mit den persönlichen Zugangsdaten, gelangt man zum Portal der Verwaltung.  

## Arbeitsbereiche

Nach der Anmeldung präsentiert das System eine Liste aller Gruppen und der darin enthaltenen Arbeitsbereiche für die angemeldete Person (Zugriffsrechte). Mit einem Klick auf den jeweiligen Arbeitsbereich wird dieser geöffnet. Zur Liste der Arbeitsbereiche kehrt man zurück, indem man auf das IQB-Logo links oben in der Ecke klickt.

In den Arbeitsbereichen können Units angelegt, gelöscht oder bestehende Units bearbeitet werden. Die Benennung der Bereiche richtet sich günstigerweise nach dem Zweck, also z. B. "Demo Deutsch Sek1" oder "Review Abi" oder "VERA Englisch".

## Unit Verwaltung

Wurde ein Arbeitsbereich geöffnet, sind alle in diesem Bereich befindlichen Units auf der linken Seite des Portals zu sehen.
Nachdem eine Unit markiert wurde, kann diese über die unten angeordneten Funktionschaltflächen gelöscht, exportiert, verschoben oder deren Eigenschaften verändert werden. Das kleine Pluszeichen legt eine neue Unit an. Oberhalb der Unit Auflistung im linken Bereich des Portals befinden sich zwei weitere Funktionsschaltflächen. Diese ermöglichen das Speichern bzw. Verwerfen von Änderungen an einer gewählten Unit.

![iqb online assessment applications with relations: Teststudio](https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/TS_FE_Unit_Verwaltung.png)

### Verschieben

Es ist möglich Units zu verschieben. Verschoben kann dabei nur in andere für die angemeldete Person freigegebene Arbeitsbereiche.

### Kopieren

Markierte Units können kopiert werden. Alle Inhalte dieser Unit werden dabei in eine neu zu benennende Unit kopiert.

### Importieren

Der Import von bestehenden Units ist ebenso möglich. Besteht die zu importierende Unit aus einer xml-/ und einer voud-Datei sollten diese zuvor in einem Zip-Format gepackt werden. Anschließend kann beim Import die Zip-Datei ausgewählt und geladen werden.

> **Voud-Dateien können nicht einzeln importiert werden. Sie müssen immer zusammen mit der zugehörigen Xml-Datei geladen werden. Daher sollten diese Dateien zuvor immer in einem Zip-Format verpackt und dann importiert werden!.**

---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Allgemeine-Arbeitsweise">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.1-Stand-der-Entwicklung%3A-Teststudio‐Lite">
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


# 3.3 Allgemeine Arbeitsweise





---

<!--++++++++++++++++++++++++++++++++++++++++++++++++++++++++forward+++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.4-Wahl-des-Editors-(Verona)">
<img src="https://github.com/iqb-berlin/iqb-berlin.github.io/blob/master/assets/Fw_Button_final.png" align="right">
</a>
</div>
<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.2-Portal-zur-Verwaltung">
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

# 3.4 Wahl des Editors (Verona)

```yaml
Dokumentstatus: Entwurf
Stand: 6.4.2021
```

Einführungsvideo:
 * [IQB-Verona Editor Dan2](https://box.hu-berlin.de/f/edc2409b79954dc3b3a1/)

---

<!--+++++++++++++++++++++++++++++++++++++++++++++++++++++++++backward++++++++++++++++++++++++++++++++++++++++++++++++++++++++-->
<a href="https://github.com/iqb-berlin/iqb-berlin.github.io/wiki/3.3-Allgemeine-Arbeitsweise">
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

