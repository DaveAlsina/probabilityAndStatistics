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

![[Pasted image 20210302002117.png]]

La probabilidad 'p' de que exactamente uno de los invitados cumpla años, el mismo día que yo es: 

$$
\displaystyle
p = \frac{1}{499} \cdot \frac{1}{365}
$$

Para calcular con Poisson es necesario definir $\lambda$ como una caracterización de la FMP de la V.A: 'D' # de invitados que cumplen el mismo día que yo.

$$
\displaystyle
f(D) = 
\begin{cases}
\displaystyle
	\frac{n}{499} \cdot \left(\frac{1}{365}\right)^{n}, \text{ donde n = 1, 2, 3, ... 499}
\end{cases}
$$

$$
\displaystyle
f(D) = 
\begin{cases}
\displaystyle
	\frac{n}{499} \cdot \left(\frac{1}{365}\right)^{n}, \text{ donde n = 1, 2, 3, ... 499}
\end{cases}
$$

-----

![[Pasted image 20210302002705.png]]





