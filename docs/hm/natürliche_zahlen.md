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

*[IdF]: In diesem Fall
*[o.S]: Obere Schranke
*[u.S]: Untere Schranke
*[dh]: das heißt
*[bzw]: beziehungsweise
*[I.M]: Induktionsmenge