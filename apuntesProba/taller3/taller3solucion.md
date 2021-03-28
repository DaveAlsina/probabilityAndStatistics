[[Valor esperado]]


![[Pasted image 20210301214319.png]]

Sea X la Variable aleatoria *\#de puntos que gana el equipo esa semana.* 

$$
\displaystyle 
f(x) =

\begin{cases}
(0.4)\cdot(0.5) \text{ es la probabilidad de ganar y empatar en el partido 1}\\
(0.7)\cdot(0.5) \text{ es la probabilidad de ganar y empatar en el partido 2}
\end{cases}
$$

----
![[Pasted image 20210301230024.png]]

Inicialmente creamos una variable aleatoria Z que corresponda al *\# de intento en que gana David*, la FMP para Z es:

$$
\displaystyle 
f(k) = 
\begin{cases}
P(tablas)^{k-1} \cdot P(Gana\;David), k = {1,2,3, ... ,10}
\end{cases}
$$

Dada la FMP, se puede calcular el valor esperado para Z, que corresponde a la probabilidad de que David gane la final como sigue: 

$$
\begin{equation}
\displaystyle
	E(Z) = \sum_{k=1}^{10}{k \cdot f(k)}
\end{equation}
$$

![[Pasted image 20210301233533.png]]

Creamos una variable aleatoria Z que corresponda al *\# de intento en que gana Diana*, la FMP para Z es:

$$
\displaystyle 
f(l) = 
\begin{cases}
P(tablas)^{k-1} \cdot P(Gana\;Diana), k = {1,2,3, ... ,10}
\end{cases}
$$

$$
\begin{equation}
\displaystyle
	E(Z) = \sum_{l=1}^{10}{l \cdot f(l)}
\end{equation}
$$

![[Pasted image 20210301233306.png]]

Sea Y nuestra V.A. que es *\# número de partidas jugadas* su correspondiente FMP es:

$$
\displaystyle 
f(j) = 
\begin{cases}
P(tablas)^{k-1} \cdot P(acabarPartida),\; k = {1,2,3, ... ,9}\\
P(tablas)^{k-1}, \text{ si k = 10}
\end{cases}
$$

----
![[Pasted image 20210302002117.png]]

De los 499 invitados(aparte de mi), existe la posibilidad de que cumplan años el mismo dia que yo, o de que no lo hagan, y en particular si solo una persona cumple años el mismo día que yo, eso implica que los demás no cumplan el mismo día que yo. Nótese que este experimento es uno que tiene variables bernulli, y se trata con probabilidad binomial así:

$$
\displaystyle
x = \binom{499}{1} \cdot \left(\frac{1}{365}\right)^{1} \cdot \left(\frac{364}{365}\right)^{498}
$$

Para calcular con Poisson es necesario definir $\lambda$ como $n \cdot p$

$$
	x = \frac{e^{- \lambda} \cdot \lambda^{k}}{k!}
	  =  \frac{e^{- \lambda} \cdot \lambda^{1}}{1!}
	  = e^{-\lambda} \cdot \lambda
	  = np \cdot e^{-n \cdot p}
$$

$$
	\displaystyle
	= \left(499 \cdot \frac{1}{365} \right) \cdot e^{-\cfrac{499}{365}}
$$


-----

![[Pasted image 20210302002705.png]]

Observe que en el problema solo hay 2 opciones, que el equipo 1 gane o no gane, este es otro experimento que se modela con probabilidad binomial. Así:

$$
	p(k) = \binom{n}{k} \cdot (p)^{k} \cdot (1-p)^{n-k}
$$

sea V nuestra variable aleatoria que indica el numero de partidos que se pueden ganar.

$$
	V = 1, ...,5
$$
$$
	\displaystyle
	
	\sum_{k=2}^{3}{\binom{3}{k} \cdot (p)^{k} \cdot (1-p)^{3-k}} \leq
	
	\sum_{k=3}^{5}{\binom{5}{k} \cdot (p)^{k} \cdot (1-p)^{5-k}}
$$

