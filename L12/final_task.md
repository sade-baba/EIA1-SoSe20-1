# Endaufgabe - Konzentrationsspiel



**Entwickeln Sie ein Browser-basiertes Konzentrationsspiels für Kinder unter Berücksichtigung folgender Anforderungen**



**Spielregeln:**

- Ziel des Spiels ist es eine immer länger werdende Folge von Tonsignalen, die vom Computer vorgegeben werden, zu wiederholen.
- Bei Spielstart kann der Spieler zunächst den Schwierigkeitsgrad des Spiels wählen (mehr dazu siehe weiter unten)
- Dann spielt der Computer den ersten Ton ab.
- Der Spieler muss durch Drücken eines entsprechenden Buttons diesen Ton wiederholen.
- Der Computer wiederholt den ersten Ton noch einmal und spielt einen weiteren Ton ab.
- Der Spieler muss nun nacheinander die entsprechenden Buttons in der richtigen Reihenfolge drücken.
- Der Computer wiederholt die ersten beiden Töne und spiel einen weiteren Ton ab.
- Der Spieler muss nun diese drei Töne in der richtigen Reihenfolge wiederholen.
- Auf diese Art wird das Spiel fortgesetzt.
- Der Spieler hat gewonnen, wenn er alle Töne in der richtigen Reihenfolge wiederholen konnte. Je nach Schwierigkeitsgrad ist das Spiel nach 5 (leicht), 15 (mittel), 25 (schwer) oder 35 (sehr schwer) Tonfolgen zu Ende.
- Der Spieler hat verloren, wenn er beim Wiederholen der Tonfolge einen Fehler macht.



