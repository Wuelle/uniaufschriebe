# Reelle Zahlen
## Körperaxiome

1. $\forall a, b, c \in \mathbb{R}: a+(b+c)=(a+b)+c$
2. $\exists 0 \in \mathbb{R} \forall a \in \mathbb{R}: a+0=a$
3. $\forall a \in \mathbb{R} \exists -a \in \mathbb{R}: a + (-a)=0$
4. $\forall a, b \in \mathbb{R}: a+b=b+a$
5. $\forall a, b, c \in \mathbb{R}: a\times(b \times c) = (a \times b ) \times c$
6. $\exists 1 \in \mathbb{R} \forall a \in \mathbb{R}: a \times 1 = a \land 1 \neq 0$
7. $\forall a \in \mathbb{R}\\{0} \exists a^{-1} \in \mathbb{R}: a \times a^{-1} = 1$
8. $\forall a, b \in \mathbb{R}: a \times b = b \times a$
9. $\forall a, b, c \in \mathbb{R}: a \times (b+c) = a \times b + a \times c$

!!! note "Schreibweise"
	Für $a, b \in \mathbb{R}: a-b := a+(-b)$<br>
	Falls auch $b \neq 0: \frac{a}{b} := a \times b^{-1}$

### Beispiel 1
Behauptung: Es gibt genau eine Null in $\mathbb{R}$<br>
Beweis: Nehmen wir an es sei $\tilde{O} \in \mathbb{R}$ mit $\forall a \in \mathbb{R}: a + \tilde{O} = a$.
Mit $a = 0$ folgt dass $0 + \tilde{O} = 0$. Außerdem gilt nach 2. $\tilde{O} + 0 = \tilde{O}$.
Also ist $0 = 0 + \tilde{O} = \tilde{O} + 0 = \tilde{O}$.<br>
Folglich ist jedes additiv neutrale Element $0$, daher gibt es nur eine Null in $\mathbb{R}$.

### Beispiel 2
Behauptung: $\forall a \in \mathbb{R}: a \times 0 = 0$<br>
Beweis: bei $a \in \mathbb{R}$ und $b: a \times 0$. 
Es gilt: $b = a \times (0 + 0) = a \times 0 + a \times 0 = b + b$.
Damit ist $0 = b + (-b)$ dasselbe wie $(b+b) + (-b) = b + (b + (-b)) = b + 0 = b$.

## Anordnungsaxiome
10. $\forall a, b \in \mathbb{R}: a \leq \lor b \leq a$
11. $(a \leq b) \land (b \leq a) \implies a = b$
12. $(a \leq b) \land (b \leq c) \implies a \leq c$
13. $(a \leq b) \land c \in \mathbb{R} \implies a + c \leq b + c$
14. $(a \leq b) \land (0 \leq c) \implies a \times c \leq b \times c$

!!! note "Schreibweise"
	* $b \geq a :\leftrightarrow a \leq b$
	* $a < b :\leftrightarrow (a \leq b) \land (a \neq 0)$
	* $b > a :\leftrightarrow a < b$

### Beispiel 1
Behauptung: $(a < b) \land (0 < c) \implies (a \times c) < (b \times c)$

### Beispiel 2 
Behauptung: $(a \leq b) \land (c \leq 0) \implies (a \times c) \geq (b \times c)$

### Beispiel 3
Behauptung: $(a \leq b) \land (c \leq d) \implies (a + b) \leq (b + d)$<br>
Beweis: $(a \leq b) \land (c \leq d) \implies (a + c) \leq (b + c) \land (c + b) \leq (d + b)$<br>
Nach 12. folgt $a + c \leq b + d$

