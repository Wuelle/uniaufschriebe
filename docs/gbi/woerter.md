# Alphabete und Wörter
## Alphabet
Ein Alphabet ist eine endliche, nichtleere Menge aus Zeichen oder Symbolen, zb Unicode, ASCII oder Dezimalzahlem.
## Wort
Ein Wort aus einem Alphabet $A$ ist eine Folge aus Zeichen aus $A$. Anders als bei einer
Menge ist die Reihenfolge der Zeichen relevant.

Definiere für $n \in \mathbb{N}_0$ Menge der $n$ kleinsten nichtnegativen ganzen Zahlen.<br>
$\mathbb{Z}_n = \{i \in \mathbb{N}_0 | 0 \leq i$ und $i < n\}$<br>

Ein Wort aus dem Alphabet $A$ ist eine surjektive Abbildung $w: \mathbb{Z}_n \rightarrow B$ mit
$B \subseteq A$.<br>
$n$ heißt **die Länge** eines Wortes, geschrieben als $|w|$.<br>
$A^n$ ist die Menge aller Wörter mit $n$ Zeichen aus $A$.<br>
Die Menge $A^*$ ist die Menge aller Wörter die aus dem Alphabet $A$ gebildet werden können.<br>
Immer enthalten ist $\epsilon$, das leere Wort.

### Das leere Wort
Das leere Wort ist vergleichbar mit der leeren Menge. Es besteht aus $0$ Symbolen und wird als
$\epsilon$ geschrieben.<br>
$\epsilon: \mathbb{Z}_0 \rightarrow \{\}$ also $\epsilon: \{\} \rightarrow \{\}$.<br>
**ABER:**<br>
Das leere Wort ist nicht die leere Menge. $|\{\epsilon\}| = 1$.

## Konkatenation von Wörtern
Wörter können aneinandergeschrieben werden, üblicherweise mit dem Operatorsymbol $\cdot$.<br>
$SCHRANK \cdot FACH = SCHRANKFACH$. Das leere Wortist das neutrale Element der Konkatenation,
also $SCHRANK \cdot \epsilon = SCHRANK$. 
Konkatenation ist **assoziativ**, aber nicht **kommutativ**.<br>
$w^n = w \cdot \w \cdot \ldots \cdot \w$.




*[zb]: zum Beispiel
*[ASCII]: American Standard Code for Information Interchange