----
![[Pasted image 20210302164454.png]]

Sea Z una V.A. que indica el numero de personas que pueden necesitar usar un canal: 

$$
	Z = 1, ... , 1000
$$

Ahora la FMP para Z es:

$$
	P_{z}(k) = \binom{1000}{k}(1 - 0.01)^{n-k} (0.01)^{k} = \binom{1000}{k}(0.99)^{1000-k}(0.01)^{k}
$$


![[Pasted image 20210302165136.png]]

Dado que hay 50 canales el máximo de personas que se pueden conectar a la vez a través de los distintos canales es 50. Ergo:

$$
\displaystyle
P(exceder \;capacidad) = 1 - \sum_{k = 0}^{50}{\binom{1000}{k}(0.99)^{1000-k}(0.01)^{k}}
 \simeq 0
$$

----
![[Pasted image 20210302172251.png]]

En esta situación en particular la probabilidad de escoger cualquier llave es la misma, y no disminuye la cantidad de llaves probadas al probar nuevas llaves, siendo así definamos: 


$$
Z = \text{\# de intentos para abrir la puerta} = 1, 2, 3,  ...
$$

$$
\displaystyle
P_{Z}(k) = 
\begin{cases}
	\displaystyle
	(1-p)^{k-1} \cdot p
	= \left(\frac{4}{5}\right)^{k-1} \cdot \left(\frac{1}{5}\right) \text{ si } k=1,2,3,...\\
	0 \text{ en otro caso}
\end{cases}
$$

![[Pasted image 20210302180559.png]]

Con esta redefinición de la situación nos queda:

$$
Z = \text{\# de intentos para abrir la puerta} = 1, 2, 3, 4, 5
$$

$$
\displaystyle
P_{Z}(k) = 
\begin{cases}
	\displaystyle
	\left(1-\frac{1}{5-k-1}\right)^{k-1} \cdot \; \frac{1}{5-k-1}
	\text{,  si } k=1,2,3,4,5\\\\
	0 \text{ en otro caso}
\end{cases}
$$

----


![[Pasted image 20210303163009.png]]
Sea X nuestra variable aleatoria bernoulli: 

$$
\displaystyle
X = éxito(1), \; fracaso(0)
$$

Así la FMP de X es: 

$$
\displaystyle
P_{X}(k) = 
\begin{cases}
	p \text{, si k es un éxito}\\
	1 - p \text{, si k es un fracaso} 
\end{cases}
$$

![[Pasted image 20210303191446.png]]

$$
\displaystyle
E(X) = (1 \cdot p) + (0 \cdot (1 - p))
= p
$$

----

![[Pasted image 20210317171845.png]]

La FMP de X es :

$$
\displaystyle
	P_{X}(k) = 
	\begin{cases}
		\text{si } k = 1, \; p \\
		\text{si } k = 0, \; 1 - p
	\end{cases}
$$


$$
\displaystyle
	P_{Y}(k) \begin{cases}
	\displaystyle
	
	\binom{n}{k} \cdot p^{k} \cdot (1 - p)^{n-k}
	\end{cases}
$$

![[Pasted image 20210317172341.png]]

$$
\displaystyle
	E[Y] = \sum_{k=0}^{n}{k\cdot \binom{n}{k} \cdot p^{k} \cdot (1 - p)^{n-k}}
$$

Note que:

$$
	k \cdot \binom{n}{k} = k \cdot \frac{n!}{(n-k)! \cdot k!}
	= n \cdot \frac{(n-1)!}{(n-1-k)!\cdot(k-1)!}
	=n \cdot \binom{n-1}{k-1}
$$

Con lo anterior:

$$
\displaystyle
	E[Y] = \sum_{k=0}^{n}{n\cdot \binom{n-1}{k-1} \cdot p^{k} \cdot (1 - p)^{n-k}}
$$

$$
= n \cdot p \cdot \cancelto{1}{\sum_{k=0}^{n-1}{\binom{n-1}{k-1}\cdot p^{k-1}(1-p)^{(n-1)-(k-1)}}}
$$

Finalmente

$$
=n\cdot p
$$

![[Pasted image 20210317172425.png]]

Dado que Y es lineal y es un función de las variables aleatorias $X_{i}$ tenga en cuenta que:

$$
\displaystyle
	E[Y] = Y[\;E[X]\;]
$$

Así:

$$
	E[Y] = E[X_{1}] + E[X_{2}] + E[X_{3}] + (...) + E[X_{n}]
$$
$$
	E[Y] = p + p + p + (...) + p
$$
$$
	E[Y] = n \cdot p
$$

![[Pasted image 20210317172522.png]]

Dado que Y es lineal observe:

$$
V[Y] = \sum_{i=1}^{n}{V(X_{i})} = n \cdot p\cdot(1-p)
$$
----

![[Pasted image 20210303194917.png]]

las funciones de masa de probabilidad tienen la característica de que la suma de sus probabilidades es igual a 1.


$$
\displaystyle

\sum_{k=0}^{\infty}{
	\displaystyle
	e^{-\lambda} \frac{\lambda^{k}}{k!}
}
=
e^{-\lambda}\cdot \sum_{k=0}^{\infty}{
	\displaystyle
	 \frac{\lambda^{k}}{k!}
}

= e^{-\lambda} \cdot (1 + \frac{\lambda}{1} + \frac{\lambda^{2}}{2} + \frac{\lambda^{3}}{6} + ...)
$$

$$
= e^{-\lambda} \cdot e^{\lambda} = 1
$$

![[Pasted image 20210303202756.png]]


$$
\displaystyle

\sum_{k=0}^{\infty}{
	\displaystyle
	k \cdot e^{-\lambda} \frac{\lambda^{k}}{k!}
}
=
 \lambda \cdot \sum_{k=0}^{\infty}{
	\displaystyle
	e^{-\lambda}\cdot \frac{\lambda^{k-1}}{k-1!}
}
$$

$$

=
 \lambda \cdot \sum_{l=1}^{\infty}{
	\displaystyle
	e^{-\lambda}\cdot \frac{\lambda^{l}}{l!}
= \lambda
}
$$

![[Pasted image 20210303204006.png]]

$$
\displaystyle

E[X^{2}] = 

\sum_{k=0}^{\infty}{
	\displaystyle
	k^{2} \cdot p_{X}(k)
}
=

\sum_{k=0}^{\infty}{
	\displaystyle
	k^{2} \cdot e^{-\lambda} \frac{\lambda^{k}}{k!}
}
=
  \sum_{k=0}^{\infty}{
	\displaystyle
	k\cdot
	e^{-\lambda}\cdot \frac{\lambda^{k}}{k-1!}
}
$$
sea $l = k-1$:
$$
	= \sum_{l = 0}^{\infty}{
	\displaystyle 
	(l + 1) \cdot e^{-\lambda} \cdot \frac{\lambda^{l+1}}{l!}
	}
	= \sum_{l = 0}^{\infty} l \cdot e^{-\lambda} \frac{\lambda^{l+1}}{l!}
	+
	\sum_{l = 0}^{\infty} e^{-\lambda} \frac{\lambda^{l+1}}{l!}
$$

$$
	
	= \lambda \cdot \cancelto{E[X]}{\sum_{l = 0}^{\infty}{
	l \cdot e^{-\lambda} \frac{\lambda^{l}}{l!}}}
	
	
	+ \lambda \cdot \cancelto{1}{\sum_{l = 0}^{\infty}{
	e^{-\lambda} \frac{\lambda^{l}}{l!}}
	}
	
$$

$$
	= \lambda \cdot \lambda + \lambda
$$

$$
	= \lambda^{2} + \lambda
$$

![[Pasted image 20210303204031.png]]

Dado lo $E[X]$ y $E[X^{2}]$:

$$
	Var(X) = E[X^{2}] - (E[X])^{2}
$$

$$
	Var(X) = \lambda^{2} + \lambda - (\lambda)^{2} = \lambda
$$





