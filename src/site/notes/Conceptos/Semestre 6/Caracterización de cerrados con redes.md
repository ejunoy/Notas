---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/caracterizacion-de-cerrados-con-redes/"}
---

#Tema/Topología #Tipo/Corolario

> [!corollary|*]
> $A$ es cerrado si y sólo si para toda [[Conceptos/Semestre 6/Red\|Red]] en $A$ que converge, se tiene que sus puntos de convergencia son elementos de $A$.

*Demostración.*
- $\rightarrow$. Supongamos que $A$ es cerrado. Sea $(x_{\lambda})_{\lambda \in \mathcal{A}}$ una [[Conceptos/Semestre 6/Red\|Red]] en $A$ convergente. Como $A= \overline{A}$, $(x_{\lambda})_{\lambda \in \mathcal{A}}$ es una [[Conceptos/Semestre 6/Red\|Red]] en $\overline{A}$ y, por lo tanto, sus puntos de convergencia pertenecen a $\overline{A}=A$.
- $\leftarrow$ Sea $x \in \overline{A}$. Entonces existe una [[Conceptos/Semestre 6/Red\|Red]] $(x_{\lambda})_{\lambda \in \mathcal{A}}$ en $A$ tal que $x_{\lambda}$ convege a $x$. Entonces $x \in A$ y $\overline{A}\subseteq A \subseteq \overline{A}$, i.e., $A=\overline{A}$ y $A$ es cerrado.