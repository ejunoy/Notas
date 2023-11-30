---
{"dg-publish":true,"permalink":"/spaces/home/notas/semestre-6/analisis-ii/espacios-clasicos-de-banach/"}
---

#Tema/Análisis  #Tipo/Nota 


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/semestre-6/espacio-lp/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Definición 

> [!definition|*] $\mathcal{L}_p$
> 
> Sea $(X,S,\mu)$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]] y $p \in (0,\infty)$ fijo. Definimos
> $\color{yellow}\mathcal{L}_{p}(X,S,\mu) \color{white} = \left\{f \in M(X,S): \left\lvert f\right\rvert^{p} \in \mathcal{L}_{1}(X,S,\mu) \right\}.$

<i> Observación. </i> Claramente
$f \in \mathcal{L}_{p}(X,S,\mu) \iff \int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu < \infty \iff \left\lvert f\right\rvert^{p} \in \mathcal{L}_{1}(X,S,\mu).$
Observa que $\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu=0 \iff f=0$ casi dondequiera.

<i> Notación. </i> Si no se presta a confusión escribiremos $\mathcal{L}_{p}(\mu)$ en lugar de $\mathcal{L}_{p}(X,S,\mu)$.

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/semestre-6/propiedades-de-cerradura-de-los-espacios-lp/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Teorema 

> [!theorem|*]
> Si $f,g \in \mathcal{L}_{p}(X,S,\mu)$ y $\alpha \in \mathbb{R}$, entonces $\alpha f, f+g \in \mathcal{L}_{p}(X,S,\mu)$.
> 

*Demostración.* Notemos que 
$\int_{}^{}\left\lvert \alpha f\right\rvert^{p} \, d\mu=\int_{}^{}\left\lvert \alpha\right\rvert^{p} \left\lvert f\right\rvert^{p} \, d\mu= \left\lvert \alpha\right\rvert^{p}\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu< \infty.$
Para la segunda afrimación, observemos que para cualesquiera números reales $a$ y $b$ se cumple que 
$\left\lvert a+b\right\rvert^{p}\leq \left(2 \max \left\{\left\lvert a\right\rvert, \left\lvert b\right\rvert \right\} \right)^{p}\leq 2^{p}\left(\left\lvert a\right\rvert^{p}+\left\lvert b\right\rvert^{p} \right).$
Así que:
$\int_{}^{} \left\lvert f+g\right\rvert^{p} \, d\mu\leq 2^{p}\left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu+\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)<\infty.$

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/semestre-6/desigualdad-de-hoelder/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Teorema 

> [!theorem|*] Desigualdad de Hölder
> 
> Sean $(X,S,\mu)$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]], $p \in (1,\infty)$ y $q \in (1,\infty)$ tales que $\frac{1}{p}+\frac{1}{q}=1$.
> Si $f \in \mathcal{L}_{p}(\mu)$ y $g \in \mathcal{L}_{q}(\mu)$ son distintas de cero casi dondequiera entonces:
> 1. $fg \in\mathcal{L}_{1}(\mu),$
> 2. $\int_{}^{}\left\lvert fg\right\rvert \, d\mu\leq \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{ \frac{1}{p} } \left(\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu \right)^{\frac{1}{q}}$,
> 3. La igualdad en $(2)$ ocurre si y sólo si existen constantes no negativas, no ambas cero, $A$ y $B$ tales que: $A \left\lvert f\right\rvert^{p}=B\left\lvert g\right\rvert^{q}$.

