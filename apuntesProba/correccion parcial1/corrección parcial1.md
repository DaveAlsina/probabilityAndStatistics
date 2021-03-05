**Ejercicio 1)**

a)  $P(F|H) = P(F \cap H)/P(H) = \frac{12/100}{45/100}$

b)   $P(M|F) = P(M \cap F)/P(F) = \frac{8/100}{20/100}$

**Ejercicio 2)** 52 cartas, 13 de cada palo. En este evento saco 5 cartas de las 52.

a) probabilidad 'j' de que salga un póker de ases, (los 4 aces de la baraja):

$$
\displaystyle
j =
\frac{\binom{4}{4} \cdot \binom{48}{1}}{\binom{52}{5}}\\
$$

*sacar 4 aces es 4C4, sacar cualquier otra carta es 48C1, sacar cualquier grupo de 5 cartas de las 52 es, 52C5*.

b) un póker de cualquier valor (4 cartas con el mismo número o figura):

$$
\displaystyle
j =
\frac{ \binom{13}{1} \cdot \binom{4}{4} \cdot \binom{48}{1}}{\binom{52}{5}}
$$

**Ejercicio 3)**

a) $R_{i} \text{ sacar una canica roja en el intento } i = 1, 2$

$$
P(R_{2}) = P(R_{1})\cdot P(R_{2}|R_{1}) + P(N_{1})\cdot P(R_{2}|N_{1})
$$

**Ejericicio 4)** lo planteado por alicia es $P(A_{1} \cap A_{2}|A_{1}) \geq P(A_{1} \cap A_{2}|A_{1} \cup A_{2})$

a) ¿alicia tiene razón?
$$
P(A_{1} \cap A_{2}|A_{1}) \geq P(A_{1} \cap A_{2}|A_{1} \cup A_{2})\\
$$
$$
\frac{P(A_{1} \cap A_{2} \cap A_{1})}{P(A_{1})} \geq P(A_{1} \cap A_{2} \cap (A_{1} \cup A_{2}))\\
$$

alicia tenía razón

**Ejercicio 5)**

$A_{1}: \text{ primer resultado es par }$
$A_{2}: \text{ primer resultado es 1 o 2 }$

a) $A_{1}$ y $A_{2}$ indep? 

$$
	P(A_{1} \cap A_{2}) = P(A_1) \cdot P(A_2)
$$

Si son independientes.

b)  B: se obtuvo un doble, $A_{1}$ y $A_{2}$, ¿son independientes condicionales?

$$
	P(A_{1} \cap A_{2} | B) = P(A_1|B) \cdot P(A_2|B)
$$

Si son independientes condicionales.