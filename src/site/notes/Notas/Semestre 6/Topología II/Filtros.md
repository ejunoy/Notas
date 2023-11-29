---
{"dg-publish":true,"permalink":"/notas/semestre-6/topologia-ii/filtros/"}
---


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/filtro/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Tema/Topología  #Tipo/Definición 

> [!definition|*] Filtro
> 
> Sea ${} X {}$ un conjunto. Un **filtro** en ${} X {}$ es una familia ${} \mathcal{F} \subseteq \mathcal{P}(x) {}$ tal que:
> 1. ${} \forall F \in \mathcal{F} {}$, ${} F \neq \emptyset {}$.
> 2. Si ${} F,G \in \mathcal{F} {}$ entonces ${} F \cap G \in \mathcal{F} {}$.
> 3. Si ${} F \in \mathcal{F} {}$ y ${} F \subseteq G \subseteq X {}$ entonces ${} G \in \mathcal{F} {}$.

</div></div>

## Ejemplos 
1. Sea ${} A\subseteq X {}$ y ${} \mathcal{F}_{A}= \left\{ F \subseteq X : A\subseteq F\right\} {}$. Entonces $\mathcal{F}_{A}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]].
2. Sea  infinito y .  es un [[Conceptos/Semestre 6/Filtro\|filtro]] llamado [[Conceptos/Semestre 6/Filtro\|filtro]] de Frechét.

## Ejemplo 
Si $(X,\tau)$ es un [[Conceptos/Semestre 6/Espacio topológico\|espacio topológico]] entonces ${} \mathcal{N}(x)= \left\{U \subseteq X: x \in Int(U) \right\} {}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]]. A ${} \mathcal{N}(x) {}$ se le llama [[Conceptos/Semestre 6/Filtro\|filtro]] de vecindades de ${} x {}$.

