---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/desigualdad-de-hoelder/"}
---

#Tema/Análisis  #Tipo/Teorema 

> [!theorem|*] Desigualdad de Hölder
> 
> Sean $(X,S,\mu)$ un [[Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]], $p \in (1,\infty)$ y $q \in (1,\infty)$ tales que $\frac{1}{p}+\frac{1}{q}=1$.
> Si $f \in \mathcal{L}_{p}(\mu)$ y $g \in \mathcal{L}_{q}(\mu)$ son distintas de cero casi dondequiera entonces:
> 1. $fg \in\mathcal{L}_{1}(\mu),$
> 2. $\int_{}^{}\left\lvert fg\right\rvert \, d\mu\leq \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{ \frac{1}{p} } \left(\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu \right)^{\frac{1}{q}}$,
> 3. La igualdad en $(2)$ ocurre si y sólo si existen constantes no negativas, no ambas cero, $A$ y $B$ tales que: $A \left\lvert f\right\rvert^{p}=B\left\lvert g\right\rvert^{q}$.

*Demostración.* Recordemos la desigualdad de Bernoulli, la cual establece que:
$$(1+t)^{p}\geq 1+ pt,\space t\geq -1,\space p>1$$
con igualdad si y sólo si $t=0$. 
Sean $a\geq0$ y $b>0$ tales que 
$$1+t=\left(\frac{a}{b^{\frac{q}{p}}} \right).$$
Sustituyendo estos valores en la desigualdad de Bernoulli obtenemos:
$$\begin{align} \frac{a^{p}}{b^{q}} &\geq 1+p\left(\frac{a}{b^{\frac{q}{p}}}-1 \right) \end{align}.$$
Multiplicando por $b^{q}$:
$$a^{p}\geq b^{q}+pab^{-\frac{q}{p}+q}-pb^{q}=b^{q}+pab^{q\left(1-\frac{1}{p} \right)}-pb^{q}=b^{q}+pab-pb^{q}.$$
Reorganizando:
$$pab=a^{p}-b^{q}+pb^{q}\leq a^{p}+b^{q}(p-1).$$
De modo que
$$ab\leq\frac{a^{p}}{p}+b^{q} \frac{p-1}{p}=\frac{a^{p}}{p}+b^{q}\left( 1-\frac{1}{p}\right)=\frac{a^{p}}{p}+\frac{b^{q}}{q},$$
con igualdad si y sólo si $a^{p}=b^{q}$. Esta es la llamda desigualdad de Young.
Ahora sí, procedemos a demostrar el teorema.
1. Por lo que ya probamos:
$$\int_{}^{}\left\lvert fg\right\rvert \, d\mu\leq \int_{}^{} \frac{\left\lvert f\right\rvert^{p}}{p}+\frac{\left\lvert g\right\rvert^{q}}{q} \, d\mu=\frac{1}{p} \int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu+\frac{1}{q}\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu<\infty.$$
	De aquí que $\left\lvert fg\right\rvert \in \mathcal{L}_{1}(\mu)$.
2.  Por hipótesis, $\int_{}^{}\left\lvert f\right\rvert \, d\mu$ y $\int_{}^{}\left\lvert g\right\rvert \, d\mu$ son diferentes de cero.
	Definimos
	$$h= \frac{\left\lvert f\right\rvert}{\left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}} \text{ y } k=\frac{\left\lvert g\right\rvert}{\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu}.$$
	Por la desigualdad ya obtenida:
$$\int_{}^{}hk \, d\mu\leq \frac{1}{p}\int_{}^{}\left\lvert h\right\rvert^{p} \, d\mu+\frac{1}{q}\int_{}^{}\left\lvert k\right\rvert^{q} \, d\mu=\frac{1}{p}+\frac{1}{q}=1,$$
	entonces
	$$\int_{}^{}\left\lvert fg\right\rvert \, d\mu\leq \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}+\left(\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu \right)^{\frac{1}{q}}.$$
3. La igualdad en $(2)$ ocurre si y sólo si $\int_{}^{}hk \, d\mu=1 \iff h^{p}=k^{q}$ casi dondequiera $\iff$ $\left(\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu \right)\left\lvert f\right\rvert^{p}=\left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)\left\lvert g\right\rvert^{q}$ casi dondequiera.
$\blacksquare$


