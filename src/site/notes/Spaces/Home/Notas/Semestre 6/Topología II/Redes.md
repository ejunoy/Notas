---
{"dg-publish":true,"permalink":"/spaces/home/notas/semestre-6/topologia-ii/redes/"}
---

<mark style="background: #FF5582A6;">Pregunta:</mark> ¿Existe una noción que unifique los conceptos de
1. límite de una sucesión 
2. límite de una función 
3. integral (de Riemann- sumas de Riemann)?

> [!definition|*] [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]]
> 
> Sea ${} \mathcal{A} {}$ un conjunto y ${} \leq  {}$ una relación en ${} \mathcal{A} {}$. Decimos que ${} (\mathcal{A},\leq) {}$ es un **[[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]]** si la relación ${} \leq {}$ cumple:
> 1. ${} \lambda \leq \lambda, \forall \lambda \in \mathcal{A} {}$.
> 2. ${} \lambda_{1}\leq \lambda_{2} {}$ y ${} \lambda_{2}\leq \lambda_{3} {} \Rightarrow \lambda_{1}\leq \lambda_{3}$.
> 3. ${} \forall \lambda_{1}, \lambda_{2} \in \mathcal{A} {}$, ${} \exists \lambda_{3} \in \mathcal{A} {}$ tal que ${} \lambda_{1}\leq \lambda_{3} {}$ y ${} \lambda_{2}\leq \lambda_{3} {}$.
> En este caso diremos que ${} \leq {}$ es **una dirección**. 

**Observación.** No pedimos antisimetría.

### Ejemplos 
- ${} (\mathbb{R}, \leq), (\mathbb{N},\leq), (\mathbb{Z},\leq) {}$ donde ${} \leq {}$ es el orden usual.
- ${} (\mathcal{P}(X),\subseteq) {}$. En este caso ${} \forall A, B \in \mathcal{P}(X) {}$ se tiene que ${} A \subseteq A \cup B {}$ y ${} B \subseteq A \cup B {}$.

### Ejemplo 
Sea ${} (X,\tau) {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${} \mathcal{N}(x) {}$ la familia de vecindades para un punto ${} x \in X {}$. Para cada ${} U,V \in \mathcal{N}(x) {}$ definimos 
$${} \boxed{U\leq V \iff V \subseteq U} {}$$
Claramente ${} \leq {}$ cumple las condiciones 1 y 2 para ser una dirección. Para comprobar la condición ${} 3 {}$ notemos que:
Para cada ${} U, V \in \mathcal{N}(x) {}$ se tiene que ${} U \cap V \in \mathcal{N}(x) {}$ y ${} U \cap V \subseteq U, V {}$, de modo que ${} U \cap V \geq U, V {}$.

### Notación
Si ${} (\mathcal{A},\leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]], usaremos la notación:
1. ${} \lambda \geq \mu \iff \mu \leq \lambda {}$.
2. ${} \lambda < \mu \iff \lambda \leq \mu \text{ y } \mu \not \leq \lambda {}$ 
3. ${} \lambda>\mu \iff \lambda\geq \mu \text{ y } \mu \not \geq \lambda {}$.

> [!definition|*] [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]]
> 
> Una **red** en un conjunto ${} X {}$ es una función ${} p: \mathcal{A} \to X {}$ donde ${} (\mathcal{A},\leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]].
> Cuando no haya confusión usaremos la notación:
> - ${} p_{\lambda}=p(\lambda) {}$ para denotar el ${} \lambda- {}$ésimo término.
> - ${} (p_{\lambda})_{\lambda \in \mathcal{A}} {}$ para denotar la red.

### Ejemplo 
Si ${} a: \mathbb{N} \to X {}$ es una sucesión entonces es una red, pues ${} (\mathbb{N},\leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]].

