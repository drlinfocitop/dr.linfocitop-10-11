---
{"dg-publish":true,"permalink":"/10-dr-linfocitop/la-tex/","noteIcon":""}
---

![Pasted image 20231227060757.png|300](/img/user/02%20Image/Pasted%20image%2020231227060757.png)
- Links: 
	- Página oficial: https://www.latex-project.org/
	- https://manualdelatex.com/tutoriales/ecuaciones
	- https://metodos.fam.cie.uva.es/~latex/apuntes/apuntes3.pdf
	- https://www.overleaf.com/learn/latex/Matrices
### Acentos
- $\acute{a}$ `\acute{a}` | $\grave{a}$ `\grave{a}`
- $\tilde{a}$ `\tilde{a}` | $\bar{a}$ `\bar{a}` | $\breve{a}$ `\breve{a}`
- $\hat{a}$ `\hat{a}` | $\check{a}$ `\check{a}` | $\vec{a}$ `\vec{a}`
- $\dot{a}$ `\dot{a}` | $\ddot{a}$ `\ddot{a}` | $\dddot{a}$ `\dddot{a}`
### Código
- $\leq$ ``\leq`` | $\nleq$ `\nleq` | $\leqslant$ ``\leqslant`` | $\ll$ ``\ll``
- $\geq$ `\geq` | $\ngeq$ `\ngeq` | $\geqslant$ ``\geqslant`` | $\gg$ `\gg`
- $\pm$ `\pm` | $\mp$ `\mp`
- $\equiv$ `\equiv` | $\cong$ `\cong` 
- $\sim$ `\sim` | $\approx$ `\approx` | $\approxeq$ `\approxeq` 
### Funciones
- $\sin$ `\sin` | $\cos$ `\cos` | $\tan$ `\tan`
- $\arcsin$ `\arcsin` | $\arccos$ `\arccos` | $\arctan$ `\arctan`
- $\csc$ `\csc` | $\sec$ `\sec` | $\cot$ `\cot`
- $\sinh$ `\sinh` | $\cosh$ `\cosh` | $\tanh$ `\tanh`
- $\log$ `\log` | $\ln$ `\ln`
### Paréntesis, llaves y corchetes
- $(2)$ `(2)` | $\{2\}$ `\{2\}` | $\langle 2 \rangle$ `\langle 2 \rangle`
- $|2|$ `|2|` | $\|2\|$ `\|2\|`
### Matrices
- $\begin{matrix} 1 & 2\\ a&b\end{matrix}$ `\begin{matrix}1&2\\a&b\end{matrix}`
- $\begin{pmatrix}1&2\\a&b\end{pmatrix}$ `\begin{pmatrix}1&2\\a&b\end{pmatrix}`
- $\begin{bmatrix}1&2\\a&b\end{bmatrix}$ `\begin{bmatrix}1&2\\a&b\end{bmatrix}`
- $\begin{Bmatrix}1&2\\a&b\end{Bmatrix}$ `\begin{Bmatrix}1&2\\a&b\end{Bmatrix}`
- $\begin{vmatrix}1&2\\a&b\end{vmatrix}$ `\begin{vmatrix}1&2\\a&b\end{vmatrix}`
- $\begin{Vmatrix}1&2\\a&b\end{Vmatrix}$ `\begin{Vmatrix}1&2\\a&b\end{Vmatrix}`
- $\left\langle\begin{matrix}1&2\\a&b\end{matrix}\right\rvert$ `\left\langle\begin{matrix}1&2\\a&b\end{matrix}\right\rvert`
- $\left\langle\begin{matrix}1&2\\a&b\end{matrix}\right\rangle$ `\left\langle\begin{matrix}1&2\\a&b\end{matrix}\right\rangle`
### Vectores
- $\vec{v}$ `\vec{v}`
- $\hat{k}$ `\hat{k}`
- $\hat{\imath}$ `\hat{\imath}` | $\hat{\jmath}$ `\hat{\jmath}`
- $\vec{u}\cdot \vec{v}$ `\vec{u} \cdot \vec{v}` | $\vec{u}\times \vec{v}$ `\vec{u}\times \vec{v}`
### Letra en modo matemático
- $\mathrm{ABCdef}$ `\mathrm{ABCdef}` 
- $\mathit{ABCdef}$ `\mathit{ABCdef}`
- $\mathnormal{ABCdef}$ `\mathnormal{ABCdef}` 
- $\mathcal{ABCdef}$ `\mathcal{ABCdef}`
- $\mathfrak{ABCdef}$ `\mathfrak{ABCdef}` 
- $\mathbb{ABCdef}$ `\mathbb{ABCdef}` 
- $\mathscr{ABCdef}$ `\mathscr{ABCdef}`
- $\mathtt{ABCdef}$ `\mathtt{ABCdef}`
- $\mathsf{ABCdef}$ `\mathsf{ABCdef}` 
- $\mathbf{ABCdef}$ `\mathbf{ABCdef}`
### Color
- $\textcolor{green}{\int_0^\infty f(x)d(x) = g(x) + C}$
- $\int_0^\infty \textcolor{blue}{f(x)d(x)} = \textcolor{red}{g(x)} + C$
### Ecuaciones