*Demostración.* Recordemos la desigualdad de Bernoulli, la cual establece que:
$(1+t)^{p}\geq 1+ pt,\space t\geq -1,\space p>1$
con igualdad si y sólo si $t=0$. 
Sean $a\geq0$ y $b>0$ tales que 
$1+t=\left(\frac{a}{b^{\frac{q}{p}}} \right).$
Sustituyendo estos valores en la desigualdad de Bernoulli obtenemos:
$\begin{align} \frac{a^{p}}{b^{q}} &\geq 1+p\left(\frac{a}{b^{\frac{q}{p}}}-1 \right) \end{align}.$
Multiplicando por $b^{q}$:
$a^{p}\geq b^{q}+pab^{-\frac{q}{p}+q}-pb^{q}=b^{q}+pab^{q\left(1-\frac{1}{p} \right)}-pb^{q}=b^{q}+pab-pb^{q}.$
Reorganizando:
$pab=a^{p}-b^{q}+pb^{q}\leq a^{p}+b^{q}(p-1).$
De modo que
$ab\leq\frac{a^{p}}{p}+b^{q} \frac{p-1}{p}=\frac{a^{p}}{p}+b^{q}\left( 1-\frac{1}{p}\right)=\frac{a^{p}}{p}+\frac{b^{q}}{q},$
con igualdad si y sólo si $a^{p}=b^{q}$. Esta es la llamda desigualdad de Young.
Ahora sí, procedemos a demostrar el teorema.
1. Por lo que ya probamos:
$\int_{}^{}\left\lvert fg\right\rvert \, d\mu\leq \int_{}^{} \frac{\left\lvert f\right\rvert^{p}}{p}+\frac{\left\lvert g\right\rvert^{q}}{q} \, d\mu=\frac{1}{p} \int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu+\frac{1}{q}\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu<\infty.$
	De aquí que $\left\lvert fg\right\rvert \in \mathcal{L}_{1}(\mu)$.
2.  Por hipótesis, $\int_{}^{}\left\lvert f\right\rvert \, d\mu$ y $\int_{}^{}\left\lvert g\right\rvert \, d\mu$ son diferentes de cero.
	Definimos
	$h= \frac{\left\lvert f\right\rvert}{\left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}} \text{ y } k=\frac{\left\lvert g\right\rvert}{\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu}.$
	Por la desigualdad ya obtenida:
$\int_{}^{}hk \, d\mu\leq \frac{1}{p}\int_{}^{}\left\lvert h\right\rvert^{p} \, d\mu+\frac{1}{q}\int_{}^{}\left\lvert k\right\rvert^{q} \, d\mu=\frac{1}{p}+\frac{1}{q}=1,$
	entonces
	$\int_{}^{}\left\lvert fg\right\rvert \, d\mu\leq \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}+\left(\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu \right)^{\frac{1}{q}}.$
3. La igualdad en $(2)$ ocurre si y sólo si $\int_{}^{}hk \, d\mu=1 \iff h^{p}=k^{q}$ casi dondequiera $\iff$ $\left(\int_{}^{}\left\lvert g\right\rvert^{q} \, d\mu \right)\left\lvert f\right\rvert^{p}=\left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)\left\lvert g\right\rvert^{q}$ casi dondequiera.
$\blacksquare$




</div></div>




<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/semestre-6/desigualdad-de-minkowski/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Teorema 

> [!theorem|*] Desigualdad de Minkowski
> 
> Sean $p \in [1,\infty)$ y $f,g \in \mathcal{L}_{p}(\mu)$ dadas, entonces:
> $\left(\int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}\leq \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}+\left(\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}.$
> 

*Demostración.* El caso $p=1$ se verifica usando la desigualdad del triángulo. Por las [[Spaces/Home/Conceptos/Semestre 6/Propiedades de cerradura de los espacios Lp\|Propiedades de cerradura de los espacios Lp]] se tiene que $f+g \in$[[Spaces/Home/Conceptos/Semestre 6/Espacio Lp\|Espacio Lp]] y 
$\begin{aligned}\int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu&=\int_{}^{}\left\lvert f+g\right\rvert^{p-1}\left\lvert f+g\right\rvert \, d\mu\leq \int_{}^{}\left\lvert f+g\right\rvert^{p-1}\left\lvert f\right\rvert \, d\mu+ \int_{}^{}\left\lvert f+g\right\rvert^{p-1}\left\lvert g\right\rvert \, d\mu .\end{aligned}$
Como $\left\lvert f+g\right\rvert^{p} \in \mathcal{L}_{1}$ y $f,g \in \mathcal{L}{p}$ entonces $\left\lvert f+g\right\rvert \in \mathcal{L}_{q}$, donde $\frac{1}{p}+\frac{1}{q}=1$. Luego, por la [[Spaces/Home/Conceptos/Semestre 6/Desigualdad de Hölder\|Desigualdad de Hölder]] se tiene que:
$\begin{aligned} \int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu &\leq \left( \int_{}^{} \left\lvert f+g\right\rvert^{q(p-1)} \, d\mu \right)^{\frac{1}{q}}  \left( \left( \int_{}^{} \left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}} + \left(\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}\right).\end{aligned}$
Si $\int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu=0$ entonces la desigualded de minkowski  se satisface trivialmente, y si $\int_{}^{} \left\lvert f+g\right\rvert^{p} \, d\mu>0$, entonces usando que $q(p-1)=p$ tenemos que
$ \begin{aligned} \left( \int_{}^{} \left\lvert f+g \right\rvert^{p} \, d\mu \right)^{\frac{1}{p}} &\leq \left( \int_{}^{} \left\lvert f+g\right\rvert^{p} \, d\mu \right)^{1-\frac{1}{q}}= \left(\int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}+\left(\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu \right)^{\frac{1}{p}}.\end{aligned}$
$\blacksquare$

