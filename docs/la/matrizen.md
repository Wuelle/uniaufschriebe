# Matrizen
## Definition
Es seien $m, n \in \mathbb{N}$ und $\mathbb{K}$ ein Körper.
Eine **Matrix** über $\mathbb{K}$ mit $m$ Zeilen und $n$ Spalten, kurz eine $m \times n$ Matrix,
ist ein rechteckiges Schema mit $m$ Zeilen und $n$ Spalten. Die einzelnen Einträge der Matrix heißen **Komponenten**.

!!! hint "Merksatz"
	Die Reihenfolge der Indizes kann man sich mit dem Merksatz "**Z**eile **z**uerst, **S**palte **s**päter"
	merken.

Die Menge aller $m \times n$  Matrizen über $\mathbb{K}$ wird auch als $\mathbb{K}^{m \times n}$ geschrieben.

## Rechenoperationen
### Addition
Es wird komponentenweise addiert. Also ist $\mathbb{K}^{m \times n}, +)$ eine abelsche Gruppe.

### Multiplikation
#### Vorraussetzungen
Zwei Matrizen $A$ und $B$ können nur miteinander multipliziert werden wenn folgende Bedingungen erfüllt sind:

* Die Anzahl der Spalten von $A$ muss die Anzahl der Zeilen von $B$ sein.
* $A$ und $B$ müssen Matrizen über den selben Körper sein. Also $A \in \mathbb{K}^{p \times q}$ und $B \in \mathbb{K}^{q \times r}$. Dann ist das Resultat $C \in \mathbb{K}^{p \times r}$


#### Rechnung
Um das Element $c_{jk}$ des Matrixprodukts $C$ zu berechnen, wird das Skalarprodukt der $j$-ten Zeile aus $A$ und der $k$-ten Spalte aus $B$ berechnet.

Die Matrixmultiplikation ist nur dann eine Verknüpfung wenn sie mit quadratischen Matrizen gleicher Größe durchgeführt wird. Dann
ist das neutrale Element die sogenannte **Einheitsmatrix**, eine Nullmatrix bei der die Diagonale mit Einsen besetzt ist.

#### Multiplikativ Neutral
Das multiplikativ neutrale Element ist die sogenannte **Einheitsmatrix**. Sie besteht aus Nullen, wobei auf der Diagonalen Einsen stehen.

#### Multiplikativ Invers
Eine Matrix $A$ besitzt nicht immer ein multiplikativ Inverses $A^{-1}$, sodass $A \times A^{-1} = E$. Existiert das Inverse, so heißt die $A$ **invertierbar**.
Demnach bilden alle invertierbaren Matrizen mit denselben Dimensionen eine Gruppe bezüglich der Multiplikation.
Die Menge aller invertierbaren Matrizen aus $\mathbb{K}^{n \times n}$ wird als $GL(n, \mathbb{K})$ geschrieben. Sie heißt **allgemeine lineare Gruppe**. (general linear group)
Es gilt: $(A \times B)^{-1} = B^{-1} \times A^{-1}$.

### Transposition
Bei der Transposition werden die Indizes einer Matrix vertauscht. Aus einer $m \times n$ Matrix wird also eine $n \times m$ Matrix.
Die Matrix $A$ wird transponiert geschrieben als $A^T$.<br>
Es gilt:

* $(A + B)^T = A^T + B^T$
* $(A \times B)^T = A^T \times B^T$
* $(A^T)^T = A$
* Für alle invertierbaren $A$ gilt: $(A^T)^{-1} = (A^{-1})^T$


