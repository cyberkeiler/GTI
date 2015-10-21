# Übung 1
## 1. Welche Behauptungen über Mengen sind wahr/falsch? Begründung?

 * __Ø ⊆ Ø__ 
-> wahr, weil beide kein Elemente haben (also jedes Element kommt in beiden vor)

 * __Ø ∈ Ø__
-> falsch, weil leere Menge keine Elemente

 * __Ø ∈ { Ø }__ 
 -> wahr, da Definition der leeren Menge (ausreichende Begründung?) *{}* ∈ {*{}*}

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
