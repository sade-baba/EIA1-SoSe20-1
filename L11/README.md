## **11 _#_** Debugging

### Debugging
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_01_Debugging.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_01_Debugging.mp4">Zum Video</a>
</video>

Debugging beschreibt das Herausfinden und Beheben von Fehlern im Code - wir entfernen quasi digitale „Wanzen“ (Bugs) aus der Anwendung.

**Debugging Strategien**
* **Sorgfältige Konzeption:** Um von vornherein Fehler zu vermindern, ist die Entwicklung eines klaren Konzeptes hilfreich.
* **Konsolenausgaben:** An allen wichtigen Punkten im Code wird eine Konsolenausgabe generiert, um direkt zu überprüfen, ob an dieser Stelle überhaupt etwas passiert ist — und gegebenenfalls sogar, was passiert ist. Tipp: Bei vielen Konsolenausgaben kann man auch mit Gruppen arbeiten. Über den Befehl `console.time();` am Anfang und `console.timeEnd();` am Ende des Skriptes kann man die Zeit messen, die für die Ausführung des Codes benötigt wird.
* **Debugger-Tool im Browser:** In den Development-Tools im Browser kann man über das setzen von Breakpoints gezielt den Code untersuchen. Breakpoints unterbrechen die Ausführung des Codes an der Stelle, an der der Breakpoint gesetzt wurde, sodass man genau anschauen kann, was an dieser Stelle passiert. Schritt für Schritt kann man so den Code weiter ausführen und Fehler nachverfolgen.
* **Visual Studio Code:** auch hier gibt es einen Code Debugger, mit dem man Breakpoints setzen kann.


### Laufzeitumgebungen
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_02_Laufzeitumgebungen.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_02_Laufzeitumgebungen.mp4">Zum Video</a>
</video>

Laufzeitumgebungen sind Anwendungskontexte, die das Ausführen von Apps, Websites, oder ähnlichem mit entsprechender Funktion und Darstellung ermöglichen. Dazu gehören zum Beispiel Betriebssysteme oder Browser: also Rahmen, in denen Softwarekomponenten laufen. <br>
Laufzeitumgebungen könne auch verschachtelt sein, wie zum Beispiel ein Betriebssystem, in dem ein Browser läuft, in welchem wiederum eine Website läuft.

**Browser**

Die Browser sind die Laufzeitumgebungen, die für uns am wichtigsten sind: da es viele unterschiedliche Browser gibt, ist es wichtig, dass unsere Anwendungen fehlerfrei in allen funktionieren.


### Emulation und Virtualisierung

<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_03_Emulation_und_Virtualisierung.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_03_Emulation_und_Virtualisierung.mp4">Zum Video</a>
</video>

**Emulation**

Um Anwendungen zu testen, lässt man sie im professionellen Bereich auf vielen verschiedenen Endgeräten durchlaufen — da wir diese Möglichkeiten Zuhause meist nicht haben, lassen sich auch über die **browsereigene Emulation** verschiedene Endgeräte simulieren. 

Mithilfe des **Throttling** kann auch die Internetgeschwindigkeit verringert werden, um zu überprüfen, ob Anwendungen auch bei langsamer Ladezeit noch solide funktionieren.

**Native Emulationen** sind eine weitere Möglichkeit, um Smartphones oder andere Ausgabegeräte zu simulieren, was dann schon sehr nah an die wirklichen Geräte kommt.

**Virtualisierung**

Auch Betriebssysteme können virtuell nachgebildet werden, sodass geprüft werden kann, ob Anwendungen auch unter anderen Betriebssystemen funktionieren.


### Take Aways
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_04_Take_Aways.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L11/L11_04_Take_Aways.mp4">Zum Video</a>
</video>

* Debugging ist die Identifizierung von Fehlern. Zur Vermeidung dieser sollte von vornherein ein solides Konzept entwickelt werden!
* In der Webentwicklung gibt es dann verschiedene Fehler-Untersuchungs-Strategien, wie das Arbeiten mit Konsolenausgaben oder das Setzen von Breakpoints.
* Web-Anwendungen sollten auf verschiedenen Endgeräten und Browsern getestet werden, da diese je nach Zielgruppen sehr unterschiedlich sind. Dies kann über Emulieren und Virtualisieren auf Softwarebene geschehen.


## **A _---_** Aufgabe #11
### Follow Up zu Aufgabe #10

Siehe Aufgabe #10. Jetzt sollten Sie die beiden letzten Punkte der ToDo-App Aufgabe bearbeiten.

- Der Zähler soll erweitert werden. Aktuell steht hier nur die Gesamtzahl der ToDos. Erweitern Sie die Anzeige, um die Anzahl der offenen und geschlossenen ToDos anzuzeigen: 6 in total, 4 open, 2 done

- Integrieren Sie die Bibiliothek Artyom. Durch Spracheingabe soll es möglich sein, ein ToDo zu erstellen, bspw. "erstelle Aufgabe 'Einkaufen gehen'"

## Abgabe bis 12. Juli um 18:00 Uhr
__Nach Abgabe und Feedback sind Korrekturmöglichkeiten bis 14. Juli, 18:00 Uhr möglich__


---


## **?! _<small>Q&A</small>_** Fragen und Antworten
(die Publikation der Zusammenfassung erfolgt nach dem Q&A Termin)
