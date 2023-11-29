---
{"dg-publish":true,"permalink":"/conceptos/semestre-6/teorema-de-tychonoff/"}
---

#Tema/Topología  #Tipo/Teorema 

> [!theorem|*] Teorema de Tychonoff
> 
> Sea ${} X= \prod_{\alpha \in \mathcal{A}}^{}X_{\alpha} {}$ un producto de espacios topológicos. Entonces ${} X {}$ es compacto si y sólo si ${} X_{\alpha} {}$ es compacto para cada ${} \alpha \in \mathcal{A} {}$.
> 

*Demostración.* 
- ${} \rightarrow {}$ Si ${} X {}$ es compacto entonces ${} X_{\alpha}=\pi_{\alpha}(X) {}$ es compacto, pues ${} \pi_{\alpha} {}$ es continua.
- ${} \leftarrow {}$ Sea ${} \mathcal{G} {}$ un [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]]. Para cada ${} \alpha \in \mathcal{A} {}$ considera el [[Conceptos/Semestre 6/Ultrafiltro\|ultrafiltro]] ${} \pi_{\alpha}(\mathcal{G}) {}$ en ${} X_{\alpha} {}$. Como ${} X_{\alpha} {}$ es compacto entonces ${} \pi_{\alpha}(\mathcal{G}) {}$ converge a algún punto ${} x_{\alpha} \in X_{\alpha} {}$ . Luego, el [[Conceptos/Semestre 6/Filtro\|filtro]] ${} \mathcal{G} {}$ converge a ${} (x_{\alpha})_{\alpha \in \mathcal{A}} {}$. Entonces ${} X {}$ es compacto.
$\blacksquare$