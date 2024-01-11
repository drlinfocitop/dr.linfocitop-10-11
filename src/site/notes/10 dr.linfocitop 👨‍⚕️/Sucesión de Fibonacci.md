---
{"dg-publish":true,"permalink":"/10-dr-linfocitop/sucesion-de-fibonacci/","noteIcon":""}
---

- Definida como la suma de los 2 anteriores número naturales, siendo el primero $a_0=0$ y el segundo $a_1=1$
$$0,1,1,2,3,5,8,13,21,34,55,89,144,233,377,610,987,1597...$$
- Definición recursiva, $n \geq 2$
$$a_{n+1}=a_n+a_{n-1}$$
## Resolución matricial
- Expresión matricial
$$\begin{pmatrix} a_{n+1}\\ a_{n}\end{pmatrix}
=
\begin{pmatrix} 1&1\\ 1&0\end{pmatrix}
\cdot
\begin{pmatrix} a_{n}\\ a_{n-1}\end{pmatrix}
$$
- Ordenando obtenemos
$$\begin{pmatrix} a_{n+1}\\ a_{n}\end{pmatrix}
=
\begin{pmatrix} 1&1\\ 1&0\end{pmatrix}^n
\cdot
\begin{pmatrix} 0\\ 1\end{pmatrix}
$$
- Resolviendo mediante autovalores
$$a_n=\frac{\phi^n-\bar{\phi}^n}{\sqrt{5}}\;\;\;\text{donde}\;\;\;\phi=\frac{1+\sqrt{5}}{2}\;\wedge\;\bar{\phi}=\frac{1-\sqrt{5}}{2}$$
- Link de resolución: https://detalesaturing.files.wordpress.com/2014/03/la-sucesic3b3n-de-fibonacci.pdf
## Fórmula explícita evaluando valores iniciales
 