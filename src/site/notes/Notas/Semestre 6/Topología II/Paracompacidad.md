---
{"dg-publish":true,"permalink":"/notas/semestre-6/topologia-ii/paracompacidad/"}
---

# Refinamientos y familias localmente fintas


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/refinamiento/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición 

> [!definition|*] Refinamiento
> Sean $\mathcal{U}$ y $\mathcal{V}$ cubiertas de $X$. Decimos que $\mathcal{V}$ **refina** a $\mathcal{U}$ (Notación: $\mathcal{V} \prec \mathcal{U}$) si para cada $V \in \mathcal{V}$ existe $U \in \mathcal{U}$ tal que $V\subseteq U$. En este caso diremos que $\mathcal{V}$ es un **refinamiento** de $\mathcal{U}$.

</div></div>


## Ejemplo
Sea $(X,d)$ un espacio métrico. Si $\mathcal{V}= \left\{B\left( x,\frac{1}{2} \right) \right\}_{x \in X}$ es un refinamiento de $\left\{B(x,1) \right\}_{x \in X}$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/familia-localmente-finita/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición 

> [!definition|*] Familia localmente finita
> Sea $(X,\tau)$ un [[Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${}\mathcal{U} \subseteq \mathcal{P}(X){}$. Diremos que ${}\mathcal{U}{}$ es **localmente finita** si ${}\forall x \in X{}$ existe ${}V \in \mathcal{N}(x){}$ tal que ${}\left\{U \in \mathcal{U}: U\cap V \neq \emptyset \right\}{}$ es finito.

</div></div>

## Ejemplo
Sea ${}(\mathbb{R},\tau){}$ y ${}\mathcal{U}= \left\{[n,n+1] \right\}_{n \in \mathbb{Z}}{}$ es localmente finita, pero ${}\mathcal{V}= \left\{[-n,n] \right\}_{n \in \mathbb{Z}}{}$ no lo es.

## Ejemplo
Si ${}X{}$ es discreto entonces ${}\left\{ \left\{x \right\} \right\}_{x \in X}{}$ es localmente finita, pero si ${}X{}$ es antidiscreto entonces ${}\left\{ \left\{x \right\} \right\}_{x \in X}{}$ es localmente finita si y sólo si ${}X{}$ es finito.

## Ejemplo
Si ${}\mathcal{U}{}$ es finita entonces ${}\mathcal{U}{}$ es localmente finita.

> [!lemma|*]
> Sea ${}\left\{U_{\alpha} \right\}_{\alpha \in \mathcal{A}}{}$ una [[Conceptos/Semestre 6/Familia localmente finita\|familia localmente finita]]. Entonces ${}\left\{ \overline{U_{\alpha}} \right\}_{\alpha \in \mathcal{A}}{}$ es localemente finita.

> [!lemma|*]
> Sea ${}\left\{B_{\alpha} \right\}_{\alpha \in \mathcal{A}}{}$ una [[Conceptos/Semestre 6/Familia localmente finita\|familia localmente finita]]. Entonces ${}\bigcup_{\alpha \in \mathcal{A}} \overline{B_{\alpha}}= \overline{\bigcup_{\alpha \in \mathcal{A}}B_{\alpha}}{}$.

# Espacios paracompactos


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/espacio-paracompacto/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Definición 

> [!definition|*] Espacio paracompacto
> Sea ${}(X,\tau){}$ un [[Conceptos/Semestre 6/Espacio topológico\|espacio topológico]]. Diremos que ${}X{}$ es **paracompacto** si ${}X{}$ es ${}T_{2}{}$ y para cada cubierta abierta ${}\mathcal{U}{}$ de ${}X{}$ existe ${}\mathcal{V}{}$ un refinamiento de ${}\mathcal{U}{}$ abierto y localmente compacto.

</div></div>


## Nota
Algunos autores <mark style="background: #FF5582A6;">NO</mark> piden que ${}X{}$ sea ${}T_{2}{}$.

## Ejemplo
Si ${}X{}$ es compacto y ${}T_{2}{}$ entonces ${}X{}$ es paracompacto.
*Desarrollo.* Sea ${}\mathcal{U}{}$ una cubierta abierta de ${}X{}$. Entonces existe ${}\mathcal{V}{}$ una subcubierta finita. Entonces ${}\mathcal{V}{}$ es un refinamiento localmente finito y abierto.

## Ejemplo 
Si ${}X{}$ es discreto entonces ${}X{}$ es paracompacto. Pues ${}X{}$ es ${}T_{2}{}$ y ${}\left\{ \left\{x \right\} \right\}_{x \in X}{}$ es un refinamiento abierto y localmente finito de cualquier cubierta de ${}X{}$.


<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/paracompacto-implica-regular/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Teorema 
 
> [!theorem|*] Paracompacto implica regular
> Si ${}X{}$ es paracompacto entonces ${}X{}$ es ${}T_{3}{}$.

</div></div>



<div class="transclusion internal-embed is-loaded"><a class="markdown-embed-link" href="/conceptos/semestre-6/paracompacto-implica-normal/" aria-label="Open link"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="svg-icon lucide-link"><path d="M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71"></path><path d="M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71"></path></svg></a><div class="markdown-embed">




#Enconstrucción
#Tema/Topología  #Tipo/Teorema 
 
> [!theorem|*] Paracompacto implica normal
> Si ${}X{}$ es paracompacto entonces ${}X{}$ es ${}T_{4}{}$.

</div></div>




 

 

 