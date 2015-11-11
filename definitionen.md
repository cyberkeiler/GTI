# Definitionen
### Symbole
Elemente eines Alphabets

### Alphabet
Nichtleere, endliche Menge von Symbolen

### Wort
Konkatenation von Symbolen (endlich)

### leere Wort
ein Wort ohne Symbole (Länge = 0)

### Sprache
Vereinigung von Wörtern?????

### Potenzmenge
Menge aller Teilmengen (Beinhaltet keine Elemente!!)

### Teilmenge
Alle Elemente kommen in beiden Mengen vor.

## Operationen
### Konkatenation

---
## Zustandsübergangsdiagramme
### Formale Notation
**allg.: $M = (K, \sum, \delta, s, F  )$**
* $M$ - Automat
* $K$ - Menge der Zustände
* $F$ - Menge Endzustände ($F \subseteq K$)
* $\sum$ - Alphabet (nicht leere, engliche Menge von Zeichen)
* $L$ - Sprache (Menge der Wörter)
* $\delta$ - Überführungsfunktion
* $s$ - Startzustand ($s \in K$)
* $\vdash$ "überführt "

### Epsilonübergang E(q)
Menge aller Zustände, die vom Zustand q über $\epsilon$-Übergänge erreicht werden können
