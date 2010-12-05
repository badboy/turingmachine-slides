!SLIDE 
## Einfaches Beispiel: Zeichen verdoppeln

!SLIDE code example

# 1 1 ○ ○ ○

!SLIDE code example

# 1 1 ○ 1 1

!SLIDE bullets incremental

* es gibt 6 Zustände
* Anfangszustand s1 
* Endzustand s6 oder auch H (_HALT_)

!SLIDE

# Überführungsfunktion

!SLIDE mytable bullets

## Für jeden Zustand:

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s1 | 1 | → | ○ | s2 | R
 s1 | ○ | → | ○ | s6 | ○
 s2 | 1 | → | 1 | s2 | R
 s2 | ○ | → | ○ | s3 | R
 s3 | 1 | → | 1 | s3 | R
 s3 | ○ | → | 1 | s4 | L
 s4 | 1 | → | 1 | s4 | L
 s4 | ○ | → | ○ | s5 | L
 s5 | 1 | → | 1 | s5 | L
 s5 | ○ | → | 1 | s1 | R

* Z: aktueller Zustand
* L: gelesenes Zeichen
* W: zu schreibendes Zeichen
* nZ: neuer Zustand
* K: Kopfrichtung

!SLIDE code mytable mytable2
    1 1 ○ ○ ○      | s1
    ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s1 | 1 | → | ○ | s2 | R
!SLIDE code mytable mytable2
    ○ 1 ○ ○ ○      | s2
      ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s2 | 1 | → | 1 | s2 | R
!SLIDE code mytable mytable2
    ○ 1 ○ ○ ○      | s2
        ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s2 | ○ | → | ○ | s3 | R
!SLIDE code mytable mytable2
    ○ 1 ○ ○ ○      | s3
          ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s3 | ○ | → | 1 | s4 | L
!SLIDE code mytable mytable2
    ○ 1 ○ 1 ○      | s4
        ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s4 | ○ | → | ○ | s5 | L
!SLIDE code mytable mytable2
    ○ 1 ○ 1 ○      | s5
      ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s5 | 1 | → | ○ | s5 | L
!SLIDE code mytable mytable2
    ○ 1 ○ 1 ○      | s5
    ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s5 | ○ | → | 1 | s1 | R
!SLIDE code mytable mytable2
    1 1 ○ 1 ○      | s1
      ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s1 | 1 | → | ○ | s2 | R
!SLIDE code mytable mytable2
    1 ○ ○ 1 ○      | s2
        ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s2 | ○ | → | ○ | s3 | R
!SLIDE code mytable mytable2
    1 ○ ○ 1 ○      | s3
          ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s3 | 1 | → | 1 | s3 | R
!SLIDE code mytable mytable2
    1 ○ ○ 1 ○      | s3
            ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s3 | ○ | → | 1 | s4 | L
!SLIDE code mytable mytable2
    1 ○ ○ 1 1      | s4
          ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s4 | 1 | → | 1 | s4 | L
!SLIDE code mytable mytable2
    1 ○ ○ 1 1      | s4
        ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s4 | ○ | → | ○ | s5 | L
!SLIDE code mytable mytable2
    1 ○ ○ 1 1      | s5
      ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s5 | ○ | → | 1 | s1 | R
!SLIDE code mytable mytable2
    1 1 ○ 1 1      | s1
        ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 s1 | ○ | → | ○ | s6 | ○

!SLIDE code mytable mytable2 tabledone
    1 1 ○ 1 1      | s6
        ↑

 Z  | L | → | W | nZ | K
----|---|---|---|----|--
 F  | E | R | T | I  | G

!SLIDE center

# Mitgezählt?

!SLIDE center

# 16 Schritte waren nötig