> [!definition|*] Base de [[Conceptos/Semestre 6/Filtro\|filtro]]
> 
> Sea ${} X {}$ un conjunto y ${} \mathcal{F} {}$ un [[Conceptos/Semestre 6/Filtro\|filtro]]. Diremos que ${} \mathcal{C}\subseteq \mathcal{F} {}$ es una **base de [[Conceptos/Semestre 6/Filtro\|filtro]]** para ${} \mathcal{F} {}$ si ${} \forall F \in \mathcal{F} {}$ ${} \exists U \in \mathcal{C} {}$ tal que ${} U\subseteq F {}$.
> 
{ #39c972}


## Ejemplo 
${} \mathcal{C}= \left\{ A \right\} {}$ es base para el [[Conceptos/Semestre 6/Filtro\|filtro]] ${} \mathcal{F}_{A} {}$.

**Observación.** Si ${} \mathcal{C} {}$ es base de [[Conceptos/Semestre 6/Filtro\|filtro]], entonces ${} \mathcal{C} {}$ cumple:
1. ${} \forall C \in \mathcal{C}, C \neq \emptyset{}$.
2. Si ${} C_{1} \land C_{2} \in \mathcal{C} {}$ entonces existe ${} C_{3} \in \mathcal{C} {}$ tal que ${} C_{3}\subseteq C_{1} \cap C_{2} {}$.

> [!proposition|*]
> Sea ${} \mathcal{C}\subseteq \mathcal{P}(X) {}$. Si ${} \mathcal{C} {}$ cumple:
> 1. ${} \forall C \in \mathcal{C} {}$, ${} C \neq \emptyset {}$.
> 2. Si ${} C_{1} \land C_{2} \in \mathcal{C} {}$ entonces ${} \exists C_{3} \in \mathcal{C} {}$ tal que ${} C_{3}\subseteq C_{1} \cap C_{2} {}$.
> Entnoces existe un único [[Conceptos/Semestre 6/Filtro\|filtro]] ${} \mathcal{F}_{\mathcal{C}} \subseteq \mathcal{P}(X) {}$ tal que ${} \mathcal{C} {}$ es base para ${} \mathcal{F}_{\mathcal{C}} {}$.
> 

*Demostración.* 
Sea ${} \mathcal{F}_{\mathcal{C}}= \left\{F \subseteq X: \exists C \in \mathcal{C}  \text{  con  }C \subseteq F \right\} {}$. Veamos que ${} \mathcal{F}_{\mathcal{C}} {}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]].
1. Sea ${} F \in \mathcal{F}_{\mathcal{C}} {}$ entonces existe ${} C \in \mathcal{C} {}$ tal que ${} C\subseteq F {}$ y, como ${} C \neq \emptyset {}$ entonces $F \neq \emptyset$.
2. Sean $F_{1},F_{2} \in \mathcal{F}_{\mathcal{C}}$. Entonces existen ${} C_{1},C_{2} \in \mathcal{C}{}$ tales que ${} C_{1}\subseteq F_{1} {}$ y ${} C_{2} \subseteq F_{2} {}$. De modo que ${} C_{1}\cap C_{2} \subseteq F_{1} \cap F_{2} {}$ y, por hipótesis existe ${} C_{3} {}$ tal que ${} C_{3} \subseteq C_{1} \cap C_{2} {}$. Por lo tanto ${} F_{1} \cap F_{2} \in \mathcal{F}_{\mathcal{C}} {}$.
3. Sea ${} F \in \mathcal{F}_{\mathcal{C}} {}$ y ${} G\subseteq X {}$ tal que ${} F\subseteq G {}$. Entonces existe ${} C \in \mathcal{C} {}$ tal que ${} C \subseteq F \subseteq G {}$ y, por lo tanto, ${} G \in \mathcal{F}_{\mathcal{C}} {}$.
Si ${} \mathcal{G} {}$ es otro [[Conceptos/Semestre 6/Filtro\|filtro]] para el cual ${} \mathcal{C} {}$ es base, entonces para cada ${} G \in \mathcal{G} {}$ se tiene que existe ${} C \in \mathcal{C} {}$ tal que ${} C \subseteq G {}$, de tal forma que ${} G \in \mathcal{F}_{\mathcal{C}} {}$. Si ${} G \in \mathcal{F}_{\mathcal{C}} {}$ entonces existe ${} C \in \mathcal{C} {}$ tal que ${} C \subseteq G {}$ y, como ${} \mathcal{C}\subseteq \mathcal{G} {}$ entonces ${} G \in \mathcal{G} {}$. Por lo tanto ${} \mathcal{F}_{\mathcal{C}}=\mathcal{G} {}$.
$\blacksquare$

## Ejemplo
Sea ${} \mathcal{C}= \left\{(a,\infty): a \in \mathbb{R} \right\} {}$. ${} \mathcal{C} {}$ es base para un [[Conceptos/Semestre 6/Filtro\|filtro]] en ${} \mathcal{F}_{\mathcal{C}} {}$ en ${} \mathbb{R} {}$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/filtro-fino-y-grueso/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición 
 
> [!definition|*] [[Conceptos/Semestre 6/Filtro\|Filtro]] fino y grueso
> 
> Si ${} \mathcal{F}_{1} {}$ y ${} \mathcal{F}_{2} {}$ son filtros en un conjunto ${} X {}$ diremos que ${} \mathcal{F}_{1} {}$ es **más fino** que ${} \mathcal{F}_{2} {}$ si ${} \mathcal{F}_{2}\subseteq \mathcal{F}_{1} {}$.
> En este caso también decimos que ${} \mathcal{F}_{2} {}$ es más grueso que ${} \mathcal{F}_{1} {}$.

</div></div>


