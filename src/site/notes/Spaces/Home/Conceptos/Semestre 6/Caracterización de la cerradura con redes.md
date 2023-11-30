---
{"dg-publish":true,"permalink":"/spaces/home/conceptos/semestre-6/caracterizacion-de-la-cerradura-con-redes/"}
---

#Tema/Topología #Tipo/Teorema

> [!theorem|*] Caracterización de la cerradura
> 
> Sea $(X,\tau)$ un [[Spaces/Home/Conceptos/Semestre 6/Espacio topológico\|Espacio topológico]], $x_{0} \in X$ y $A \subseteq X$. Entonces $x_{0} \in \overline{A}$ si y sólo si existe una [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]] $(x_{\lambda})_{\lambda \in \mathcal{A}}$ en $A$ que converge a $x_{0}$.

*Demostración.*
- $\rightarrow$. Si $x_{0} \in \overline{A}$ entonces $\forall U \in \mathcal{N}(x_{0})$ existe $x_{u} \in U \cap A$. Entonces $(x_{U})_{U \in \mathcal{N}(x_{0})}$ es una [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]] que converge a $x_{0}$.
- $\leftarrow$. Supongamos que existe una [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]] $(x_{\lambda})_{\lambda \in \mathcal{A}}$ en $A$ que converge a $x_{0}$. Entnoces para cada $U \in \mathcal{N}(x_{0})$ se tiene que existe $\lambda_{U} \in \mathcal{A}$ tal que si $\lambda\geq \lambda_{U}$ entonces $x_{\lambda} \in U$. En particular, para cada $U \in \mathcal{N}(x_{0})$ existe $\lambda_{U}$ tal que $x_{\lambda_{U}} \in U \cap A$. Entonces $x_{0} \in \overline{A}$.