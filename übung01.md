# Übung 1
## 1. Welche Behauptungen über Mengen sind wahr/falsch? Begründung?

 * __Ø ⊆ Ø__
-> wahr, weil beide kein Elemente haben (also jedes Element kommt in beiden vor)
Ø ist Teilmenge jeder Mengr

 * __Ø ∈ Ø__
-> falsch, weil leere Menge enthält keine Elemente

 * __Ø ∈ { Ø }__
 -> wahr,  *{}* ∈ {*{}*} Menge enthält {} als Element

 * __Ø ⊆ { Ø }__
 -> wahr, Leere Menge ist Teilmenge jeder Menge!

 * __Ø ⊆ 2^Ø__
-> wahr, laut Definition:

Def. 2^A Potenzmenge: Menge aller Teilmengen von A

Potenzmenge von Ø umfasst nur Ø.

 * __Ø ∈ 2^Ø__
-> wahr ???



## 2. Welche Behauptungen über Mengen sind wahr/falsch? Begründung?
__Alphabet:__ Jede nicht leere Menge (>= 1 Symbole)

 * __*{a,b}* ∈ {a,b,*{a,b}*}__
-> wahr: Alphabet {a,b} kommt als Symbol im anderen Alphabet vor

 * __{a,b} ⊆ {a,b,{a,b}}__
 -> wahr: a, b kommen als Element in der rechten Menge vor.

 *2^{a,b,{a,b}}: {Ø, {a}, {b}, {{a,b}}, {a,b}, {a,{a,b}}, {b,{a,b}}, {a,b,{a,b}}}*
 * __{a,b} ⊆ 2^{a,b,{a,b}}__
 -> falsch, weil Element a,b nicht rechts als Element vorkommt

 * __{{a,b}} ⊆ 2^{a,b,{a,b}}__
 -> wahr, weil Menge {a,b} als Element rechts vorkommt

 * __{a, {a,b}} ⊆ 2^{a,b,{a,b}}__
 -> falsch, weil Element a rechts nicht als Element vorkommt

 * __{a, {a,b}} ⊆ 2^{a,b,{a,b}}__
 -> wahr, Potenzmenge = { ..., {{a,b}}, ..}



## 3. Wahr oder falsch. Begründung?
#### $$ \forall L_1,L_2,L_3: (L_1 L_2) L_3 = L_1 ( L_2 L_3) $$
-> wahr, Assoziativität

---
#### $$ \forall L_1,L_2,L_3: (L_1 \cup L_2) L_3 = (L_1 L_3) \cup (L_2 L_3) $$
-> wahr, Distributivität

---
#### $$ \forall L_1,L_2,L_3: (L_1 \cap L_2) L_3 = L_1 * L_3 \cap L_2 * L_3 $$
-> falsch, Konkatenation nicht kommutativ:

Gegenbeispiel:
$$ L_1 = \{ a \}; L_2 = \{ aa \}; L_3 = \{ \varepsilon, a \} $$


$$ \text{l.S.: }
 (L_1 \cap L_2) L_3 = \emptyset * L_3= \{ a \} $$

$$ \text{r.S.: }
L_1 * L_3 \cap L_2 * L_3 = \{ a, aa\} \cap \{aa, aaa\} = \{aa\} $$
$$ \text{Links} \ne \text{Rechts}$$

---
#### $$  \forall L_1,L_2,L_3: (L_1 L_2) \cup L_3 = (L_1 \cup L_3)(L_2 \cup L_3)$$
-> falsch, Konkatenation nicht kommutativ:

Gegenbeispiel:
$$ L_1 = \{ a \}; L_2 = \{ b \}; L_3 = \{ c \} $$
$$ \text{l.S.: }
  (L_1 L_2) \cup L_3  = \{ a,b\} \cup \{c\} = \{a, b, c\} $$
$$ \text{r.S.: }
  (L_1 \cup L_3)(L_2 \cup L_3)  = \{ a,c \} \{ b,c \} = \{ab, ac, cb, cc\} $$
$$ \text{Links} \ne \text{Rechts}$$

---

---
## 4. Wahr oder falsch? Begründe!
#### $$ \{\varepsilon\}^* = \emptyset $$
 -> falsch, Menge mit leerem Wort ist nicht leer!

---
#### $$ \emptyset \cup \emptyset^* = \{\varepsilon\} $$
-> wahr:
$$\emptyset \cup \emptyset^* = \{\} \cup \{\varepsilon\} = \{\varepsilon\}  $$

---
#### $$ \forall L:(L^+)^* = L^* $$
-> wahr, da Kleene Star Abschluss. $L^+$ ohne ε mit $^*$ wieder mit ε

---
#### $$ \{\varepsilon\}^* = \{\varepsilon\} $$
-> wahr

---
#### $$ \forall L: \emptyset L^* = \{ \varepsilon \}$$
-> falsch, wenn L aus mehr als ε besteht, daher nicht ∀L

---
#### $$ \forall L: \emptyset \cup L^+=L^* $$
-> flasch, $\emptyset \neq \varepsilon$:
$$ L^+ \cup \emptyset = L^+ $$
$$ L^* = L^+ \cup \varepsilon $$

---

---
## 5.
 * ∀L1,L2 :(L1L2)∗ =L∗1L∗2
 *
 * ∀L1,L2 :(L1∪L2)∗ =(L2∪L1)∗
-> wahr, da kommutativ

 * ∀L1,L2 :(L1∪L2)∗ =L∗1∪L∗2
-> falsch

 * ∀L1,L2 :L∗1∩L∗2 =(L1∩L2)∗
-> falsch

## 6.
### a) {w ∈ {a,b}∗ | genau ein Suffix von w beginnt mit a}
Alle Wörter können gebildet werden.

aa gilt nicht weil Unentscheidbar

### b) {w ∈ {a,b}∗ | alle Präfixe von w mit Länge mindestens 1 enden mit b}
Jedes Wort mit Präfix (ungleich ε) enthält ein b
beim Vorkommen von einem a ist keine Eindeutigkeit vorhanden
