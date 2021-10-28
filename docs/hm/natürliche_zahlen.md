## Natürliche Zahlen
Eine Menge $A \subseteq \mathbb{R}$ heißt Induktionsmenge wenn $1 \in A$ und $x \in A \implies (x + 1) \in A$.<br>
Die natürlichen Zahlen N sind definiert als $\mathbb{N} := \{x \in \mathbb{R}: x$ gehört zu jeder I.M $\}$.
Also $\mathbb{N} \subseteq A$ für jede I.M $A$.

!!! note "Satz 1.3"

	* $\mathbb{N}$ ist eine I.M.
	* $\mathbb{N}$ ist nicht nach oben beschränkt.
	* Ist $x \in \mathbb{R}$, so existiert ein $n \in \mathbb{N}$ mit $n > x.

!!! note "Satz 1.4 (Prinzip der vollständigen Induktion)"
	Ist $A \subseteq \mathbb{N}$ und ist $A$ eine I.M. so ist $A = \mathbb{N}$,<br>
	da $A \subseteq \mathbb{N}$ und $\mathbb{N} \subseteq A$ gilt.

## Beweis durch vollständige Induktion
Es sei $A(n)$ eine Aussage, die für jedes $n \in \mathbb{N}$ definiert ist. Für $A(n)$ gelte:<br>

1. $A(1)$ ist wahr
2. Ist $n \in \mathbb{N}$ und $A(n)$ wahr, so ist $A(n+1)$ wahr.
Dann ist $A(n)$ wahr für alle $n \in \mathbb{N}$.
!!! tip "Beweis"
	Es sei $A := \{n \in \mathbb{N}: A(n)\}$. Dann ist $A \subseteq \mathbb{N}$ und wegen 1. und 2. ist $A$ eine Induktionsmenge.
	Nach Satz 1.4 ist $A$ folglich $\mathbb{N}$.

Beispiel: Es wird behauptet $\forall n \in \mathbb{N}: 1+2+3+4+...+n = \frac{n\times(n+1)}{2}$.
Induktionsanfang: Es gilt: $1 = \frac{1 \times (1+1)}{2}$. Also ist $A(1)$ wahr.<br>
Induktionsvoraussetzung: Es sein $n \in \mathbb{N}$ und $A(n)$ sei wahr.<br>
Induktionsschluss: Es gilt $1 + 2 + ... + n + (n+1) = \frac{n \times (n+1)}{2} + (n+1) = (n+1) \times (\frac{n}{2} + 1) = \frac{(n+1) \times (n+2)}{2}$

!!! note "Definitionen"

	* $\mathbb{N}_0 := \mathbb{N} \cup \{0\}$
	* $\mathbb{Z} := \mathbb{N0} \cup {-n: n \in \mathbb{N}}$
	* $\mathbb{Q}: \{\frac{p}{q}: p \in \mathbb{Z}, q \in \mathbb{N}\}$

!!! hint "Satz 1.5"
	Sind $x, y \in \mathbb{R}$ mit $x < y$, so gilt: $\exists r \in (x,y) \cap \mathbb{Q}$.
	In Worten: Zwischen jeden zwei reellen Zahlen existiert eine rationale Zahl.



## Ganzzahlige Potenzen:
 Für $a \in \mathbb{R}, n \in \mathbb{N}$ gilt $a^n = a \times a \times a \ldots \times a$. Und $a^0 = 1$.
Für $a \in \mathbb{R}\\\{0\}, n \in \mathbb{N}$ gilt $a^{-n} = \frac{1}{a^n}$
Rechenregeln: $a^n \times a^m = a^{n+m}$ und $(a^n)^m = a^{n \times m}$

## Fakultäten
$n! = 1 \times 2 \times 3 \times \ldots \times n, n \in \mathbb{N}$ und $0! = 1$.

## Binomialkoeffizienten
Für $n, k \in \mathbb{N}_0, k \leq n$ gilt $\binom{n}{k} = \frac{n!}{k! \times (n-k)!}$
Es gilt $\binom{n}{k} + \binom{n}{k-1} = \binom{n+1}{k}$ für $1 \leq k \leq n$.
* Für $a, b \in \mathbb{R}$ und $n \in \mathbb{N}$ gilt: $(a-b)\times(a^n + a^{n-1}b + a^{n-2}b^2 + \ldots + ab^{n-1} + b^n)$ ist gleich $a^{n+1}-b^{n+1}$. (Ausmultiplizieren!)
Also $a^{n+1}-b^{n+1} = (a-b) \times \Sigma a^{n-k} \times b^k = (a-b) \times \Sigma a^{n} \times b^{n-k}$

### Binomischer Satz
Für $a, b \in \mathbb{R}$ und $n \in \mathbb{N}_0$ gilt $(a+b)^n = \Sigma(\binom{n}{k} \times a^k \times b^{n-k})$.

### Bernoullische Ungleichung
Sei $x \in \mathbb{R}$ und $x \geq -1$. Dann $\forall n \in \mathbb{N}: (1+x)^n \geq 1 + nx$.

!!! hint "Hilfssatz 1.7"
	Für $x, y \geq 0$ und $n \in \mathbb{N}$ gilt: $x \leq y \leftrightarrow x^n \leq y^n$.

!!! hint "Satz 1.7"
	Sei $a \geq 0$ und $n \in \mathbb{N}$. Dann gibt es genau ein $x \geq 0$ mit $x^n =a$. Dann heißt
	$x$ die n-te Wurzel aus $a$.

Außerdem gilt $\forall x \in \mathbb{R}: \sqrt{x^2} = |x|$.<br>
Nach 1.6 folgt: $0 \leq x \leq y, n \in \mathbb{N} \rightarrow \sqrt[n]{x} \leq \sqrt[n]{y}$.

## Rationale Exponenten
### Nichtnegative Basis
Es sei $a \geq 0$ und $r \in \mathbb{Q}, r > 0$. Dann existieren $n, m \in \mathbb{N}$ mit $r = \frac{n}{m}$.
Wir definieren:

* $a^r = (\sqrt[n]{a})^m$.

Problem: ist auch $r = \frac{p}{q}$ mit $p, q \in \mathbb{N}$ gilt dann $(\sqrt[n]{a})^m = (\sqrt[q]{a})^p$?<br>
Beweis: Sei $x = (\sqrt[n]{a})^m$ und $y = (\sqrt[q]{a})^p$. Es gilt $x, y \geq 0$ und $m \times q = n \times p$.<br>
$x^q = (\sqrt[n]{a})^{mq} = (\sqrt[n]{a})^{np} = ((\sqrt[n]{a})^{n})^p = a^p = ((\sqrt[q]{a})^{q})^p = ((\sqrt[q]{a})^{p})^q = y^q$. Nach 1.6 folgt $x=y$.

### Positive Basis
Es sie $a > 0, r \in \mathbb{Q}$ und $r < 0$. Wir definieren $a^r = \frac{1}{a^{-r}}$.
Rechenregeln: $a^n \times a^m = a^{n+m}$ und $(a^n)^m = a^{n \times m}$

*[IdF]: In diesem Fall
*[o.S]: Obere Schranke
*[u.S]: Untere Schranke
*[dh]: das heißt
*[bzw]: beziehungsweise
*[I.M]: Induktionsmenge