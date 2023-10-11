# Logik

|A|B|$`A \land B`$|$`A \lor B`$|$`\overline A = \neg A`$|$`A \rightarrow B`$|$`A \leftrightarrow B`$|$`A \text{ XOR } B`$|
|--|-|-|-|-|-|-|-|
|0|0|0|0|1|1|1|0|
|0|1|0|1|1|1|0|1|
|1|0|0|1|0|0|0|1|
|1|1|1|1|0|1|1|0|

## Wichtige Logikgesetze

```math
A \rightarrow B = \overline A \lor B
```

### De Morgan

```math
\overline {A \lor B} = \overline A \land \overline B \\
\overline {A \land B} = \overline A \lor \overline B
```

### Assoziativgesetze

```math
A \lor (B \lor C) = (A \lor B) \lor C \\
A \land (B \land C) = (A \land B) \land C \\
```

### Distributivgesetze

```math
A \land (B \lor C) = (A \land B) \lor (A \land C) \\
A \lor (B \land C) = (A \lor B) \land (A \lor C) \\
```


## Aufgaben

### 1. Quantoren

Welche der folgenden Aussagen ist wahr?

1. $`\forall x \in \N: x \gt 0`$
1. $`\exists x \in \N: x = 0`$
1. $`\exists! x \in \R: x > 0`$

### 2. Vereinfache

1. $`(\overline A \lor A) \land B`$
1. $`\overline { (A \lor B) } \land \overline {A \lor C}`$
1. $`A \lor (A \lor B) \lor C`$
1. $`(A \rightarrow B) \lor B`$
1. $`(A \rightarrow B) \lor \overline B`$
1. $`\overline {((\overline A ∨ B) ∧ (\overline B ∨ C))} ∨ (\overline A ∨ C)`$


### 3. Wahrheitstabelle

Für welche Belegungen von $`A`$, $`B`$ und $`C`$ sind die Aussagen aus Aufgabe 2 wahr?