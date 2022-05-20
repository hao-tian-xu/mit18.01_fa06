# **FUNDAMENTAL**

- **Derivative**: slope of tangent line (geometric view)
  $$
  \lim _{\Delta x \rightarrow 0} \frac{\Delta f}{\Delta x}=\lim _{\Delta x \rightarrow 0} \frac{f\left(x_{0}+\Delta x\right)-f\left(x_{0}\right)}{\Delta x}=f^{\prime}\left(x_{0}\right)
  $$
- **Integrals**
  $$
  \lim _{n \rightarrow \infty} \sum_{i=1}^{n} f\left(c_{i}\right) \Delta x=\int_{a}^{b} f(x) d x \quad \leftarrow \quad \text { called a definite integral }
  $$
- **FTC 1**
  - if $f(x)$ is continuous and $F^{\prime}(x)=f(x)$, then
    $$
    \int_{a}^{b} f(x) d x=F(b)-F(a)
    $$
- **FTC 2**
  - If $F(x)=\int_{a}^{x} f(t) d t$ and $f$ is continuous, then
    $$
    F^{\prime}(x)=f(x)
    $$

# **MAIN**

- **Derivative Formulas**
  $$
  \frac{d}{d x} \sin x=\cos x ; \quad \frac{d}{d x} \cos x=-\sin x
  $$
- **Product formula**
  $$
  (u v)^{\prime}=u^{\prime} v+u v^{\prime}
  $$
- **Quotient formula**
  $$
  \left(\frac{u}{v}\right)^{\prime}=\frac{u^{\prime} v-u v^{\prime}}{v^{2}}
  $$
- **Chain Rule (composition)**
  - for $y=f(x), x=g(t)$
    $$
    \frac{d y}{d t}=\frac{d y}{d x} \cdot \frac{d x}{d t}
    $$
    - another notation: $\frac{d}{d t} f(g(t))=f^{\prime}(g(t)) g^{\prime}(t)$
- **Higher Derivatives**
  $$
  f^{\prime \prime \prime}(x)=D^{3} f=\frac{d^{3} f}{d x^{3}}
  $$
- **Inverse Functions**
  - If $y=f(x)$ and $g(y)=x$, we call $g$ the inverse function of $f, f^{-1}$ :
    $$
    x=g(y)=f^{-1}(y)
    $$
- **Exponential Differentiation**
  $$
  \frac{d}{d x} a^{x}=\lim _{\Delta x \rightarrow 0} \frac{a^{x+\Delta x}-a^{x}}{\Delta x}=\lim _{\Delta x \rightarrow 0} a^{x} \frac{a^{\Delta x}-1}{\Delta x}=a^{x} \lim _{\Delta x \rightarrow 0} \frac{a^{\Delta x}-1}{\Delta x}
  $$
  - define $e$: $\lim _{\Delta x \rightarrow 0} \frac{e^{\Delta x}-1}{\Delta x}=1 \quad \rightarrow \quad \frac{d}{d x}\left(e^{x}\right)=e^{x}$
  - define $\ln (x)$: if $y=e^{x}$, then $\ln (y)=x$
- **Differentials**
  - New notation: 
    $$
    d y=f^{\prime}(x) d x \quad(y=f(x))
    $$
    - Both $d y$ and $f^{\prime}(x) d x$ are called differentials
- **Anti-derivatives**
  $$
  F^{\prime}(x)=f(x) \quad \rightarrow \quad F(x)=\int f(x) d x
  $$
- **Parametric Equations**
  $$
  x=a \cos t ; \quad y=a \sin t ; \quad \rightarrow y^{2}+x^{2}=a^{2}
  $$
- **Polar Co-ordinates**
  $$
  x=r \cos \theta \quad \text { and } \quad y=r \sin \theta
  $$
- **Improper Integrals**
  $$
  \int_{a}^{\infty} f(x) d x=\lim _{M \rightarrow \infty} \int_{a}^{M} f(x) d x
  $$
  is said to converge if the limit exists (diverges if the limit does not exist).
  - Improper Integrals of the Second Type
    $$
    \int_{0}^{1} \frac{d x}{\sqrt{x}}
    $$

# **ADVANCED**

- **Implicit differentiation**
  - e.g. $y=x^{\frac{m}{n}} \quad \rightarrow \quad y^{n}=x^{m} \quad \rightarrow \quad \frac{d}{d x} y^{n}=\frac{d}{d x} x^{m} \quad \rightarrow$
    $$
    \left(\frac{d}{d y} y^{n}\right) \frac{d y}{d x}=n y^{n-1} \frac{d y}{d x}=m x^{m-1} \quad \rightarrow \quad \frac{d y}{d x}=\frac{m}{n} \frac{x^{m-1}}{y^{n-1}}
    $$