### Ejemplo 
Sea ${} [a,b] {}$ un intervalo y ${} \mathcal{P} {}$ el conjunto de todas las particiones de ${} [a,b] {}$.
Dadas dos particiones ${} P {}$, ${} Q {}$ de ${} [a,b] {}$ diremod que ${} P \leq Q {}$ si ${} P \subseteq Q {}$, es decir, si ${} Q {}$ es un refinamiento de ${} P {}$.
De esta manera, ${} (\mathcal{P},\leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]].
Dada ${} f: [a,b] \to \mathbb{R} {}$, podemos considerar ${} U(f,P) {}$ y ${} L(f,P) {}$ la suma superior e inferior de ${} f {}$ con respecto a la partición ${} P {}$.
Entnoces ${} (U(f,P))_{P \in \mathcal{P}} {}$ y ${} (L(f,P))_{P \in \mathcal{P}} {}$ son [[Spaces/Home/Notas/Semestre 6/Topología II/2023-10-30#Redes\|redes]] en ${} \mathbb{R} {}$. También, si para cada ${} P \in \mathcal{P} {}$, ${} S(f,P) {}$ denota una suma de Riemann entonces ${} (S(f,P))_{P \in \mathcal{P}} {}$ es una red en ${} \mathbb{R} {}$.

# Convergencia de una red

> [!definition|*] Convergencia de una red
> 
> Sea ${} (X,\tau) {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${} (x_{\lambda})_{\lambda \in \mathcal{A}} {}$ una red en ${} X {}$. Diremos que ${} (x_{\lambda})_{\lambda \in \mathcal{A}} {}$ **[[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]]** al punto ${} x \in X {}$ si para cada ${} U \in \mathcal{N}(x) {}$ existe ${} \lambda_{0} \in \mathcal{A} {}$ tal que si ${} \lambda\geq \lambda_{0} {}$ entonces ${} x_{\lambda} \in U {}$.
> 

### Notación 
- ${} x_{\lambda} \to x {}$
- ${} (x_{\lambda})_{\lambda \in \mathcal{A}} \to x {}$
- ${} \lim_{ \lambda \to \infty } x_{\lambda}= x {}$
- ${} (x_{\lambda})_{\lambda \geq \lambda_{0}} {}$ se llama cola de la red.
- Si ${} x_{\lambda} \in U {}$ para cada ${} \lambda\geq \lambda_{0} {}$, se dice que la red ${} (x_{\lambda})_{\lambda \in \mathcal{A}} {}$ está residualmente en ${} U {}$ (o eventualemente en ${} U {}$). 

### Ejemplo 
Si  es una sucesión ${}a_{n}{}$ entonces  [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]] a ${}a{}$ como sucesión si y sólo si  [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]] a ${}a{}$ como red.

### Ejemplo
La integral inferior de ${} f {}$, denotada por ${} \underline{\int_{}^{}}f {}$ se define por: ${} \underline{\int_{}^{}}f = \sup \left\{L(f,P): P \in \mathcal{P} \right\} {}$. 
Entonces ${} (L(f,P))_{P \in \mathcal{P}} \to \underline{\int_{}^{}}f{}$.
Analogamente ${} (U(f,P))_{P \in \mathcal{P}} \to \overline{\int_{}^{}}f {}$.
Si ${} f {}$ es Riemann integrable entonces ${} (L(f,P)), (U(f,P)) {}$ y ${}(S(f,P)) {}$ [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|convergen]] (como [[Spaces/Home/Notas/Semestre 6/Topología II/2023-10-30#Redes\|redes]]) a ${} \int_{}^{} f {}$.

### Ejemplo 
Sea ${} (X,\tau) {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${} x \in X {}$. Consideremos ${} (N(x),\leq) {}$ con ${} U\leq V \iff V \subseteq U{}$.
Si para cada ${} U \in \mathcal{N}(x) {}$ escohemos ${} x_{u} \in U {}$, entonces ${} (x_{U})_{U \in \mathcal{N}(x)} {}$ [[Spaces/Home/Conceptos/Semestre 6/Convergencia de filtros\|converge]] a ${} x {}$.
*Demostración.* Sea ${} V \in \mathcal{N}(x) {}$. Si ${} U \geq V {}$ entoncse ${} U \subseteq V {}$ y ${} x_{U} \in V {}$.
Por lo tanto ${} (x_{U})_{U \in \mathcal{N}(x)}  \to x{}$.
$\blacksquare$ 

### Ejemplo 
Sea ${} x \in \mathbb{R}^{n} {}$. Diremos que ${} y\geq z {}$ con ${} y,z \in \mathbb{R}^{n}\setminus \left\{x \right\} {}$ si ${} \lvert\lvert y-x \rvert\rvert\leq \lvert\lvert z-x \rvert\rvert {}$.
**Observación.** ${} (\mathbb{R}^{n}\setminus \left\{x \right\},\leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]]. Además, ${} \leq {}$ no es antisimétrica.
**Observación.** Para cada ${} f: \mathbb{R}^{n}\setminus \left\{x \right\} \to \mathbb{R}^{k} {}$ define una red en ${} \mathbb{R}^{k} {}$: ${} (f(z))_{z \in \mathbb{R}^{n}\setminus \left\{x \right\}} {}$.
**Observación.** Dado ${} w \in \mathbb{R}^{k}{}$, ${} (f(z)) \to w {}$ si y sólo si para cada ${} U \in \mathcal{N}(w) {}$ existe ${} z_{0} \in \mathbb{R}^{n}\setminus \left\{x \right\}{}$ tal que si ${} y\geq z_{0} {}$ entonces ${} f(y) \in U {}$. Lo cual sucede si y sólo si para cada ${} U \in \mathcal{N}(w) {}$ existe ${} z_{0} \in \mathbb{R}^{n} \setminus \left\{ x \right\} {}$ tal que si ${} \lvert\lvert y-x \rvert\rvert \leq \lvert\lvert z_{0}-x \rvert\rvert {}$ entonces ${} f(y) \in U {}$. Y esto sucede si y sólo si para cada ${} \varepsilon >0 {}$ existe ${} \delta>0 {}$ tal que si ${} y \in \mathbb{R}^{n} \setminus \left\{x \right\} {} \land \lvert\lvert y-x \rvert\rvert< \delta$ entonces ${} \lvert\lvert f(y)- w \rvert\rvert< \varepsilon {}$.
Esto último sucede si y sólo si ${} \lim_{ y \to x } f(y)=w {}$ en el sentido de cálculo.

### Ejemplo 
Definimos en ${} \mathbb{N} {}$ la dirección dada por ${} m \preceq n \iff m\vert n {}$.
**Observación.** ${} (\mathbb{N},\preceq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]] ya que ${} \preceq {}$ es reflexiva, transitiva y ${} \forall n,m \in \mathbb{N} {}$, ${} n\preceq nm {}$ y ${} m \preceq nm {}$.
Sea ${} (a_{n})_{n \in \mathbb{N}} \subseteq \mathbb{R}{}$ dada por 
$${} a_{n}= \begin{cases}0 \text{ si } n=2m \\
1 \text{ si } n=2m+1. \end{cases}  {}$$
Entnoces ${} (a_{n})_{n \in \mathbb{N}} {}$ no converge como sucesión pero sí como red, pues si ${} 2 \preceq n {}$ entonces ${} n {}$ es par y ${} a_{n}=0 {}$. De modo que ${} a_{n} {} \to 0$.     

# Conjuntos cerrados y [[Spaces/Home/Notas/Semestre 6/Topología II/2023-10-30#Redes\|redes]]

> [!theorem|*]
> Sea ${} (X,\tau) {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${} E \subseteq X {}$. Entoces ${} x \in \overline{E} {}$ si y sólo si existe una red ${} (x_{\lambda})_{\lambda \in \mathcal{A}}\subseteq E {}$ que [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]] a ${} x {}$.
> 

*Demostración.* 
- ${} \rightarrow {}$ Sea ${} x \in \overline{E} {}$. Para cada ${} U \in \mathcal{N}(x){}$ existe ${} x_{U} \in E {}$ tal que ${} x_{U} \in U {}$. Considera el [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]] ${} (\mathcal{N}(x),\leq) {}$. Considera la red ${} (x_{U})_{U \in \mathcal{N}(x)} {}$. Veamos que ${} (x_{U})_{x_{U}\in \mathcal{N}(x)} {}$ [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]] a ${} x {}$. Sea ${} U \in \mathcal{N}(x) {}$. Si ${} V \geq U {}$ entonces ${} x_{V} \in V \subseteq U {}$. Por lo tanto ${} (x_{U})_{x_{U}\in \mathcal{N}(x)} {}$ está residualmente en ${} U {}$ y ${} (x_{U})_{x_{U}\in \mathcal{N}(x)} {}$ [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]] a ${} x {}$.
- ${} \leftarrow {}$ Suponamgos que existe una red ${} (x_{\lambda})_{\lambda\in \Lambda} {}$ contenida en ${} E {}$ que [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]] a ${} x {}$. Sea ${} U \in \mathcal{N}(x) {}$ entonces ${} (x_{\lambda})_{\lambda\in \Lambda} {}$ está residualmente en ${} U {}$, entonces existe ${} \lambda \in \Lambda {}$ con ${} x_{\lambda} \in U \cap E {}$ y, por lo tanto, ${} U \cap E \neq \emptyset {}$. Entonces ${} x \in \overline{E} {}$.
$\blacksquare$ 

