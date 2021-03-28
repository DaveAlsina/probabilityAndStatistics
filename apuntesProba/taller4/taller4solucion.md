![[Pasted image 20210313164742.png]]

La FMP de *Y = g(x)* es: 

$$
\displaystyle
	Y_{g(x)}(x) = 
	\begin{cases}
	\displaystyle
		c_{1} \text{ si  $x = 1$}\\
		c_{2} \text{ si  $x = 2$}\\
		0 \text{ en otro caso.}
	\end{cases}
$$

Teniendo en cuenta que X es uniforme en $[0,1]$ la probabilidad de obtener cualquier $x$ es 1, y tendiendo en cuenta los intervalos en los que se define $Y_{g(x)}(X)$: 

$$
\displaystyle
	Y_{g(x)}(x) = 
	\begin{cases}
	\displaystyle
		1/3 \text{ si  $x = 1$}\\
		2/3 \text{ si  $x = 2$}\\
		0 \text{ en otro caso.}
	\end{cases}
$$

$$
\displaystyle
	E[Y] = 1 \cdot \cancelto{\cfrac{1}{3}}{Y_{g(x)}(1)} + 
	2 \cdot \cancelto{\cfrac{2}{3}}{Y_{g(x)}(1)}  
	= \frac{1}{3} + \frac{4}{3} = \frac{5}{3}
$$

![[Pasted image 20210313175645.png]]

$$
\begin{align*}
\int_{-\infty}^{\infty}{g(x) \cdot f_{x}(x)} \; dx
\\
\displaystyle 
= \int_{0}^{1/3}{\cancelto{1}{g(x)}\cdot \cancelto{1}{f_{x}(x)}}
+
\int_{1/3}^{1}{\cancelto{2}{g(x)}\cdot \cancelto{1}{f_{x}(x)}}
&= \frac{1}{3} + \frac{4}{3} = \frac{5}{3}
\end{align*}
$$

----

![[Pasted image 20210313190030.png]]

$$
\displaystyle
\begin{align*}
	E[X] = \int_{-\infty}^{\infty}{x \cdot e^{-\lambda x}}
	= \int_{0}^{\infty}{x \cdot \lambda e^{-\lambda x}} &= 
	\frac{1}{\lambda}\int_{0}^{\infty}{u \cdot e^{u}} du \\
	&= \frac{1}{\lambda}\left[u \cdot e^{u} \bigg|_{0}^{\infty} + \cancelto{0}{\frac{-1}{\lambda}\int_{0}^{\infty}{e^{u} \; du}}\right]\\
	&=  \frac{1}{\lambda}
	\left[\cancelto{0}{u \cdot e^{u} \;\; \bigg|_{0}^{\infty}} + \cancelto{1}{-\lambda \frac{-1}{\lambda}}
	\cdot \cancelto{1}{\int_{0}^{\infty}{e^{w} \; dw}}\right]\\
	&= \frac{1}{\lambda}
\end{align*}\\
$$

$$
\displaystyle
\begin{align*}
	E[X^{2}] = \int_{-\infty}^{\infty}{x^{2} \cdot e^{-\lambda x}}
	&= \int_{0}^{\infty}{x^{2} \cdot \lambda e^{-\lambda x}}\;\;
	(u = x^{2},\; du=2x\;dx,\; dv = \lambda e^{-\lambda} x\; dx,\; v= -e^{-\lambda x})\\
	&= \cancelto{0}{-x^{2}\cdot e^{-\lambda x} \bigg|_{0}^{\infty}} -  \left(\frac{-2}{\lambda}
	\cancelto{E[X]}{\int_{0}^{\infty} x\lambda e^{-\lambda x} }\right)\\
	&= \frac{2}{\lambda^{2}}
\end{align*}\\
$$

$$
\begin{align*}
	V[X] &=  (E[X^{2}]) - (E[X])^{2}\\
	&= \frac{2}{\lambda^{2}} - \frac{1}{\lambda^{2}} \\
	&= \frac{1}{\lambda^{2}}
\end{align*}
$$

---

![[Pasted image 20210313210617.png]]


![[Pasted image 20210313210630.png]]

----

![[Pasted image 20210313210645.png]]

----

