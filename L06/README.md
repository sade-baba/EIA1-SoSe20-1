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
(die Zusammenfassung der Q&A-Session wurden von Teilnehmern verfasst und ggf. angepasst und ergänzt)

Von [saravo306](https://github.com/saravo306)


**Funktionen **= Sammlung von Anweisungen bzw. Anweisungsblöcke, die bestimmte Aufgaben zu einem von uns festgelegten Zeitpunkt ausgeführt werden 

**DOM Manipulation **=bezeichnet das Manipulieren von Inhalten (inhaltlich, visuell oder funktional) zur Laufzeit des Browsers, wichtig um Inhalte interaktiv zu gestalten

**Events **= wird verwendet um Funktionen zu einem bestimmten Zeitpunkt (z.B. bei einer Nutzerinteraktion) aufzurufen, Um ein Event aufzurufen, verwenden wir einen Event-Listener

„Ein Ereignis kann durch Benutzerinteraktionen ausgelöst werden; z.B. das Klicken einer Maustaste oder Eingaben der Tastatur."

**Wie kann ein Event Listener eine Funktion aufrufen? Kann er nur eine oder mehrere gleichzeitig aufrufen?**

- technisch geht beides, also entweder nur eine Funktion oder mehrere innerhalb der anonymen Funktion

- wenn man den Code gut lesbar machen möchte, dann wäre es sinnvoll, wenn man die Funktionsaufrufe wie eine Kaskade voneinander abhängig macht (werden wir in anderen Lektionen noch vertiefen)

**Thema Anführungsstriche: mit nur einem einem oder mit zwei Anführungsstrichen arbeiten?**

- Bei TypeScript als auch bei JavaScript ist es egal ob man mit einfachen oder doppelten Anführungsstrichen arbeitet

- nur „Codestyle"

- allerdings mit Linter (=Codequalitätswerkzeug) achtet darauf, dass man immer doppelte Anführungszeichen nutzt (werden wir erst in Lektion 8 vertiefen)

- man kann beides machen, aber vorsichtig bei Verschachtelungen von Textelementen

    - Bsp: console.log ("Hallo Welt");

    - Nur „Welt" in Anführungsstrichen   console.log ("Hallo 'Welt' ");

**oder** escapen um doppelte Anführungsstriche zu erhalten  console.log ("Hallo \"Welt\"");

**Funktionsklammern**

- müssen immer vorhanden sein, unabhängig davon, ob darin Parameter stehen oder nicht

- Bsp. function myFunction**() **{

}

- Auch wenn man die Funktion später nochmal aufrufen möchte, ist die runde Klammer essentiell

**Wie kann man Elemente manipulieren?**

- eine Methode ist das Arbeiten mit .innerHTML

- die andere Methode mit .setAttribute

    - diese erwartet zwei Parameter  einen qualified Name + einen value

    - Bsp. document.querySelector ('a').setAttribute ('blabla' , '123');

§  Wie heißt das Attribut? Also was wird erstellt?   „blabla" mit dem Wert „123 „

**Das Parsen des DOM's und des Skripts**

- am besten in der TypeScript Datei direkt am Anfang mit...

window.addEventListener ('load', funktion() {

.....

}

...arbeiten, damit auch alle Skriptanweisungen berücksichtigt werden

**Welche Werte sollen in das Balkendiagramm?**

- Entweder die relativen oder absoluten Werte, aber in Prozentangabe

**Was sind anonyme Funktionen?**

- Anonyme Funktionen, sind im Vergleich zu regulären Funktionen, Funktionen ohne Funktionsname 

    - Schreibweise: function() {

}

- Reguläre Funktion

    - Schreibweise: function meinName() {

}

    - „meinName" steht dabei stellvertretend für irgendein Funktionsname


### Anmerkung zu Video "Funktionen"

Von [lemon-pie](https://github.com/lemon-pie)

- in Zeile 1+2 werden für die Variablen fuel... und kilo..., die mit var gekennzeichnet werden, die Werte 7 und 30 festgelegt
-  Sie können sich das vorstellen wie damals in Mathe, dass man z.B. gesagt hatte X sei eine Zahl, hier also in Zeile 1 z.B. 7 (Also x=7, nur sagt man hier nicht x sondern hat dem einen Namen gegeben, nämlich fuel...)
-  schlussendlich steht da also nur z.B. x=7 und y=30
- die Bezeichnung ist dabei etwas worauf man sich später auch beziehen kann, sodass man statt den Wert die Bezeichnung nennt
- in Zeile 3 wird dann eine neue Variable definiert, nämich emission...
- da können Sie auch sehen was möglich ist, und zwar wurde hier eine Rechnung eingegeben, die sich auf die Variablen, also quasi x und y von zuvor, bezieht und das Ergebnis bzw. die Summe dieser Rechnung ist dann der Wert einer neuen Variablen
- der Browser ließt hier also, die Variable emission... wird berechnet aus 7 * 30 * 0.238 (hier auch wieder beachten, kein Komma sondern Punkt zu wählen)
-  das ergibt also * öffnet Rechner * aha, 49,98. Das bedeutet die Variable emission...=49,98 quasi sowas wie z=49,98
- und in der nächsten Zeile, oder eigentlich die übernächste Zeile weil man gerne für die Übersicht leere Zeile einfügt, sehen Sie was auch möglich ist... Man kann auch sagen, dass eine Variable ein vollständiger Satz ist und sich aus Text und Zahlen zusammensetzen kann
- die 4. Variable, mit dem Namen result, besteht also aus dem Text "co2..." und dem Ergebnis der Rechnung von emission..., also 49,98 und das wird man in der Konsole dann schön hintereinander, eben wie man es hier vorgegeben hat, lesen können
- dazu muss man natürlich auch erst noch sagen, dass etwas und was im Browser bzw. der console angezeigt werden soll
- man schreibt also console.... und sagt dem Browser, zeige mir nur dass an, was du für result berechnet hast bzw. die Summe von der Berechnung und dem Text
- wenn man die leeren Zeilen weglässt, hat man also 5 Zeilen und man hat in den vier Zeilen darüber nur dem Browser gesagt, was er schlussendlich machen soll, wenn er mir result anzeigen soll
- zuerst also Variablen definiert, sich auf die dann in der nächsten Zeile bezogen indem man sie in eine Rechnung einbaut, das Ergebnis davon wieder als eine neue Variable definiert auf die man sich dann in Zeile 4 bezieht und wieder eine neue Variable festlegt, die diesesmal aus einer Zahl UND einem Text besteht und hat sich das Ergebnis dann mit console hier * öffnet console im Browser * anzeigen lassen
- was Sie hier sehen ist wiederum auch die ausführliche Variante, weil Sie alles gestückelt und einzelnd definiert haben... Wenn Sie das nicht mögen können Sie sich auch Zeilen sparen, indem Sie z.B. die Variable result nicht definieren und einfach das, was bei dieser Variable nach dem = steht, also "co2... und emission..., direkt in die console schreiben
- das würde für diese Aufgabe auch ausreichen aber später kann es vorteilhafter sein, wenn das so zerstückelt wird, weil (hier ein Beispiel aus Ihrer Erfahrung nennen) aber das werden Sie wahrscheinlich später auch selbst bemerken, was Sie wann sinnvoll finden und entsprechend nutzen werden
- abschließend sehen Sie hier also schlussendlich, wenn man jetzt in Zeile 1 und 2 nur den Wert von 7 und 30 austauschen würde, also z.B. ähm 90 uuund 400, würde der Browser * öffnet console im Browser * die ganzen Zeilen nochmal neu durchgehen und berechnen, sodass, wie Sie hier lesen können *zeigt auf Zeile in console* jetzt bei gleicher Vorgehensweise etwas Anderes stehen würde.