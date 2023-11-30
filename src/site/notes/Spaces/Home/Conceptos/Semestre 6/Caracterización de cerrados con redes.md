---
{"dg-publish":true,"permalink":"/spaces/home/conceptos/semestre-6/caracterizacion-de-cerrados-con-redes/"}
---

#Tema/Topología #Tipo/Corolario

> [!corollary|*]
> $A$ es cerrado si y sólo si para toda [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]] en $A$ que [[Spaces/Home/Notas/Semestre 6/Topología II/Redes#Convergencia de una red\|converge]], se tiene que sus puntos de [[Spaces/Home/Notas/Semestre 6/Topología II/Redes#Convergencia de una red\|convergencia]] son elementos de $A$.

*Demostración.*
- $\rightarrow$. Supongamos que $A$ es cerrado. Sea $(x_{\lambda})_{\lambda \in \mathcal{A}}$ una [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]] en $A$ convergente. Como $A= \overline{A}$, $(x_{\lambda})_{\lambda \in \mathcal{A}}$ es una [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]] en $\overline{A}$ y, por lo tanto, sus puntos de [[Spaces/Home/Notas/Semestre 6/Topología II/Redes#Convergencia de una red\|convergencia]] pertenecen a $\overline{A}=A$.
- $\leftarrow$ Sea $x \in \overline{A}$. Entonces existe una [[Spaces/Home/Conceptos/Semestre 6/Red\|Red]] $(x_{\lambda})_{\lambda \in \mathcal{A}}$ en $A$ tal que $x_{\lambda}$ convege a $x$. Entonces $x \in A$ y $\overline{A}\subseteq A \subseteq \overline{A}$, i.e., $A=\overline{A}$ y $A$ es cerrado.