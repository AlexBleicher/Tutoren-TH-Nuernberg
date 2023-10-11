# Vollständige Induktion 

1. Induktionsanfang
    * Kleinstes Element (z.B. 1 bei $`n \in \N`$) auf beiden Seiten einsetzen und berechnen.
2. Induktionsvoraussetzung
    * Man nimmt an, dass die Aussage für ein *festes* $`n`$ gilt.
3. Induktionsschritt
    * $`n`$ durch $`n+1`$ ersetzen (Induktionsbehauptung)
    * Aus der Summe das letzte Element "herausziehen"
    * Verbleibendes Summenzeichen durch Induktionsvoraussetzung ersetzen
    * Gleichheit zu Induktionsbehauptung zeigen

## Aufgaben

### Aufgabe 1
Zeige durch vollständige Induktion, dass folgende Formel für alle $` n \in \N `$ gilt: 
```math
\sum_{k=1}^{n}{k^2}= \frac{n \cdot (n+1) \cdot (2n+1)}{6}
```

### Aufgabe 2
Zeige durch vollständige Induktion für $`n \in \N \land n \ge 2`$: 

```math
\prod_{k=2}^{n}{(1- \frac{1}{k^2})} = \frac{n+1}{2n}
```

### Aufgabe 3
Zeige durch vollständige Induktion: Für alle $`n \in \N`$ gilt: $`2n^3 + 4n`$ ist durch 6 teilbar.

### Aufgabe 4
Zeige durch vollständige Induktion: Für alle $`n \in \N_0`$ gilt: $`n^5 - n`$ ist durch 5 teilbar.