## **03 _#_** Einstieg in CSS


### Einführung
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/01_Einstieg_in_CSS.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/01_Einstieg_in_CSS.mp4">Zum Video</a>
</video>

CSS (steht für Cascading Style Sheets) ist eine browser-basierte Gestaltungssprache, mit der Webanwendungen visuell angepasst werden können. CSS-Anweisungen können auf drei Arten eingebunden werden: 
* **Inline**: nicht zu empfehlen, da Redundanzen in der Regeldefinition mehrerer Elemente entsteht und ab einer gewissen Deklarationsmenge die Eigenschafts-Werte-Paare nicht mehr pflegbar sein. Zudem ist eine klare Trennung zwischen Inhalt und Gestlatung nicht mehr möglich.
* **Style-Tag im Head**: schafft eine Trennung zwischen Inhalt und Gestaltung, verursacht aber auch eine Redundanz über mehrere HTML-Seiten. 
* **externes CSS-Stylesheet**: im Head des HTML-Dokuments verlinkt ist. Schafft eine klare Trennung zwischen Inhalt und Gestaltung, kann in beliebig vielen HTML-Seiten genutzt und an einer zentralen Stelle administiert werden.

Eine CSS-Anweisung besteht immer aus einem Selektor und der Deklaration, die aus Eigenschaft und Wert besteht.

**Links im Video**

Übersicht von sämtlichen aktuellen CSS-Anweisungen mit Beispielen:

<a href="https://www.w3schools.com/css/">https://www.w3schools.com/css/</a>

### Eigenschaften
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/02_CSS_Eigenschaften.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/02_CSS_Eigenschaften.mp4">Zum Video</a>
</video>

Die aktuellen Möglichkeiten der visuellen Gestaltung mit CSS sind scheinbar endlos. In diesem Video werden die gängigsten Eigenschaften sowie ein effizienter Workflow mit Visual Studio Code vorgestellt und die Funktionen der verschiedenen CSS-Anweisungen erklärt.

Eigenschaften stehen immer in Abhängigkeit zu dem entsprechenden Element, sodass nicht alle Eigenschaften bei allen Elementen sinnvoll sind oder schlicht keine Auswirkung haben.


### Selektoren
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/03_CSS_Selektoren.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/03_CSS_Selektoren.mp4">Zum Video</a>
</video>

Um CSS-Anweisungen an bestimmte Elemente eines HTML-Dokument zu adressieren, kann man mithilfe von Selektoren auf ein oder mehrere Elemente zugreifen.

Es gibt verschiedene Arten von Selektoren: die drei Haupt-Selektoren sind **Element-Selektoren** (gebildet aus dem Tag-Namen), **ID-Selektoren** (wirken sich auf Elemente aus, die mit einer eindeutigen ID versehen wurden) und **Klassen-Selektoren** (ermöglichen die Auswahl mehrerer HTML-Elemente, auf die mit der Formatierung zugegriffen werden soll).

Kleine Anmerkung: auf einer Folie im Video hat sich ein Fehler eingeschlichen (8. Minute): Klassenselektoren werden natürlich mit einem "." eingeleitet.

### Kaskadierung und Vererbung
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/04_Kaskadierung_und_Vererbung.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/04_Kaskadierung_und_Vererbung.mp4">Zum Video</a>
</video>

Das Grundprinzip der Kaskadierung bewirkt eine Reihen- oder Rangfolge, in der Eigenschaften in CSS vererbt werden, denn die einzelnen CSS-Selektoren werden unterschiedlich schwer gewichtet. Es ist hilfreich, diese Regeln zu kennen, um zu verstehen, wann welche Anweisungen umgesetzt werden (bzw. warum nicht) und welche Anweisungen andere überschreiben.

Definierte Eigenschaften werden an die (semantisch untergeordneten) Kinderelemente des selektierten Elements vererbt. Werden jedoch die Eigenschaften für die untergeordneten Elemente neu definiert, überschreiben diese die vererbten Eigenschaften.

### Box Model und Masseinheiten
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/05_CSS_Box_Model_und_Masseinheiten.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L03/05_CSS_Box_Model_und_Masseinheiten.mp4">Zum Video</a>
</video>

Das CSS-Box-Model beschreibt, dass alle Elemente im Browser auf Basis einer Box beschrieben werden können, die aus einer bestimmten Größe (Höhe x Breite), einem Innenabstand (**padding**), einem Rahmen (**border**) und einem Außenabstand (**margin**) bestehen.

Der Browser arbeitet mit verschiedenen Maßeinheiten, für den Anfang genügt das Pixelmaß (**px**). Ansonsten gibt es beispielsweise noch Angaben in **pt** (statisch, Anwendung im Druck), **em** und **rem** (relative Angabe) oder **Prozent**.

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

[CSS Cheatsheet](Cheatsheet_CSS.pdf)

---

## **A _---_** Aufgabe #03

Die Portfolio-Website aus der letzten Aufgabe wird nun mit CSS ergänzt, um verschiedene Gestaltungsaspekte zu realisieren.

Für dieses Projekt erstellen Sie einen Unterordner (bspw. /Aufgabe3) in Ihrem bestehenden EIA1-Git-Repository und erstellen Sie dort eine Kopie Ihres aktuellen Portfolios aus der vorherigen Aufgabe, an dem Sie nun weiterarbeiten werden.

**Die Aufgabe ist erfüllt, wenn alle Anmerkungen des Kunden berücksichtigt wurden.**
Kundenanmerkungen siehe [Anmerkungen](task_material/Anmerkungen.pdf)

Designentwürfe als Orientierung siehe [Ordner "Screenshots"](https://github.com/gabriel-rausch/EIA1-SoSe20/tree/master/L03/task_material/screenshots)

Grafikelemente für Untergrund und Pixel-Icon [im Ordner "Images"](https://github.com/gabriel-rausch/EIA1-SoSe20/tree/master/L03/task_material/images)


## Abgabe bis Sonntag 17. Mai, 18:00 Uhr
__Nach Abgabe und Feedback sind Korrekturmöglichkeiten bis 19. Mai möglich__

Bitte erstellen Sie einen Link in Ihrer Steckbrief HTM, der auf das Ergebnis verweist.


---


## **?! _<small>Q&A</small>_** Fragen und Antworten
(die Zusammenfassung der Q&A-Session wurden von Teilnehmern verfasst und ggf. angepasst und ergänzt)

Von [janzonca](https://github.com/janzonca)


### Was ist CSS für einer Sprache?
CSS ist eine Gestaltungssprache

### Kann man sich die Namensvergabe von den Selektoren ausdenken?

Den Selektor bzw. die ID oder die Klassen kann man sich ausdenken. Es gibt Herangehensweisen denen man folgen kann, aber dies ist für den Kurs vorerst nicht notwendig.

### Wird das box model im head angegeben?
Nein. Es wird im stylesheet angegeben. Es ist für jedes einzelne Element und nur für CSS relevant.

### Sollen wir das Design aus der Vorlage übernehmen?
Nein, das ist nicht zwingend notwendig. Es dient als Designvorlage. Das Design sollte zwar vom Aufbau gleich sein, allerdings darf man sich selbst kreativ ausleben. Wichtig ist, dass es ästhetisch sein soll.

### Wie bekommt man einen Kreis in das Portfolio?
Dafür gibt es verschiedene Varianten.  Durch HTML und CSS kann man probieren einen Kreis nachzubauen (aufwendige Variante) oder man kann mit Pixelgrafiken/Bildelemente arbeiten und diese einfügen.
