---
{"dg-publish":true,"permalink":"/spaces/home/notas/semestre-6/topologia-ii/puntos-de-acumulacion-y-subredes/"}
---

> [!definition|*] Punto de acumulación
> 
> Sean ${} X {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${} (x_{\lambda})_{\lambda\in \Lambda}\subseteq X {}$ una red. Diremos que ${} x \in X {}$ es un **punto de acumulación** de la red (o que **la red se acumula** en ${} x {}$ ) si para cada ${} U  \in \mathcal{N}(x){}$ y para cada ${} \lambda_{0} \in \Lambda {}$ existe ${} \lambda\geq \lambda_{0} {}$ tal que ${} x_{\lambda} \in U {}$ ( la red está cofinalmente en cada vecindad de ${} x {}$).
> 

### Ejemplo 
Si ${} \lim_{ \lambda \to \infty } x_{\lambda}= x {}$ entonces ${} x {}$ es un punto de acumulación de la red.

### Ejemplo 
Sea ${} (\mathbb{N}),\preceq {}$ donde ${} n \preceq m  \iff n\vert m{}$. Definimos la red ${} (a_{n})_{n\in \mathbb{N}} {}$ como 
$${} a_{n}= \begin{cases} 0 \text{ si } n=2m \\
1 \text{ si  } n=2m+1. \end{cases}  {}$$
Entonces ${} 1 {}$ no es un punto de acumulación de la red, ya que si tomamos ${} U=\left( \frac{1}{2},\frac{3}{2} \right) {}$ y ${} n_{0}=2 {}$ entonces no existe ${} m\geq n_{0} {}$ tal que ${} a_{m} \in U {}$.
Sin embargo, si consideramos el orden unusal en ${} \mathbb{N} {}$ entonces tanto 0 como 1 son puntos de acumulación de la red (sucesión).

> [!definition|*] función creciente y cofinal
> 
> Sean ${} (\mathcal{M}, \preceq) {}$ y ${}(\mathcal{A},\leq) {}$ conjutnos dirigidos y sea ${} q: \mathcal{M} \to \mathcal{A} {}$ una función. Diremos que 
> 1. ${} q {}$ es **creciente** si cuando ${} \mu_{1} \preceq \mu_{2} {}$ se tiene también que ${} q(\mu_{1})\leq q(\mu_{2}) {}$.
> 2. ${} q {}$ es **cofinal** si para cada ${} \lambda \in \mathcal{A} {}$ existe ${} \mu \in \mathcal{M} {}$ tal que ${} \lambda \leq q(\mu) {}$.

> [!definition|*] Subred
> 
> Sea ${} p: \mathcal{A} \to X{}$ una red en ${} X {}$. Una **subred** es la composición ${} p \circ q: \mathcal{M} \to X {}$, donde ${} (\mathcal{M}, \leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]] y ${} q: \mathcal{M} \to \mathcal{A} {}$ es una función creciente y cofinal.
> 

### Notación 
Si ${} (p_{\lambda})_{\lambda \in \mathcal{A}} {}$ es la red original entonces ${} (p_{\lambda_\mu})_{\mu \in \mathcal{M}} {}$ o ${} (p_{q(\mu)})_{\mu \in \mathcal{M}} {}$ son notaciones válidas para una subred.

### Ejemplo 
Si ${} (a_{n}) {}$ es una sucesión y ${} (a_{k(n)}) {}$  es una subsucesión, entonces ${} (a_{k(n)}) {}$ es una subred, pues ${} k: \mathbb{N} \to \mathbb{N} {}$ es estrictamente creciente y para cada ${} n \in \mathbb{N} {}$ se tiene que ${} k(n)\geq n {}$.   

> [!exercise|*]
> Si ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$ entonces toda subred ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{M}} {}$ converge a ${} x {}$.
> 

*Demostración.* Supongamos que ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$. Sea ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{M}} {}$ una subred de ${} (x_{\lambda})_{\lambda\in \Lambda} {}$.
Como ${} (x_{\lambda})_{\lambda\in \Lambda} {}$ converge a ${} x {}$ entonces para cada ${} U \in \mathcal{N}(x) {}$ existe ${} \lambda_{0} {}$ tal que si ${} \lambda\geq \lambda_{0} {}$ entonces ${} x_{\lambda} \in U {}$.  Como ${} \lambda_{\mu} {}$ es creciente y cofinal, existe ${} \mu_{0} \in \mathcal{M} {}$ tal que si ${} \mu\geq \mu_{0} {}$ entonces ${} \lambda_{\mu}\geq \lambda_{0} {}$ y, por lo tanto ${} x_{\lambda_{\mu}} \in U {}$. Entonces ${} (x_{\lambda_{\mu}})_{\mu\in \mathcal{M}} {}$ converge a ${} x {}$. 
$\blacksquare$ 