![[Pasted image 20210313210701.png]]

$$
X = \sqrt{x^{2} + y^{2}} \; | \; (x,y) \in x^{2} + y^{2} = r  
$$


$$
\begin{align*}
\displaystyle
	F_{X} = \int_{0}^{2\pi}\int_{0}^{r} r \cdot dr d\theta &= 
	\int_{0}^{2\pi} \frac{r^{2}}{2}\bigg|_{0}^{r} \; d\theta \\
  &= \frac{1}{2} \cdot r^{2} \cdot \cancelto{2\pi}{\theta \bigg|_{0}^{2\pi}}\\
  &= r^{2}\pi
\end{align*}
$$

Tenga en cuenta que este es un acumulado respecto a el círculo de radio completo R, luego la función de densidad de probabilidad acumulada es:

$$
F_{X} = P(X \leq x) = \frac{\pi r^{2}}{\pi R^{2}} = \left(\frac{r}{R}\right)^{2}
$$


![[Pasted image 20210313212420.png]]

Con base al anterior resultado
$$
\frac{d(F_{X})}{dr} = f_{X}(r)= 
\begin{cases}
\displaystyle
	\frac{2r}{R^{2}}, \text{\; si $ 0 \leq r\leq R$}\\
	0, \; \text{ en otro caso.}
\end{cases}

$$

![[Pasted image 20210313213537.png]]

$$
\begin{align*}
	\displaystyle
	E[X]&= \int_{0}^{R} r \cdot  f_{X}(r)
	= \int_{0}^{R} r \cdot \frac{2r}{R^{2}} dr = \frac{2}{R^{2}}\int_{0}^{R} r^{2} dr\\
	&= \frac{2}{R^{2}} \cdot \frac{r^{3}}{3} \bigg|_{0}^{R}\\
	&= \frac{2R}{3}
\end{align*}
$$


$$
\begin{align*}
	\displaystyle
	E[X^{2}]&= \int_{0}^{R} r^{2} \cdot  f_{X}(r)
	= \int_{0}^{R} r^{2} \cdot \frac{2r}{R^{2}} dr = \frac{2}{R^{2}}\int_{0}^{R} r^{3} dr\\
	&= \frac{2}{R^{2}} \cdot \frac{r^{4}}{4} \bigg|_{0}^{R}\\
	&= \frac{R^{2}}{2}
\end{align*}
$$

Recuerde la definición de la varianza de X: 

$$
	\begin{align*}
		V[X] &= (E[X^{2}]) - (E[X])^{2}\\
		&= \left(\frac{R^{2}}{2}\right) - \left(\frac{2R}{3}\right)^{2}\\
		&= \frac{R^{2}}{18} 
	\end{align*}
$$

![[Pasted image 20210317175200.png]]

La función que muestra la cantidad de puntos a obtener dados un lanzamiento:

$$
\displaystyle

f_{S}(r) = 
	\begin{cases}
	\displaystyle
		\frac{1}{r}\; \text{ si ($r \leq d$)}\\
		0 \; \text{ si ($r \gt d$)}
	\end{cases}
$$

Ahora para calcular la funcion acumulada de probabilidad de S.

$$
\begin{align*}
	F_{S} = P(S \leq s) = 
	\begin{cases}
		\displaystyle
		0 \text{, si s $\lt 0$} \\
		P(r \gt d) = 1 - P(r \lt d) = 1 - \cfrac{d^{2}}{R^{2}} ,\;\;\text{ si }0 \leq s \lt \cfrac{1}{d}\\
		P(r \leq d) = 1 - \cfrac{1}{s^{2}d^{2}} ,\;\;\text{ si } s \geq \cfrac{1}{d}
	\end{cases}
\end{align*}
$$

$$
	\text{esta última probabilidad de } F_{s} \text{ tiene esta forma porque: }\\
$$

$$
\begin{align*}
	P(S \leq s) &= P\left(\frac{1}{X} \leq s\right) = P\left( \frac{1}{d} \leq s\right) = P\left(d \geq \frac{1}{s}\right)\\
	&= 1 - P\left(d \lt \frac{1}{s} \right) = 1 - \cfrac{1}{s^{2}d^{2}}
\end{align*}
$$




---- 