- **Linear Approximations**
  $$
  f(x) \approx f\left(x_{0}\right)+f^{\prime}\left(x_{0}\right)\left(x-x_{0}\right)
  \\ \\
  \Delta f \approx f^{\prime} \Delta x
  $$
- **Quadratic Approximations** 
  $$
  f(x) \approx f\left(x_{0}\right)+f^{\prime}\left(x_{0}\right)\left(x-x_{0}\right)+\frac{f^{\prime \prime}\left(x_{0}\right)}{2}\left(x-x_{0}\right)^{2}
  $$
- **Mean-Value Theorem (MVT)**
  If $f(x)$ is differentiable on $a<x<b$, and continuous on $a \leq x \leq b$, then
  $$
  \frac{f(b)-f(a)}{b-a}=f^{\prime}(c) \quad(\text { for some } c, a<c<b)
  $$
  - change the name of $b$ to $x: f(x)=f(a)+f^{\prime}(c)(x-a) \quad(\text { for some } c, a<c<x)$
- **Method of substitution and "advanced guessing"**
  - e.g. $\int \frac{d x}{x \ln x}$
  	Let $\quad u=\ln x \quad \rightarrow \quad d u=\frac{1}{x} d x$
    $$
    \int \frac{d x}{x \ln x}=\int \frac{1}{u} d u=\ln u+c=\ln (\ln (x))+c
    $$
- **Ordinary Differential Equations (ODEs)**
  - e.g. $\left(\frac{d}{d x}+x\right) y=0 \quad\left(\right.$ or $\left.\frac{d y}{d x}+x y=0\right)$
  	separate variables : $\quad \frac{d y}{y}=-x d x$
  	take the antiderivative of both sides:
    $$
    \begin{aligned}
    &\int \frac{d y}{y}=-\int x d x  &\rightarrow \\
    &\ln |y|=-\frac{x^{2}}{2}+c  &\rightarrow \\
    &|y|=e^{c} e^{-x^{2} / 2}  &\rightarrow \\
    &y=a e^{-x^{2} / 2} \ \ \left(a=\pm e^{c}\right)
    \end{aligned}
    $$
- **Change of Variable (method of substitution)**
  If $f(x)=g(u(x))$, then we write $d u=u^{\prime}(x) d x$ and
  $$
  \int g(u) d u=\int g(u(x)) u^{\prime}(x) d x=\int f(x) u^{\prime}(x) d x \quad \text { (indefinite integrals) }
  $$
  - For definite integrals:
    $$
    \int_{x_{1}}^{x_{2}} f(x) u^{\prime}(x) d x=\int_{u_{1}}^{u_{x}} g(u) d u \quad \text { where } u_{1}=u\left(x_{1}\right), u_{2}=u\left(x_{2}\right)
    $$
- **Riemann Sum**
  with left endpoints:
  $$
  \text{Area}=\left(y_{0}+y_{1}+\ldots+y_{n-1}\right) \Delta x
  $
- **Trapezoidal Rule**
  $$
  \text{Area}=\left(\frac{y_{0}+y_{1}}{2}+\frac{y_{1}+y_{2}}{2}+\frac{y_{n-1}+y_{n}}{2}\right) \Delta x
  $$
- **Simpson's Rule**
  $$
  \text { Area under parabola } \approx \text { (base)(weighted average height })=(2 \Delta x)\left(\frac{y_{0}+4 y_{1}+y_{2}}{6}\right)
  $$
  $$
  \begin{aligned}
  \text { Area }&=(2 \Delta x)\left(\frac{1}{6}\right)\left[\left(y_{0}+4 y_{1}+y_{2}\right)+\left(y_{2}+4 y_{3}+y_{4}\right)+\ldots+\left(y_{n-2}+4 y_{n-1}+y_{n}\right)\right] \\
  &=\left(\frac{\Delta x}{3}\right)\left(y_{0}+4 y_{1}+y_{2}+4 y_{3}+2 y_{4}+\ldots+2 y_{n-2}+4 y_{n-1}+y_{n}\right)
  \end{aligned}
  $$
  - Roughly Speaking, the error, | Simpson's - Exact | , has order of magnitude $(\Delta x)^{4}$
