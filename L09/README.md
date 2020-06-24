## **09 _#_** Programmiergrundlagen IV

### Fortgeschrittene Variablendeklaration
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_01_Fortgeschrittene_Variablendeklarationen.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_01_Fortgeschrittene_Variablendeklarationen.mp4">Zum Video</a>
</video>

Außer mit `var` können wir Variablen auch als **Konstanten** oder als Variablen mit **eingeschränktem Gültigkeitsbereich** deklarieren.
* **Variablen mit eingeschränktem Gültigkeitsbereich (`let`)**: `let`-Variablen sind nur in dem Bereich gültig, in dem sie deklariert wurden (nicht mit global/lokal verwechseln). Im Gegensatz zu `var`-Variablen können wir ihnen also nicht in anderen Blöcken andere Werte zuweisen, sondern deklarieren dabei eine neue Variable — wobei die ursprüngliche Variable unverändert bleibt. `let`-Variablen kann man **nicht mehrfach deklarieren**.
* **Konstanten (`const`)**: `const`-Variablen sind in der Gültigkeit ebenfalls auf den lokalen Block begrenzt und ihr Wert kann nicht durch Wertzuweisung oder Neudeklaration verändert werden: Sie sind also **konstant**. Bei der Deklaration muss der `const`-Variable direkt ein Wert zugewiesen werden.


### Objekte
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_02_Objekte.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_02_Objekte.mp4">Zum Video</a>
</video>

Objekte sind **komplexe Variablentypen**, die viele Informationseinheiten unterschiedlicher Datentypen speichern können.

Deklariert werden Objekte wie eine Variable mit dem Schlüsselwort `var`, dem ausgewählten `Objektnamen`, dem `Typ` (Name des zu verwendenden Interfaces, siehe nächstes Video) und den Inhalten. Die einzelnen Werte innerhalb eines Objektes sind **kommasepariert**.

**Beispiel:** 
```typescript
var objName: InterfaceName = {
    key1: "value",
    key2: 123
    key3: true,
    key4: [1, 2, 3]
};
```

**Objekt-Instanzen** sind einzelne Objekte, die auf Vorlage eines Interfaces erstellt wurden.


### TypeScript Interfaces
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_03_Interfaces.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_03_Interfaces.mp4">Zum Video</a>
</video>

Um Objekt-Instanzen zu deklarieren, muss zuerst ein **Interface** definiert werden. Dieses Interface dient als **Datentyp und Grundstruktur** für die Informationen und deren Datentypen, die später in den Objekt-Instanzen gespeichert werden sollen.

Interface-Definitionen werden über das Schlüsselwort `interface` angesagt und mit einem selbstgewählten (aussagekräftigen) Namen versehen. 

**Beispiel:**
```typescript
interface InterfaceName {
    key1: string;
    key2: number;
    key3: boolean;
    key4: string[];
}
```

**Objekte und Arrays**
Ein Objekt kann auch Arrays enthalten oder ein Array kann eine Liste von Objekten aufführen. Durch die Verkettung von Interfaces können einzelne Objekt-Instanzen innerhalb eines Arrays genutzt werden.


### Algorithmen
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_04_Algorithmen.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_04_Algorithmen.mp4">Zum Video</a>
</video>

Algorithmen sind **Problemlösungsstrategien** in Form von Handlungsvorschriften, die aus ganz vielen kleinen, konkreten Einzelschritten bestehen.

Das Grundprinzip hier heißt **Divide & Conquer** („Teile und Herrsche“): dabei werden Probleme so lange in kleine Teilprobleme unterteilt, bis jedes einzelne Problem ganz einfach und trivial zu verstehen und zu lösen ist. Diese Teilprobleme können dann Schritt für Schritt in eine Programmiersprache übersetzt werden.

