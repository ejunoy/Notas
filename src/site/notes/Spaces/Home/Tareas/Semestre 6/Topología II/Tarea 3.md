---
{"dg-publish":true,"permalink":"/spaces/home/tareas/semestre-6/topologia-ii/tarea-3/"}
---

# Parte 1

> [!exercise|1]
> Demuestra que un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] ${} X {}$ es Hausdorff si y sólo si toda red convergente tiene un único límite.
> 

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} X {}$ es Hausdorff. Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red convergente. Supongamos que ${} x {}$ y ${} y {}$ son límites distintos de la red. Como ${} x \neq y  {}$ y ${} X {}$ es Hausdorff entonces existen ${} U \in \mathcal{N}(x) {}$ y ${} V \in \mathcal{N}(y) {}$ tales que ${} U \cap V = \emptyset {}$. Como la red converge a ${} x {}$ y ${} y {}$ entonces se queda residualmente en ${} U {}$ y en ${} V {}$, lo cual es imposible pues ${} U {}$ y ${} V {}$ son ajenos.
- ${}\leftarrow {}$ Supongamos que toda red tiene límite único. Supongamos que ${} X {}$ no es Hausdorff. Entonces existen ${} x,y \in X {}$ tales que para cada ${} U,V \subseteq X {}$ abiertos con ${} x \in U {}$ y ${} y \in V {}$ se tiene que ${} U \cap V \neq \emptyset {}$. En el conjunto ${} \mathcal{N}(x) \times \mathcal{N}(y) {}$ definimos ${} (U,V)\leq (Z,W) {}$ si y sólo si ${} Z \subseteq U {}$ y ${} W \subseteq V {}$. Para cada ${} (U,V) \in \mathcal{N}(x)\times \mathcal{N}(y) {}$ sea ${} q((U,V))= x_{(U,V)} {}$ donde ${} x_{(U,V)} {}$ es un punto en ${} U \cap V {}$. Veamos que ${} q {}$ converge a ${} x {}$. Sea ${} U \in \mathcal{N}(x) {}$ y ${} V \in \mathcal{N}(x) {}$. Si ${} (Z,W)\geq (U,V) {}$ entonces ${} Z \subseteq U {}$, entonces ${} q((Z,W)) \in Z \subseteq U{}$. Así que ${} q {}$ está residualmente en ${} U {}$. Así que ${} q {}$ converge a ${} x {}$. Similarmente, si ${} (Z,W)\geq (U,V) {}$ entonces ${} W \subseteq V {}$ y ${} q((Z,W)) \in W \subseteq V {}$. Entonces ${} q {}$ está residualmente en ${} V {}$ y ${} q {}$ converge a ${} y {}$. Esto contradice que toda red tenga límite único. 
	Entonces ${} X {}$ es Hausdorff 
$\blacksquare$

> [!exercise|2]
> Sea ${} X {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] y ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red en ${} X {}$. Demuestra los siguientes enunciados:
> 1. Si ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$, entonces cualquier subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ también converge a ${} x {}$.
> 2. Si ${} x_{\lambda} = x {}$ para todo ${} \lambda \in \Lambda {}$, entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$.
> 3. Una subred de una subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ es una subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
> 4. Si ${} y {}$ es un punto de acumulación de una subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$, entonces también es un punto de acumulación de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
> 5. Si toda subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$tiene una subred que converge a ${} x {}$, entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$.

*Demostración.* 
1. Supongamos que ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$. Sea ${} q: \mathcal{A} \to \Lambda {}$ una función creciente y cofinal y consideremos la subred ${} (x_{q(\lambda)})_{\lambda \in \mathcal{A}} {}$.
	Sea ${} U \in \mathcal{N}(x) {}$. Como ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$ entonces existe ${} \mu \in \lambda {}$ tal que si ${} \lambda \geq \mu {}$ entonces ${} x_{\lambda} \in U {}$. Como ${} q {}$ es cofinal, existe ${} \lambda_{0} \in \mathcal{A} {}$ tal que ${} q(\lambda_{0})\geq \mu {}$. Si ${} \lambda \geq \lambda_{0} {}$ entonces ${} q(\lambda)\geq \mu {}$ y ${} x_{q(\lambda)} \in U {}$. Entonces ${} (x_{q(\lambda)})_{\lambda \in \mathcal{A}} {}$ está residualmente en ${} U {}$, así que converge a ${} x {}$.

2. Sea ${} U \in \mathcal{N}(x) {}$. Entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ está residualmente en ${} U {}$ y ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$.
3. La composición de funciones crecientes es creciente y la composición de funciones cofinales es cofinal.
4. Supongamos que ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$ es una subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ y que ${} x {}$ es un punto de acumulación de la subred. Sea ${} U \in \mathcal{N}(x) {}$.
	Sea ${} \lambda_{0} \in \Lambda {}$. Como ${} \lambda_{\mu}: \mathcal{A} \to \Lambda {}$ es cofinal entonces existe ${} \mu_{0} \in \mathcal{A} {}$ tal que ${} \lambda_{\mu_{0}}\geq \lambda_{0} {}$. Como ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$ se acumula en ${} x {}$ entonces existe ${} \mu\geq \mu_{0} {}$ tal que ${} x_{\lambda_{\mu}} \in U {}$. Pero ${} \lambda_{\mu} \geq \lambda_{\mu_{0}} {}$ entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ se acumula en ${} x {}$.
