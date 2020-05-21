## **04 _#_** CSS Vertiefung

### Komplexe Selektoren
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/01_CSS_Komplexe_Selektoren.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/01_CSS_Komplexe_Selektoren.mp4">Zum Video</a>
</video>

Man kann die grundlegenden CSS-Selektoren, die in der letzten Lektion vorgestellt wurden, auch verketten, um komplexere Selektionen zu machen. So kann entweder auf einzelne, spezielle Elemente konkret zugegriffen oder auf nur ganz bestimmte Gruppen oder Folgen von Elementen selektiert werden. Mit Pseudoklassen können auch Elemente in ganz bestimmten Zuständen manipuliert werden, wie zum Beispiel bei einem Link der Zustand des Herüberfahrens mit der Maus („hovern“).

**Links im Video**

<a href="https://flukeout.github.io">https://flukeout.github.io</a>

### Positionierung, Flussverhalten und Layout
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/02_CSS_Flussverhalten_Positionierung.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/02_CSS_Flussverhalten_Positionierung.mp4">Zum Video</a>
</video>

Aufgrund der vielen verschiedenen Ausgabegeräte kann das Thema der Positionierung sehr komplex werden, in diesem Video wurden aber die grundlegenden Herangehensweisen erklärt.
Die Positionierung der Elemente auf einer gerenderten Seite hat oft wenig mit der Position im DOM-Tree zu tun.

Das Flussverhalten beschreibt das Verhalten der Elemente im Textfluss, sodass ein Element beispielsweise von den nachfolgenden Elementen in einer Zeile umflossen werden kann oder einen Zeilenumbruch bewirkt. Dieser Textfluss kann über Float und die Positionierung auch individuell manipuliert werden.

Für differenziertere Seiten-Arrangements kann man Eigenschaften, wie Grid oder Flexbox, nutzen.

**Links im Video**

Float:

<a href="https://codepen.io/philtim/pen/KrZmdN">https://codepen.io/philtim/pen/KrZmdN</a>

Positionierung:

<a href="https://codepen.io/philtim/pen/GwyWBP">https://codepen.io/philtim/pen/GwyWBP</a>

### Responsive Design
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/03_Responsive_Design.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/03_Responsive_Design.mp4">Zum Video</a>
</video>

Responsive Design heißt, alle (relevanten) Endgerätegrößen zu bedienen, wie Smartphones, Laptops, Tablets, Bildschirme...

Technisch gesehen bedeutet Responsive Design im Web-Kontext, dass die Darstellung der Benutzeroberfläche zwar an unterschiedliche Ausgabegeräte angepasst wird, die Datenbasis bleibt jedoch gleich. Konzeptionell bedeutet Responsive Design, dass eine interaktive Anwendung in möglichst vielen (relevanten) Anwendungsszenarien (am Schreibtisch, unterwegs im Bus usw...) genutzt werden kann. 

In CSS lässt sich eine **adaptive** (stufenweise) oder **responsive** (stufenlose) Darstellung beispielweise durch Breakpoints und Mediaqueries oder flexible Größen- und Positionierungsanweisungen realisieren.

**Links im Video**

Responsive Cat:

<a href="http://roxik.com/cat/">http://roxik.com/cat/</a>

Responsive Design Check:

<a href="http://ami.responsivedesign.is/">http://ami.responsivedesign.is/</a>

### CSS Transition und Animation
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/04_CSS_Transition_und_Animation.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/04_CSS_Transition_und_Animation.mp4">Zum Video</a>
</video>

Mit **Übergängen** (Transitions) und **Animationen** können in Webanwendungen zeitbasierte Effekte genutzt werden, die ein Design lebendig und flüssig wirken lassen oder dem Nutzer auf narrativer Ebene den Interaktionsfluss beschreibt. Die Animation von CSS Eigenschaften lässt sich durch viele Parameter steuern, bspw. auch durch die Definition der Beschleunigung der Animation.

**Links im Video**

CSS Transition Beispiel:

<a href="https://codepen.io/grausch/pen/XWWeZXW">https://codepen.io/grausch/pen/XWWeZXW</a>

CSS Animationen:

<a href="https://codepen.io/ajerez/pen/EaEEOW">https://codepen.io/ajerez/pen/EaEEOW</a>

Eigene Bezierkurve zeichnen:

<a href="http://cubic-bezier.com/">http://cubic-bezier.com/</a>

### Take Aways
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/05_Take_Aways.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L04/05_Take_Aways.mp4">Zum Video</a>
</video>

* Komplex verkettete Selektoren ermöglichen es, spezifischere Auswahlpfade zu erstellen.
* Elemente haben individuelle Positionen und Flussverhalten, die manipuliert werden können.
* Über Responsive Design lassen sich viele relevante Endgeräte bedienen.
* Über Transition und Animation lassen sich Elemente, oder deren Eigenschaften, animieren.

---

## **A _---_** Aufgabe #04
### CSS Greeting Cards - Stationsarbeit

Bevor wir die Büchse der Pandora von TypeScript öffnen können Sie sich hier noch einmal in verschiedene Darstellungsaspekte mit HTML und CSS vertiefen.

