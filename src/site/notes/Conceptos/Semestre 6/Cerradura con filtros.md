---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/cerradura-con-filtros/"}
---

#Enconstrucción
#Tema/Topología  #Tipo/Teorema  
> [!theorem|*] Cerradura con filtros
> Sea ${}(X,\tau){}$ un [[Conceptos/Semestre 6/Espacio topológico\|espacio topológico]]. ${}A\subseteq X{}$. Entonces un punto ${}x{}$ está en ${}\overline{ A}{}$ si y solo si existe un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}{}$ tal que ${}A \in \mathcal{F}{}$ y ${}\mathcal{F} \to x{}$.

*Demostración.* 
- ${}\rightarrow{}$ Sea ${}x \in \overline{A}{}$. Sea ${}\mathcal{C}= \left\{ U \cap A : U \in \mathcal{N}(x) \right\}{}$. Entonces ${}\mathcal{C}{}$ es base para un [[Conceptos/Semestre 6/Filtro\|filtro]] ${}\mathcal{F}= \mathcal{F}_{\mathcal{C}}{}$. Además, se cumple que ${}A \in \mathcal{F}{}$ y ${}\mathcal{N}(x)\subseteq \mathcal{F}{}$.
- ${}\leftarrow{}$ Supongamos que ${}\mathcal{F}{}$ es un [[Conceptos/Semestre 6/Filtro\|filtro]] tal que ${}A \in \mathcal{F}{}$ y ${}\mathcal{N}(x) \subseteq \mathcal{F}{}$. Entonces para cada ${}U \in \mathcal{N}(x){}$ se tiene que ${}U \cap A \in \mathcal{F}{}$, de modo que ${}U \cap A \neq \emptyset{}$ y ${}x \in \overline{A}{}$.
$\blacksquare$