5. Supongamos que toda subred tiene una subred que converge a ${} x {}$. Por contradicción supongamos que ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ no converge a ${} x {}$. Entonces existe ${} U \in \mathcal{N}(x) {}$ tal que para cada ${} \lambda_{0} \in \Lambda {}$ existe ${} \lambda \geq \lambda_{0} {}$ tal que ${} x_{\lambda} \not \in U {}$. Sea ${} \mathcal{B} = \left\{ \lambda: x_{\lambda} \not \in U \right\} {}$. ${} \mathcal{B} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]]. Considera ${} i: \mathcal{B} \hookrightarrow \Lambda{}$. Nota que ${} i {}$ es creciente y también es cofinal, entonces ${} (x_{i(k)})_{k \in \mathcal{B}} {}$ es una subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$. Además, ${} (x_{i(k)})_{k \in \mathcal{B}} {}$ no puede tener ninguna subred convergente a ${} x{}$ pues ${} (x_{i(k)})_{k \in \mathcal{B}} {}$ está eventualmente afuera de ${} U \in \mathcal{N}(x) {}$.
$\blacksquare$

> [!exercise|3]
> Sea ${} X = \prod_{\alpha \in \mathcal{A}}^{}X_{\alpha} {}$ un producto de espacios topológicos (equipado con la topología de Tychonoff) y sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red en ${} X {}$. Denotemos por ${} \pi_{\alpha}:X \to X_{\alpha} {}$ la proyección en el factor ${} X_{\alpha} {}$. Demuestra que ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x \in X {}$ si y śolo si para todo ${} \alpha \in \mathcal{A} {}$, la red ${} (\pi_{\alpha}(x_{\lambda}))_{\lambda \in \Lambda} {}$ converge a ${} \pi_{\alpha}(x) {}$.
> 

*Demostración.* 
- ${} \Rrightarrow {}$ Supongamos que ${} (x_{\lambda})_{\lambda \in \Lambda} \subseteq \prod_{\alpha \in \mathcal{A}}^{} X_{\alpha} {}$ converge a ${} x {}$. Como ${} \pi_{\alpha} {}$ es continua para cada ${} \alpha \in \mathcal{A} {}$ entonces por un teorema visto en clase se tiene que ${} (\pi_{\alpha}(x_{\lambda}))_{\lambda \in \Lambda} {}$ converge a ${} \pi_{\alpha}(x) {}$.
- ${} \Lleftarrow {}$ Supongamos que ${} (\pi_{\alpha}(x))_{\alpha \in \Lambda} {}$ converge a ${} \pi_{\alpha}(x) {}$ para cada ${} \alpha \in \mathcal{A} {}$. Sea 
	$${} U= \left(\prod_{i=1}^{n} \pi _{\alpha _{i} }^{-1} (U_{\alpha _{i} } )\right) \times \prod_{\alpha  \neq \alpha _{i} }^{} X_{\alpha _{i} }.    {}$$
	Un conjunto básico tal que ${} x \in U {}$. Como ${} (\pi_{\alpha}(x_{\lambda}))_{\lambda} {}$ converge a ${} \pi_{\alpha}(x) {}$ para cada ${} \alpha \in \mathcal{A} {}$ entonces existen ${} \lambda_{1},\dots,\lambda_{n} {}$ tales que si ${} \lambda \geq \lambda_{i} {}$ entonces ${} \pi_{\alpha_{i}}(x_{\lambda}) \in \pi_{\alpha_{i}}^{-1}(U_{\alpha_{i}}){}$. Sea ${} \lambda_{0} {}$ tal que ${} \lambda_{0}\geq \lambda_{1},\dots,\lambda_{n} {}$. Si ${} \lambda\geq \lambda_{0} {}$ entonces ${} \pi_{\alpha_{i}}(x_{\lambda}) \in \pi_{\alpha_{i}}^{-1}(U_{\alpha_{i}}){}$ para cada ${} i \in \left\{1,\dots,n \right\} {}$. Por lo tanto
	$${} (((\pi_{\alpha})(x_{\lambda}))_{\alpha \in \mathcal{A}})_{\lambda  \in  \Lambda } \in  U   {}$$
	Y ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ está residualmente en ${} U {}$. Entnoces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge a ${} x {}$.
$\blacksquare$

> [!exercise|4]
> Sea ${} \mathbb{R}^{\mathbb{R}} {}$ equipado con la topología producto. Considera el conjunto ${} Z \subset R^{\mathbb{R}} {}$ dado por
> $${} Z= \left\{ f \in  \mathbb{R}^{\mathbb{R} } \vert   f(x)  \in  \left\{0,1 \right\} \text{ para todo } x \in  \mathbb{R} \land  f(x) =0 \text{ solo para una cantidad finita de } x \in  \mathbb{R}    \right\}.  {}$$
> Sea ${} \phi: \mathbb{R} \to \mathbb{R} {}$ la función constante cero.
> 1. Demuestra que ${} \phi \in \overline{Z} {}$.
> 2. Encunetra una red ${} (f_{\lambda})_{\lambda \in \Lambda} \subset Z {}$ que converja a ${} \phi {}$.

*Demostración.* 
1. Sean $U_{x_{1}},\dots U_{x_{n}}$ conjuntos abiertos en ${} \mathbb{R} {}$ tales que ${} 0 \in U_{x_{1}},\dots, U_{x_{n}} {}$. Considera el conjunto
	$$U={} \prod_{i=1}^{n} U_{x_{i} } \times \prod_{x \neq x_{n}  }^{}\mathbb{R}   {}$$
	Entonces ${} (f(x))_{x \in \mathbb{R}} {}$ con ${} f(x)= 0 {}$ si ${} x= x_{i} {}$ y ${} f(x)=1 {}$ en otro caso, es tal que ${} f \in Z \cap U {}$. Entonces ${} \phi \in \overline{Z} {}$.
