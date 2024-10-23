![[homework2.pdf]]

# 1.
### Proposition
$$
\lim_{ n \to \infty } \frac{{n+1}}{2n+3}=\frac{1}{2}
$$
$$
x_{n} = \frac{{n+1}}{2n+3}
$$

### Definition
$$
\lim_{  n \to \infty } x_{n} = l \quad\quad \forall \varepsilon > 0 ,\ \exists N_{\varepsilon} \in \mathbb{N} : |x_{n} - l| < \varepsilon, \forall n \geq N_{\varepsilon}
$$

### Solution
$l=\frac{1}{2}$
$$
\left| {\frac{n+1}{2n+3} - \frac{1}{2}} \right| <\varepsilon\quad \quad \Bigg|\text{we amplify with }2 \text{ and } (2n+3)
$$
$$
\left| \frac{{2n+2}}{4n+6} - \frac{{2n+3}}{4n+6}\right|<\varepsilon
$$
$$
\left| -\frac{1}{4n+6}\right| <\varepsilon
$$
$$
\frac{1}{4n+6}<\varepsilon
$$


condition for above statement to be true:
$$
1 < \varepsilon(4n+6)
$$
$$
0< 4\varepsilon n +6\varepsilon -1
$$
$$
-4\varepsilon n<6\varepsilon-1
$$
$$
n> \frac{{6\varepsilon-1}}{4\varepsilon}
$$
let's try to prove it false
$$
\exists N_{\varepsilon} : \forall n\geq N_{\varepsilon}\ ,\ n< \frac{{6\varepsilon-1}}{4\varepsilon}
$$
but
$$
n \in [0, \infty)
$$
therefore
$$
\exists n = \frac{{6\varepsilon-1}}{4\varepsilon}+1\ :\quad n> \frac{{6\varepsilon-1}}{4\varepsilon}, \forall \varepsilon >0
$$

