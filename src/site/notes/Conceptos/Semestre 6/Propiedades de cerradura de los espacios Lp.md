---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/propiedades-de-cerradura-de-los-espacios-lp/"}
---

#Tema/Análisis  #Tipo/Teorema 

> [!theorem|*]
> Si $f,g \in \mathcal{L}_{p}(X,S,\mu)$ y $\alpha \in \mathbb{R}$, entonces $\alpha f, f+g \in \mathcal{L}_{p}(X,S,\mu)$.
> 

*Demostración.* Notemos que 
$$\int_{}^{}\left\lvert \alpha f\right\rvert^{p} \, d\mu=\int_{}^{}\left\lvert \alpha\right\rvert^{p} \left\lvert f\right\rvert^{p} \, d\mu= \left\lvert \alpha\right\rvert^{p}\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu< \infty.$$
Para la segunda afrimación, observemos que para cualesquiera números reales $a$ y $b$ se cumple que 
$$\left\lvert a+b\right\rvert^{p}\leq \left(2 \max \left\{\left\lvert a\right\rvert, \left\lvert b\right\rvert \right\} \right)^{p}\leq 2^{p}\left(\left\lvert a\right\rvert^{p}+\left\lvert b\right\rvert^{p} \right).$$
Así que:
$$\int_{}^{} \left\lvert f+g\right\rvert^{p} \, d\mu\leq 2^{p}\left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu+\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)<\infty.$$