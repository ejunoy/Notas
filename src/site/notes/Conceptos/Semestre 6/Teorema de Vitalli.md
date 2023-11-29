---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/teorema-de-vitalli/"}
---

#Enconstrucción
#Tema/Análisis  #Tipo/Teorema  
> [!theorem|*] Vitalli
> Si se supone el axioma de elección el problema en ${}\mathbb{R}{}$ no tiene solución.

*Demostración.* Supongamos que ${}p: \mathcal{P}(\mathbb{R}) \to [0,\infty]{}$ es solución.
En ${}[0,1]{}$ se define la relación de equivalencia ${}x \sim y \iff x-y \in \mathbb{Q}{}$.
**Observación.** ${}[x]= \left\{x+q: q \in \mathbb{Q} \right\}{}$ es numerable.
Como ${}[0,1]{}$ es una unión disjunta de clases de equivalencia, entonces por el axioma de elección existe ${}V\subseteq [0,1]{}$ con ${}[0,1]= \bigcup_{v \in V}{}[v]$.
${}\therefore V{}$ es no numerable.
${}V{}$ cumple las siguientes propiedades:
1. Si ${}r,s \in \mathbb{Q}{}$ con ${}r \neq s{}$ entonces ${}(V+r) \cap (V+s) = \emptyset{}$.
2. ${}[0,1]\subseteq \bigcup_{r \in \mathbb{Q}^{'}} V+r \subseteq [-1,2],{}$ con ${}\mathbb{Q}'= \mathbb{Q} \cap [-1,1]{}$.
*Desarrollo.* 
1. Supongamos que ${}(V+r) \cap (V+s) \neq \emptyset{}$. Entonces existen ${}v_{1},v_{2} \in V{}$ tales que ${}v_{1}+r=v_{2}+s{}$. Como ${}r \neq s{}$ entonces ${}v_{1} \neq v_{2}{}$.
	Como ${}v_{1}+r=v_{2}+s{}$ entonces ${}v_{1}-v_{2} = s-r \in \mathbb{Q}{}$ entonces ${}v_{1} \sim v_{2}{}$, de modo que ${}v_{1}= v_{2}{}$, lo cual es imposible.
2. Si ${}x \in [0,1]{}$ entonces existe un único ${}v \in V{}$ tal que ${}x\sim v{}$ y ${}x-v =r\in \mathbb{Q} \cap [-1,1]{}$. Por lo tanto, ${}x \in V+r {}$.
	Si ${}v \in V, r \in \mathbb{Q}'{}$ entonces ${}v \in [0,1]{}$, ${}r \in [-1,1]{}$ con ${}v+r \in [-1,2]{}$.
Para terminar:
$${}  [0,1] \subseteq  \bigcup_{r \in  \mathbb{Q}'} V+r \subseteq  [-1,2]   {},$$ entonces 
$${}1= \rho([0,1]) \leq \rho\left( \bigcup_{r \in \mathbb{Q}'} V+r \right)\leq \rho([-1,2])=3{}$$
También
$${} \sum_{r\in  \mathbb{Q}'}^{} \rho (V+r) = \sum_{r\in  \mathbb{Q}'}^{} \rho (V)  .  {}$$
Por lo tanto, 
$${}  1\leq \sum_{r\in  \mathbb{Q}'}^{} \rho (V) \leq  3 .{}$$
Como ${}\rho(V)>0{}$ entonces existe ${}N \in \mathbb{N}{}$ tal que ${}N \rho(V) >3{}$, lo cual es una contradicción, pues ${}\mathbb{Q}'{}$ es infinito numerable.
$\blacksquare$