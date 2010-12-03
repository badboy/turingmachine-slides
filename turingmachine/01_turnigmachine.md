!SLIDE

# Die Turingmaschine selbst

!SLIDE center

### Erstmals formuliert in

> On Computable Numbers, with an Application to the "Entscheidungsproblem"

### (28. Mai 1936)

!SLIDE bullets incremental

* grundlegendes Konzept der Informatik
* Modell des mathematisch arbeitenden Menschen

!SLIDE bullets incremental

* drei Operationen: schreiben, lesen, bewegen
* alle mathematischen Grundoperationen möglich

!SLIDE center

> Alles, was so berechnet werden kann, ist eine turingberechenbare Funktion
!SLIDE center

### Church-Turing-These

> Die Klasse der Turing-berechenbaren Funktionen ist genau die Klasse der intuitiv berechenbaren Funktionen.

!SLIDE bullets incremental

* Halteproblem __nicht__ mit Turingmaschine berechenbar
* ↓
* auch __nicht__ von Menschen berechenbar

!SLIDE

# Formale Definition

!SLIDE center

![M = ...](M_equal.png)

!SLIDE smbullets left

* ![Q](Q.png) ist die endliche Zustandsmenge
* ![Sigma](Sigma.png) ist das Eingabealphabet
* ![Gamma](Gamma.png) ist das endliche Bandalphabet und es gilt ![Sigma subset Gamma](Sigma_subset_Gamma.png)
* ![delta](delta.png) ist die (partielle) Überführungsfunktion
* ![q_0](q_0.png) ist der Anfangszustand
* ![square](square.png) steht für das leere Feld (_blank_)
* ![q_f](q_f.png) ist die Menge der akzeptierten Zustände

!SLIDE

## Überspringen wir den Mathe-Hokuspokus
