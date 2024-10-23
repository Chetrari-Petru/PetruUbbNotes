

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


# 4.
$$
x_{n} = 1+ \frac{1}{2} + \dots+ \frac{1}{n} - \ln(n)
$$

$$
x_{n+1} = 1+\frac{1}{2}+\dots+\frac{1}{n}+\frac{1}{n+1}-\ln(n+1)
$$
## Monotony
$$
x_{n+1} \leq x_{n}
$$
$$
x_{n+1}-x_{n}\leq_{0} 
$$
$$
 \frac{1}{n+1} - \ln(n+1)+\ln(n)\leq {0}
$$
$$
\frac{1}{n+1} - \ln\left( \frac{{n+1}}{n} \right) \leq 0
$$
$$
\ln\left( 1+\frac{1}{n} \right) \geq \frac{1}{n+1}
$$
$$
1+\frac{1}{n} \geq e^{{\tfrac{1}{n+1}}}\quad (True)
$$
It implies that the sequence, $x_{n}$ is decreasing
This implies that it has supremum $x_{1}$ , $x_{1} \geq x_{n} \forall n \in \mathbb{N}$

## Lower Boundary
$$
x_{n} = \left( \sum_{i=1}^n \frac{1}{n} \right)-\ln(n) 
$$

we approximate $\sum_{i=1}^n \frac{1}{n}$ with integrals

$$
\int_{1}^n \frac{1}{x} dx \leq \sum _{i=1}^n \frac{1}{i} \leq 1+\int_{1}^{n} \frac{1}{x}dx
$$

sum functions are very similar to integrals, integrals being \*intuitively\* sums of very small rectangles that compose the function [An interesting video on this topic](https://youtu.be/5M2RWtD4EzI?si=CzTt8DANU_ShPfAX&t=160)

$$
\ln n \leq \sum _{i=1}^n \frac{1}{i} \leq 1+\ln n
$$
therefore 
$$
\sum _{i=1}^n \frac{1}{i} \in [\ln n, 1+\ln n]
$$

this implies that 
$$
\operatorname{inf}(x_{n}) \in [\ln n, 1+\ln n] - \ln n
$$
$$
\Leftrightarrow 
$$
$$
\operatorname{inf}(x_{n}) \in [0, 1]
$$
which implies that
$$
\exists l \in [0,1] : \forall x \in x_{n}, x\geq l
$$
this proves that $x_{n}$ is bounded
## Conclusion

because $x_{n}$ is descending and bounded, it is convergent
