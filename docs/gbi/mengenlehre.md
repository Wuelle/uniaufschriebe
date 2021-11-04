# Mengenlehre
## Was ist eine Menge

Eine Menge ist eine Ansammlung von Objekten, zum Beispiel Zahlen.
Eine bestimmte Menge kann ein bestimmtes Objekt enthalten oder nicht.

$x$ ist ein Element von $A$ wenn es in $A$ enthalten ist.
!!! note "Schreibweise" 
    Eine Menge $A$ die die Zahlen $1$, $2$ und $3$ enthält, wird geschrieben als
    $A = \{1, 2, 3\}$.<br>
    $x$ ist ein Element von $A$ wird geschrieben als $x \in A$.<br>
    $x \notin A$ bedeutet das $x$ **kein** Element von $A$ ist.<br>
    Große Mengen werden außerdem als $\{x \in M | P(x) \}$ geschrieben,
    was synonym für "Alle Elemente aus M für die die Aussage P wahr ist" ist.

Die leere Menge $\emptyset$ enthält keine Elemente.<br>
Reihenfolge und mehrfach enthaltene Elemente spielen keine Rolle, es geht
immer um die Frage ob Element $x$ in der Menge enthalten ist oder nicht.

Zwei Mengen $A$ und $B$ sind gleich wenn für jedes Objekt $x$ gilt:
wenn $x \in A$ dann $x \in B$ und wenn $x \in B$ dann $x \in A$.

$A$ ist eine Teilmenge von $B$ und $B$ Obermenge von $A$ wenn jedes Element
von $A$ auch in $B$ enthalten ist. 

!!! note "Schreibweise"
    $A$ ist eine Teilmenge von $B$ wird geschrieben als $A \subseteq B$ oder
    $B \supseteq A$
Folglich ist $A = B$ wenn $A \subseteq B$ und $B \subseteq A$.

A wird genau dann eine **echte Teilmenge** genannt wenn $A \subseteq B$ aber $A \neq B$.

!!! note "Schreibweise"
    Eine echte Teilmenge wird notiert als $A \subsetneq B$ oder $A \subset B$

## Vereinigung und Durchschnitt
Eine Vereinigungsmenge $A \cup B$ enthält sowohl alle Elemente aus $A$ als auch aus $B$.<br>
Beispiel: $\{1, 2, 3\} \cup \{3, 4, 5\} = \{1, 2, 3, 4, 5 \}$<br>

Eine Schnittmenge $A \cap B$ enthält alle Elemente aus $A$ die auch in $B$ enthalten sind.<br>
Beispiel: $\{1, 2, 3\} \cap \{3, 4, 5\} = \{3\}$<br>

Zwei Mengen $A$ und $B$ werden als **disjunkt** bezeichnet wenn $A \cap B = \emptyset$

Für alle Mengen $A$, $B$ und $C$ gilt:

* $A \cup A = A$ und $A \cap A = A$ (Idempotenz von $\cup$ und $\cap$)
* $A \cup B = B \cup A$ und $A \cap B = B \cap A$ (Kommutativität von $\cup$ und $\cap$)
* $(A \cup B) \cup C = A \cup (B \cup C)$ und $(A \cap B) \cap C = A \cap (B \cap C)$ (Assoziativität von $\cup$ und $\cap$)
* $(A \cup B) \cap C = (A \cap C) \cup (B \cap C)$ und $(A \cap B) \cup C = (A \cup C) \cap (B \cup C)$ (Distributivität von $\cup$ und $\cap$)
* $A \subseteq A \cup B$ und $A \cap B \subseteq A$

Die Differenz zweier Mengen $A$ und $B$ wird geschrieben als $A \\ B$, das heißt "Alle Elemente aus
$A$ die nicht in $B$ enthalten sind".

## Kardinalität
Die Kardinalität einer Menge $A$ beschreibt die Anzahl ihrer Elemente, wird vorerst nur für 
endliche Menge definiert. Notiert wird diese als $|A|$.
**Beispiele**

* $|\emptyset| = 0$
* $|\{1,2,3\}| = 3$
* $|\{1,2,3,3,3\}| = 3$

Für alle endlichen Mengen $A$ und $B$ gilt<br>
$|A \cup B| = |A| + |B| - |A \cap B|$

## Paare
Es seien $A$ und $B$ zwei Mengen und $a \in A$ und $b \in B$.
Das Tupel $(a, b)$ wird ein paar genannt sind.
Zwei Paare $(a_1, b_1)$ und $(a_2, b_2)$ sind genau dann gleich wenn
$a_1 = a_2$ und $b_1 = b_2$.

Das kartesische Produkt $A \times B = \{(a, b) | a \in A \land b \in B\}$<br>
Verallgemeinerung mit mehr Menge, zum Beispiel drei:
$M_1 \times M_2 \times M_3 = \{(m_1, m_2, m_3) | m_1 \in M_1 \land m_2 \in M_2 \land m_3 \in M_3\}$.
<br>
Außerdem gilt $M^{2} = M \times M$.
Da $|\emptyset| = 0$ gilt $A \times \emptyset = \emptyset$

## Relationen
Relationen sind Teilmengen aller Paare, das heißt $R \subseteq A \times B$ ist eine Relation.

### Eigenschaften

* $R$ ist linkstotal, wenn für jedes $a \in A$ ein $b \in B$ existiert mit $(a, b) \in R$
* $R$ ist rechtseindeutig oder surjektiv, wenn es für kein $a \in A$ zwei $b_1 \in B$ und $b_2 \in B$ mit $b_1 \neq b_2$ gibt, so dass $(a, b_1) \in R$ und $(a, b_2) \in R$.
* $R$ ist rechtstotal wenn $\forall b \in B \exists a \in A: (a, b) \in R$.
* $R$ ist linkseindeutig oder injektiv wenn $\forall b \in B$ **höchstens** ein $a \in A$ existiert, sodass $(a, b) \in R$.

Relationen die linkstotal und rechtseindeutig sind heißen **Abbildungen** oder **Funktionen**. Sie
werden als bijektiv bezeichnet.

## Abbildungen
Abbildungen sind bijektive Relationen. Sie werden wie folgt definiert:
$f: A \rightarrow B, n \rightarrow F(n)$.

## Potenzmengen 
Potenzmengen sind alle Teilmengen einer Menge.<br>
Sie wird geschrieben als $2^M$ oder $P(M)$.

## Beweisschema: Gleichheit von Mengen
Da die Identität einer Menge allein durch ihre Elemente gegeben ist, kann $A=B$ bewiesen werden
indem gezeigt wird dass $A \subseteq B$ und $B \subseteq A$.

## Menge von Abbildungen
Für $A, B$ ist $A^B = \{f | f$ Abb. von $A$  nach $B \}$ also die Menge aller Abbildungen von $A$ nach $B$.	