> [!theorem|*]
> Sea ${} (X,\tau) {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${} (x_{\lambda})_{\lambda \in \mathcal{A}} \subseteq X {}$ una red. Entonces ${} x {}$ es un punto de acumulación de la red si y sólo si existe una subred que converge a ${} x {}$.
> 

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} x {}$ es un punto de acumulación de la red ${} (x_{\lambda})_{\lambda\in \Lambda} {}$. Entonces para cada ${} U \in \mathcal{N}(x) {}$ y para cada ${} \lambda_{0} \in \Lambda {}$ existe ${} \lambda\geq \lambda_{0} {}$ tal que ${} x_{\lambda} \in U {}$. Considera el conjunto ${} \mathcal{A} = \left\{ (\lambda, U) \in \Lambda \times \mathcal{N}(x) \vert x_{\lambda} \in U \right\} {}$. Digamos que ${} (\lambda,U)\leq (\mu,V) {}$ si y sólo si ${} \lambda \leq \mu {}$ y ${} V \subseteq U {}$. Veamos que ${} (\mathcal{A}, \leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]]. 
	1. Sea ${} (\lambda,U) \in \mathcal{A} {}$. Como ${} \lambda\leq \lambda {}$ y ${} U \subseteq U {}$ entonces ${} (\lambda, U)\leq (\lambda,U) {}$.
	2. Sean ${} (\lambda,U),(\mu,V),(\sigma,W) \in \mathcal{A}{}$ tales que ${} (\lambda,U)\leq (\mu, V) {}$ y ${} (\mu,V)\leq (\sigma, W) {}$. Entonces ${} \lambda\leq \mu \leq \sigma {}$ y ${} W \subseteq V \subseteq U {}$, de modo que ${} \lambda \leq \sigma {}$ y ${} W \subseteq U {}$, entonces ${} (\lambda,U)\leq (\sigma,W) {}$.
	3. Si ${} (\lambda, U) {}$ y ${} (\mu, V) {} \in \mathcal{A}$ entonces existe ${} \sigma \geq \lambda, \mu {}$. Entonces ${} (\sigma, U \cap V) {}$ es tal que ${} (\sigma,U \cap V)\geq (\lambda,U) {}$ y ${} (\sigma, U \cap V) \geq (\mu,V){}$.
	Entonces ${} (\mathcal{A},\leq) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]].
	Considera la función ${} q: \mathcal{A} \to \Lambda {}$ dada por ${} q(\lambda,U)= \lambda {}$. Entonces ${} q {}$ es creciente y, como para cada ${} \lambda_{0} {}$ y ${} U \in \mathcal{N}(x) {}$ existe ${} \lambda\geq \lambda_{0} {}$ tal que ${} x_{\lambda} \in U {}$, se tiene que existe ${} q(\lambda,U)\geq \lambda_{0} {}$, así que ${} q {}$ es cofinal.
	Considera la subred ${} (x_{q(\lambda,U)})_{(\lambda,U) \in \mathcal{A}} {}$. Sea ${} U \in \mathcal{N}(x) {}$. Entonces para ${} \mu_{0} \in \Lambda  {}$ existe ${} \lambda \in \Lambda {}$ tal que ${} x_{\lambda} \in U {}$. Si ${} (\mu, V)\geq (\lambda,U) {}$ entonces ${} \mu \geq \lambda {}$ y ${} V \subseteq U {}$, entonces ${} x_{\mu} \in V \subseteq U {}$, de modo que ${} x_{(\mu,V)} \in U {}$ y ${} (x_{(\lambda,U)})_{(\lambda,U) \in \mathcal{A}} {}$ es una subred que converge a ${} x {}$.
- ${} \leftarrow {}$ Supongamos que existe una subred ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$ de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ que converge a ${} x {}$. Sea ${} U \in \mathcal{N}(x) {}$. Sea ${} \lambda_{0}  \in \Lambda{}$. Como ${} \lambda_{\mu} {}$ es creciente y cofinal, existe ${} \mu_{0} {}$ tal que si ${} \mu\geq \mu_{0} {}$ entonces ${} \lambda_{\mu}> \lambda_{0}{}$. También, como ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$ converge a ${} x {}$ entonces existe ${} \mu_{1} {}$ tal que si ${} \mu\geq \mu_{1} {}$ entonces ${} x_{\mu_{1}} \in U {}$. Sea ${} \mu_{2} {}$ con ${} \mu_{0}\leq\mu_{2} {}$ y ${} \mu_{1}\leq \mu_{2} {}$. Entonces ${} x_{\lambda_{\mu_{2}}} \in U {}$ y ${} \lambda_{\mu_{2}}\geq \lambda_{0} {}$.
	Por lo tanto ${} x {}$ es un punto de acumulación de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
$\blacksquare$   
