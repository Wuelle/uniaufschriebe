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

!!! hint "Sath 2.2"
	Seien $(a_n), (b_n), (c_n), (\alpha _n)$ Folgen und $a, b, \alpha \in \mathbb{R}$.

	* $(a_n) \rightarrow a \leftrightarrow |a_n - a| \rightarrow 0$
	* Gilt $|a_n - a| \leq \alpha _n$ ffa $n \in \mathbb{N}$ und $\alpha _n \rightarrow 0$ so gilt $a_n \rightarrow a$

	* Es gelte $a_n \rightarrow a$ und $b_n \rightarrow b$. Dann gilt $|a_n| \rightarrow |a|$ und $a_n + b_n \rightarrow a + b$. Außerdem gilt $\alpha \times a_n \rightarrow \alpha \times a$ und $a_n \times b_n \rightarrow a \times b$. Ist $a \neq 0$ dann existiert ein $m \in \mathbb{N}$ mit $a_n \neq 0$ für $n \geq m$ und für die Folge $\frac{1}{a_n}$ mit $m \leq n \leq \infty$ gilt $\frac{1}{a_n} \rightarrow \frac{1}{a}$.
	* Es gelte $a_n \rightarrow a$ und $b_n \rightarrow b$ und $a_n \leq b_n$ ffa $n \in \mathbb{N}$. Dann ist $a \leq b$.
	* Es gelte $a_n \rightarrow a$ und $b_n \rightarrow a$ und $a_n \leq c_n \leq b_n$ ffa $n \in \mathbb{N}$. Dann gilt $c_n \rightarrow a$

## Monotoniekriterium
$(a_n)$ heißt **monoton wachsend** wenn $\forall n \in \mathbb{N}: a_n \leq a_{n+1}$.<br>
$(a_n)$ heißt **monoton fallend** wenn $\forall n \in \mathbb{N}: a_n \geq a_{n+1}$.<br>
$(a_n)$ heißt **streng monoton wachsend** wenn $\forall n \in \mathbb{N}: a_n < a_{n+1}$.<br>
$(a_n)$ heißt **streng monoton fallend** wenn $\forall n \in \mathbb{N}: a_n > a_{n+1}$.<br>

!!! hint "Satz 2.3"
	
	* $(a_n)$ sei wachsend und nach oben beschränkt. Dann ist $(a_n)$ konvergent und $\lim a_n = \sup a_n$.
	* $(a_n)$ sei fallend und nach unten beschränkt. Dann ist $(a_n)$ konvergent und $\lim a_n = \inf a_n$.

## Teilfolgen
Sei $(a_n)$ eine Folge und $(n_k)$ eine Folge in $\mathbb{N}$ die streng monoton wächst. Setze
$b_k = a_{n_k}$ mit $k \in \mathbb{N}$. Dann heißt $(b_k)$ eine **Teilfolge** von $(a_n)$.<br>
Zum Beispiel könnte man dadurch jedes Zweite Element einer Folge erhalten.<br>
Eine Zahl $\alpha \in \mathbb{R}$ heißt **Häufungswert** von $(a_n)$, wenn eine TF $(a_{n_k})$ existiert
mit $a_{n_k} \rightarrow \alpha$. Die Menge $H(a_n)$ ist definiert als die Menge aller Häufungswerte
von $(a_n)$.

!!! hint "Satz 2.10"
	Es gilt $\alpha \in H(a_n) \leftrightarrow \forall \epsilon > 0: a_n \in U_{\epsilon}(\alpha)$ für unendlich
	viele $n \in \mathbb{N}$.

!!! hint "Satz 2.11"
	Die Folge $(a_n)$ sei gegen $a$ konvergent und $(a_{n_k})$ sei eine TF von $(a_n)$. Dann
	gilt auch $(a_{n_k}) \rightarrow a$.

Jede Folge besitzt entweder monoton wachsende oder monoton fallende Teilfolgen. (Siehe Skript)

!!! hint "Satz 2.13 (Bolzano-Weierstrauß)"
	Die Folge $(a_n)$ sei beschränkt. Dann ist $H(a_n) \neq \emptyset$.
	Folglich besitzt

!!! hint "Satz 2.14"
	Sei $(a_n)$ eine beschränkte Folge. Also ist nach 2.13 $H(a_n) \neq \emptyset$.
	Es gilt

		* Die Menge der Häufungswerte ist beschränkt 
		* $\sup H(a_n) \in H(a_n)$ und $\inf H(a_n) \in H(a_n)$

$\max H(a_n)$ wird $\limsup a_n$ (und $\min H(a_n)$ $\liminf a_n$) genannt.

## Cauchy-Folge
Eine Folge $(a_n) heißt **Cauchy Folge** $\leftrightarrow \forall \epsilon > 0: \exists n_0 \in \mathbb{N} \forall m, n \geq n_0: |a_m - a_n| < \epsilon$. Konvergente Folgen sind immer Cauchy Folgen und Cauchy Folgen sind
immer konvergent.


*[ffa]: für fast alle
*[TF]: Teilfolge
*[HW]: Häufungswert