```
$$
\begin{align}
((a+b)^2& = a^2 + 2ab + b^2\\  
(a-b)^2& = a^2 - 2ab + b^2\\  
(a+b)(a-b)& = a^2 - b^2
\end{align}
$$
```
$$
\begin{align}
((a+b)^2& = a^2 + 2ab + b^2\\  
(a-b)^2& = a^2 - 2ab + b^2\\  
(a+b)(a-b)& = a^2 - b^2
\end{align}
$$
```
$$
\begin{multline}
(x+y+z)^3+k = x^3+y^3+z^3 \\  
+ 3x^2y + 3x^2z + 3xy^2 + 3y^2z + 3xz^2 + 3yz^2 + 6xyz + k
\end{multline}
$$
```
$$
 \begin{multline}
(x+y+z)^3+k = x^3+y^3+z^3 \\  
+ 3x^2y + 3x^2z + 3xy^2 + 3y^2z + 3xz^2 + 3yz^2 + 6xyz + k
\end{multline}
$$
## Sumatorio y productorio
- $\sum_{n=1}^{10}n$ `\sum_{n=1}^{10}n`
- $\prod_{n=1}^{10}n$ `\prod_{n=1}^{10}n`
- $\sideset{_{a}^{b}}{_{c}^{d}}\prod_{j=1}^{k+1}$ `\sideset{_{a}^{b}}{_{c}^{d}}\prod_{j=1}^{k+1}`
## Símbolos sobre otros
```
$$ 
\sideset{_{a}^{b}}{_{c}^{d}}\prod_{j=1}^{k+1}
$$
```
$$ \sideset{_{a}^{b}}{_{c}^{d}}\prod_{j=1}^{k+1} $$
```
$$
\overbrace{x+\underbrace{y+z}_{2} +w}^{4}
$$
```
$$\overbrace{x+\underbrace{y+z}_{2} +w}^{4}$$
## Letras griegas
- $\alpha$ `$\alpha$`
- $\beta$ `$\beta$`
- $\gamma$ `$\gamma$` 
- $\delta$ `$\delta$`
- $\theta$ `$\theta$` 
- $\epsilon$ `$\epsilon$`
- $\varepsilon$ `$\varepsilon$`
- $\zeta$ `$\zeta$`
- $\eta$ `$\eta$`
- $\tau$ `$\tau$`
- $\vartheta$ `$\vartheta$`
- $\pi$ `$\pi$`
- $\upsilon$ `$\upsilon$` 
- $\iota$ `$\iota$`
- $\varpi$ `$\varpi$`
- $\phi$ `$\phi$`
- $\kappa$ `$\kappa$` 
- $\rho$ `$\rho$`
- $\varphi$ `$\varphi$` 
- $\lambda$ `$\lambda$`
- $\varrho$ `$\varrho$`
- $\chi$ `$\chi$`
- $\mu$ `$\mu$`
- $\sigma$ `$\sigma$`
- $\psi$ `$\psi$`
- $\nu$ `$\nu$`
- $\varsigma$ `$\varsigma$`
- $\omega$ `$\omega$`
- $\xi$ `$\xi$`
- $\Gamma$ `$\Gamma$`
- $\Lambda$ `$\Lambda$`
- $\Sigma$ `$\Sigma$`
- $\Psi$ `$\Psi$`
- $\Delta$ `$\Delta$`
- $\Xi$ `$\Xi$`
- $\Upsilon$ `$\Upsilon$`
- $\Omega$ `$\Omega$
- $\Theta$ `$\Theta$`
- $\Pi$ `$\Pi$`
- $\Phi$ `$\Phi$`
## Imágenes
 - ![Pasted image 20231227012527.png](/img/user/02%20Image/Pasted%20image%2020231227012527.png)
