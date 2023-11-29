---
{"dg-publish":true,"permalink":"/tareas/semestre-6/topologia-ii/examen-3/"}
---


> [!exercise] Ejercicio 1
>1.  Sea ${}X:= \prod_{\alpha \in \mathcal{A}}^{} X_{\alpha}{}$ un producto de espacios topológicos (equipado con la topología de Tychonoff) y sea ${}(x_{\lambda})_{\lambda \in \Lambda}{}$ una red en ${}X{}$. Supongamos que ${}y \in X{}$ es un punto de acumulación de la [[Conceptos/Semestre 6/Red\|Red]]. Demuestra que ${}\pi_{\alpha}(y){}$ es un punto de acumulación de la red ${}(\pi_{\alpha}(x_{\lambda}))_{\lambda \in \Lambda}{} \subseteq X_{\alpha}$.
>2. Muestra con un ejemplo que el recíproco del inciso anterior es falso, incluso si hay una cantidad finita de factores.

*Demostración.* 
1. Sea ${}U \in \mathcal{N}(\pi_{\alpha}(y)){}$. Como ${}\pi_{\alpha}{}$ es continua, entonces ${}\pi_{\alpha}^{-1}(U) \in \mathcal{N}(y){}$. Como ${}(x_{\lambda})_{\lambda \in \Lambda}{}$ converge a ${}y{}$ entonces existe ${}\lambda_{0}{}$ tal que si ${}\lambda\geq \lambda_{0}{}$ entonces ${}x_{\lambda} \in \pi_{\alpha}^{-1}(U){}$. Por lo tanto, ${}\pi_{\alpha}(x_{\lambda}) \in U{}$. Así, para cada ${}U \in \mathcal{N}(\pi_{\alpha}(y)){}$ existe ${}\lambda_{0} \in \Lambda{}$ tal que si ${}\lambda\geq \lambda_{0}{}$ entonces ${}\pi_{\alpha}(x_{\lambda}) \in U{}$, es decir, ${}\pi_{\alpha}(y){}$ es un punto de acumulación de ${}(\pi_{\alpha}(x_{\lambda}))_{\lambda \in \Lambda}{}$.
2. Considera la sucesión ${}(x_{n},y_{n}): \mathbb{N} \to \mathbb{R}^{2}{}$, donde ${}x_{n}=y_{n}=(-1)^{n}{}$ para cada ${}n \in \mathbb{N}{}$. 
	Observa que ${}-1{}$ es un punto de acumulación de ${}(x_{n})_{n \in \mathbb{N}}{}$, pues para cada ${}n_{0} \in \mathbb{N}{}$ existe ${}n\geq n_{0}{}$ tal que ${}x_{n}=-1{}$ y, en particular, dado ${}U \in \mathcal{N}(-1){}$ se tiene que ${}x_{n} \in U.{}$ Análogamente ${}y_{n}{}$ se acumula en ${}1{}$. 
	Nota que ${}(x_{n},y_{n}){}$ no se acumula en ${}(-1,1){}$, pues para ${}\mathbb{B}\left( \frac{1}{2}, (-1,1) \right){}$ se tiene que ${}(x_{n},y_{n}) \not \in \mathbb{B}\left( \frac{1}{2},(-1,1) \right){}$.
$\blacksquare$

> [!exercise] Ejercicio 2
> Sea ${}\mathcal{G}{}$ un filtro.
> 1. Si ${}\mathcal{G}{}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]], demuestra que la red [[Conceptos/Semestre 6/Red basada en un filtro\|basada]] en ${}\mathcal{G}{}$ es una ultrared.
> 2. Si además ${}\mathcal{G}{}$ es un ultrafiltro libre, demuestra que la ultrared [[Conceptos/Semestre 6/Red basada en un filtro\|basada]] en ${}\mathcal{G}{}$ es no trivial (no constante).

*Demostración.*
Recuerda la definición: [[Conceptos/Semestre 6/Red basada en un filtro\|Red basada en un filtro]]
1. Sea ${}\mathcal{G}{}$ un ultrafiltro. Sea ${}E \subseteq X{}$. Entonces ${}X\setminus E \in \mathcal{G}{}$ o ${}E \in \mathcal{G}{}$.
	- Supongamos que ${}X\setminus E \in \mathcal{G}{}$. Sea ${}x \in X \setminus E{}$. Entonces, si ${}(x,X\setminus E)\leq(y,V){}$ se tiene que ${}y \in V \subseteq X\setminus E{}$, de modo que ${}y \in X \setminus E{}$. Entonces ${}(q(x,F))_{(x,F) \in \mathcal{A}_\mathcal{G}}{}$ está residualmente en ${}X \setminus E{}$, donde ${}q(x,F)=x{}$ para cada ${}(x,F) \in \mathcal{A}_{\mathcal{F}}{}$.
	- Supongamos que ${}E \in \mathcal{G}{}$. Sea ${}x \in E{}$. Entonces, si ${}(x,E)\leq (y, V){}$ se tiene que ${}y \in V \subseteq E{}$ y ${}y \in E{}$. Por lo tanto, ${}(q(x,F))_{F \in \mathcal{A}_{\mathcal{\mathcal{G}}}}{}$ está residualmente en ${}E{}$.
	En cualquier caso, la red basada en el filtro está residualmente en ${}E{}$ o en ${}X\setminus E{}$.
	Entonces la red basada en ${}\mathcal{G}{}$ es una [[Conceptos/Semestre 6/Ultrared\|Ultrared]].