2. Considera ${} \mathcal{A}= \left\{ F \subseteq \mathbb{R}\vert F \text{ es finito } \right\} {}$ con la dirección determinada por ${} \subseteq {}$. Considera ${} f_{F}= \mathbb{1}_{\mathbb{R}\setminus F} {}$. Sea
	$$U={} \prod_{i=1}^{n} U_{x_{i} } \times \prod_{x \neq x_{n}  }^{}\mathbb{R}   {}$$
	Considera ${} F= \left\{x_{1},\dots,x_{n} \right\} {}$. Si ${} G \geq F {}$ entonces ${} f_{F} \in U {}$. Entonces ${} (f_{F})_{F \in \mathcal{A}} {}$ converge a ${} \phi {}$.
$\blacksquare$

> [!exercise|5]
> Considera el espacio de los ordinales ${} \Omega {}$ y denotemos por ${} \omega_{0}=\omega\setminus \left\{\omega_{1} \right\} {}$. Sea ${} M {}$ un espacio métrico y ${} p: \Omega_{0} \to M {}$ una función. Como ${} \Omega_{0} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Conjunto dirigido\|Conjunto dirigido]], la función ${} p {}$ determina una red ${} (p(\alpha))_{\alpha \in \Omega_{0}} {}$ en ${} M {}$. Demuestra que dicha red converge a un punto ${} x {}$ en ${} M {}$ si y sólo si existe un ordinal ${} \alpha_{0} \in \Omega_{0} {}$, tal que ${} p(\alpha)=x {}$ para todo ${} \alpha\geq \alpha_{0} {}$.
> 

*Demostración.* 
- ${} \rightarrow {}$Supongamos que ${} (p(\alpha))_{\alpha \in \Omega_{0}} {}$ converge a un punto ${} x \in M {}$. Como ${} M {}$ es un espacio métrico entonces es primero numerable. Sea ${} B= \left\{B\left( x,\frac{1}{n}:=B_{n} \right) \right\}_{ n \in \mathbb{N}} {}$ una base para ${} M {}$ en ${} x {}$. Sea ${} n \in \mathbb{N} {}$ . Como ${} (p(\alpha))_{\alpha \in \Omega_{0}} {}$  converge a entonces está residualmente en ${} B_{n} {}$. Entonces para cada ${} n \in \mathbb{N} {}$ existe ${} \alpha_{n} \in \mathbb{N} {}$ tal que si ${} \alpha \geq \alpha_{n} {}$ entonces ${} p(\alpha) \in B_{n}  {}$. Considera el conjunto ${} A=\left\{\alpha_{n} \right\}_{n \in \mathbb{N}} {}$. Nota que ${} A {}$ está acotado superiormente por ${} \omega_{1} {}$. Como ${} \Omega {}$ es un conjunto bien ordeado entonces ${} \sup A {}$ existe. Sea ${} \alpha_{0}=\sup A {}$. Si ${} \alpha\geq \alpha_{0} {}$ entonces ${} p(\alpha) \in B_{n} {}$ para cada ${} n \in \mathbb{N} {}$ de modo que ${} d(p(\alpha),x)<\frac{1}{n} {}$ para cada ${} n \in \mathbb{N} {}$ y ${} d(p(\alpha),x)=0 {}$. Así, ${} p(\alpha)= x {}$. 
	Nota que ${} \alpha<\omega_{1} {}$ pues si ${} \alpha= \omega_{1} {}$ entonces ${} \omega_{1} = \bigcup_{n \in \mathbb{N}} \alpha_{n} {}$ y, como cada ${} \alpha_{n} {}$ es numerable entonces ${} \omega_{1} {}$ sería numerable, lo cual es imposible. 
	Entonces ${} \alpha_{0} \in \Omega_{0} {}$ es tal que si ${} \alpha\geq \alpha_{0} {}$ entoces ${} p(\alpha)=x {}$.
$\blacksquare$

> [!exercise|6]
> Una red  ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ en un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] ${} X {}$ es una **ultrared** o **red universal** si para cada subconjunto ${} E\subseteq X {}$, la red se encuentra residualmente en ${} E {}$ on ${} X\setminus E {}$.
> 1. Demuestra que toda red constante es una ultrared.
> 2. Si ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ es una ultrared en ${} X {}$ y ${} f: X \to Y {}$ es una función, demuestra que ${} (f(x_{\lambda}))_{\lambda \in \Lambda} {}$ es una ultrared en ${} Y {}$.
> 3. Demuestra que toda subred de una ultrared es una ultrared.
> 4. Demuestra que toda red tiene una subred que es una ultrared.

*Demostración.* 
1. Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red con ${} x_{\lambda}= x {}$ para cada ${} \lambda \in \Lambda {}$. Sea ${} E \subseteq X {}$. Si ${} x \in E {}$ entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ está residualmente en ${} E {}$. Si ${} x \not \in E {}$ entonces ${} x {}$ está residualmente en ${} X\setminus E {}$.
2. Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una ultrared en ${} X {}$ . Sea ${} f: X \to Y{}$ una función. Sea ${} E \subseteq Y {}$. Si ${} f ^{-1}(E) = \emptyset {}$ entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ está residualmente en ${} X\setminus f^{-1}(E)= f^{-1}(Y\setminus E) {}$. De modo que ${} (f(x_{\lambda}))_{\lambda \in \Lambda} {}$ está residualmente en ${} Y\setminus E {}$. 
	Supongamos que ${} f^{-1}(E) \neq \emptyset {}$. Como ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ es una ultrared en ${} X {}$ entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ se encuentra resiudalmente en ${} f^{-1}(E) {}$ o en ${} f^{-1}(Y\setminus E) {}$. Entonces ${} (f(x_{\lambda}))_{\lambda \in \Lambda} {}$ está resdiualemente en ${} E {}$ o en ${} Y\setminus E {}$.
3. Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una ultrared. Sea ${} q: \mathcal{A} \to \Lambda {}$ una función creciente y cofinal. Sea ${} E \subseteq X {}$ arbitrario. Como ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ es una ultrared entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ está resiudualemente en ${} E {}$ o en ${} X\setminus E {}$. De modo que ${} (x_{q(\mu)})_{\mu \in \mathcal{A}} {}$ está residualmente en ${} E {}$ o en ${} X\setminus E {}$. Por lo tanto ${} (x_{q(\mu)})_{\mu \in \mathcal{A}} {}$ es una ultrared.
4. Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red. Considera el [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${} \mathcal{F}= \left\{ T_{\lambda} \vert \lambda \in \Lambda \right\} {}$. Entonces existe un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] ${} \mathcal{G} {}$ tal que ${} \mathcal{F} \subseteq \mathcal{G} {}$. Considera ${} (q((x,G)))_{(x,G) \in \mathcal{A}_{\mathcal{G}}} {}$ la red generada por[[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]]ltro ${} \mathcal{G} {}$. Entonces la red generada por ${} \mathcal{G} {}$ es una subred de la red generada por ${} \mathcal{F} {}$, pero la red generada por ${} \mathcal{F} {}$ es ${} (x_{\lambda})_{\lambda \in \Lambda} {}$, además, como ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]], la red generada por ${} \mathcal{G} {}$ es una ultrared. Entonces la red generada por ${} \mathcal{G} {}$ es una subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ que es una ultrared.
$\blacksquare$

> [!exercise|7]
> Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ una red en un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]] ${} X {}$. Para cada ${} \lambda_{0}  \in \Lambda{}$, definamos el conjunto ${} T_{\lambda_{0}}= \left\{x_{\lambda}: \lambda\geq \lambda_{0} \right\} {}$. Demuestre que un un punto ${} y {}$ es punto de acumulación de la red ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ si y sólo si ${} y \in \overline{T_{\lambda_{0}} } {}$ para todo ${} \lambda_{0} \in \Lambda{}$.

*Demostración.* 
- ${} \rightarrow {}$ Supongamso que ${} y {}$ es un punto de acumulación de la red ${} (x_{\lambda})_{\lambda \in \Lambda} {}$. Sea ${} U \in \mathcal{N}(y) {}$.  Como ${} y {}$ es punto de acumulación entonces para cada ${} \lambda_{0} \in \Lambda {}$ existe ${} \lambda\geq \lambda_{0} {}$ tal que ${} x_{\lambda} \in U {}$. Así, para cada ${} \lambda_{0} \in \Lambda {}$  se tiene que ${} U \cap T_{\lambda_{0}} \neq \emptyset {}$. Entonces para cada ${} \lambda_{0} \in \Lambda {}$ se tinen que ${} y \in \overline{T_{\lambda_{0}}} {}$.
- ${} \leftarrow {}$ Supongamos que ${} y {}$ es tal que para cada ${} \lambda_{0} \in \Lambda{}$ se tiene que ${} y \in \overline{T_{\lambda_{0}}} {}$. Sea ${} U \in \mathcal{N}(y) {}$ y sea ${} \lambda_{0} \in \Lambda{}$. Como ${} y \in \overline{T_{\lambda_{0}}} {}$ entonces ${} U \cap T_{\lambda_{0}} \neq \emptyset {}$. Por lo tanto, existe ${} \lambda\geq \lambda_{0} {}$ tal que ${} x_{\lambda}\in U {}$. Por lo tanto ${} y {}$ es un punto de acumulación de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
$\blacksquare$ 

> [!exercise|8]
> ¿Es posible encontrar un espacio ${} X {}$ y una sucesión ${} (x_{n})_{n \in \mathbb{N}} \subset X{}$, la cual tiene una subred que no sea una sucesión?
> 

*Demostración.* Considera la sucesión ${} (x_{n})_{n \in \mathbb{N}} {}$ dada por ${} x_{n}=(-1)^{n} {}$. Considera ${} \mathcal{N} {}$ con la dirección defininida por la relación de divisibilidad. Nota que ${} p: (\mathbb{N},\vert) \to \mathbb{R} {}$ es una subred de ${} (x_{n})_{n \in \mathbb{N}} {}$. Si ${} p {}$ fuera una sucesión entonces el complemento de cada cola debería ser finito. Considera la cola ${} T_{2}= \left\{x_{2n}: n \in \mathbb{N} \right\} {}$. Observa que para cada ${} k \in \mathbb{N} {}$ se tiene que ${} x_{3^{k}} \not \in T_{} {}$. Entonces hay una cantidad infinita de elementos que no están en la cola ${} T_{2} {}$. Así que ${} p {}$ no es una sucesión.
$\blacksquare$ 

# Parte 2

> [!exercise|1]
> Sea ${} \mathcal{F} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] en un conjunto ${} X {}$. Demuestra que ${} \bigcap_{i=1}^{n} F_{i} \in \mathcal{F} {}$ para cualquier subcolección finita ${} \left\{F_{1},\dots F_{n} \right\} \subseteq \mathcal{F} {}$.    
{ #2c5595}


*Demostración.* Como la intersección de dos elementos de ${} \mathcal{F} {}$ sigue siendo un elemento de ${} \mathcal{F} {}$ entonces por inducción la intersección de una cantidad finita de elementos de ${} \mathcal{F} {}$ sigue siendo un elemento de ${} \mathcal{F} {}$.
$\blacksquare$ 

> [!exercise|2]
> Sea ${} (X,\tau) {}$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]].
> 1. Si ${} X {}$ es Hausdorff y ${} \mathcal{F} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] que converge a un punto ${} x {}$, demuestra que ${} x {}$ es único.
> 2. Si cada [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] en ${} X {}$ converge a lo más a un punto en ${} X {}$, demuestra que ${} X {}$ es Hausdorff.

