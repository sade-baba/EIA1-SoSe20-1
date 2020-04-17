## **03 _#_** Einstieg in CSS


### Einführung
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/01_Einstieg_in_CSS.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/01_Einstieg_in_CSS.mp4">Zum Video</a>
</video>

CSS (Abkürzung für Cascading Style Sheets) ist eine Gestaltungssprache, mit der Webanwendungen visuell angepasst werden können. CSS-Anweisungen können auf drei Arten eingebunden werden: <b>inline</b>, was aufgrund der schwierigen Pflege und Unübersichtlichkeit nicht zu empfehlen ist, als <b>Style-Tag im Head</b>, was aufgrund der komplizierten Pflege ebenfalls nur bedingt empfohlen wird, oder als <b>externes CSS-Stylesheet</b>, was im Head des HTML-Dokuments verlinkt ist.<br>
Eine CSS-Anweisung besteht immer aus einem Selektor und der Deklaration, die aus Eigenschaft und Wert besteht.

<b>Links im Video</b><br>
Übersicht von sämtlichen aktuellen CSS-Anweisungen mit Beispielen:<br>
<a href="https://www.w3schools.com/css/">https://www.w3schools.com/css/</a>

### Eigenschaften
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/02_CSS_Eigenschaften.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/02_CSS_Eigenschaften.mp4">Zum Video</a>
</video>

Die aktuellen Möglichkeiten der visuellen Gestaltung mit CSS sind scheinbar endlos. In diesem Video werden die gängigsten Eigenschaften sowie ein effizienter Workflow mit Visual Studio Code vorgestellt und die Funktionen der verschiedenen CSS-Anweisungen erklärt.<br>
Eigenschaften stehen immer in Abhängigkeit zu dem entsprechenden Element, sodass nicht alle Eigenschaften bei allen Elementen sinnvoll sind oder schlicht keine Auswirkung haben.

### Selektoren
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/03_CSS_Selektoren.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/03_CSS_Selektoren.mp4">Zum Video</a>
</video>

Um CSS-Anweisungen für bestimmte Elemente in einem HTML-Dokument zu schreiben, kann man mithilfe von Selektoren auf ein oder mehrere Elemente zugreifen.<br>
Es gibt verschiedene Arten von Selektoren: die drei Haupt-Selektoren sind <b>Element-Selektoren</b> (gebildet aus dem Tag-Namen), <b>ID-Selektoren</b> (wirken sich auf Elemente aus, die mit einer eindeutigen ID versehen wurden) und <b>Klassen-Selektoren</b> (ermöglichen die Auswahl mehrerer HTML-Elemente, auf die mit der Formatierung zugegriffen werden soll).

### Kaskadierung und Vererbung
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/04_Kaskadierung_und_Vererbung.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/04_Kaskadierung_und_Vererbung.mp4">Zum Video</a>
</video>

Das Grundprinzip der Kaskadierung bewirkt eine Reihen- oder Rangfolge, in der Eigenschaften in CSS vererbt werden, denn die einzelnen CSS-Selektoren werden unterschiedlich schwer gewichtet. Es ist hilfreich, diese Regeln zu kennen, um zu verstehen, wann welche Anweisungen umgesetzt werden (bzw. warum nicht) und welche Anweisungen andere überschreiben.<br>
Definierte Eigenschaften werden an die (semantisch untergeordneten) Kinderelemente des selektierten Elements vererbt. Werden jedoch die Eigenschaften für die untergeordneten Elemente neu definiert, überschreiben diese die vererbten Eigenschaften.

### Box Model und Masseinheiten
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/05_CSS_Box_Model_und_Masseinheiten.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/05_CSS_Box_Model_und_Masseinheiten.mp4">Zum Video</a>
</video>

Das CSS-Box-Model beschreibt, dass alle Elemente im Browser auf Basis einer Box beschrieben werden können, die aus einer bestimmten Größe (Höhe x Breite), einem Innenabstand (<b>padding</b>), einem Rahmen (<b>border</b>) und einem Außenabstand (<b>margin</b>) bestehen.<br>
Der Browser arbeitet mit verschiedenen Maßeinheiten, für den Anfang genügt das Pixelmaß (<b>px</b>). Ansonsten gibt es beispielsweise noch Angaben in <b>pt</b> (statisch, Anwendung im Druck), <b>em</b> und <b>rem</b> (relative Angabe) oder <b>Prozent</b>.

### Take Aways
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/06_Take_Aways.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/06_Take_Aways.mp4">Zum Video</a>
</video>

* CSS definiert die Darstellung von Inhalten im Browser und kann auf drei Wegen eingebunden werden: Inline, im Head oder als externes Stylesheet.
* CSS-Anweisungen bestehen aus Selektor(-pfad/-kette) und Deklaration und es gibt viele verschiedene CSS-Eigenschaften zur Manipulation der Darstellung im Browser.
* Es gibt drei Haupt-Selektoren, welche eine Art Rangfolge besitzen.
* Eigenschaften werden von Eltern- an Kinderelemente vererbt, können aber auch überschrieben werden.
* Das CSS-Box-Model beschreibt verschiedene Abstandsmaße für Elemente.

---

## Aufgabe

tba