2. Supongamos que ${}\mathcal{G}{}$ es un ultrafiltro libre. Sea ${}(q(x,F))_{(x,F) \in \mathcal{A}_{\mathcal{G}}}{}$ la red basada en ${}\mathcal{G}{}$.
	Supongamos que ${}(q(x,F))_{(x,F) \in \mathcal{A}_{\mathcal{G}}}{}$ es constante e igual a ${}x{}$. Sea ${}F \in \mathcal{G}{}$ y ${}y \in F{}$. Entonces ${}(y,F) \in \mathcal{A}_{\mathcal{G}}{}$ y ${}y=q(y,F)=x{}$, de modo que ${}y=x{}$ y ${}x \in \mathcal{F}{}$. Por lo tanto, ${}x \in F{}$ para cada ${}F \in \mathcal{G}{}$, i.e, ${}\mathcal{G}{}$ es fijo. En consecuencia, ${}(q(x,F))_{(x,F)\in \mathcal{A}_{\mathcal{G}}} {}$ no es constante.
$\blacksquare$ 

> [!exercise] Ejercicio 3
> Sea ${}X{}$ un conjunto y ${}\mathcal{F}{}$ un ultrafiltro. Demuestra que los siguientes enunciados son equivalentes.
> 1. ${}\mathcal{F}{}$ es fijo.
> 2. El kernel de ${}\mathcal{F}{}$ es un elemento de ${}\mathcal{F}{}$.
> 3. Existe ${}x \in X{}$ tal que ${}\left\{x \right\} \in \mathcal{F}{}$.
> 4. Existe ${}x \in X{}$ tal que ${}\mathcal{F}= \left\{ F \subseteq X : x \in F\right\}{}$.
> 5. ${}\mathcal{F}{}$ no contiene al filtro de Frechet en ${}X{}$.

*Demostración.* 
- ${}1 \rightarrow 2{}$ Supongamos que ${}\mathcal{F}{}$ es fijo. Entonces $Ker(\mathcal{F})={}\bigcap_{ F \in \mathcal{F}}F \neq \emptyset{}$. Como ${}\mathcal{F}{}$ es un ultrafiltro entonces ${}Ker(F) \in \mathcal{F}{}$ o ${}X\setminus Ker(F) \in \mathcal{F}{}$. Si ${}X \setminus Ker(\mathcal{F}) \in \mathcal{F}{}$ entonces se tendría que ${}Ker(\mathcal{F}) \cap \bigcap_{ }\mathcal{F}= \emptyset{}$, lo cual es imposible. Entonces ${}Ker(F)\in \mathcal{F}{}$.
- ${}2 \rightarrow 3{}$ Supongamos que ${}Ker(\mathcal{F}) \in \mathcal{F}{}$. Sea ${}x \in Ker (\mathcal{F}){}$. Si ${}X \setminus \left\{x \right\} \in \mathcal{F}{}$ entonces ${}x \not \in \bigcap_{ F \in \mathcal{F}}F{}$, lo cual es imposible. Entonces ${}\left\{x \right\} \in \mathcal{F}{}$, pues ${}\mathcal{F}{}$ es ultrafiltro.
- ${}3 \rightarrow 4{}$ Sea ${}F \in \mathcal{F}{}$. Entonces ${}\left\{x \right\}\cap F \neq \emptyset{}$ y ${}x \in F{}$. Por otro lado, si ${}x \in F{}$ entonces ${}\left\{x \right\} \subseteq F{}$ y, por lo tanto, ${}F \in \mathcal{F}{}$.
- ${}4\rightarrow 5{}$ Supongamos que ${}\mathcal{F}{}$ contiene el filtro de Frechet. Sea ${}x \in X{}$ tal que ${}\mathcal{F}= \left\{F \subseteq X : x \in F\right\}{}$. Entonces ${}X\setminus \left\{x \right\} \in \mathcal{F}{}$, pues ${}X\setminus \left\{x \right\}{}$ tiene complemento finito, pero ${}x \not \in X\setminus \left\{x \right\}{}$, lo cual es imposible. Entonces ${}\mathcal{F}{}$ no contiene el filtro de Frechet.
- ${}5 \rightarrow 1{}$ Supongamos que existe ${}G{}$ con ${}X\setminus G{}$ finito tal que ${}G \not \in \mathcal{F}{}$. Como ${}\mathcal{F}{}$ es un ultrafiltro, entonces ${}X\setminus G \in \mathcal{F}{}$. Supongamos que ${}\bigcap_{F \in \mathcal{F}}F = \emptyset{}$. Entonces, para cada $x \in X\setminus G$ existe ${}F_{x} \in \mathcal{F}{}$ tal que ${}x \not \in F_{x}{}$, pues de lo contario ${}\cap \mathcal{F}{}$ no sería vacío. Como ${}X \setminus G{}$ es finito, entonces existen ${}F_{x_{1}},\dots F_{x_{n}}{}$ tales que ${}x_{i} \not \in F_{x_{i}}{}$ para cada ${}i= 1,\dots,n{}$ y donde ${}X\setminus G = \left\{x_{1},\dots,x_{n} \right\}{}$. Luego, como los filtros son cerrados bajo intersecciones finitas, entonces ${}X\setminus G \cap F_{x_{1}} \cap\dots \cap F_{x_{n}} \in \mathcal{F}{}$. Pero como ${}F_{x_{i}}{}$ no tiene a ${}x_{i}{}$ como elemento, entonces ${}X \setminus G \cap F_{x_{1}} \cap \dots \cap F_{x_{n}}= \emptyset{}$, lo caules es imposible. Por lo tanto ${}\cap \mathcal{F} \neq \emptyset{}$ y ${}\mathcal{F}{}$ es un filtro fijo.
$\blacksquare$