*Demostración.* 
1. Supongamos que ${} X {}$ es Hausdorff y sea ${} \mathcal{F} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] que converge a un punto ${} x {}$. Por contradicción supongamos que existe ${} y \in X {}$ con ${} x \neq y {}$ tal que ${} \mathcal{F} {}$ converge a ${} x {}$.
	Como ${} X {}$ es Hausdorff, existen ${} U \in \mathcal{N}(x) {}$ y ${} V \in \mathcal{N}(y) {}$ tales que ${} U \cap V = \emptyset{}$. Como ${} \mathcal{F} {}$ converge a ${} x {}$ y a ${} y {}$ entonces ${} \mathcal{N}(x),\mathcal{N}(y) \subseteq \mathcal{F} {}$. Luego, como los filtros son cerrados bajo intersecciones se tiene que ${} \emptyset= U \cap V \in \mathcal{F}{}$, lo cual es imposible. 
	Entonces ${} \mathcal{F} {}$ converge a un único punto.
2. Supongamos que todo [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] converge a lo más a un punto en ${} X {}$. Por contradicción supongamos que ${} X {}$ no es Hausdorff. Entonces existen ${} x,y \in X {}$ con ${} x \neq y {}$ tales que para cada ${} U \in \mathcal{N}(x) {}$ y ${} V \in \mathcal{N}(y) {}$ se tiene que ${} U \cap V \neq \emptyset {}$. Considera
	$${} \mathcal{B} = \left\{U \cap  V: U \in  \mathcal{N} (x) , V \in  \mathcal{N} (y)   \right\}.   {}$$
	Observa que ${} \mathcal{B} {}$ es cerrado bajo intersecciones. Entonces es [[Spaces/Home/Conceptos/Semestre 6/Base de filtro\|base]] para un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${} \mathcal{F} {}$. Nota que ${} \mathcal{N}(x),\mathcal{N}(y)\subseteq \mathcal{B} \subseteq \mathcal{F} {}$, entonces ${} \mathcal{F} {}$ converge a ${} x {}$ y a ${} y {}$, lo cual es imposible. Entonces ${} X {}$ es Hausdorff.    
$\blacksquare$ 

> [!exercise|3]
> Sea ${} X {}$ un conjunto.
> 1. Si ${} X {}$ tiene la topología discreta ¿cómo son los filtros que convergen a un punto ${} x \in X {}$?
> 2. Si ${} X {}$ tiene la topología antidiscreta ¿cómo son los filtros que convergen a un punto ${} x \in X {}$.

*Desarrollo.*
1. Supongamos que ${} X {}$ tiene la topología discreta. Nota que si ${} U {}$ es tal que ${} x \not \in U {}$ entonces se tendría que ${} \left\{x \right\} \cap U = \emptyset {}$, de modo que ${} U \not \in \mathcal{F} {}$ para cada ${} U {}$ con ${} x \not \in U {}$. Entonces se debe tener que ${} \mathcal{F}= \mathcal{N}(x) {}$.
2. Supongamos que ${} X {}$ tiene la topología antidiscreta. Sea ${} \mathcal{F} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] que converge a ${} X {}$. Tenemos que ${} \mathcal{N}(x)= \left\{X \right\} {}$. Entonces ${} X \in \mathcal{F} {}$. De hecho, ${} \mathcal{N}(y)= \left\{X\right\} {}$ para cada ${} y \in X {}$, de modo que ${} \mathcal{F} {}$ converge a todo punto en ${} X {}$.
$\blacksquare$ 