## Der Betrag
Für $a \in \mathbb{R}$ heißt $|a| := 
\left\{
	\begin{array}{ll}
		a  & \mbox{if } a \geq 0 \\
		-a & \mbox{if } a < 0
	\end{array}
\right.$
<br>
Für $a, b \in \mathbb{R}$ heißt $|a-b|$ der Abstand von $a$ und $b$.

Beispiele:

* $|1| = 1$<br>
* $|-7| = -(-7)=7$

### Rechenregeln
Für $a, b \in \mathbb{R}$ gilt:

1. $|-a| = |a|$ und $|a-b| = |b-a|$
2. $|a| \geq 0$ 
3. $|a| = 0 \leftrightarrow a = 0$
4. $|a \times b| = |a| \times |b|$
5. $|\pm a \leq |a|$
6. $|a+b| \leq |a| + |b|$ (**wichtig**)
7. $||a|-|b|| \leq |a-b|$

Beweis von 6:<br>
Fall 1: $a + b \geq 0$. Dann gilt $|a+b| = a+b \leq |a| + |b|$<br>
Fall 2: $a + b < 0$. Dann gilt $|a+b| = -(a+b) = (-a) + (-b) \leq |a| + |b|$<br>

Beweis von 7:<br>
Sei $c := |a| - |b|$. Es gilt: $|a| = |(a - b) + b| \leq |a - b| + |b|$<br>
Daraus folgt:<br>
$|a| - |b| \leq |a - b|$<br>
Analog zeigt man:<br>
$-c = |b| - |a| \leq |b - a| = |a - b|$<br>
Also $\pm c \leq | a - b |$<br>

Daraus folgt $|c| \leq |a - b|$.<br>

## Definitionen
Sei $M \subseteq \mathbb{R}$

* $M$ heißt **nach oben beschränkt** $:\leftrightarrow \exists \gamma \in \mathbb{R} \forall x \in M: x \leq \gamma$.
IdF. heißt $\gamma$ eine **obere Schranke** von $M$.

* Ist $\gamma$ eine o.S von $M$ und gilt $\gamma \leq \delta$ für jede o.S $\delta$ von $M$, so heißt $\gamma$ das **Supremum** von $M$. 

* $M$ heißt **nach unten beschränkt** $:\leftrightarrow \exists \gamma \in \mathbb{R} \forall x \in M: x \geq \gamma$.
IdF heißt $\gamma$ eine **untere Schranke** von $M$.

* Ist $\gamma$ eine u.S von $M$ und gilt $\gamma \geq \delta$ für jede u.S $\delta$ von $M$, so heißt
$\gamma$ das **Infimum** von $M$. 

!!! note "Schreibweise" 
	$\gamma = \sup M$ bzw $\gamma = \inf M$

## Intervalle
Es seien $a, b \in \mathbb{R}: a < b$.<br>
$[a, b] := \{x \in \mathbb{R}:  a \leq x \leq b\}$<br>
$(a, b) := \{x \in \mathbb{R}:  a < x < b\}$<br>
$(a, b] := \{x \in \mathbb{R}:  a < x \leq b\}$<br>
$[a, b) := \{x \in \mathbb{R}:  a \leq x < b\}$<br>
$[a, \infty) := \{x \in \mathbb{R}:  x \geq a\}$<br>
$(a, \infty) := \{x \in \mathbb{R}:  x > a\}$<br>
$(-\infty, a] := \{x \in \mathbb{R}:  x \leq a\}$<br>
$(-\infty, a) := \{x \in \mathbb{R}:  x < a\}$<br>
$(-\infty, \infty) := \mathbb{R}$<br>

Ist $\sup M$ bzw. $\inf M$ vorhanden und gilt $\sup M \in M$ bzw $\inf M \in M$ so heißt $\sup M$ das Maximum
bzw $\inf M$ das Minimum von $M$.

!!! note "Schreibweise"
	$\min M$ bzw $\max M$.<br>

### Beispiel
Es sei $M = (1, 2)$. Es ist $\sup M = 2 \notin M$ und $\inf M = 1 \notin M$, dh $M$ hat kein Maximum und kein Maximum.

Weitere Beispiele

* $M = (1, 2]$. Hier $\sup M = 2 \in M$ also ist $\max M = 2$
* $M = (3, \infty)$. Hier ist $M$ nach oben unbeschränkt. $\inf M = 3 \notin M$ also hat $M$ weder Minimum noch Maximum.
* $M = \emptyset$. Jedes $\gamma \in \mathbb{R}$ ist eine u.S und eine o.S von $M$.

## Vollständigkeitsaxiom
15. Ist $\emptyset \neq M \subseteq \mathbb{R}$ und ist $M$ nach oben beschränkt, so ist $\sup M$ vorhanden.

!!! note "Satz 1.1"
	Ist $\emptyset \neq M \subseteq \mathbb{R}$ und $M$ ist nach unten beschränkt, so ist $\inf M$ vorhanden.
	Beweis folgt in der Übung.

Es sei $M \subseteq \mathbb{R}$. $M$ heißt **beschränkt** $:\leftrightarrow$ $M$ ist nach oben und nach unten beschränkt.
Äquivalent ist folgende Eigenschaft: $\exists c \geq 0 \forall x \in M: |x| \leq c$

!!! note "Satz 1.2"
	Sei $\emptyset \neq B \subseteq A \subseteq \mathbb{R}$. Es gelten folgende Aussagen:

	* Wenn $A$ beschränkt ist, dann ist $\inf M \leq \sup M$.
	* Wenn $A$ nach oben bzw. nach unten beschränkt ist, so ist $B$ ebenfalls nach oben bzw. unten beschränkt und $\sup B \leq \sup A$ und $\inf B \geq \inf A$.
	* $A$ sei nach oben beschränkt und $\gamma$ sei eine o.S von $A$. Dann gilt $\gamma = \sup A \leftrightarrow \forall \epsilon > 0 \exists x \in A: x > \gamma - \epsilon$
	* $A$ sei nach unten beschränkt und $\gamma$ eine u.S von $A$. Dann gilt $\gamma = \inf A \leftrightarrow \forall \epsilon > 0 \exists x \in A: x < \gamma + \epsilon$


*[IdF]: In diesem Fall
*[o.S]: Obere Schranke
*[u.S]: Untere Schranke
*[dh]: das heißt
*[bzw]: beziehungsweise
*[I.M]: Induktionsmenge