Auch wenn es dieses Jahr schwierig wird mit dem Reisen, die Urlaubspost dürfen Sie trotzdem schon einmal vorbereiten.
Sie finden hier acht Einzel-Stationen, jeweils mit Start-Material und einer Aufgabenbeschreibung.
**Station 1** ist für alle Pflicht. Darüberhinaus dürfen Sie sich vier Stationen Ihrer Wahl heraussuchen, die Sie bearbeiten. Die Aufgabe ist also erfüllt, wenn Sie **insgesamt fünf Stationen** gelöst haben.

[Zu den Stationen](https://github.com/gabriel-rausch/EIA1-SoSe20/tree/master/L04/task_material)

Sie werden auch erkennen, dass viele Bausteine in den Stationen ähnlich sind. Das Grundgerüst der Grußkarten, das Positionieren und Arrangieren von Elementen werden Sie hier wiederholend üben.

Bearbeitung wie gehabt: als Unterordner in Ihrem Git Repository (bspw /Aufgabe4, hier dann weitere Unterordner /Station1 .../Station_X); das fertige Arbeitspaket wieder auf Github pushen und auf Ihrem Kursseiten-Steckbrief verlinken.

## Abgabe von 5 Stationen bis Sonntag, 24. Mai, 18:00 Uhr.

Die schönste Ihrer Grußkarte dürfen Sie auch gerne (als Link) an Kommilitonen oder Lehrende schicken (Jirka R. Dell'Oro-Friedl freut sich immer über Post) ;-)



---


## **?! _<small>Q&A</small>_** Fragen und Antworten
(die Zusammenfassung der Q&A-Session wurden von Teilnehmern verfasst und ggf. angepasst und ergänzt)

Von [fionavi](https://github.com/fionavi)


**Fragen an Studenten:**

-      Welche Komplexe Selektoren gibt es?

zB. „hover" (Zustand eines Elements), gehört zu Pseudoklassen

-      Bitte von Herrn Rausch

Feedback zu Lehrvideos geben, eventuell Verbesserungsvorschläge äußern

**Fragen von Studenten:**

-      Allgemeine Frage zur Vorlesung

man darf Aufgaben und Lektionen auch schon früher bearbeiten, als sie vorgesehen sind

-      Können die Tabellen/Grafiken aus den Lehrvideos als Dokumente zu Verfügung gestellt werden? 

Ja, Herr Rausch bot an PDF-Dateien zu erstellen. Außerdem bietet <https://www.w3schools.com/> eine ausführliche Übersicht von CSS-Befehlen.

**Individuelle Fragen nach offizieller Session:**

-      Probleme mit "position: absolute;"

"position: absolute center;" gibt es nicht, korrekt ist "position: absolute;"

"position: absolute;" funktioniert nur wenn die Position des Elternelements nicht "static" ist

Verschachtelung müssen genau beachtet werden, damit sich die "position: absolute;" der Kinderelemente auf das richtige übergeordnete Element beziehen kann

-      Icon verschiebt sich obwohl es auf der Position bleiben sollte

Developer Tool nutzen, um zu sehen wo genau das Element verschachtelt ist (wenn die Elemente nicht ineinander verschachtelt sind, wird nichts vererbt)

durch "position: relative;" und bestimmte Werte für margin-bottom/-top ist die Positionierung auf der Y-Achse stabil, jetzt auf X-Achse zentral positionieren

In diesem Fall war der header das umschließende Element indem alle Kinderelemente sind

header Positionierungseigenschaft "relative" geben, damit er zum Ursprungselement des Koordinatensystems für alle Kinderelemente wird

-      Schwierigkeiten beim Hovern mit Bildern

Bildelemente haben bestimmte Größe, diese entspricht der Hovergröße

Statt mit echten Bildern in html zu arbeiten, kann man in html eine Klasse erstellen (<div class ="image">) und die Bilder mit CSS einfügen, damit man diese einfacher skalieren/manipulieren kann

.image {

background-image: url("https....");

}

Eigenschaften height und width definieren   je größer diese sind, desto mehr sieht man vom Bild

jetzt über "hover" dieses Bild austauschen:

.image:hover { 

background-image: url("https....");

}

.image { 

transition: all .5s;

}

-      Probleme bei Github Desktop (es kann nicht gepullt und gepusht werden, da der Repository Ordner nicht gefunden wird)

Liegt an Konflikt zwischen lokalem und online Repository (sie sind nicht synchron)

Um den Konflikt lösen, wird ein Klon über Github Desktop des aktuellen Repositorys erstellt (in diesem Fall das online R.). Dieser Klon ist jetzt lokal gespeichert und kann lokal bearbeitet und danach gepusht werden

-      Allgemeine Grundfunktionen und Workflow von Github Desktop

Ablauf: 

Dateien im Repository abspeichern, diese Änderungen werden auf Github Desktop angezeigt

bei Github Desktop "committ to master" klicken, dazu Beschreibung angeben, was geändert wurde (commiten ist lokal)

dann auf Server pushen (pushen ist online)

Gute Struktur: Immer erst alles lokal erstellen und bearbeiten, dann erst Kopie über Github Desktop auf Server pushen