> [!exercise|4]
> Sea ${} X {}$ un conjunto infinito y sea ${} \mathcal{F}= \left\{F\subset X: X\setminus F \text{ es finito }\right\} {}$ el [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] de Fréchet.
> 1. Demuestra que ${} \mathcal{F} {}$ es libre.
> 2. Si ${} X {}$ tiene la topología cofinita, ¿a qué punto de ${} X {}$ converge el [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${} \mathcal{F} {}$?

*Desarrollo.*
1. Sea ${} x \in X {}$. Entonces ${} F= X\setminus \left\{x \right\} {}$ tiene complemento finito, así que ${} F \in \mathcal{F} {}$. De modo que ${} x \not \in \bigcap_{F \in \mathcal{F}} F {}$. Así que ${} \bigcap_{F \in \mathcal{F}}F = \emptyset {}$. Entonces ${} \mathcal{F} {}$ es libre.
2. Sea ${} x \in X {}$. Nota que si ${} U \in \mathcal{N}(x) {}$ entonces existe ${} V {}$ abierto tal que ${} x \in V \subseteq U {}$. Como ${} V {}$ es abierto, tiene complemento finito, de modo que ${} X\setminus U {}$  también tiene complemento finito, así que es abierto. De este modo, ${} \mathcal{N}(x)= \left\{U\subseteq X : x \in U \land X\setminus U \text{ es finito }\right\} {}$.
	Entonces ${} \mathcal{N}(x)\subseteq \mathcal{F} {}$ y ${} \mathcal{F} {}$ converge a ${} x {}$. Entonces ${} \mathcal{F} {}$ converge a todo punto en ${} X {}$.
$\blacksquare$      

> [!exercise|5]
> Sea ${} f: X \to Y {}$ una función entre dos conjuntos. Si ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] en ${} X {}$, demuestra que ${} f(\mathcal{G}) {}$ es un [[[[Ultrafiltro\|[[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]|[[ultrafilt\|ultrafilt]]ro]] en ${} Y {}$.
> 

*Demostración.* Sea ${} f: X \to Y {}$ y ${} \mathcal{G} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] en ${} X {}$. Sea ${} E\subseteq Y {}$ un subconjunto cualquiera. Si ${} f^{-1}(E)= \emptyset {}$ entonces se tiene que ${} X\setminus f^{-1}(E) \in \mathcal{G} {}$, de modo que ${} f^{-1}(Y\setminus E) \in \mathcal{G} {}$. Así, ${} f(f^{-1}(Y\setminus E)) \in f(\mathcal{G}) {}$. Además, ${} f(f^{-1}(Y\setminus E)) \subseteq Y\setminus E {}$, entonces ${} Y\setminus E \in f(\mathcal{G}){}$.
Supongamos que ${} f^{-1}(E) \neq \emptyset {}$. Entonces ${} f^{-1}(E) \in \mathcal{G} {}$ o ${} X\setminus f^{-1}(E) \in \mathcal{G} {}$. Si ${} f^{-1}(E) \in \mathcal{G} {}$ entonces se tiene que ${} f(f^{-1}(E)) \in f(\mathcal{G}) {}$ y, como ${} f(f^{-1}(E))\subseteq E {}$ entonces ${} E \in f(\mathcal{G}) {}$. Si ${} X\setminus f^{-1}(E) \in \mathcal{G} {}$ entonces ${} f^{-1}(Y\setminus E) \in \mathcal{G} {}$, de modo que ${} f(f^{-1}(Y\setminus E)) \in f(\mathcal{G}) {}$, pero ${} f(f^{-1}(Y\setminus E)) \subseteq Y\setminus E {}$ entonces ${} Y\setminus E \in f(\mathcal{G}){}$.
En cualquier caso, si ${} E\subseteq Y {}$ entonces ${} E \in f(\mathcal{G}) {}$ o ${} X\setminus E \in f(\mathcal{G}) {}$. Por lo tanto, ${} f(\mathcal{G}) {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] en ${} Y {}$.
$\blacksquare$ 

> [!exercise|6]
> Sea ${} X {}$ un conjunto finito.
> 1. Demuestra que todo [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] en ${} X {}$ es fijo.
> 2. Demuestra que ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] en ${} X {}$ si y sólo si existe ${} a \in X {}$ tal que 
> 	$${} \mathcal{G} = \left\{ A\subset X: a \in  A \right\} . {}$$

*Desarrollo.*
1. Sea ${} \mathcal{F} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] en ${} X {}$. Como ${} \mathcal{F} \subseteq \mathcal{P}(X) {}$ y ${} \mathcal{P}(X) {}$ es finito, entonces ${} \mathcal{F} {}$ es finito. Luego por el [[Spaces/Home/Tareas/Semestre 6/Topología II/Tarea 3#^2c5595\|#^2c5595]] se tiene que ${} \cap \mathcal{F} \neq \emptyset {}$ y, por lo tanto, ${} \mathcal{F} {}$ es fijo.
2. Sea ${} \mathcal{G} {}$ un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] en ${} X {}$.
	- ${} \rightarrow {}$ Supongamos que ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]. Por el primer inciso se tiene que ${} \mathcal{G} {}$ es fijo. Sea ${} a \in \cap \mathcal{G} {}$. Sea ${} F \subseteq X {}$ tal que ${} a \in F {}$. Como ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] entonces ${} F \in \mathcal{G} {}$ o ${} X\setminus F \in \mathcal{G}{}$. ${} X\setminus F {}$ es imposible pues ${} a \not \in X\setminus F {}$ y ${} a \in \cap \mathcal{G} {}$. Por lo tanto ${} F \in \mathcal{G} {}$. Así:
		$${} \mathcal{G} = \left\{ F \subseteq  X: a \in  F \right\}.  {}$$
	- ${} \leftarrow {}$ Supongamos que 
		$${} \mathcal{G} = \left\{F \subseteq  X: a \in  F \right\} , {}$$
		para alguna ${} a \in X {}$. Veamos que ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]. Sea ${} F\subseteq X {}$ un subconjunto cualquiera. Si ${} a \in F {}$ entonces ${} F \in \mathcal{G} {}$. Si ${} a \not \in F {}$ entonces ${} a \in X\setminus F {}$ y ${} X\setminus F \in \mathcal{G} {}$. 
		En cualquier caso, si ${} F \subseteq X {}$ entonces ${} F \in \mathcal{G} {}$ o ${} X\setminus F \in \mathcal{G} {}$.
		Entonces  es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] en  
$\blacksquare$ 

> [!exercise|7]
> Sean ${} \mathcal{F} {}$ y ${} \mathcal{G} {}$ dos filtros tales que ${} \mathcal{G} {}$ es más fino que ${} \mathcal{F} {}$.
> 1. Si ${} \mathcal{F} {}$ es libre demuestra que ${} \mathcal{G} {}$ es libre.
> 2. Si ${} \mathcal{G} {}$ es fijo demuestra que ${} \mathcal{F} {}$ es fijo.