## Ejemplo
Sea ${} \mathcal{F}_{\mathcal{C}} {}$ el [[Conceptos/Semestre 6/Filtro\|filtro]] del ejemplo anterior y $\mathcal{F} {}$ el [[Conceptos/Semestre 6/Filtro\|filtro]] de Fréchet en $\mathbb{R}$. Claramente $\forall F \in \mathcal{F}$ $\exists a \in \mathbb{R}\setminus F$ tal que $a\geq x$ $\forall x \in \mathbb{R}\setminus F$, pues $\mathbb{R} \setminus F$ es finito.
Si $x>a$ entonces $x \not \in \mathbb{R}\setminus F {}$ y $x \in \mathbb{R}$. Entonces $(a,\infty)\subseteq F$ y, por lo tanto, $F \in \mathcal{F}_{\mathcal{C}}$.
$\therefore \mathcal{F} \subseteq \mathcal{F}_{\mathcal{C}}$
$\therefore \mathcal{F}_{\mathcal{C}}$ es más fino que $\mathcal{F}$.

## Ejemplo
$\mathcal{N}(x)$ es más grueso que $\mathcal{F}_{\left\{x \right\}}$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/filtro-fijo-y-filtro-libre/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición 
> [!definition|*] [[Conceptos/Semestre 6/Filtro\|Filtro]] fijo y libre
> 1. Diremos que $\mathcal{F}$ es **fijo** si $\bigcap_{F \in \mathcal{F}}F \neq \emptyset$.
> 2. Diremos que $\mathcal{F}$ es **libre** si $\bigcap_{F \in \mathcal{F}} F = \emptyset$.

</div></div>


## Nota
$\bigcap_{F \in \mathcal{F}}F$ se llama el **kernel** del [[Conceptos/Semestre 6/Filtro\|filtro]].

## Ejemplo
$\mathcal{N}(x)$ y $\mathcal{F}_{A}= \left\{F \subseteq X: A\subseteq X \right\}$ son filtros fijos.

