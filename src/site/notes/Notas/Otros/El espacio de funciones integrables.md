---
{"dg-publish":true,"permalink":"/notas/otros/el-espacio-de-funciones-integrables/"}
---

#Tema/Análisis  #Tipo/Nota 

# Introducción


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/funcion-integrable/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Definición 



> [!definition|*] Función integrable
> 
> Sea $(X,S,\mu)$ un [[Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]] dado. Denotaremos por $\overline{\mathcal{L}_{1}}(X,S,\mu)$ a la clase de funciones $f \in \overline{M}(X,S)$ tales que:
> $\int_{}^{} f^{+} \, d\mu <\infty \text{ y } \int_{}^{} f^{-} \, d\mu <\infty$
> A dichas funciones las llamaremos **integrables con respecto a $\mu$**. Para $f \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ y $E \in S$ dados, definimos:
> $\int_{E}^{} f \, d\mu = \int_{E}^{} f^{+} \, d\mu - \int_{E}^{} f^{-} \, d\mu .$

</div></div>


> [!remark|*]
> Notemos que $\int_{E}^{} f^{+} \, d\mu$ y $\int_{E}^{} f^{-} \, d\mu$ son finitas para todo $E \in S$, por lo que la diferencia tiene sentido y prueba que $f\cdot \chi_{E} \in \overline{\mathcal{L}_{1}}(X,S,\mu)$. 

Denotamos por $\mathcal{L}_{1}(X,S,\mu)$ a la subclase de funciones $\mu-$integrables que toman valores en $\mathbb{R}.$


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/propiedades-de-las-funciones-integrables/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Teorema 



> [!theorem|*] Propiedades de las funciones integrables
> 
> Sea $(X,S,\mu)$ un [[Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]] dado, entonces:
> 1. $f \in \overline{\mathcal{L}_{1}}(X,S,\mu) \iff \left\lvert f\right\rvert=f^{+}+f^{-} \in \overline{\mathcal{L}_{1}}(X,S,\mu)$. En cuyo caso
> 	$\left\lvert \int_{}^{} f \, d\mu \right\rvert\leq \int_{}^{} \left\lvert f\right\rvert \, d\mu .$
> 2. Si $f \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ y $g \in \overline{M}(X,S)$ es tal que $\left\lvert g\right\rvert\leq \left\lvert f\right\rvert$, entonces $g \in \overline{\mathcal{L}_{1}}(X,S,\mu).$

</div></div>