*Demostración.* Observa que como ${} \mathcal{F} \subseteq \mathcal{G} {}$ entonces ${} \cap \mathcal{G} \subseteq \cap \mathcal{F}{}$. Si ${} \cap \mathcal{F}= \emptyset {}$ entonces ${} \cap \mathcal{G} = \emptyset{}$ y, si ${} \cap \mathcal{G} \neq \emptyset {}$ entonces ${} \cap \mathcal{F} \neq \emptyset {}$. Así, si ${} \mathcal{F} {}$ es libre, entonces ${} \mathcal{G} {}$ es libre y, si ${} \mathcal{G} {}$ es fijo entonces ${} \mathcal{F} {}$ es fijo.
$\blacksquare$

> [!exercise|8]
> Desmuestra que si un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${} \mathcal{F} {}$ está contenido en un único [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] ${} \mathcal{G} {}$, entonces ${} \mathcal{F}= \mathcal{G} {}$.    

*Demostración.* Veamos que ${} \mathcal{F} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]. Sea ${} E \subseteq X {}$. Por contradicción supongamos que ${} E \not \in \mathcal{F} {}$ y ${} X\setminus E \not \in \mathcal{F} {}$. Entonces se debe tener que ${} E \cap F, X\setminus E \cap F \neq \emptyset {}$ para cada ${} F \in \mathcal{F} {}$ pues, de lo contrario, se tendría que ${} F \subseteq X\setminus E {}$ o ${} F \subseteq E {}$, lo cual implicaría que ${} X\setminus E \in \mathcal{F} {}$ o ${} E \in \mathcal{F} {}$. Sean 
$${} \mathcal{B} _{1}= \mathcal{F}  \cup  \left\{ E \cap  F: F \in  \mathcal{F}  \right\}, \mathcal{B} _{2}= \mathcal{F} \cup  \left\{ X\setminus  E \cap  F: F \in  \mathcal{F}  \right\} .$$
Notemos que ${} \mathcal{B}_{1} {}$ y ${} \mathcal{B}_{2} {}$ son cerrados bajo intersecciones, entonces son bases para filtros ${} \mathcal{F}_{1} {}$ y ${} \mathcal{F}_{2} {}$ en ${} X {}$. Además, todo [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] está contenido en un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]], entonces existen ultrafiltros ${} \mathcal{G}_{1} {}$ y ${} \mathcal{G}_{2} {}$ tales que ${}\mathcal{F} \subseteq \mathcal{F}_{1}\subseteq \mathcal{G}_{1} {}$ y ${} \mathcal{F} \subseteq \mathcal{F}_{2}\subseteq \mathcal{G}_{2} {}$. Pero ${} \mathcal{G} {}$ es el único [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] que contiene a ${} \mathcal{F} {}$ entonces ${} \mathcal{G}_{1}= \mathcal{G}= \mathcal{G}_{2} {}$. Además, ${} E \in \mathcal{G}_{1} {}$ y ${} X\setminus E \in \mathcal{G}_{2} {}$, de modo que ${} E, X\setminus E \in \mathcal{G} {}$ y, por lo tanto, ${} \emptyset= E \cap X\setminus E \in \mathcal{G} {}$, lo cual es imposible, pues ${} \mathcal{G} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]].
Entonces ${} E \in \mathcal{F} {}$ o ${} X\setminus E \in \mathcal{F} {}$ y ${} \mathcal{F} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]. Luego, como ${}\mathcal{F} \subseteq \mathcal{G} {}$ entonces se tiene que ${} \mathcal{F}= \mathcal{G} {}$.
$\blacksquare$

