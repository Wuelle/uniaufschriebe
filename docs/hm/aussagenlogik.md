# Aussagenlogik

## Definition einer Aussage
Eine Aussage ist eine Feststellung stets entweder wahr oder falsch ist.
Beispiele für Aussagen:

* $1 = 1$
* $1 = 0$
* $3x^{2} = 2$
* "Dieser Hund ist braun"

Beispiele die keine Aussagen sind:

* $5x^{3}+3$

## Operatoren
Aussagen können durch Operatoren zu neuen Aussagen verknüpft werden.

| Name          | Schreibweise         | Umgangssprachlich                          |
| ------------- | -------------------- | ------------------------------------------ |
| Negation      | $\neg A$             | **nicht** $A$                              |
| Konjunktion   | $A\land B$           | $A$ **und** $B$                            |
| Disjunktion   | $A\lor B$            | $A$ **oder** $B$                           |
| Implikation   | $A\implies B$        | Aus $A$ folgt $B$                          |
| Äquivalenz    | $A\leftrightarrow B$ | Aus $A$ folgt $B$ **und** aus $B$ folgt $A$ |

!!! note
    Seien $A, B$ mathematische Aussagen. Wenn $A\implies B$ gilt, so ist $A$
    eine hinreichende Bedingung für $B$ und $B$ ist eine notwendige Bedingung 
    für $A$.

## De Morgan'sche Regeln
Augustus de Morgan formulierte folgende Regeln zur Umformung von Aussagen:

* $\neg (A\lor B)\leftrightarrow \neg A\land \neg B$
* $\neg (A\land B)\leftrightarrow \neg A\lor \neg B$

### Weitere Regeln

* $A \implies B \leftrightarrow \neg A \lor B$
* $A \implies B \leftrightarrow \neg B \implies \neg A$
* $\neg (A \implies B) \leftrightarrow A \land \neg B$


## Quantoren
Quantoren beschreiben die Existenz von Objekten, sie können benutzt werden um Aussagen
zu formulieren.

| Name            | Schreibweise | Umgangssprachlich |
| --------------- | ------------ | ----------------- |
| Existenzquantor | $\exists$    | Es existiert      |
| Allquantor      | $\forall$    | Für alle          |

Der Existenzquantor $\exists$ kann außerdem mit einem Ausrufezeichen verbunden werden
($\exists!$) um die Existenz **genau eines** Objektes zu spezifizieren.

### Quantorenbeispiel
$\forall x \in \mathbb{R} \exists y \in \mathbb{R}: x < y$
<br>
bedeutet
<br>
"Für jedes Element der Reellen Zahlen gibt es ein weiteres Element der Reellen Zahlen
das größer ist."
