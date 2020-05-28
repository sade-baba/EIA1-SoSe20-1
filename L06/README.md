## **06 _#_** Programmiergrundlagen I

### Einführung
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_01_Einfuehrung.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_01_Einfuehrung.mp4">Zum Video</a>
</video>

### Funktionen
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_02_Funktionen.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_02_Funktionen.mp4">Zum Video</a>
</video>

Um zu verhindern, dass alle Skriptanweisungen automatisch nacheinander abgearbeitet werden, benutzen wir Funktionen. Funktionen sind Anweisungsblöcke, die bestimmte Aufgaben zu einem von uns festgelegten Zeitpunkt ausgeführt werden können (z.B. wenn der Benutzer auf einen Button klickt). Um die Funktion auszuführen, muss sie innerhalb im Skript aufgerufen werden, dabei kann sie immer wieder verwendet werden.

Eine Funktion wird folgendermaßen deklariert:
* `function myFunction() { … }`
* `function` ist das Keyword, das anzeigt, dass hier eine Funktion folgt
* `myFunction` repräsentiert hier den Funktionsnamen, der selbst gewählt werden kann
* in die Funktionsklammern `()` können optional Argumente (= Werte für den Funktionsaufruf) mitgegeben werden
* zwischen die Anweisungsklammern `{}` kommt die eigentliche Anweisung

**Gültigkeitsbereich von Variablen**
* Variablen, die außerhalb einer Funktion (= global) deklariert werden, sind überall verfügbar
* Variablen, die innerhalb einer Funktion (= lokal) deklariert werden, sind nur innerhalb dieser Funktion verfügbar 


### Events
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_03_Events.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_03_Events.mp4">Zum Video</a>
</video>

Um Funktionen zu einem bestimmten Zeitpunkt (z.B. bei einer Nutzerinteraktion) aufzurufen, verwenden wir **Events**. Um ein Event aufzurufen, verwenden wir einen **Event-Listener**, der zum Beispiel so aussehen könnte: 
`document.querySelector("h1").addEventlistener("click", myFunction)`


### Ladereihenfolge un Parsen des Skripts
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_04_Ladereihenfolge.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_04_Ladereihenfolge.mp4">Zum Video</a>
</video>

Da der Browser Dokumente von oben nach unten parst, kommt er zuerst beim Skript an, bevor er den DOM liest. Wenn man also Event-Listener an bestimmte Elemente gehängt hat, kennt der Browser diese Elemente zu dem Zeitpunkt, zu dem er das Skript liest, noch gar nicht — so können Fehler beim Ausführen des Events entstehen.

Um das Skript erst auszuführen, wenn der DOM schon geladen wurde, verwenden wir am besten einen **Window-Eventlistener**, der die Funktionen erst ausführt, wenn der DOM vollständig geladen ist.


### DOM Manipulation
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_05_DOM_Manipulation.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_05_DOM_Manipulation.mp4">Zum Video</a>
</video>

**DOM-Manipulation** bezeichnet das manipulieren von Inhalten (inhaltlich, visuell oder funktional) zur Laufzeit des Browsers.
Übliche Methoden dazu sind unter anderem:
* `innerHTML`: Damit kann ein Element (zum Beispiel ein leeres div-Element) selektiert und dort ein neuer Wert hineingeschrieben werden. Dazu schreiben wir eine Zeichenkette mit ganz normalem HTML-Code. 
* `setAttribute`: um z.B. den Style zu verändern, oder 
* `createElement`: zur Erschaffung eines ganz neuen Elements, welches dann bearbeitet und dem DOM übergeben werden kann.


### Take Aways
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_06_Take_Aways.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L06/L06_06_Take_Aways.mp4">Zum Video</a>
</video>

* **Funktionen** sind Anweisungsblöcke, die (ggf. mit Argumenten) gezielt aufgerufen werden können.
* **Events** sind Ereignisse, die Funktionen auslösen können.
* Der DOM kann durch verschiedene Methoden über das Skript manipuliert werden.




## **A _---_** Aufgabe #06
### Interaktive Infografik II

Als Grundlage für Aufgabe 6 muss Aufgabe 5 gelöst worden sein.
Mit Aufgabe 5 werden Werte als Konsolenausgbe generiert. Jetzt sollen die generierten Daten in das HTML Dokument überführt und angezeigt werden.

Folgende Anforderungen an die Aufgabe:

1. Die Infografik bildet die CO2 Emission ab.

2. Bei Klick auf eine Region soll sich der Titel ändern ("...Emission in Asia / Europe / North America") und die Daten entsprechend anpassen. Kapseln Sie also Ihre Skript-Anweisungen in Funktionen und nutzten Sie Events, um die Bild-Elemente in HTML klickbar zu machen. Bei Klick auf eine Region sollen die entsprechenden Emissionswerte dieser Region angezeigt werden. Der entsprechende Code-Block muss also aufgerufen werden, die generierten Inhalte werden jetzt nicht mehr als Konsolenausgabe generiert, sondern an der entsprechende Stellen im HTML angezeigt.

3. Neben der Darstellung der Werte als Text soll darüberhinaus das Balkendiagramm angepasst werden. Versuchen Sie das HTML und CSS Konstrukt in der Vorlage emission.html zu verstehen und ergänzen Sie, dass sich die Höhe des Balken dynamisch an die entsprechende Region anpasst.

4. Als Startpaket finden Sie in der HTML-Datei "emission.html" eine Grundstruktur der Darstellung mit statischen Inhalten. Der Fokus der Aufgabe bleibt also wieder in der Skript-Welt, der HTML- und CSS-Part ist rudimentär schon vorbereitet (natürlich müssen Sie hier aber auch einige Ergänzungen vornehmen).

5. Nicht Teil der Aufgabe, wird aber honoriert: passen Sie das Design der Infografik an eine eigene Darstellung an (bspw. Balkendiagramm oder die Wertedarstellung sind in der Vorlage noch sehr lieblos).


Im Projektordner finden Sie noch einmal das HTML + CSS Grundgerüst (wie schon aus vorheriger Aufgabe):

[Grundgerüst HTML und CSS](https://github.com/gabriel-rausch/EIA1-SoSe20/tree/master/L06/task_material)

Bearbeitung wie gehabt: als Unterordner in Ihrem Git Repository (/Aufgabe_6); das fertige Arbeitspaket wieder auf Github pushen und auf Ihrem Kursseiten-Steckbrief verlinken.

## Abgabe bis Sonntag, 7. Juni um 18:00 Uhr
__Nach Abgabe und Feedback sind Korrekturmöglichkeiten bis Dienstag, 9. Juni, 18:00 Uhr möglich__


---


## **?! _<small>Q&A</small>_** Fragen und Antworten
(die Publikation der Zusammenfassung erfolgt nach dem Q&A Termin)


### Erste Frage?
Lorem labore cillum mollit pariatur reprehenderit dolor laboris reprehenderit dolor sit officia ea non. Lorem reprehenderit exercitation labore eiusmod aute do nostrud officia aute proident sunt. Labore non tempor aliqua voluptate. Exercitation culpa officia ut aliqua nostrud laborum irure est. Minim eu sunt culpa adipisicing laborum consectetur aliqua quis.

### Zweite Frage?
Mollit aliquip veniam sit eiusmod tempor anim ipsum tempor. Aliqua sunt voluptate ea dolor. Nulla est mollit consectetur cupidatat ut cillum ipsum minim. Est ex et nulla laborum fugiat dolore. Aliquip laboris sint exercitation commodo dolor sint mollit qui sunt ipsum fugiat occaecat id enim.
