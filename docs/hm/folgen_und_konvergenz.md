# Folgen und Konvergenz
## Definition einer Folge
Sei $X$ eine Menge, $X \neq \emptyset$. Eine Funktion $a: \mathbb{N} \rightarrow X$ heißt eine **Folge** in $X$.
Ist $X = \mathbb{R}$, so heißt $X$ eine reelle Folge.

!!! note "Schreibweise"
	$a_n$ statt $a(n)$. Dabei ist $a_n$ das n-te Folgenglied.

**Anmerkung:** Ist $p \in \mathbb{Z}$ und $a: \{p, p+1, p+2, \ldots \} \rightarrow X$ eine Funktion
so nennt man sie ebenfalls eine Folge.

## Bildmenge
Die Bildmenge ist die Zielmenge der Folge. Ist also $(a_n)$ eine Folge so ist die Bildmenge
$M = \{a_1, a_2, a_3,\ldots \}$.

## Begriffsdefinitionen
Sei $X$ eine Menge, $X \neq \emptyset$.
* $X$ heißt **abzählbar** wenn es eine Folge $(a_n)$ in $X$ mit $X=\{a_1, a_2, \ldots \}$ gibt.
* $X$ heißt **überabzählbar** wenn $X$ nicht abzählbar ist.

Ist $X$ endlich, so ist $X$ abzählbar.<br>
$\mathbb{N}$ ist abzählbar, denn $\mathbb{N} = \{a_1, a_2, \ldots \}$ mit $a_n = n$ mit $n \in \mathbb{N}$.<br>
$\mathbb{Z}$ ist abzählbar, denn $\mathbb{Z} = \{a_1, a_2, \ldots \}$ mit $a_1 = 0$ und $a_{2n} = n$ und $a_{2n+1} = -n$ für alle $n \in \mathbb{N}$.<br>
$\mathbb{Q}$ ist abzählbar.<br>
$\mathbb{R}$ ist überabzählbar.<br>

Sei $(a_n)$ eine Folge und $M$ die Bildmenge von $(a_n)$.

* $(a_n)$ heißt **nach oben beschränkt** wenn $M$ nach oben beschränkt ist. $\sup a_n = \sup M$.
* $(a_n)$ heißt **nach unten beschränkt** wenn $M$ nach unten beschränkt ist. $\inf a_n = \inf M$.
* $(a_n)$ heißt **beschränkt** wenn $M$ beschränkt ist.

!!! note "Definition"
	Sei $A(n)$ eine $n \in \mathbb{N}$ definierte Aussage. $A(n)$ gilt für **fast** alle $n \in \mathbb{N}$ bedeutet
	$\exists n_0 \in \mathbb{N} \forall n \geq n_0: A(n)$ ist wahr. (also ist $A(N)$ nur für eine endliche Menge $n$ unwahr)

!!! note "Definition"
	Es sie $a \in \mathbb{R}$ und $\epsilon > 0$. Das Intervall $U_{\epsilon}(a) := (a-\epsilon, a+\epsilon)$
	heißt $\epsilon$-Umgebung von $a$.

## Konvergenz und Divergenz
Eine Folge $(a_n)$ heißt **konvergent** wenn $\exists a \in \mathbb{R}: \forall \epsilon > 0 \exists n_0 \in \mathbb{N}: \forall n \in \mathbb{N}| n \geq n_0: |a_n - a| < \epsilon$.
<br>
In Worten: Eine Folge ist konvergent wenn sie ab einer bestimmten Stelle $n_0$ die $\epsilon$-Umgebung eines
Grenzwerts $a$ nicht mehr verlässt., das heißt $a_n \in U_{\epsilon}(a)$ ffa $n \in \mathbb{N}$. Konvergenz kann auch so geschrieben werden: $a_n \rightarrow a$ für $n \rightarrow \infty$.
<br>
Ist $(a_n)$ nicht konvergent, so nennt man sie divergent.

!!! hint "Satz 2.1"
	Sei $(a_n)$ konvergent und $a := lim a_n$. Dann 

	* Gilt auch noch $a_n \rightarrow b$ so ist $a = b$.
	* $(a_n)$ ist beschränkt

## Rechenoperationen
Seien $(a_n)$ und $(b_n)$ Folgen in $\mathbb{R}$.<br>
$(a_n) \pm (b_n) := (a_n \pm b_n)$.<br>
$\alpha \times (a_n) = (\alpha \times a_n)$.<br>
$(a_n) \times (b_n) := (a_n \times b_n)$.<br>
Ist $b_n \neq 0$ so ist $\frac{(a_n)}{(b_n)}$ definiert.<br>



*[ffa]: für fast alle