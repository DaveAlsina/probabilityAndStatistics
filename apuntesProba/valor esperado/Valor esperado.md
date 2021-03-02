# Variable aleatoria y Valor esperado

#### _Función de masa de probabilidad_ 


Una -**función de masa de probabilidad**- es una función que le de probabilidad a las variables aleatorias definidas, ej: 

 $$
 \displaystyle
 P(k) =
 \begin{cases} 
 \text{si k  $= 0$, hay probabilidad y}\\
 \text{si k  $= 1$, hay probabilidad z}\\
 \text{si no es ninguno de los casos anteriores}, 0
\end{cases}$$
 
 ej2: 
 ![[Pasted image 20210224183011.png]]
 ----
 
 #### _Valor esperado, media o esperanza_
 
**media o esperanza:** sea X una V. Aleatoria discreta con FMP  $P_{x}$, definimos el valor esperado de x:

![[Pasted image 20210224190307.png]]

_ejercicio:_
Sea y = |x|, calcule el valor esperado de y.

$$P(y) = \begin{cases}
	\text{1/9 cuando y = 0}\\
	\text{2/9 si $y=$ 1,2,3,4}\\
	\text{0 en otro caso}
 \end{cases}$$

$$
E(y) = 0\cdot1/9 + 1 \cdot 2/9 + 2 \cdot 2/9 + ...
$$

ej: tirar una moneda con probabilidad 3/4 de atrerrizar en cara, 2 veces: 

$X: \# de\; caras, X = 0,1,2$

![[Pasted image 20210224193249.png]]
Resumiendo en una forma comprimida la probabililidad para X es: 

$$
\displaystyle
P_{X}(k)=
\begin{cases}
	\binom{n}{k}(P_{caras})^{k}(P_{no caras})^{n-k}, \text{donde n es el número de tiros}
\end{cases}
$$

$$
\displaystyle
E(X) = \sum_{k = 0}^{n}{
\left[\binom{n}{k}(P_{caras})^{k}(P_{no caras})^{n-k}
\right] \cdot k
}
$$

_El valor esperado es análogo al centro de gravedad._

_ejericio tipo parcial:_

![[Pasted image 20210224195417.png]]

P(Gana Diana) = 0.4
P(Gana Pepa) = 0.3
P(hay tablas) = 0.3

_¿cual es la probabilidad de que diana gane el torneo?_

Necesito hacer las suma de las probabilidades de que diana gane en la primera, segunda, ... , 10ma partida jugada.

Note que para que se den más intentos debe haberse dado tablas antes.

$$
\sum_{k = 1}^{10} = P(tablas)^{k} \cdot P(gana\;diana)
$$

