Diese Spielmechanik ist angelehnt an den ["Senso" von MB](https://www.youtube.com/watch?v=wrYVLmADhtA)



**Weitere Anforderung an die Anwendung:**

- Die Tonfolgen **variieren** bei jedem Spiel.
- Das Spiel besteht aus **fünf** Grundtönen, die eine Tonfolge ergeben.
- Das Spiel ist **optimiert für eine Desktop** Auflösung von 1280x800 Pixel.



### Beurteilung

Note der End-Abgabe basiert auf den erreichten Anforderungs-Punkten (siehe weiter unten). Bis zu einem Punkt darf dabei nicht erfüllt sein um die Note 1 zu erhalten.

Jeder weitere fehlende Punkt verringert die Note um 1. (4.0 >= Bestanden) 

Jedes erfüllte optionale Ziel erhöht die Note um 1. (Maximale Bestnote: 1).

Der Kurs wird im Studi-Portal mit "bestanden" / "nicht bestanden" bewertet.



### Herangehensweise

Entwickeln Sie ein Konzept auf Papier, das den grundlegenden Mechanik der Anwendung beschreibt, bevor Sie mit der Programmierung beginnen!

Versuchen Sie den Spielfluss in einem Flowchart/Anwendungsfalldiagramm darzustellen.
An welchen Punkten werden Entscheidungen gefällt? Muss der Computer gewisse Dinge abfragen?
Wann muss der Spieler interagieren, wie interagiert er, was sind seine Optionen? Wie sehen die Eingabgemöglichkeiten (bspw. Buttons) für den Spieler aus?
Welchen Ablauf hat der Computer, wie signalisiert er die Tonfolge aus? Wie validiert der Computer die Nutzereingaben?



### Anforderungspunkte

Gesamt: 24  
(24 = 1.0, 23 = 1.0, 22 = 2.0, 21 = 3.0, 20 = 4.0, <= 19 = NB)


Nach folgenden Kriterien wird Ihre Abgabe bewertet:

**Konzeptentwurf**

- [ ]  In einem Flußdiagramm haben Sie den grundsätzlichen Interaktionsfluß der Anwendung dargestellt. Den Papier-Entwurf bitte als Scan / Foto digitalisieren und beilegen.
- [ ]  Ein Entwurf der grafischen Benutzeroberfläche gibt einen groben Überblick über die UI-Elemente des Spiels. Hier bitte auch: den Papier-Entwurf / Entwürfe als Scan / Foto digitalisieren und beilegen.


**HTML**

- [ ]  Ein schlichter Footer der mit Ihrem Namen und Matrikelnummer. 
- [ ]  Semantische HTML-Tags wurden genutzt, Tags werden sinnvoll eingesetzt.

**CSS**

- [ ]  Die Spielflächen besitzt eine passende Hintergrundfarbe (oder Hintergrundtextur).
- [ ]  Vor dem Spiel wird dem Nutzer eine Möglichkeit zur Auswahl des Schwierigkeitsgrads angezeigt.
- [ ]  Nach Auswahl des Schwierigkeitsgrads werden dem Nutzer auf der Spielfläche (mindestens) vier Buttons angezeigt. Jeder Button repräsentiert einen Ton.
- [ ]  Die Buttons haben eine einheitliche Größe aber unterscheiden sich in ihrer visuellen Darstellung (Farbigkeit oder Piktogramm-Darstellung).

TIPP 1: Sie können zur Gestaltung der Buttons auch Bilder nutzen.

TIPP 2: Sie können auch auf die Icon-Font [Fontawesome](https://fontawesome.com/icons?d=gallery) zurückgreifen, um passende Piktogramme für die entsprechenden Töne darstellen zu können.

**Programmierung**

- [ ]  Das Skript erzeugt keine Fehler in der Konsole.
- [ ]  Die Code-Style Regeln des Linters wurden berücksichtigt (bspw. Typisierung von Variabilen).
- [ ]  Der Computer generiert zu Beginn des Spiel eine zufällige Tonfolge in der Länge des ausgewählten Schwierigkeitsgrads. Tipp: starten Sie bei der Entwicklung zunächst mit einer statischen, manuell definierten Reihenfolge. Im nächsten Schritt können Sie nach Möglichkeiten recherchien, um eine zufällige Zahl (mit _Math.random()_) zur Generierung einer Zufallsliste einzusetzen.
- [ ]  Die Tonfolge besteht aus einer zufälligen Reihenfolge von mindestens fünf Tönen (es dürfen auch gerne mehr "Grundtöne" für das Spiel genutzt werden, aber mindestens fünf). Eine Auswahl von möglichen Tönen finden Sie im Materialordner. Sie dürfen auch gerne eigene Töne (Urheberrecht berücksichtigen!) einsetzen.
- [ ]  Der Computer kann diese Töne nacheinander abspielen. Tipp: dafür wird Ihnen eine Methode _setInterval_ oder auch _setTimeout_ behilflich sein (wie schon in vorherigen Lektionen geübt).
- [ ]  Beim Abspielen eines Tons durch den Computer wird der entsprechende Button hervorgehoben.
- [ ]  Die Abspiellänge der Tonfolge nimmt im Spielverlauf zu. Der Computer spiel zunächst nur den ersten Ton dieser Tonfolge ab. Nach Nutzerinteraktion die ersten zwei, danach die ersten drei Töne usw.
- [ ]  Der Nutzer kann durch Klick auf einen Button einen Ton abspielen. 
- [ ]  Klickt der Nutzer auf einen Button wird ebenfalls der entsprechende Button hervorgehoben.
- [ ]  Der Computer validiert die Eingabe des Nutzers mit der aktuellen Tonfolge.
- [ ]  Bei Fehleingabe des Nutzers wird ein Fehler-Ton abgespielt und wird eine Meldung angezeigt ("Spiel verloren").
- [ ]  Ist das Spiel verloren, wir dem Nutzer eine negative Nachricht angezeigt.
- [ ]  Ist die vom Nutzer eingegebene Reihenfolge richtig, dann spielt der Computer die bestehende Tonfolge mit einem weiteren Ton ab.
- [ ]  Hat der Nutzer die maximale Anzahl an Tönen richtig wiederholt bzw. ist das Ende der Tonfolge erreicht, dann wird eine Nachricht angezeigt, dass das Spiel gewonnen ist.
- [ ]  Der Nutzer kann das Spiel erneut starten, wenn es zu Ende ist.


**Annotationen**

- [ ]  Erklären Sie Ihren Code. Die Skript-Datei sollte mit Kommentarblöcken ergänzt sein, um relevante Anwendungsblöcke und Anweisungen beschreiben zu können (vgl. letzte Aufgaben-Vorlage).




**Optional**
Diese Punkte MÜSSEN nicht erfüllt werden! Sie fließen jedoch positiv in die Berwertung mit ein (siehe oben).

- [ ]  Zusätzliche Regel: nachdem der Computer die aktuelle Tonfolge gespielt hat, muss der Spieler innerhalb von drei Sekunden reagieren. Reagiert der Nutzer zu spät, ist das Spiel verloren.
- [ ]  Zusätzliches Verhalten des Computers: der Computer erhöht im Spielverlauf das Tempo.
- [ ]  Ein visueller Fortschrittsbalken plus Textinformation (bspw. Level 1 von 25) wird am Bildschirm angezeigt.
- [ ]  Wenn ein Spieler gewinnt, wir eine Nachricht mit einer Zusammenfassung des Spiels angezeigt: Gewählter Schwierigkeitsgrad, feierliche Nachricht und Dauer des Spiels (bspw. 53 Sekunden).
- [ ]  Das Spiel funktioniert auch auf mobilen Endgeräten mit Touch-Input. Achtung: mobile Browser unterdrücken das automatische Abspielen von Sounds, hier müssen Sie auf die Audio API zurückgreifen, siehe Beispiel [hier](https://github.com/gabriel-rausch/Example-AudioAPI-Drumpad).



[Link zum Materialordner](https://github.com/gabriel-rausch/EIA1-SoSe20/tree/master/L10/task_material)


### Abgabe

Die Abgabe der Arbeit erfolgt diesmal nicht über die Kursseite, sondern per E-Mail. Verpacken Sie also Ihr Ergebnis am Ende als ZIP-Datei und senden Sie diese an gabriel.rausch(at)hs-furtwangen.de. Sollte Ihre ZIP-Datei Größer als 15MB betragen, dann legen Sie die Datei auf einem Datei-Austauschserver ab (HFU interner FTP oder WeTransfer) und senden Sie den Downloadlink. Der Eingang Ihrer E-Mail wird von mir bestätigt (d.h. wenn Sie innerhalb von 24h keine Bestätigung bekommen, dann ist Ihre E-Mail wahrscheinlich nicht angekommen).

**Abgabe bis Sonntag, 02.08.2020 18:00 Uhr**





---



Samples von freesound.org, Creative Commons 0 License