**Herangehensweise bei der Problemlösung:**
1. **UI-Skizze zeichnen:** grobe Übersicht, wie die Anwendung für den User aussehen soll (User-Interface), und welche Elemente welche Funktionen haben sollen. Daraus lässt sich gut ableiten, welche Einzelbauteile zur Lösungsentwicklung benötigt werden.
2. **Aktivtätsdiagramm aufstellen:** Diagramm über den Ablauf/Interaktionsfluss des Programms, z.B. als Flowchart („Was passiert wann?“)
3. **Implementieren:** Aktivitätsdiagramm Schritt für Schritt in Code-Anweisungen übersetzen


### Take Aways
<video controls width="100%"> 
    <source src="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_05_Take_Aways.mp4" type="video/mp4"> 
    <a href="https://lehre.gabriel-rausch.de/HFU/EIA1_SoSe20/L09/L09_05_Take_Aways.mp4">Zum Video</a>
</video>

* Neben `var` gibt es in TypeScript auch `let`- und `const`-Variablen. Diese haben einen eingeschränkten Gültigkeitsbereich und `const` ist zudem unveränderbar („konstant“).
* **Objekte** sind Instanzen von **Interfaces** (selbst definierter Objekttypen) und können als komplexe Variablentypen mehrere Eigenschaften von unterschiedlichen Datentypen zu einem Objekt speichern.
* **Algorithmen** sind Problemlösungsstrategien, bei denen komplexe Probleme auf kleinste Teilprobleme heruntergebrochen werden, welche einfach(er) verstanden und gelöst werden können.


## **A _---_** Aufgabe #09
### ToDo App

Als Student werden Sie sich in Ihrer Studienlaufbahn immer weiter selbst organisieren müssen - deshalb erstellen Sie mit dieser Aufgabe Ihre eigene ToDo App.
Prototypisch wurde die Anwendung schon vom (fiktiven) "Designteam" vorbereitet, an dieser Vorlage sollten Sie sich orientieren:

[Prototyp ToDo App](task_material/prototype_example)  
(Dieser Prototyp wurde mit einem einfachen Prototyping Tool erstellt, die Skriptdateien sind für Sie unbrauchbar)

1. Die ToDo App soll es ermöglichen, dass Aufgaben als einfache Textbeschreibung eingegeben werden können. Um ein ToDo abzuspeichern können Sie entweder einen Button "add Task" erstellen oder (das wäre eine schönere Variante) beim Drücken der Entertaste - entscheiden Sie hier selbst, welche Variante Sie umgesetzt bekommen.

2. Aufgaben können auch als erledigt markiert werden.

3. Ebenfalls können Aufgaben gelöscht werden. 

4. Die Anwendung zeigt darüberhinaus die aktuelle Anzahl aller Aufgaben an (unabhängig von done und open).


Vorgehen: 
1. Erstellen Sie wieder ein Flussdiagramm, um die relevanten Interaktionschritte abzubilden. Teilen Sie also diese Aufgabe in Ihre Teilaufgaben.

2. Auf Basis des Flussdiagramms können Sie Schritt für Schritt die Problemstellungen angehen.

3. Icons bitte aus der Icon Font Library Fontawesome einsetzen (siehe Aufgabe 8)

Bearbeitung wie gehabt: als Unterordner in Ihrem Git Repository (/Aufgabe_9); das fertige Arbeitspaket wieder auf Github pushen und auf Ihrem Kursseiten-Steckbrief verlinken.

## Abgabe bis 28. Juni um 18:00 Uhr
__Nach Abgabe und Feedback sind Korrekturmöglichkeiten bis 30. Juni, 18:00 Uhr möglich__


---


## **?! _<small>Q&A</small>_** Fragen und Antworten
(die Zusammenfassung der Q&A-Session wurden von Teilnehmern verfasst und ggf. angepasst und ergänzt)

