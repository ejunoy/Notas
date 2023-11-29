---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/caracterizacion-de-continuidad-con-redes/"}
---

#Tema/Topología  #Tipo/Teorema 

> [!theorem|*]
> Sea $f:X \to Y$ y $x_{0} \in X$. Entonces $f$ es continua en $x_{0}$ si y sólo si para toda [[Conceptos/Semestre 6/Red\|Red]] $(x_{\lambda})_{\lambda \in \mathcal{A}}$ que converge a $x_{0}$ se tiene que la [[Conceptos/Semestre 6/Red\|Red]] $(f(x_{\lambda}))_{\lambda \in \mathcal{A}}$ converge a $f(x_{0})$.

*Demostración.* 
- $\rightarrow$. Supongamos que $f$ es continua en $x_{0}$ y $(x_{\lambda})_{\lambda \in \mathcal{A}}$ converge a $x_{0}$. Sea $U \in \mathcal{N}(f(x_{0}))$. Entonces $f^{-1}(U) \in \mathcal{N}(x_{0})$. Y, como $(x_{\lambda})_{\lambda \in \mathcal{A}}$ converge a $x_{0}$ entonces existe $\lambda_{0} \in \mathcal{A}$ tal que si $\lambda\geq \lambda_{0}$ entonces $x_{\lambda} \in f^{-1}(U)$, de modo que $f(x_{\lambda}) \in U$ y, por lo tanto, $(f(x_{\lambda}))_{\lambda \in \mathcal{A}}$ converge a $f(x_{0})$.
- $\leftarrow$. Supogamos que para toda [[Conceptos/Semestre 6/Red\|Red]] $(x_{\lambda})_{\lambda \in \mathcal{A}}$ que converge a $x_{0}$ se tiene que $(f(x_{\lambda}))_{\lambda \in \mathcal{A}}$ converge a $f(x_{0})$.
	Supongamos que $f$ no es continua. Entonces existe $U \in \mathcal{N}(f(x_{0}))$ tal que para cada $V \in \mathcal{N}(x_{0})$ se tiene que $f(V) \not \subseteq U$.
	Sea $x_{V} \in V$ con $f(x_{V}) \not \in U$. Entonces $(x_{V})_{V \in \mathcal{N}(x_{0})}$ converge a $x_{0}$, así que $f(x_{V})$ converge a $f(x_{0})$. Así que existe $V \in \mathcal{N}(x_{0})$ tal que si $M\subseteq V$ entonces $f(x_{M}) \in U$. Lo cual es una contradicción.