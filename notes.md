# Turingmaschine

## Alan Turing

geboren: 23. Juni 1912 in London
gestorben: 7.Juni 1954 in Wilmslow
(41 Jahre)

Demnach war er Brite
außerdem: Marathonläufer (5. bei olymp. Sommerspielen 1948 in London)
2h46min

Seit Kindesbeinen kluges Köpfchen (Anzeichen von Genialität)
1928 stieß er auf Albert Einsteins Arbeiten.
Verstand Einsteins Bewegungsgesetz (nicht explizit erwähnt)

Logiker, Mathematiker und Kryptoanalytiker. 
einer der einflussreichsten Theoretiker der frühen Computerentwicklung und Informatik. 
schuf Großteil der theoretischen Grundlagen für die moderne Informations- und Computertechnologie. 
Auch richtungsweisend: Beiträge zur theoretischen Biologie

im zweiten Weltkrieg: arbeitete fürs britische Militär
entschlüsselte dt. Funksprüche
mathematische Modelle zur Entschlüsselung der Enigma

1936 entwickelte er das Modell der Turingmaschine (Thema des Referats)
1950 Turingtest, um Intelligenz eines Computerprogramms zu messen
1953 entwickelte er ein Schachprogramm, geringe Computerleistung vorhanden → per Hand berechnet

Turing war homosexuell → verboten im damaligen England
1952 angeklagt wegen "grober Unzucht und sexueller Perversion"
(nach Einbruch bei ihm)
Wahl: Gefängnis oder "psychatrische Behandlung"
triebhemmendes Hormon (Östrogen)
→ körperliche Veränderungen nahm er mit Humor (Entwicklung von Brüsten, Gewichtszunahme)
→ Depression → Selbstmord

Selbstmord mit vergifteten Apfel (nicht völlig bestätigt)
→ aus "Schneewittchen und die sieben Zwerge"

> Tauch den Apfel ins Gebräu / Lass den Schlaftod einziehen

↓

> Dip the apple in the brew <br/>
> Let the sleeping death seep through

Nach seinem Tod erst größere Würdigung:

Statue im Sackville Park
zwischen den wissenschaftlichen Gebäuden der Universität Manchester und dem Homosexuellenviertel der Canal Street.

Turing-Award
jährlich, Association for Computing Machinery
Nobelpreis der Informatik
bislang kein Deutscher, aber bekannte Informatiker wie Dijkstra, meist Amerikaner
mit $250.000 dotiert

10.09.2009 offizielle Entschuldigung durch Gordon Brown, Premierminister

> So on behalf of the British government [...] I am very proud to say: we're sorry, you deserved so much better.


## Turingmaschine selbst

formuliert in On Computable Numbers, with an Application to the "Entscheidungsproblem" (1936)

Beitrag zum Hilbertprogramm (1920)
Hilbertprogramm: Widerspruchsfreiheit der Axiomensysteme der Mathematik nachzuweisen mit finiten Methoden (endlichen) (ursprüngliches Programm nicht durchführbar)

grundlegendes Konzept der Informatik
beabsichtigt als Modell des mathematische arbeitenden Menschen

Grundlegender Aufbau:
unendlich langes Speicherband mit unendlich vielen Feldern
jedes Feld kann genau ein Zeichen speichern
programmgesteuerter Lese-/Schreibkopf

Genau drei Operationen nötig:
Schreiben, Lesen, bewegen

→ alle mathematischen Grundoperationen möglich


> Alles, was so berechnet werden kann, ist eine turingberechenbare Funktion
## Church-Turing-These

> Die Klasse der Turing-berechenbaren Funktionen ist genau die Klasse der intuitiv berechenbaren Funktionen.


* Halteproblem __nicht__ mit Turingmaschine berechenbar
* ↓
* auch __nicht__ von Menschen berechenbar

Halteproblem:
Bestimmung ob bestimmtes Berechnungsvorschrift zu einem Ende gelangen kann.
Kann man ein Programm entwickeln, das als Eingabe den Quelltext eines zweiten Programms sowie dessen Eingabewerte erhält, welches entscheiden kann, ob das zweite Programm terminiert, d. h. nicht endlos weiterläuft?


Formale Definition

M = (Q, Sigma, Gamma, Delta, q0, Leeres Feld, qf)

* Q ist die endliche Zustandsmenge
* Sigma ist das Eingabealphabet
* Gamma ist das endliche Bandalphabet und es gilt 
  Sigma ist ein Teil von Gamma
* delta ist die (partielle) Überführungsfunktion
* q0 ist der Anfangszustand
* Quadrat steht für das leere Feld (blank)
* qf ist die Menge der akzeptierten Zustände

Überspringen wir den Mathe-Hokuspokus

Beispiel: Zahlen verdoppeln

von 11000 zu 11011

vorherige Definitionen:
6 Zustände nötig, Anfangszustand s1, Endzustand s6 (auch H(alt) genannt)o

Überführungsfunktion

als Zustandstabelle

aktueller Zustand, gelesenes Zeichen, Schreibzeichen, neuer Zustand, Kopfrichtung


Beispiel folgt → Abarbeitung der Zustandstabelle / Überführungsfunktion

Wieviele Schritte waren nötig? → 16
→ selbst kleinste Probleme schon rechenaufwändig
ABER: Maschine nur als Modell → mathematische Richtigkeit bewiesen.
Maschinelle "Nachbauten", aber eben kein "unendlich langes Band" möglich

Zusammenhang mit formalen Sprachen
Sprache L akzeptiert, wenn Eingabe des Wortes in endlich vielen Schritten in definierten Endzustand führt
Sprache L durch Turingmaschine definiert, wenn bei Eingabe, die nicht zur Sprache gehört, Turingmaschine anhält.


# Weiteres Beispiel

Nur angedeutet, zu viele Schritte nötig

## Addition:
5 + 3 wird zu 8
111110111 wird zu 11111111

(|, ○) akzeptierte Zeichen

### Möglicher Ansatz:

* ersten Strich mit ○ überschreiben
* Trennpunkt mit einem | überschrieben
* Kopf wieder bis zum ersten Strich bewegen

## Addition mal richtig:

5 + 3 wird zu 5 + 3 = 8
11111+111 wird zu 11111+111=11111111


(|, ○, +, =) akzeptierte Zeichen

### Möglicher Ansatz:
* beide Summanden nach einander hinter das zweite Trennzeichen kopieren

# Diese Folie ist in deinem Land nicht verfügbar. Oops.

# Fragen?

# Ende (Quellenverzeichnis)
