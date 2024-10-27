

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

# 2.

## a)
$$
(1+2+3+4+\dots+n)^{1/n}
$$
$$
\lim_{ n \to \infty }\left( \frac{n(n+1)}{2} \right) ^ \frac{1}{n}
$$
$$
\lim_{ n \to \infty } e ^ { \ln\left( \tfrac{n(n+1)}{2} \right)^ \frac{1}{n}  } 
$$
$$
\lim_{ n \to \infty } e^  \left( \tfrac{1}{n} \cdot \ln{\tfrac{n(n+1)}{2}} \right) 
$$

we take the exponent separately
$$
\lim_{ n \to \infty } \frac{{\ln \frac{{n(n+1)}}{2}}}{n}
$$
apply stolz cesaro
$$
\lim_{ n \to \infty } \frac{{\ln \frac{{(n+1)(n+2)}}{2} - \ln \frac{{n(n+1)}}{2}}}{n+1-n}
$$

$$
\lim_{ n \to \infty }    \frac{\ln\left({\frac{{(n+1)(n+2)}}{2}\cdot \frac{2}{n(n+1)}} \right)}{1}
$$
$$
\lim_{ n \to \infty } \ln \frac{{n+2}}{n}
$$
$$
\lim_{ n \to \infty } \ln \left( 1 + \frac{2}{n} \right) = 0
$$
coming back to the main limit
$$
\lim_{ n \to \infty } x_{n} = \lim_{ n \to \infty } e^0 = 1
$$


## b)

$$
x_{n} = \left( \frac{\ln(n+1)}{\ln n} \right) ^n
$$
calculating limit

$$
\lim_{ n \to \infty } \left( 1+\frac{{\ln(n+1)}}{\ln n} -1 \right)^n
$$
$$
\lim_{ n \to \infty } \left( 1+ \frac{{\ln(n+1)- \ln n}}{\ln n} \right)^n
$$
$$
\lim_{ n \to \infty } \left(\left( 1+ {\frac{\ln \frac{n+1}{n}}{\ln n}} \right)^ \tfrac{{\ln n}}{\ln \tfrac{n+1}{n}}  \right)^ \tfrac{{n \cdot \ln {\tfrac{n+1}{n}}}}{\ln n}
$$
$$
e^{\lim_{ n \to \infty } \tfrac{n \cdot \ln \tfrac{n+1}{n}}{\ln n}}
$$
$$
e^{\lim_{ n \to \infty } \tfrac{\left(  \ln \tfrac{n+1}{n}\right)^n }{\ln n} }
$$
$$
e^0 = 1
$$

## c)
$$
x_{n} = \frac{n^n}{1^1+2^2+3^3+..+n^n}
$$
$$
\lim_{ n \to \infty } \frac{e^{\ln{n^n}}}{e^{\ln{n^n}}\left( \frac{1^1+2^2+3^3+\dots}{e^{\ln n^n}}+1 \right) }

$$
$$
\lim_{ n \to \infty } \frac{1^1+2^2+3^3+\dots}{e^{n \ln n}} +1
$$
$$
\lim_{ n \to \infty } x_{n} = 1
$$


# 3.
i'm going to have this handwritten because i'm running out of time, aand now i have the means to do so (i'm doing the hw at home)
![[SABHDSABSDA|800x300]]

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