> [!exercise|9]
> Demuestra que un punto ${} x {}$ es un punto de acumulación de una red ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ si y sólo si ${} x {}$ es un punto de acumulación del [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
> 

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} x {}$ es un punto de acumulación de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$. Sea ${} U \in \mathcal{N}(x) {}$. Entonces para cada ${} \lambda_{0} \in \Lambda {}$ existe ${} \lambda\geq \lambda_{0} {}$ tal que ${} x_{\lambda} \in U {}$. Entonces para cada ${} \lambda_{0} \in \Lambda {}$ se tiene que ${} T_{\lambda_{0}} \cap U \neq \emptyset {}$. Así, ${} x {}$ es un punto de acumulación del [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
- Supongamos que ${} x {}$ es un punto de acumulación del [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por ${} (x_{\lambda})_{\lambda \in \Lambda} {}$. Entonces para cada ${} U \in \mathcal{N}(x) {}$ y para cada ${} \lambda_{0} \in \Lambda {}$ se tiene que ${} T_{\lambda_{0}} \cap U \neq \emptyset {}$. Entonces Para cada ${} \lambda_{0} \in \Lambda {}$ existe ${} \lambda \geq \lambda_{0} {}$ tal que ${} x_{\lambda} \in U {}$. Entonces ${} x {}$ es un punto de acumulación de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
$\blacksquare$

> [!exercise|10]
> Demuestra que ${} x {}$ es un punto de acumulación de un [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] ${} \mathcal{F} {}$ si y sólo si ${} x {}$ es un punto de acumulación de la red basada en ${} \mathcal{F} {}$. 
> 

*Demostración.* 
- ${} \rightarrow {}$ Supongamos que ${} x {}$ es un punto de acumulación de ${} \mathcal{F} {}$. Sea ${} U \in \mathcal{N}(x){}$. Entonces para cada ${} F \in \mathcal{F} {}$ se tiene que ${} F \cap U \neq \emptyset{}$. Así, para cada ${} F \in \mathcal{F} {}$ existe ${} x_{F} \in X {}$ tal que ${} x_{F} \in U {}$.
	Sea ${} (z,G) \in \mathcal{A}_{\mathcal{F}}= \left\{(x,F) \in X \times \mathcal{F} \vert x \in F \right\} {}$ y ${} q:\mathcal{A}_{\mathcal{F}} \to X {}$ dada por ${} q(x,F)=x {}$. Como ${} G \in \mathcal{F} {}$ entonces existe ${} x_{G} \in G{}$ tal que ${} x_{G} \in U {}$. Nota que ${} (x_{G},G)\geq (z,G) {}$, pues ${} G \subseteq G {}$. Además, ${} x_{G} \in U {}$. Entonces para cada ${} (z,G) \in \mathcal{A}_{\mathcal{F}} {}$ existe ${} (x_{G},G)\geq (z,G) {}$ tal que ${} q(x_{G},G) \in U {}$. Por lo tanto ${} (q(x,F))_{(x,F) \in \mathcal{A}_{\mathcal{F}}} {}$ converge a ${} x {}$.
- ${} \leftarrow {}$ Supongamos que ${} (q(x,F))_{(x,F) \in \mathcal{A}_{\mathcal{F}}} {}$ tiene a ${} x {}$ como punto de acumulación. Sea ${} U \in \mathcal{N}(x) {}.$ Entonces para cada ${} (x,F) {}$ existe ${} (z,G)\geq (x,F) {}$ tal que ${} q(z,G)=z \in U {}$. Así, para cada ${} F \in \mathcal{F}{}$ existe ${} G\subseteq F {}$ tal que ${} G \cap U \neq \emptyset{}$. Por lo tanto, ${} F \cap U \neq \emptyset {}$. Entonces ${} x {}$ es un punto de acumulación de ${} \mathcal{F} {}$.
$\blacksquare$

> [!exercise|11]
> Supongamos que ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$ es una subred de la red ${} (x_{\lambda})_{\lambda \in \Lambda} {}$. Demuestra que el [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$ es más fino que el [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.

*Demostración.* Como ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$ es una subred de ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ entonces ${} \lambda_{\mu}: \mathcal{A} \to \Lambda {}$ es una función creciente y cofinal. Sea ${} \lambda \in \Lambda {}$. Considera el conjunto ${} T_{\lambda} {}$. Como ${} \lambda_{\mu} {}$ es cofinal entonces existe ${} \mu \in \mathcal{A} {}$ tal que ${} \lambda_{\mu}\geq \lambda {}$. Si ${} \sigma\geq \mu {}$ entonces como ${} \lambda_{\mu} {}$ es creciente ${} \lambda_{\sigma} \geq \lambda_{\mu} {}$. De modo que ${} x_{\lambda_{\sigma}} \in T_{\lambda} {}$. Así, ${} T_{\lambda_{\mu}} \subseteq T_{\lambda}{}$. Así que ${} T_{\lambda} {}$ es un elemento del [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por la subred ${} (x_{\lambda_{\mu}})_{\mu \in \mathcal{A}} {}$.
$\blacksquare$

> [!exercise|12]
> Demuestra que el [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por una ultrared es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]. Análogamente, demuestra que la red generada por un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] es una ultrared.

*Demostración.* 
1. Supongamos que ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ es una ultrared. Sea ${} E \subseteq X {}$. Como ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ es una ultrared entonces ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ se encuenta residualmente en ${} E {}$ o en ${} X\setminus E {}$. Sin pérdida de generalidad supongamos que ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ se encuentra residualmente en ${} E {}$. Entonces existe ${} \lambda_{0} \in \Lambda {}$ tal que si ${} \lambda\geq \lambda_{0} {}$ se tiene que ${} x_{\lambda} \in E {}$. Es decir, ${} T_{\lambda_{0}} \subseteq E {}$. Entonces ${} E {}$ es un elemento del [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] generado por ${} (x_{\lambda})_{\lambda \in \Lambda} {}$.
2. Supongamos que ${} \mathcal{F} {}$ es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]]. Sea ${} E\subseteq X {}$. Como ${} \mathcal{F} {}$  es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] entonces ${} E \in \mathcal{F} {}$ o ${} X\setminus E \in \mathcal{F}{}$. Sin pérdida de generalidad supongamos que ${} E \in \mathcal{F} {}$. Sea ${} x \in E {}$. Supongamos que ${} (z,G)\geq (x,E) {}$ entonces ${} G\subseteq E {}$ y, por lo tanto, ${} z \in E {}$. Entonces ${} (q(x,F))_{(x,F) \in \mathcal{A}_{\mathcal{F}}} {}$ está residulamente en ${} E {}$. Por lo tanto ${} (q(x,F))_{(x,F) \in \mathcal{A}_{\mathcal{F}}} {}$ es una ultrared.
$\blacksquare$

> [!exercise|13]
> Demuestra que un espacio ${} X {}$ es compacto si y sólo si toda utlrared en ${} X {}$ converge.
> 

*Demostración.* 
1. Supongamos que ${} X {}$ es compacto. Sea ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ es una ultrared. Entonces su [[Spaces/Home/Conceptos/Semestre 6/Filtro\|Filtro]] asociado es un [[Spaces/Home/Conceptos/Semestre 6/Ultrafiltro\|Ultrafiltro]] y como ${} X {}$ es compacto, entonces converge. Luego ${} (x_{\lambda})_{\lambda \in \Lambda} {}$ converge.
2. Supongamos que toda ultrared converge. Sea ${} \mathcal{F} {}$ un [[Ultrafiltro]]. Entonces la [[Spaces/Home/Conceptos/Semestre 6/Ultrared\|ultrared]] asociada a ${} \mathcal{F} {}$ converge y ${} \mathcal{F} {}$ también lo hace. Entonces ${} X {}$ es compacto.    
$\blacksquare$ 