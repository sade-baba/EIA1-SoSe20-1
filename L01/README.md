## **01 _#_** Einstieg HTML


### HTML Basics
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L01/GIS-EIA1-HTML-Basics.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L01/GIS-EIA1-HTML-Basics.mp4">Zum Video</a>
</video>

### HTML Syntax
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L01/GIS-EIA1-HTML-Syntax.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L01/GIS-EIA1-HTML-Syntax.mp4">Zum Video</a>
</video>


**Links zum Thema**

[W3C](https://www.w3.org)

[https://www.w3schools.com/html/](https://www.w3schools.com/html/)

[MDN - MozillaDeveloper Network](https://developer.mozilla.org/de/docs/Learn/HTML)

[HTML Cheatsheet](Cheatsheet_HTML.pdf)


### Bilder Verweise / Pfade
<iframe src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L01/GIS-EIA1-HTML-Bilder-Verweise.pdf" width="100%" height="400px" style="border:none"></iframe>

Den Foliensatz zu "Bilder Verweise / Pfade" können Sie auch [hier](https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L01/GIS-EIA1-HTML-Bilder-Verweise.pdf) als PDF herunterladen

---


## **A _---_** Aufgabe #01

In den ersten Aufgaben sollten Sie **nur** mit der Technologie HTML arbeiten.

Erstellen Sie mit dem vorgegebenen Material (im Ordner [/assets](https://github.com/gabriel-rausch/EIA1-SoSe20/tree/master/L01/assets)) eine Portfolio-Website (also eine einfach HTML-Website, die ein fiktives Portfolio von bisherigen Arbeiten präsentiert). 

Es soll eine HTML-Seite erstellt werden, die verschiedene Bilder (foto1, foto2, foto3, foto4 aus dem Unterordner "foto" von dem Ordner "assets") /Videos (clip1, clip2, clip3, clip4 aus dem Unterordner "animation" von dem Ordner "assets") präsentiert. Eine kleine Unteraufgabe: bei Klick auf das Foto1 soll eine neue Seite geöffnet werden und das Foto1_Big dargestellt werden.

### Abgabe erfolgt nach Fertigstellung von Aufgabe #02 zum 10. Mai um 18:00 in Ihrem Steckbrief bzw. auf der Kursseite.


---


## **?! _<small>Q&A</small>_** Fragen und Antworten
(die Zusammenfassung der Q&A-Session wurden von Teilnehmern verfasst und ggf. angepasst und ergänzt)

---

Von [naominoller](https://github.com/naominoller)


### Was ist das DOM?
 
Das Document Object Model (kurz. DOM) ist in erster Linie ein abstraktes Objekt, welches hierarchisch die Eigenschaften, Werte und Verschachtelungen der einzelnen Elemente aufzeigt. Es repräsentiert den strukturierten Inhalt einer Website und bietet die Grundlage für das fertige Browserbild.
 
### Was ist der Unterschied zwischen einem relativen und einem absoluten Pfad?
 
Der absolute Pfad kann bspw. auf eine externe URL verweisen, also auf eine Datei, welche nicht im gleichen Datei- oder Domainkontext liegt. Ein absoluter Pfad kann aber auch im selben Domainkontext liegen, dann wird auf die Datei absolut vom Domainurspung verwiesen (URL beginnt mit "/").
 
Der relative Pfad hingegen nimmt Bezug auf einen Pfad relativ vom **Dokumentenursprung** im selben Domainkontext bzw. in der selben Dateistruktur (vereinfacht) liegt.

Durch ".." kann in einem Pfad auf eine Pfad-Ebene höher gesprungen werden. Bspw. zeigt "videos/video1.mp4" auf eine Videodatei in einem Unterverzeichnis "videos", dagegen zeigt "../videos/video1.mp4" auf eine Datei, die eine Ebene höher in der Dateistruktur liegt und dort in einem Ordner "videos" liegt.

Ein Pfad bildet im einfachsten Fall die Dateistruktur / Ordnerstruktur ab (diese Analogie ist für den Einstieg in die Webentwicklung vollkommen ausreichend). D.h. "https://domain.de/products/product1.html" zeigt auf eine HTML Datei (product1.html), die in einem Ordner "products" auf einem Server, der unter der Adresse domain.de erreichbar ist, liegt.
 
### Was ist der Unterschied zwischen den zwei Grafikmodi retained und immediate?
 
"retained mode“ = die Inhalte und Grafiken können über sichtbaren Bereich (hier Browserfenester) hinausgehen und verlustfrei skaliert werden; die Render Pipeline des Browers übernimmt das Neu-Rendern bei Positions- oder Transformationänderungen der Inhalte. HTML oder auch SVG werden vom Browser nach dem "retained mode" gerendert.
 
„immediate mode“= nur die Inhalte im sichtbaren Bereich (im Viewport) werden gerendert -> ressourcenschonender, es können deutlich komplexere Visualisierungen gerendert werden. Dabei ist aber auch mehr Entwicklungsarbeit notwendig. Sämtliche Transformationsänderungen (bspw. das Skalieren eines Objekts) würde ohne neu-berechnen und neu-rendern des Viewports zu einer fehlerhaften Darstellung führen (bspw. Pixelartefakte beim Skalieren eines Objekts). Es gibt ein HTML-Element, das nach nach dem "immadiate mode" gerendert wird: der Canvas-Tag (wird im 2. Semester behandelt)
 