</div></div>


Como consecuencia de la de la [[Spaces/Home/Conceptos/Semestre 6/Desigualdad de Minkowski\|Desigualdad de Minkowski]] se tiene que 
$$\int_{}^{}\left\lvert f+g\right\rvert^{p} \, d\mu\leq \int_{}^{}\left\lvert f\right\rvert^{p} \, d\mu+\int_{}^{}\left\lvert g\right\rvert^{p} \, d\mu.$$
Este hecho se sigue de la desigualdad:
$$(a+b)^{p}\leq a^{p}+b^{p} \space a,b\geq 0 \text{ y } 0<p<1.$$


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/semestre-6/seminorma-p/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Definición 

> [!definition|*] Seminorma p
> 
> Sea $p \in [1,\infty)$. Definimos la **seminorma-p** en $\mathcal{L}_{p}(\mu)$,  $\lvert\lvert \cdot \rvert\rvert_{p}:\mathcal{L}_{p}(\mu) \to [0,\infty)$ como 
> $\lvert\lvert f \rvert\rvert_{p}= \left( \int_{}^{} \left\lvert f\right\rvert^{p} \, d\mu. \right)^{\frac{1}{p}}$

</div></div>


> [!theorem|*]
> Sean $p \in [0,\infty)$ fija y $\lvert\lvert \cdot \rvert\rvert_{p}:\mathcal{L}_{p}(\mu) \to R$ la [[Spaces/Home/Conceptos/Semestre 6/Seminorma p\|Seminorma p]], entonces $\lvert\lvert \cdot \rvert\rvert_{p}$ es una seminorma en $\mathcal{L}_{p}(\mu)$.
> 

*Demostración.* Nota que:
1. $f=0 \rightarrow \lvert\lvert f \rvert\rvert_{p}=0$ y $\lvert\lvert f \rvert\rvert_{p}=0 \rightarrow f=0$ casi dondequiera.
2. $\lvert\lvert \alpha f \rvert\rvert_{p}= \left\lvert \alpha\right\rvert \lvert\lvert f \rvert\rvert_{p}$ $(\alpha \in \mathbb{R})$.
3. $\lvert\lvert f+g \rvert\rvert_{p}\leq \lvert\lvert f \rvert\rvert_{p}+\lvert\lvert g \rvert\rvert_{p}$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/spaces/home/conceptos/semestre-6/equivalencia-de-funciones-en-lp/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Definición 

> [!definition|*]
> Sea $p \in [0,\infty)$ fija. Definimos una relación $\sim$ en $\mathcal{L}_{p}(\mu)$ como sigue:
> $f \sim g \iff \lvert\lvert f-g \rvert\rvert_{p}=0.$
> *Observación.* $\sim$ define una relación de equivalencia en $\mathcal{L}_{p}(\mu)$. Si $[f]$ denota la clase de equivalencia de $f$ relativa a $\mu$, definimos
> $\lvert\lvert [f] \rvert\rvert=\lvert\lvert f \rvert\rvert_{p},$
> este valor es independiente del representante y esta función constituye una norma en el espacio vectorial constituido por las clases con las operaciones naturales.
>

</div></div>
    