Von [olifabio](https://github.com/olifabio)



Fragen zur Aufgabenstellung
===========================

**I.     **Frage Prof: Was haben Sie aus der aktuellen Lektion mitgenommen? 

Antwort:      Die Grundelemente in Bezug auf -let- Variablen: die Gültigkeit einer -let- Variable lässt sich sehr gut innerhalb eine Code Blocks steuern. 

                     Zusätzlich gibt es die Konstanten -const-. Konstanten sind sinnvoll um einen konstanten Wert, bzw. eine Variable mit einem Wert zu beschreiben, der später nicht mehr geändert werden kann.

                     Empfehlung durch den Prof.: es ist zu empfehlen, nur mit -let- Variablen zu arbeiten. Wenn aber nur einmal definiert werden muss am Anfang des Codes, dann kann man die -const- Variable verwenden. 

                     Interface:

                     Objekte können idealerweise als Interface angegeben werden, die Interface Definition, also der gemeinsame Nenner wird als Interface angegeben.

Der Name des Interfaces kann frei definiert werden. Danach werden die Eigenschaften Wert für Wert definiert. (s. Erklärvideo Lektion: Programmiergrundlagen IV_Objekte und Interfaces)

**II.     **Frage:         Kann ein Steckbrief für mehrere Peronen angegeben werden? 

Prof: Überlegen Sie im aktuellen Aufgbenkontext, würde es da Sinn machen ein Objekt einzusetzen oder nicht?

Antwort:      Nein, es wurde so verstanden, dass nur ein Objekt gebraucht wird, wenn verschiedene Produkte gelagert werden und dann die entsprechenden Dinge ausgegeben werden. Prof: Bei einer To do Liste haben Sie eine Liste von to do's die dann irgendwo abgespeichert werden müssen. 

                     Eine Liste von einzelnen Schnipseln kann mit einem Array gemacht werden. 

                     Prof: Es wurde noch nicht aufgelöst, es gibt verschieden Ansätze, wie eine to do Liste erstellt werden kann. Wir sind frei in der Herangehensweise. 

Antwort:      In der nächsten Lektion, in der nächsten Woche wird ein Paket mit Code Schnipseln zur Verfügung gestellt, mit dem weitergearbeitet werden kann. 

                     Diese Woche lediglich die To Do App, wie wir sie gerne konzipiert haben.

                     Ansatz für die Zukunft: Best of Version of Code nach der Aufgabenstellung zur Verfügung stellen. 

**III.     **Frage:         Prof: Hat Ihnen der Ansatz bezüglich der Algorithmen geholfen? Haben Sie ein 

Gefühl davon bekommen die Aufgabe in Teilprobleme zu unterteilen?

Antwort:      Je kleiner die Problemmenge ist, desto besser ist sie zu handhaben. Das Problem kleinstmöglich halten und im Endeffekt mit einem Fahrplan, z.B. einem Flussdiagram richtig an einen komplizierten Ansatz heran zu gehen. 

Frage:          Prof: Haben Sie das schon einmal versucht einzusetzen? 

Antwort:      Es wurde schon mal angefangen, aber auch wieder entfernt, da es noch relativ schwierig ist, sich einen Plan zu machen. 

                     Prof: Wenn Sie die Logik nicht beschreiben können, dann können Sie es nicht programmieren. 

                     Daher ist es sehr wichtig, ein richtiges Konzept zu haben, um dann dementsprechend das Problem richtig lösen zu können. 

                     **Eine Grundherangehensweise ist CRUD: es beschreibt 1. Create: Datensatz anlegen, 2. Read or Retrieve: Datensatz lesen, 3. Update: Datensatz aktualisieren, 4. Deleat or Destroy: Datensatz annulieren, löschen. **

                        Eine To Do App ist eine Liste von Einzelelementen. 

**IV.     **Frage: Gibt es noch eine Frage zur Lektion 9?

Antwort: Nein. 

**Nächste Woche**: Es wird Zeit genommen, jede Einzelfragmente, die wir gelernt haben zu ordnen. Es wird eine Ask the Teacher Lesson geben. 

Es können alle möglichen Fragen gestellt werden, die uns beschäftigen und auch weiterbringen könnten. 

Es soll vorbereitet werden für die nächste Woche: Genaue Formulierungen der Problemstellungen. Die jeweiligen Problemstellungen sollen selektiert werden in ihrer Gewichtung (schwierig, sehr wichtig, nicht so wichtig, weniger wichtig) etc. pp.