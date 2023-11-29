---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/lema-del-promedio/"}
---

#Tema/Análisis  #Tipo/Ejercicio 

> [!exercise|51] Lema del promedio
> 
> Sea $f \in \mathcal{L}_{1}(X,S,\mu)$ tal que $\left\lvert \frac{1}{\mu(E)}\int_{E}^{}f \, d\mu \right\rvert\leq k$ con $k\geq 0$ constante, para todo $E \in S$ con $0<\mu(E)<\infty$. Pruebe que $\left\lvert f\right\rvert\leq k$ casi dondequiera relativo a $\mu$.

*Demostración.* 
Tenemos que 
$$\left\lvert \int_{E}^{}f \, d\mu\right\rvert\leq k \left\lvert \mu(E)\right\rvert=k \mu(E), \space \forall E \in S,\mu(E)<\infty.$$
Considera los conjuntos 
$$E_{\alpha}=\left\{x \in X: \left\lvert f(x)\right\rvert > \alpha\right\}.$$
Por la desigualdad de Markov, tenemos que 
$$\mu(E_{\alpha})\leq \frac{1}{\alpha} \int_{}^{}f \, d\mu.$$
Entonces
$$\frac{1}{\mu(E_{k})} \left\lvert \int_{E_{k}}^{}f \, d\mu \right\rvert\leq k.$$
Pero 
$$k \mu(E_{k})=\int_{}^{}k \chi_{E_{k}} \, d\mu\leq \left\lvert \int_{E_{k}}^{}f \, d\mu \right\rvert\leq k\mu(E_{k}).$$
Entonces 
$$k\mu(E_{k})= \left\lvert \int_{E_{k}}^{}f \, d\mu \right\rvert= \int_{E_{k}}^{}k \, d\mu,$$ Por lo tanto 
$$\left\lvert \int_{E_{k}}^{}f \, d\mu\right\rvert- \left\lvert \int_{E_{k}}^{}k \, d\mu\right\rvert=0.$$
Pero $f$ es positiva en $E_{k}$ entonces 
$$\int_{E_{k}}^{}f-k \, d\mu=0.$$
Entonces $f$ es igual a $k$ casi dondequiera en $E_{k}$ y, por lo tanto, $f$ es igual a $k$ casi dondequiera en $X$.
$\blacksquare$