> [!corollary|*]
> ${} E {}$ es cerrado si y sólo si para cada ${} (x_{\lambda})_{\lambda\in \Lambda} \subseteq E {}$ convergente se tiene que ${} \lim_{ \lambda \to \infty } x_{\lambda} \in E {}$.
> 

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} E {}$ es cerrado. Sea ${} (x_{\lambda})_{\lambda \in \Lambda}\subseteq E {}$ una red convergente. Entonces ${} \lim_{ \lambda \to \infty } x_{\lambda} {}$  es un punto de acumulación de ${} E {}$ y, como ${} E {}$ es cerrado, ${} \lim_{ \lambda \to \infty } x_{\lambda} \in E {}$.
- ${} \leftarrow {}$ Supongamos que toda red ${} (x_{\lambda})_{\lambda\in \Lambda} \subseteq E {}$ convergente [[Spaces/Home/Conceptos/Semestre 6/Convergencia de redes\|converge]] a un punto en ${} E {}$. Sea ${} x \in \overline{E} {}$. Entonces existe ${} (x_{\lambda})_{\lambda\in \Lambda}\subseteq E {}$ convergente tal que ${} x = \lim_{ \lambda \to \infty } x_{\lambda} {}$, así que ${} x \in E {}$. Por lo tanto ${} E {}$ es cerrado.
$\blacksquare$ 