## Ejemplo
El [[Conceptos/Semestre 6/Filtro\|filtro]] de Frechét $\mathcal{F}= \left\{ F\subseteq X : X\setminus F \text{ es finito }\right\}$ es libre. Si $x \in X$ entonces $X\setminus \left\{x \right\} \in \mathcal{F}$, así que $\bigcap_{F \in \mathcal{F}} F\not \ni x$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/convergencia-de-filtros/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición  
> [!definition|*] Convergencia de filtros
> Sea ${}X{}$ un [[Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${}\mathcal{F}{}$ un [[Conceptos/Semestre 6/Filtro\|filtro]] en ${}X{}$. Diremos que ${}\mathcal{F}{}$ **converge** a ${}x \in X{}$ (Notación ${}\mathcal{F} \to x{}$) si ${}\mathcal{N}(x)\subseteq \mathcal{F}{}$, es decir, ${}\mathcal{F}{}$ es más fino que ${}\mathcal{N}(x){}$.

</div></div>

## Ejemplo 
${}\mathcal{N}(x) \to x{}$ para cada ${}x \in X{}$.

## Ejemplo 
Sea ${}\mathcal{F}{}$ el [[Conceptos/Semestre 6/Filtro\|filtro]] de Frechet en ${}\mathbb{R}{}$. Sea ${}x \in \mathbb{R}{}$ y sea ${}\varepsilon>0{}$. Entonces ${}(x-\varepsilon,x+\varepsilon){}$ es una vecindad de ${}x{}$ cuyo complemento es infinito. Entonces ${}\mathcal{F}{}$ no [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x{}$.
**Pero [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x{}$ con la topología cofinita.**


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/punto-de-acumulacion-de-un-filtro/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición  
>[!definition|*] Punto de acumulación de un [[Conceptos/Semestre 6/Filtro\|filtro]]
>Sea ${}X{}$ un [[Conceptos/Semestre 6/Espacio topológico\|espacio topológico]] y ${}\mathcal{F}{}$ un [[Conceptos/Semestre 6/Filtro\|filtro]] en ${}X{}$. Diremos que ${}x{}$ es un **punto de acumulación** de ${}\mathcal{F}{}$ o que ${}\mathcal{F}{}$ **se acumula** en ${}x{}$ si para cada ${}F \in \mathcal{F}{}$ y para cada ${}U \in \mathcal{N}(x){}$ se tiene que ${}F \cap U \neq \emptyset{}$.

</div></div>


**Observación.** 
- ${}x{}$ es un punto de acumulación de ${}\mathcal{F}{}$ si y solo si ${}x \in \bigcap_{F \in \mathcal{F}}\overline{F }{}$.
- Si ${}\mathcal{F} \to x{}$ entonces ${}x{}$ es punto de acumulación de ${}\mathcal{F}{}$.

## Ejemplo
Sea ${}X{}$ un [[Conceptos/Semestre 6/Espacio topológico\|espacio topológico]], ${}A\subseteq X{}$. Entonces cada punto ${}x \in \overline{A}$ es un punto de acumulación del [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}_{A}= \left\{ U\subseteq X : A\subseteq U\right\}{}$. Nota que si ${}x \in \overline{A}{}$ entonces para cada ${}U \in \mathcal{N}(x){}$ se tiene que ${}U \cap A \neq \emptyset{}$. Sea ${}V \subseteq X{}$ tal que ${}A \subseteq V{}$. Entonces para cada ${}U \in \mathcal{N}(x){}$, ${}U \cap V \neq \emptyset{}$. Así, para cada ${}U \in \mathcal{N}(x){}$, para cada ${}V \in \mathcal{F}_{A}{}$ se tiene que ${}U \cap V \neq \emptyset{}$ y, por lo tanto, ${}x{}$ es un punto de acumulación de ${}\mathcal{F}_{A}{}$.

**Observación.** Si ${}x \not \in \overline{A}{}$ entonces ${}X\setminus \overline{A} \in \mathcal{N}(x){}$. Como ${}\overline{A} \in \mathcal{F}{}$ y ${}\overline{A} \cap (X\setminus \overline{A}) = \emptyset{}$, entonces ${}x{}$ no es un punto de acumulación de ${}\mathcal{F}{}$.
${}\therefore{}$ los únicos puntos de acumulación de ${}\mathcal{F}{}$ son los puntos de ${}\overline{A}{}$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/convergencia-y-acumulacion-de-base-de-filtro/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición  
> [!definition|*] Convergencia y puntos de acumulación de una base para [[Conceptos/Semestre 6/Filtro\|filtro]]
> Sea ${}\mathcal{C}{}$ una [[Conceptos/Semestre 6/Base de filtro\|base de filtro]]. 
> 1. Diremos que ${}\mathcal{C}{}$ **converge** a ${}x{}$ si para cada ${}U \in \mathcal{N}(x){}$ existe ${}C \in \mathcal{C}{}$ tal que ${}C \subseteq U{}$ ${}\iff{}$ ${}\mathcal{F}_{\mathcal{C}} \to x{}$.
> 2. Diremos que ${}\mathcal{C}{}$ **se acumula** en ${}x{}$ si para cada ${}C \in \mathcal{C}{}$ y para cada ${}U \in \mathcal{N}(x){}$ se tiene que ${}C \cap U \neq \emptyset{}$ ${}\iff{}$ ${}\mathcal{F}_{\mathcal{C}}{}$ se acumula en ${}x{}$.

</div></div>


## Ejemplo 
En ${}\mathbb{R}{}$ con la topología usual el [[Conceptos/Semestre 6/Filtro\|filtro]] generado por ${}\mathcal{C}= \left\{(a,\infty): a \in \mathbb{R} \right\}{}$ no tiene puntos de acumulación. Pues, para cada ${}x \in X{}$ se tiene que ${}(x-\varepsilon,x+\varepsilon)\cap (x+\varepsilon,\infty)= \emptyset{}$.

## Ejemplo 
Sea ${}\mathcal{C}= \left\{(0,\varepsilon): \varepsilon>0 \right\}{}$ y ${}\mathcal{F}_{\mathcal{C}}{}$ el [[Conceptos/Semestre 6/Filtro\|filtro]] generado por ${}\mathcal{C}{}$. Sea ${}U \in \mathcal{N}(0){}$. Entonces existe ${}\varepsilon>0{}$ tal que ${}(-\varepsilon,\varepsilon)\subseteq U{}$, de modo que ${}(0,\varepsilon) \subseteq U{}$ y ${}U \in \mathcal{F}_{\mathcal{C}}{}$ entonces ${}\mathcal{N}(0)\subseteq \mathcal{C}{}$ y ${}\mathcal{F}_{\mathcal{C}}{}$ [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}0{}$.

> [!proposition|*]
> Sea ${}\mathcal{F}{}$ un [[Conceptos/Semestre 6/Filtro\|filtro]] en ${}X{}$ y ${}x \in X{}$. Entonces ${}x{}$ es punto de acumulación de ${}\mathcal{F}{}$ si y solo si existe un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{G}{}$ en ${}X{}$ tal que ${}\mathcal{G}{}$ [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x{}$ y ${}\mathcal{F} \subseteq \mathcal{G}{}$.

*Demostración.* 
- ${}\rightarrow{}$ Sea ${}\mathcal{C}= \left\{ U \cap F: F \in \mathcal{F} \land U \in \mathcal{N}(x)\right\}{}$. Como ${}x{}$ es un punto de acumulación de ${}\mathcal{F}{}$ entonces ${}U \cap F \neq \emptyset{}$ para cada ${}U \in \mathcal{N}(x){}$ y ${}F \in \mathcal{F}{}$. Además, si ${}U\cap F, V \cap F \in \mathcal{C}{}$ entonces ${}(U \cap F)\cap (V \cap F)= (U \cap V) \cap F \in \mathcal{C}{}$. 
	${}\therefore{}$ ${}\mathcal{C}{}$ es base para un [[Conceptos/Semestre 6/Filtro\|filtro]] en ${}X{}$.
	Sea ${}\mathcal{G} = \mathcal{F}_{\mathcal{C}}{}$. Para cada ${}U \in \mathcal{N}(x){}$ y para cada ${}F \in \mathcal{F}{}$ se tiene que ${}U \cap F \subseteq U,F{}$, entonces ${}U,F \in \mathcal{G}{}$. De modo que ${}\mathcal{N}(x), \mathcal{F} \subseteq \mathcal{G}{}$.
- ${}\leftarrow{}$ Supongamos que existe un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{G}{}$ que [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x{}$ tal que ${}\mathcal{F} \subseteq \mathcal{G}{}$. Veamos que ${}x{}$ es un punto de acumulación de ${}\mathcal{F}_{\mathcal{C}}$. 
	Sea ${}F \in \mathcal{F}{}$ y ${}U \in \mathcal{N}(x){}$. Como ${}F \in \mathcal{F} \subseteq \mathcal{G} {}$ y ${}U \in \mathcal{N}(x)\subseteq \mathcal{G}{}$, de modo que ${}F \cap U \in \mathcal{G}{}$ y, por lo tanto, ${}F \cap U \neq \emptyset{}$.
$\blacksquare$

# Caracterización de la [[Conceptos/Semestre 6/Cerradura con filtros\|cerradura con filtros]]


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/cerradura-con-filtros/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Teorema  
> [!theorem|*] Cerradura con filtros
> Sea ${}(X,\tau){}$ un [[Conceptos/Semestre 6/Espacio topológico\|espacio topológico]]. ${}A\subseteq X{}$. Entonces un punto ${}x{}$ está en ${}\overline{ A}{}$ si y solo si existe un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ tal que ${}A \in \mathcal{F}{}$ y ${}\mathcal{F} \to x{}$.

*Demostración.* 
- ${}\rightarrow{}$ Sea ${}x \in \overline{A}{}$. Sea ${}\mathcal{C}= \left\{ U \cap A : U \in \mathcal{N}(x) \right\}{}$. Entonces ${}\mathcal{C}{}$ es base para un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}= \mathcal{F}_{\mathcal{C}}{}$. Además, se cumple que ${}A \in \mathcal{F}{}$ y ${}\mathcal{N}(x)\subseteq \mathcal{F}{}$.
- ${}\leftarrow{}$ Supongamos que ${}\mathcal{F}{}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]] tal que ${}A \in \mathcal{F}{}$ y ${}\mathcal{N}(x) \subseteq \mathcal{F}{}$. Entonces para cada ${}U \in \mathcal{N}(x){}$ se tiene que ${}U \cap A \in \mathcal{F}{}$, de modo que ${}U \cap A \neq \emptyset{}$ y ${}x \in \overline{A}{}$.
$\blacksquare$

</div></div>


> [!corollary|*]
> ${}A{}$ es cerrado si y solo si para cada [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ que [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a algún punto ${}x{}$ con ${}A \in \mathcal{F}{}$ se tiene que ${}x \in A{}$.

*Demostración.* 
- ${}\rightarrow{}$ Supongamos que ${}A{}$ es cerrado. Si existe un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ con ${}A \in \mathcal{F}{}$ y que [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x{}$ entonces ${}x \in \overline{A}= A{}$.
- ${}\leftarrow{}$ Sea ${}x \in \overline{A}{}$. Entonces existe un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ con ${}A \in \mathcal{F}{}$ y que [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x{}$ y, por hipótesis, ${}x \in A{}$.
$\blacksquare$

# Continuidad y filtros 

<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/filtro-bajo-una-funcion/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición  
> [!definition|*] [[Conceptos/Semestre 6/Filtro\|Filtro]] bajo una función
> Sea ${}\mathcal{F}{}$ un [[Conceptos/Semestre 6/Filtro\|filtro]] en ${}X{}$ y ${}f: X \to Y{}$ una función. Definimos ${}f(\mathcal{F}){}$ como el [[Conceptos/Semestre 6/Filtro\|filtro]] en ${}Y{}$ generado por la base ${}\mathcal{C}= \left\{ f(F): F \in \mathcal{F} \right\}{}$.

</div></div>


> [!theorem|*] Continuidad con filtros
> Sea ${}f: X \to Y{}$ una función. Entonces ${}f{}$ es continua en ${}x_{0}{}$ si y solo si para todo [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ que [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x_{0}{}$ sucede que ${}f(\mathcal{F}){}$ [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}f(x_{0}){}$.


*Demostración.* 
- ${}\rightarrow{}$ Supongamos que ${}f{}$ es continua en ${}x_{0}{}$. Sea ${}\mathcal{F}{}$ un [[Conceptos/Semestre 6/Filtro\|filtro]] que [[Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${}x_{0}{}$. Sea ${}U \in \mathcal{N}(f(x_{0})){}$. Como ${}f{}$ es continua, entonces ${}f^{-1}(U) \in \mathcal{N}(x_{0}){}$. Como ${}\mathcal{F}{}$ converge a ${}x_{0}{}$ entonces ${}f^{-1}(U) \in \mathcal{F}{}$ y, por lo tanto, ${}U=f(f^{-1}(U)) \in f(\mathcal{F}){}$. Entonces ${}\mathcal{N}(f(x_{0}))\subseteq f(\mathcal{F}){}$, es decir, ${}f(\mathcal{F}){}$ converge a ${}x_{0}{}$.
- ${}\leftarrow{}$ Sea ${}A \subseteq X{}$. Tomemos ${}x \in \overline{A}{}$. Entonces existe un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ que converge a ${}x{}$ con ${}A \in \mathcal{F}{}$. Como ${}\mathcal{F}{}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]] que converge a ${}x{}$ entonces ${}f(\mathcal{F}){}$ converge a ${}f(x){}$, también, ${}f(A) \in f(\mathcal{F}){}$. Entonces ${}f(\mathcal{F}){}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]] que converge a ${}f(x){}$ y ${}f(A) \in f(\mathcal{F}){}$entonces ${}f(x) \in \overline{f(A)}{}$. 
	$\therefore$ ${}f(\overline{A})\subseteq \overline{f(A)}{}$ y ${}f{}$ es continua.

# Filtros y productos 
#Tema/Topología  #Tipo/Teorema  
> [!theorem|*] [[Conceptos/Semestre 6/Convergencia de filtros\|Convergencia de filtros]] en el producto
> Sea ${}X = \prod_{\alpha \in \mathcal{A}}^{} X_{\alpha}{}$ un producto de espacios topológicos. Un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ en ${}X{}$ converge a ${}x \in X{}$ si y solo si ${}\forall \alpha \in \mathcal{A}{}$ ${}\pi_{\alpha}(\mathcal{F}){}$ converge a ${}x_{\alpha}:= \pi_{\alpha}(x){}$.

*Demostración.* 
- ${}\rightarrow{}$ Como ${}\mathcal{F}{}$ converge a ${}x{}$ y ${}\pi_{\alpha}{}$ es continua, entonces ${}\pi_{\alpha}(\mathcal{F}){}$ converge a ${}\pi_{\alpha}(x){}$.
- ${}\leftarrow{}$ Sea ${}U \in \mathcal{N}(x){}$. Sea ${}\alpha \in \mathcal{A} {}$. Como ${}\pi_{\alpha}{}$ es abierta, entonces ${}\pi_{\alpha}(U) \in \mathcal{N}(\pi_{\alpha}(x)){}$. Pero ${}\pi_{\alpha}(\mathcal{F}){}$ converge a ${}x_{\alpha}{}$ entonces ${}\pi_{\alpha}(U) \in \pi_{\alpha}(\mathcal{F}){}$. Por lo tanto, existe ${}F \in \mathcal{F}{}$ tal que ${}\pi_{\alpha}(F) \subseteq \pi_{\alpha}(U){}$, de modo que ${}F \subseteq \pi_{\alpha}^{-1}(\pi_{\alpha}(F)) \subseteq \pi_{\alpha}^{-1}(\pi_{\alpha}(U)){}$, entonces ${}\pi_{\alpha}^{-1}(\pi_{\alpha}(U)) \in \mathcal{F}{}$.

# Ultrafiltros

> [!definition|*] [[Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]
> Sea ${}\mathcal{F}{}$ un [[Conceptos/Semestre 6/Filtro\|filtro]]. Diremos que ${}\mathcal{F}{}$ es un **[[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]]** si no existe ningún [[Conceptos/Semestre 6/Filtro\|filtro]] más fino que ${}\mathcal{F}{}$, i.e., ${}\mathcal{F}{}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]] maximal.

## Ejemplo 
Sea ${}X{}$ un conjunto y ${}a \in X{}$. Entonces ${}\mathcal{F}_{a}= \left\{B \subseteq X: a \in B \right\}{}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]].

> [!theorem|*]
> Sea ${}X{}$ un conjunto. Un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]] si y solo si ${}\forall B \subseteq X{}$ se tiene que ${}B \in \mathcal{F}{}$ o ${}X\setminus B \in \mathcal{F}{}$.

> [!corollary|*]
> Si ${}\mathcal{G}{}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]] en ${}X{}$ y ${}f: X \to Y{}$ es una función, entonces ${}f(\mathcal{G}){}$ es un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]] en ${}Y{}$.

> [!theorem|*] Todo [[Conceptos/Semestre 6/Filtro\|filtro]] está contenido en un ultrafilro
> Todo [[Conceptos/Semestre 6/Filtro\|filtro]] está contenido en un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]].

> [!theorem|*]
> Si ${}x{}$ es un punto de acumulación de un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]], entonces el [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]] converge a ${}x{}$.