> [!lemma|*]
> Sea $f \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ dada. Si $f=f_{1}-f_{2}$ casi dondequiera con $f_{1},f_{2} \in \overline{M^{+}}(X,S)$ con 
> $$\int_{}^{} f_{i} \, d\mu <\infty.$$
> Entonces
> $$\int_{E}^{} f \, d\mu =\int_{E}^{} f_{1} \, d\mu -\int_{E}^{} f_{2} \, d\mu \text{ para todo } E \in S.$$
{ #fadc9d}


 
<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/linealidad-de-la-integral/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis #Tipo/Teorema

> [!theorem|*] Linealidad de la integral
> 
> Sean $f,g \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ y $\alpha \in \mathbb{R}$ dados, entonces $\alpha f ,f+g \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ y 
> $\int_{E}^{} \alpha f \, d\mu = \alpha \int_{E}^{} f \, d\mu \text{ y } \int_{E}^{} f+g \, d\mu =\int_{E}^{} f \, d\mu +\int_{E}^{} g \, d\mu .$
> Para todo $E \in S$.






</div></div>


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/propiedades-de-la-integral/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis #Tipo/Teorema

> [!theorem|*] Propiedades de la integral
> 
> Sean $F,G \in S$ ajenos entre sí y $f,g \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ dados. Entonces
> 1. $\int_{F \cup G}^{} f \, d\mu= \int_{F}^{} f \, d\mu+ \int_{G}^{} f \, d\mu$,
> 2. $\int_{E}^{} f \, d\mu\leq \int_{E}^{} g \, d\mu$ para todo $E \in S$ si y sólo si $f\leq g$ casi dondequiera relativo a $\mu$,
> 3. $\int_{E}^{} f \, d\mu=\int_{E}^{} g \, d\mu$ para todo $E \in S$ si y sólo si $f=g$ casi dondequiera relativo a $\mu$.



</div></div>


# El teorema de la convergencia dominada de Lebesgue


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/teorema-de-la-convergencia-dominada/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis #Tipo/Teorema

> [!theorem|*] De la convergencia dominada
> 
> Sean $(X,S,\mu)$ un [[Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]] y $(f_{n})_{n \in \mathbb{N}}$ una sucesión de funciones en $\overline{\mathcal{L}_{1}}(X,S,\mu)$ tal que $f_{n}$ converge puntualmente a $f$ casi dondequiera relativo a $\mu$ para alguna $f \in \overline{M}(X,S)$. Supongamos que existe $g \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ tal que $\left\lvert f_{n}\right\rvert\leq g$ casi dondequiera relativo a $\mu$ para todo $n \in \mathbb{N}$. Entonces:
> 1. $f \in \overline{\mathcal{L}_{1}}(X,S,\mu)$,
> 2. $\int_{E}^{} f \, d\mu=\lim_{ n \to \infty }\int_{E}^{} f_{n} \, d\mu$ para todo $E \in S$.



</div></div>


## Observaciones
1. Un caso particular que aparece con frecuencia es el siguiente: La medida del esapcio es *finita* y existe $k>0$ constante tal que $\left\lvert f_{n}\right\rvert\leq k$ para todo $n \in \mathbb{N}$. Es claro que $g=k \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ y las conclusiones del teorema se satisfacen. En este contexto, el [[Conceptos/Semestre 6/Teorema de la convergencia dominada\|Teorema de la convergencia dominada]] se conoce como el **teorema de la convergencia acotada**
2. Para integrales de Riemann, en el que $X=[a,b]$, el teorema de la convergencia acotada (conocido como el teorema de Arzela-Osgood) es más débil, pues se exige queu la función límite sea Riemann-integrable, hecho que no se sigue de suponer sólamente la convergencia puntual.
3. La presencia de una función $g$ que domine es indispendable aún si $\mu(X)<\infty$, por ejemplo; Sean $X=\mathbb{N}$, $S=\mathcal{P}(\mathbb{N})$ y $\mu:S \to \mathbb{R}$ dada por 
$$\mu(E)=\sum_{j\in E}^{} \frac{1}{2^{j}}$$
	o $0$ si $E=\emptyset$. Sea $f_{n}=2^{n} \chi_{n+1,n+2,\dots}$, entonces
	$$\int_{\mathbb{N}}^{} f_{n} \, d\mu =1 \text{  para todo }n \text{ y } f_{n}\to 0.$$
	por lo que la conclusión del [[Conceptos/Semestre 6/Teorema de la convergencia dominada\|Teorema de la convergencia dominada]] falla.

> [!corollary|*]
> Sean $(X,S,\mu)$ un [[Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]] y $a<b$ en $\mathbb{R}$ fijas. Si $f:X\times(a,b) \to \mathbb{R}$ es una función tal que $f^{t}:X \to \mathbb{R}$ dada por $f^{t}(x)=f(x,t)$ es $S$-medible para todo $t \in (a,b)$ y $f_{x}:(a,b)\to \mathbb{R}$ dada por $f_{x}(t)=f(x,t)$ es continua para todo $x \in X$ y además existe $g \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ tal que $\left\lvert f(x,t)\right\rvert\leq g(x)$ para todo $x,t$, entonces la función $F:(a,b)\to \mathbb{R}$ definida por:
> $$F(t)=\int_{X}^{} f^{t} \, d\mu.$$
> Es una función continua.

> [!corollary|*]
> Usando la notación del corolario anterior. Supongamos ahora que existe $t_{0} \in (a,b)$ tal que $f^{t_{0}} \in \mathcal{L}_{1}(X,S,\mu)$, que $\frac{ \partial f }{ \partial t }$ existe en $X\times(a,b)$ y que existe $g \in \overline{\mathcal{L}_{1}}(X,S,\mu)$ tal que $\left\lvert \frac{ \partial f }{ \partial t }(x,t)\right\rvert\leq g$, entonces $F$ es diferenciable en $t$ y $F'(t)=\int_{}^{} \frac{ \partial f }{ \partial t }(x,t) \, d\mu.$

# Funciones integrables con valores complejos


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/integral-de-funciones-complejas/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Definición 

> [!definition|*] Integral de funciones complejas
> 
> Sea $(X,S,\mu)$ un [[Conceptos/Semestre 6/Espacio de medida\|Espacio de medida]], denotemos por $M_{\mathbb{C}}(X,S)$ al espacio de funciones $f:X \to \mathbb{C}$ que son $S$-medibles. Definimos
> $\mathcal{L}_{1}^{\mathbb{C}}(X,S,\mu)=\left\{ f \in M_{\mathbb{C}}(X,S): \Re(f),\Im(f) \in \mathcal{L}_{1}(X,S,\mu) \right\}.$
> Y para $f \in \mathcal{L}_{1}^{\mathbb{C}}(X,S,\mu)$ y $E\in S$, definimos
> $\int_{E}^{} f \, d\mu =\int_{E}^{} \Re(f)  \, d\mu + i \int_{E}^{} \Im(f) \, d\mu.$
> Si $f \in \mathcal{L}_{1}^{\mathbb{C}}(X,S,\mu)$, entonces decimos que $f$ es **integrable**.
>

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/propiedades-de-las-funciones-integrables-complejas/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Análisis  #Tipo/Teorema 



> [!theorem|*] Propiedades de las funciones integrables complejas
> 
> 1. $f \in \mathcal{L}_{1}^{\mathbb{C}}(X,S,\mu) \iff \left\lvert f\right\rvert=\left( (\Re(f))^{2}+ (\Im(f))^{2} \right)^{\frac{1}{2}} \in \mathcal{L}_{1}(X,S,\mu).$ En cuyo caso 
> 	$\left\lvert \int_{}^{} f \, d\mu \right\rvert\leq \int_{}^{} \left\lvert f\right\rvert \, d\mu .$
> 2. Si $f \in \mathcal{L}_{1}^{\mathbb{C}}(X,S,\mu)$ y $g \in M_{\mathbb{C}}(X,S)$ es tal que $\left\lvert g\right\rvert\leq \left\lvert f\right\rvert$, entonces $g \in \mathcal{L}_{1}^{\mathbb{C}}(X,S)$.

</div></div>


> [!remark|*]
> $$\left\lvert \int_{E}^{} f \, d\mu \right\rvert=\int_{E}^{} \left\lvert f\right\rvert \, d\mu \iff \text{ existe } \theta \in \mathbb{R} \text{ tal que } \mu(\left\{ x \in E: f(x)\not= e^{i\theta}\left\lvert f(x)\right\rvert \right\})=0.$$
> Es decir, la función $f$ toma sus valores casi dondequiera en $E$ sobre un rayo que parte del origen.







