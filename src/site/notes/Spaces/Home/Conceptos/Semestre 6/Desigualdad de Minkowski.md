---
{"dg-publish":true,"permalink":"/spaces/home/conceptos/semestre-6/desigualdad-de-minkowski/"}
---

#Tema/Análisis  #Tipo/Teorema 

> [!theorem|*] Desigualdad de Minkowski
> 
> Sean $p \in [1,\infty)$ y $f,g \in \mathcal{L}_{p}(\mu)$ dadas, entonces:
> $$\left(\int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}\leq \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}+\left(\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}.$$
> 

*Demostración.* El caso $p=1$ se verifica usando la desigualdad del triángulo. Por las [[Spaces/Home/Conceptos/Semestre 6/Propiedades de cerradura de los espacios Lp\|Propiedades de cerradura de los espacios Lp]] se tiene que $f+g \in$[[Spaces/Home/Conceptos/Semestre 6/Espacio Lp\|Espacio Lp]] y 
$$\begin{aligned}\int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu&=\int_{}^{}\left\lvert f+g\right\rvert^{p-1}\left\lvert f+g\right\rvert \, d\mu\leq \int_{}^{}\left\lvert f+g\right\rvert^{p-1}\left\lvert f\right\rvert \, d\mu+ \int_{}^{}\left\lvert f+g\right\rvert^{p-1}\left\lvert g\right\rvert \, d\mu .\end{aligned}$$
Como $\left\lvert f+g\right\rvert^{p} \in \mathcal{L}_{1}$ y $f,g \in \mathcal{L}{p}$ entonces $\left\lvert f+g\right\rvert \in \mathcal{L}_{q}$, donde $\frac{1}{p}+\frac{1}{q}=1$. Luego, por la [[Spaces/Home/Conceptos/Semestre 6/Desigualdad de Hölder\|Desigualdad de Hölder]] se tiene que:
$$\begin{aligned} \int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu &\leq \left( \int_{}^{} \left\lvert f+g\right\rvert^{q(p-1)} \, d\mu \right)^{\frac{1}{q}}  \left( \left( \int_{}^{} \left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}} + \left(\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}\right).\end{aligned}$$
Si $\int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu=0$ entonces la desigualded de minkowski  se satisface trivialmente, y si $\int_{}^{} \left\lvert f+g\right\rvert^{p} \, d\mu>0$, entonces usando que $q(p-1)=p$ tenemos que
$$ \begin{aligned} \left( \int_{}^{} \left\lvert f+g \right\rvert^{p} \, d\mu \right)^{\frac{1}{p}} &\leq \left( \int_{}^{} \left\lvert f+g\right\rvert^{p} \, d\mu \right)^{1-\frac{1}{q}}= \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}+\left(\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}.\end{aligned}$$
$\blacksquare$