- **Trigonometric Integrals and Substitution**
  - Method A. either $n$ or $m$ is odd:
    to use $\sin ^{2} x+\cos ^{2} x=1$ torewrite the integral
  - Method B. both $m$ and $n$ to be even:
    to use double - angle formulae $\cos ^{2} x=\frac{1+\cos 2 x}{2} ; \quad \sin ^{2} x=\frac{1-\cos 2 x}{2}$
    $\left(\cos 2 x=\cos ^{2} x-\sin ^{2} x=\cos ^{2} x-\left(1-\cos ^{2} x\right)=2 \cos ^{2} x-1\right)$
    $(\sin 2 x=2 \sin x \cos x)$
  | Integral                          | Substitution | Trig identity               |
  | --------------------------------- | ------------ | --------------------------- |
  | $\int \frac{d x}{\sqrt{x^{2}+1}}$ | $x=\tan u$   | $\tan ^{2} u+1=\sec ^{2} u$ |
  | $\int \frac{d x}{\sqrt{x^{2}-1}}$ | $x=\sec u$   | $\sec ^{2} u-1=\tan ^{2} u$ |
  | $\int \frac{d x}{\sqrt{1-x^{2}}}$ | $x=\sin u$   | $1-\sin ^{2} u=\cos ^{2} u$ |
- **Partial Fractions**
	- Definition: rational function as the ratio of two polynomials: 
	  $$
	  \frac{P(x)}{Q(x)}
	  $$
- **Integration by Parts**
  $$
  (u v)^{\prime}=u^{\prime} v+u v^{\prime} \quad \rightarrow \quad u v^{\prime}=(u v)^{\prime}-u^{\prime} v \quad \rightarrow \quad \int u v^{\prime} d x=u v-\int u^{\prime} v d x
  $$
- **Reduction Formulas (Recurrence Formulas)**
  - e.g.3 $\int(\ln x)^{n} d x$
    $$
    \begin{aligned}
    &u=(\ln x)^{n} \rightarrow u^{\prime}=n(\ln x)^{n-1}\left(\frac{1}{x}\right) ; \quad v^{\prime}=d x \rightarrow v=x \\
    
    &\begin{aligned}
    \int(\ln x)^{n} d x&=x(\ln x)^{n}-\int n(\ln x)^{n-1} x\left(\frac{1}{x}\right) d x \\
    &=x(\ln x)^{n}-n\left(x(\ln x)^{n-1}-\int(n-1)(\ln x)^{n-2} x\left(\frac{1}{x}\right) d x=\ldots \ldots\right.
    \end{aligned}
    \end{aligned}
    $$
- **Arc Length**
  $$
  \begin{aligned}
  &d s=\sqrt{(d x)^{2}+(d y)^{2}}=\sqrt{1+(d y/d x)^2}dx \\
  &\int_{P_{0}}^{P_{1}} d s=\int_{a}^{b} \sqrt{1+\left(\frac{d y}{d x}\right)^{2}} d x
  \end{aligned}
  $$
	- Surface Area (surfaces of revolution)
    $$
    \text { Area }=\int 2 \pi y d s
    $$
- **Indeterminate Forms - L’'Hôpital's Rule**
	when $f(a)=g(a)=0(f(a)=g(a)=\infty$ also works $),\left(g^{\prime}(a) \neq 0\right)$
  $$
  \lim _{x \rightarrow a} \frac{f(x)}{g(x)}=\lim _{x \rightarrow a} \frac{\frac{f(x)}{x-a}}{\frac{g(x)}{x-a}}=\frac{\lim _{x \rightarrow a} \frac{f(x)-f(a)}{x-a}}{\lim _{x \rightarrow a} \frac{g(x)-g(a)}{x-a}}=\frac{f^{\prime}(a)}{g^{\prime}(a)}
  $$
- **Geometric Series**
  $$
  \begin{aligned}
  &1+a+a^{2}+a^{3}+\ldots=S \\
  &a+a^{2}+a^{3}+a^{4}+\ldots=a S \\
  &S-a S=1 \quad \rightarrow \quad S=\frac{1}{1-a}
  \end{aligned}
  $$
	- General Power Series
    $$
    \begin{aligned}
    a=-u \quad &\rightarrow \quad \frac{1}{1+u}=1-u+u^{2}-u^{3}+\ldots \\
    a=-u^{2} \quad &\rightarrow \quad \frac{1}{1+u^{2}}=1-u^{2}+u^{4}-u^{6}+\ldots \\
    \left(\frac{1}{1-x}\right)\left(\frac{1}{1-x}\right)&=\left(1+x+x^{2}+\ldots\right)\left(1+x+x^{2}+\ldots\right) \\
    &=1+2 x+3 x^{2}+\ldots
    \end{aligned}
    $$
- **Taylor Series**
  $$
  \begin{aligned}
  &a_{n}=\left(\frac{1}{n !}\right) f^{(n)}(0) \\
  &f(x)=\sum_{n=0}^{\infty} \frac{f^{(n)}(0)}{n !} x^{n}
  \end{aligned}
  $$















