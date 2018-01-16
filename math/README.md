# Readme

Used https://www.codecogs.com/latex/eqneditor.php

## Images recepies

### Shuffle matrix

```
\begin{pmatrix}

 & K^{1}_{C} & K^{1}_{E} & K^{3}_{M} & \cdots & K^{2}_{X}  &  \\
 & K^{2}_{C} & K'^{1}_{E} & K'^{3}_{M} & \cdots & K'^{2}_{X}  &  \\
 & K^{3}_{C} & K''^{1}_{E} & K^{4}_{M} & \cdots & K^{3}_{X}  &  \\
 & K^{4}_{C} & K^{2}_{E} & K'^{4}_{M} & \cdots & K'^{3}_{X}  &  \\
 & \vdots  & \vdots  & \vdots  & \ddots  & \vdots  & \\
 & K^{5}_{C} & K'^{2}_{E} & K''^{4}_{M}  & \cdots & K''^{3}_{X}  &  \\
\end{pmatrix}

Shuffle

\begin{pmatrix}

 & K^{1}_{C} & K'^{2}_{E} & K'^{3}_{M}  & \cdots & K^{2}_{X}  &  \\
 & K^{2}_{C} & K^{1}_{E} & K''^{4}_{M}  & \cdots & K^{3}_{X}  &  \\
 & K^{3}_{C} & K^{2}_{E} & K^{3}_{M}  & \cdots & K^{2}_{X}  &  \\
 & K^{4}_{C} & K''^{1}_{E} & K'^{4}_{M}  & \cdots & K''^{3}_{X}  &  \\
 & \vdots  & \vdots  & \vdots  & \ddots  & \vdots  & \\
 & K^{5}_{C} & K^{1}_{E} & K^{4}_{M}  & \cdots & K^{3}_{X}  &  \\
\end{pmatrix}
```

### Message types

1. messagetype.client.gif   `(K^{i}_{C}, \{ IP^{i}_{C} \} _{K^{i}_{E}})`
2. messagetype.entry.gif    `(K^{i}_{E}, \{ IP^{i}_{E} \} _{K^{i}_{C}}, \{IP^{i}_{E}\}_{K^{i}_{M}} )`
3. messagetype.middles.gif  `(K^{i}_{M}, \{ IP^{i}_{M} \} _{K^{i}_{E}}, \{IP^{i}_{M}\}_{K^{i}_{X}} )`
4. messagetype.exit.gif     `(K^{i}_{X}, \{ IP^{i}_{X} \} _{K^{i}_{M}} )`

### Path lookup

1. 3pathlookup.matrix.gif  `M: CS_{i} = (Hash(M), i).`

### Proof of Bandwidth

1. pob.hash1.gif         `R'_{*} = Hash(R_{*})`
2. pob.tuple2.gif        `(coin\#, R'_{C} ),`
3. pob.tuples3.gif       `R'_{E}, R'_{M}, and R'_{X}`
4. pob.blob4.gif         `B = (coin\#, R'_{C}, R'_{E}, R'_{M}, R'_{X})`
5. pob.signature5.gif    `S^{B}_{X},`
6. pob.reveal5.gif       `R_{X}`
7. pob.tuple5.gif        ` (B, S^{B}_{X}, R_{X})`
8. pob.signature6.gif    `S^{B}_{i},`
9. pob.proof7.gif        `P = (B, S^{B}_{X}, S^{B}_{M}, S^{B}_{E} , S^{B}_{C} , R_{X}, R_{M}, R_{E}, R_{C} )`
10. pob.hash8.gif        `Hash ( CS_{i},B,R_{X}, R_{M},R_{E}, R_{C}) == 0`


