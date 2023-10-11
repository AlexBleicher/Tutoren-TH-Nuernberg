# Zahlentheorie

## Grundbegriffe
* Teilbarkeit
* Vielfaches
* Primzahlen
* Primfaktorzerlegung, z.B. $`140 = 2^2 * 5 * 7`$
* Größter gemeinsamer Teiler, z.B. $`ggT(12, 16) = 4`$
* Kleinstes gemeinsames Vielfaches, z.B. $`kgV(12, 16) = 48`$

## Euklidischer Algorithmus

```math
r_0 = a, r_1 = b \\
\text{ }\\

r_0 = q_2 · r_1 + r_2 \\
r_1 = q_3 · r_2 + r_3 \\
...\\
r_{n−2} = q_n · r_{n−1} + r_n \\
r_{n−1} = q_{n+1} · r_n + 0 \\
\text{ }\\

\Rightarrow ggT(a,b) = r_n
```

## Erweiterter euklidischer Algorithmus

```math
x_0 = 1, x_1 = 0, y_0 = 0, y_1 = 1 \\
\text{ }\\
x_2 = x_0 - q_2 * x_1\\
x_3 = x_1 - q_3 * x_2\\
x_4 = x_2 - q_4 * x_3\\
...\\
x_n = x_{n-2} - q_n * x_{n-1}\\
\text{ }\\
y_2 = y_0 - q_2 * y_1\\
y_3 = y_1 - q_3 * y_2\\
y_4 = y_2 - q_4 * y_3\\
...\\
y_n = y_{n-2} - q_n * y_{n-1}\\
\text{ }\\
\Rightarrow a * x_n + b * y_n = ggT(a,b)
```

## Diophantische Gleichungen

```math
a*x+b*y = c * ggT(a,b) \\
a, b, c \in \Z, (a,b) \ne (0,0)
```

1. Prüfen, ob Ergebnis durch $`ggT(a,b)`$ teilbar ist
1. Erweiterten euklidischen Algorithmus ausführen
1. $`x_n`$ und $`y_n`$ mit $`c`$ multiplizieren => Erste Lösung $`x'`$ und $`y'`$
1. Alle Lösungen berechnen

```math
x = x' + \frac{b}{ggT(a,b)} * k, y = y' - \frac{a}{ggT(a,b)} * k, k \in \Z
```

# Aufgaben

## Aufgabe 1

Zerlege in Primfaktoren:

1. $`100`$
1. $`1234`$
1. $`42`$
1. $`37`$


## Aufgabe 2

Berechne mit Hilfe des euklidischen Algorithmus:

1. $`ggT(12, 16)`$
1. $`ggT(20, 100)`$
1. $`ggT(336, 315)`$
1. $`ggT(648, 140)`$
1. $`ggT(1896, 2765)`$
1. $`ggT(168, 245)`$
1. $`ggT(336, 1960)`$
1. $`ggT(546, 104)`$

## Aufgabe 3

Berechne, falls möglich, mit Hilfe des erweiterten euklidischen Algorithmus:

1. $`12 * x + 16 * y = 4`$
1. $`12 * x + 16 * y = 32`$
1. $`12 * x + 16 * y = 5`$
1. $`648 * x + 140 * y = 16`$
1. $`1480 * x + 2109 * y = 333`$
1. $`1140 * x + 3325 * y = 285`$
1. $`10 * x + 20 * y = 5`$
1. $`1896 * x + 2765 * y = 395`$
1. $`168 * x + 245 * y = 42`$
1. $`336 * x + 1960 * y = 560`$
1. $`546 * x + 104 * y = 26`$