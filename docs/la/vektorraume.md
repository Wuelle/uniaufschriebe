# Vektorräume
## Definition
Sei $\mathbb{K}$ ein Koerper. Eine Menge $V$ mit der Addition<br>
$+: V + V \rightarrow V, (a, b) \righarrow a + b$ <br>
und der skalaren Multiplikation<br>
$\times: \mathbb{K} \times V \rightarrow V, (\lambda, x) \rightarrow \lambda \times x$<br>
heißt $\mathbb{K}$-Vektorraum falls die folgenden Axiome gelten: <br>

* $(V, +)$ ist eine abelsche Gruppe
* für alle $\lambda, \alpha \in \mathbb{K}$ und alle $x, y \in V$ gilt:
    * $1 \times x = x$
    * $\lambda \times (\alpha \times x) = (\lambda \times \alpha) \times x$
    * $(\lambda + \alpha) \times x = \lambda \times x + \alpha \times x$
    * $\lambda \times (x + y) = \lamda \times x + \lambda \times y$

Elemente aus $V$ heißen Vektoren, Elemente aus $\mathbb{K}$ heißen Skalare.
Das Nullelement von $(V, +)$ heißt Nullvektor und wird meistens mit $0_v$ bezeichnet um es
vom Nullelement aus $\mathbb{K}$ zu unterscheiden

Elemente aus dem Vektorraum haben eine bestimme Länge. Die Vereinigung aller 
Vektorlängen heißt $\mathbb{K}^{\mathbb{N}_0}$.

# Verbindung mit Polynomen
Ein Polynom hat eine endliche Menge an Vorfaktoren. Es kann also als Element
von $\mathbb{K}^{\mathbb{N}_0}$ angesehen werden, wobei nur eine endliche Anzahl
an Vofaktoren ungleich $0$ sind.

## Linearkombination
Die Linearkombination beschreibt die Summe von $n$ Vektoren multipliziert mit
einer Konstanten $\lambda_n$. (Einem LGS nicht unähnlich).
Man kann also den Nullvektor als Linearkombination von beliebigen anderen Vektoren
darstellen. (Mit $\lambda_n = 0$). Diese Darstellung heißt **trivial**. Eine
nichttriviale Darstellung des Nullvektors ist nicht immer machbar.

## Lineare Unabhängigkeit
Ein Vektorraum heißt **linear unabhängig** wenn keine nichttriviale Darstellung
des Nullvektors existiert. Ist ein Vektorraum nicht linear unabhängig, so heißt er
**linear abhängig**.<br>

Die leere Menge ist als linear unabhängig definiert.

