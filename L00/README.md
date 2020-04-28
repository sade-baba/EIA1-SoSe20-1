## **00 _#_** Preface

### Einführung
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L00/GIS-EIA1-Einfuehrung.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L00/GIS-EIA1-Einfuehrung.mp4">Zum Video</a>
</video>


### Vorbereitung / Tools
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L00/00_Arbeitsumgebung.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L00/00_Arbeitsumgebung.mp4">Zum Video</a>
</video>

#### Tools / Software
- [Visual Studio Code](https://code.visualstudio.com/)
- [Git](https://git-scm.com/)
- [GitHub](https://github.com/)
- [Github Desktop](https://desktop.github.com/)
- [Gitkraken](https://www.gitkraken.com/)
- [Sourcetree](https://www.sourcetreeapp.com/)


---

## **A _---_** Aufgabe #00

Starten Sie mit ein paar "Hygiene-Aufgaben", damit Sie arbeitsfähig werden und bereit für den Kurs sind:

1. Registrieren Sie sich auf der Entwicklerplattform **github.com**.

2. Installieren Sie sich die ersten Bausteine Ihrer Entwicklungsumgebung: **Visual Studio Code**, GIT und **Github Desktop** (Erklärung siehe Video "Vorbereitung / Tools").

3. Fügen Sie ihren Steckbrief auf der EIA1-Kursseite ein (Link siehe DM-Intranet), dafür gehen Sie wie folgt vor:

    1. [Steckbrief-Vorlage](Steckbrief.zip) herunterladen.
    2. Dateien mit eigenen Inhalten ergänzen (die Dateinamen, wie sie in der Vorlage definiert sind, dürfen nicht verändert werden! D.h. die HTML Datei **muss** __steckbrief.htm__ heißen, das Profilbild muss eine JPG-Datei sein und __portrait.jpg__ heißen, beide Dateinamen mit Kleinbuchstaben).
    3. Ein neue Github Repository mit dem Namen EIA1-SoSe20 auf github.com erstellen
    4. dann lokal ebenfalls den Ordner, in dem die Steckbrief Dateien liegen (bspw. Ordnername ebenfalls "EIA1-SoSe20") zu einem neuen Github Repository hinzufügen und auf Github in das erstelle Repository pushen (Anleitung dazu siehe Video "Vorbereitung / Tools").
    5. Jetzt in den Einstellungen vom Github Repository die Inhalte in der Hosting-Umgebung **Github Pages** veröffentlichen.
    6. Prüfen, ob der eigene Steckbrief als Website auf Github Pages veröffentlicht wurde, dazu Ihre Dateien im Gihub-Pages (github.io) Kontext, nicht auf Github (githum.com) prüfen (bspw. https://mein-nutzername.github.io/eia1-sose20/steckbrief.htm).
    7. EIA1-Kursseite (siehe Link in DM-Intranet) öffnen und Steckbrief registrieren. Bitte korrekte URL (der Link zur IO-Seite ohne "steckbrief.htm", also bspw. https://mein-nutzername.github.io/eia1-sose20) angeben.
    8. Auf der EIA1-Kursseite wird jetzt Ihr Profilbild und Ihr Steckbrief in einem Fensterchen angezeigt.


### Aufgabe bis Sonntag, 26. April 2020, 18:00 Uhr

Ziel der Aufgabe: Sie sind arbeitsfähig, d.h. Sie haben sich auf der Kursseite registriert und kennen sich mit den grundlegensten Funktionen von GIT aus. Sie sind dazu in der Lage Ihre Abgaben auf GitHub hochzuladen und wissen wie Sie Ihre steckbrief.htm aktualisieren können.


---


## **?! _<small>Q&A</small>_** Fragen und Antworten

In den ersten Aufgaben sollten Sie **nur** mit der Technologie HTML arbeiten.

Erstellen Sie mit dem vorgegebenen Material (im Ordner [/assets](https://github.com/gabriel-rausch/EIA1-SoSe20/tree/master/L01/assets)) eine Portfolio-Website (also eine einfach HTML-Website, die ein fiktives Portfolio von bisherigen Arbeiten präsentiert). 

Es soll eine HTML-Seite erstellt werden, die verschiedene Bilder (foto1, foto2, foto3, foto4 aus dem Unterordner "foto" von dem Ordner "assets") /Videos (clip1, clip2, clip3, clip4 aus dem Unterordner "animation" von dem Ordner "assets") präsentiert. Eine kleine Unteraufgabe: bei Klick auf das Foto1 soll eine neue Seite geöffnet werden und das Foto1_Big dargestellt werden.

### Abgabe erfolgt nach Fertigstellung von Aufgabe #02 zum 10. Mai um 18:00 in Ihrem Steckbrief bzw. auf der Kursseite.


---


## **?! _<small>Q&A</small>_** Fragen und Antworten
(die Zusammenfassung der Q&A-Session wurden von Teilnehmern geschrieben und nicht verändert)

---

Von [BeateG](https://github.com/BeateG)

###	Was ist das W3C?
= World Wide Web Consortium

Das W3C, gegründet von Tim Berners-Lee, ist ein Zusammenschluss aus Unternehmen, gemeinnützigen Organisationen, Universitäten, Privatpersonen und Regierungsmitgliedern, welche ein Gremium zur Standardisierung von Web Standards bilden, also Richtlinien entwickeln und empfehlen (Bsp.: HTML, CSS, SVG, etc.). 
Web Standard Entwicklungsprozess:
1.	Arbeitsentwurf	working draft
2.	Empfehlungskandidat	candidate recommendation
3.	Empfehlungsvorschlag	proposed recommendation
4.	W3C Empfehlung	W3C recommendation

###	Was ist HTML?
= Hypertext Markup Language

HTML ist die Kernsprache jeglicher Webinhalte. Alles was im Webbrowser zu sehen ist, sowie verfügbare Interaktionen, sind über HTML definiert. 
(Aktuell: HTML5)
HTML wird über HTTP ( = Hypertext Transfer Protocol) transferiert, d.h. die Client und Server kommunizieren über HTTP.
HTTPS, wie im Browser angezeigt (https://nfjfnjskf.com), steht für Hypertext Transfer Protocol Secure, also ein sicheres Hypertext-Übertragungsprotokoll, welches die Client-Server Kommunikation verschlüsselt.

###	Was bedeuten die unterschiedlichen Begriffe “webpage”, “website” und “home-/landingpage”?

- Webpage = HTML Dokument, oft eine Seite eines Webauftritts
- Website = der gesamte Webauftritt, also mehrere webpages, welche miteinander verknüpft sind
- Home-/Landingpage = Eingangsseite eines Webauftritts


### GitHub Stuff

GitHub.com = Funktion ähnlich zu DropBox, enthält Dateistruktur, z.B. Kurse für EIA, welche dann auf GitHub pages (= um Dateien zu publizieren ;
Endung im Browser = github.io./; z.B.: https://gabriel-rausch.github.io/EIA1-SoSe20/L00/ ) als website angezeigt werden.

Dateien werden von der lokalen Festplatte auf github.com gepusht, welche dann, nach dem Hochladen, über github pages durch eine website zur Verfügung gestellt werden.
Um den Link des repositories zu generieren klickt man auf das jeweilige repository > settings > runterscrollen bis ‘GitHub Pages’ > source > von “none” auf “master branch” umstellen. 

---

Von [AnnetteWdm](https://github.com/AnnetteWdm)

## Fragen zum Einführungsvideo

### Was genau macht Git? 
Git ist eine Arbeitsumgebung auf der Festplatte, die zur Versionsverwaltung von Projekten dient. 
Es bietet die Möglichkeit, während der Entwicklung eines Projekts zu alten Produktionsständen zurückzuspringen, um auf diese Weise die eigenen Änderungen kontrollieren zu können.

### Was ist GitHub.com?
Ist eine Platform für Softwareentwickler. Sie ermöglicht das Teilen von Softwarecodes, Diskutieren, Erstellen von Reviews, Organisieren von Projekten und das gemeinsame Entwickeln.
Kann mit Dropbox verglichen werden. Der wesentliche Unterschied zu Dropbox ist, dass manuell aktualisiert werden muss (manuelles Bestätigen des aktuellen Standes durch commit message)
Repositorys können auch als Website gerendert werden. 

### Was ist das W3C?
Das W3C ist eine Organisation (Zusammenschluss von Experten), die die Richtlinien für Web Standards entwickelt.

### Was ist die aktuelle HTML Version?
HTML 5.0

## Fragen zur Aufgabe 00

### Git Installation für Apple User?
Für IOSCatalina: Binary Installer herunterladen um Git für IOS zu installieren
		
Um zu prüfen ob Git installiert ist: Terminal Prüfung nutzen (Powershell bei Windows), 
Terminal Öffnen, „git--version“ rein schreiben. 
Wird eine Versionsnummer angezeigt ist Git installiert.

### Error 404, was tun?
Es wurde eine falsche URL angegeben.
 Diese kann nur von Hr. Rausch oder den HiWis geändert werden.
 Mail mit der richtigen URL an die HiWis.

### Was ist der begriffliche Unterschied zwischen lokalem server upload und repository?
Bei einem server upload wird etwas hochgeladen
Das repository ist ein Ordner, der schon online existiert und nur rumliegt.
Das Repository kann durch pushen (vergleichbar mit Upload) aktualisiert werden.

### Mein Ordner wird nach Umbennenung von GitHubDesktop nicht mehr gefunden, was tun?
Der Ordner muss mit GitHub Desktop neu verknüpft werden unter dem Befehl „locate“.

### Statt 2 wurden 3 Dateien hochgeladen, ist das ein Problem?
Nein, das ist kein Problem.
Die „.DS_Store“ ist eine, für Mac spezifische, Konfigurationsdatei.

### Muss das Profilbild auf der Kursseite von mir sein?
Generell nicht wichtig, es wäre aber schön alle Kursteilnehmer zu sehen.

### Sind die Aufgabenlinks im Steckbrief wichtig?
Die Aufgabenlinks sind nur Platzhalter.

### Wie viele neue repositorys muss man erstellen? 
Ein repository reicht für dieses Semester.
Dieses muss aber durch pushen mit GitHub Desktop wöchentlich aktualisiert werden.
Neue Datei in lokalem Ordner hinzufügen --> commit message erstellen --> dann pushen (mehrere commits können gesammelt und gleichzeitig gepushed werden)

### Reicht GitHub Desktop?
Ausreichend fürs komplette Studium.

### Wann ist GitKraken besser als Desktop?
Wenn mit verschiedenen Branches gearbeitet wird z.B. bei Gruppenprojekten.

### Wie ist der allgemeine Ablauf des Kurses?
Ablauf siehe Kursplan 
Lektion und die dazugehörige Aufgabe wird selbständig bearbeitet, Abgabedatum steht auf der Kursseite
Mittwochs: Q&A zur Lektion
Freitags: Aufgabenbesprechung, Beantworten von Fragen zur Aufgabe

**Allgemeiner Hinweis: Eine gute Ordnerstruktur ist wichtig!!**

