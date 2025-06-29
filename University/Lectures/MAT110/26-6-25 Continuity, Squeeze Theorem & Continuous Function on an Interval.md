# Continuity
A function, $f(x)$, is said to be continuous at $x=a$, if:
1. $f$ is defined.
2. Both the LHL & RHL exist.
3. Both the limits are equal to each other & to $f(a)$.

So, we can say that:
1. If $f(a)=\lim\limits_{ x \to a^+ }f(x)$ & $f(a)\neq\lim\limits_{ x \to a^- }f(x)$, $f$ is not continuous, but is continuous from the right.
2. If $f(a)\neq\lim\limits_{ x \to a^+ }f(x)$ & $f(a)=\lim\limits_{ x \to a^- }f(x)$, $f$ is not (again) continuous, but is continuous from the left.
3. If $f(a)=\lim\limits_{ x \to a^+ }f(x)=\lim\limits_{ x \to a^- }f(x)$, $f$ is continuous.

**Ex 1.** $$
f(x) = \begin{cases}
  x^2+1 &\text{ if } x>0
  \\
  1 &\text{ if } x=0
  \\
  1+x &\text{ if } x<0
\end{cases}
$$
Find the limit for $f$ as $x\to0$. Is $f$ continuous at $x=0$? 
Ans:
if $x=0$, $f(0)=1$
$\therefore f(x)$ is defined.
LHL: $\lim\limits_{ x \to 0^- }(1+x)=1+0=1$
RHL: $\lim\limits_{ x \to 0^+ }(x^2+1)=0+1=1$
As LHL$=$RHL, $\lim\limits_{ x \to 0^+ }f(x)=1$
As LHL$=$RHL$=f(0)$, $f$ is continuous.

**Ex 2.** $$
f(x) = \begin{cases}
  e^{-\frac{|x|}{2}} &\text{ if } -1<x<0
  \\
  x^2 &\text{ if } 0 \leq x < 2
\end{cases}
$$
Test the continuity for $f$ at $x=0$.
Ans:
if $x=0$, $f(0)=0$
$\therefore f(x)$ is defined.
LHL: $\lim\limits_{ x \to 0^- }e^{-\frac{|x|}{2}}=\lim\limits_{ x \to 0^- }e^{\frac{x}{2}}=e^0=1$
RHL: $\lim\limits_{ x \to 0^+ }x^2=0$
As $f(0)$ is only equal to RHL, $f$ is continuous from the right.

**Ex 3.** $$
f(x) = \begin{cases}
  \frac{|x-3|}{x-3} &\text{ if } x\neq3
  \\
  0 &\text{ if } x=3
\end{cases}
$$
Test the continuity for $f$ at $x=3$. Also, find out its limit as $x\to3$.
Ans:
if $x=3$, $f(3)=0$
$\therefore f(x)$ is defined.
LHL: $\lim\limits_{ x \to 3^- }(-1)=-1$
RHL: $\lim\limits_{ x \to 0^+ }1=1$
As LHL$\neq$RHL, $f$ has no limits.
As LHL$\neq$RHL$\neq f(0)$, $f$ is not continuous.

# Squeeze/Pinching/Sandwich Theorem
Let $f$, $g$ & $h$ be functions satisfying $g(x) \leq f(x) \leq h(x)$, for all values of $x$ in some open interval, containing the number $a$, with one possible exception that the inequalities need not hold at $a$.

If $g$ & $h$ have the same limits, for example $\lim\limits_{ x \to a }g(x)=\lim\limits_{ x \to a }h(x)=L$, then $f$ also has a limit as $x$ approaches $a$, i.e. $\lim\limits_{ x \to a }f(x)=L$.

**Ex 4a.** Prove that $\lim\limits_{ x \to 0 }x\sin(\frac{1}{x})=0$.
Ans: Since $-1 \leq \sin(\frac{1}{x}) \leq 1$,
$\therefore -x \leq \sin(\frac{1}{x}) \leq x$
$\therefore g(x)=-x$
$f(x)=x\sin(\frac{1}{x})$
$h(x)=x$
$\lim\limits_{ x \to 0 }g(x)=\lim\limits_{ x \to 0 }-x=0$
$\lim\limits_{ x \to 0 }h(x)=\lim\limits_{ x \to 0 }x=0$
$\therefore \lim\limits_{ x \to 0 }x\sin(\frac{1}{x})=0$

**Ex 4b.** Prove that $\lim\limits_{ x \to 0 }x\cos(\frac{1}{x})=0$. (To be done as H/W.)

**Ex 5.** Prove that $\lim\limits_{ x \to \infty } \frac{\sin x}{x}=0$.
Ans: Since $-1 \leq \sin x \leq 1$,
$\therefore -\frac{1}{x} \leq \frac{\sin x}{x} \leq \frac{1}{x}$
$\therefore g(x)=-\frac{1}{x}$
$f(x)=\frac{\sin(x)}{x}$
$h(x)=\frac{1}{x}$
$\lim\limits_{ x \to \infty }g(x)=\lim\limits_{ x \to \infty }-\frac{1}{x}=0$
$\lim\limits_{ x \to \infty }h(x)=\lim\limits_{ x \to \infty } \frac{1}{x}=0$
$\therefore \lim\limits_{ x \to \infty } \frac{\sin(x)}{x}=0$

**Ex 6a.** $$
f(x)=\begin{cases}
  x\sin(\frac{1}{x}) &\text{if } x \neq 0 \\
  0 &\text{if } x=0
\end{cases}
$$
Test the continuity for $f$ at $x=0$.
Ans: if $x=0$, $f(0)=0$
$\therefore f(x)$ is defined.
LHL: $\lim\limits_{ x \to 0^- }x\sin(\frac{1}{x})=0$
RHL: $\lim\limits_{ x \to 0^+ }x\sin(\frac{1}{x})=0$
\[Given that $\lim\limits_{ x \to 0 }x \sin(\frac{1}{x})=0$]
As $f(0)=$LHL$=$, $f$ is continuous.

**Ex 6b.** $$
f(x)=\begin{cases}
  x\cos(\frac{1}{x}) &\text{if } x \neq 0 \\
  0 &\text{if } x=0
\end{cases}
$$
Test the continuity for $f$ at $x=0$. (To be done as H/W.)

# Continuous Function on an Interval
A function, $f$, is said to be continuous on a closed interval $[a,b]$ or $a \leq x \leq b$, if:
1. $f$ is continuous on $(a,b)$.
2. $f$ is continuous from the right at $a$. $$\lim\limits_{ x \to a^+ } f(x)=f(a)$$
3. $f$ is continuous from the left at $b$. $$\lim\limits_{ x \to b^+ } f(x)=f(b)$$

**Ex 7a.** $$
\begin{align}
f(x)=x^2 && 1 \leq x \leq 5
\end{align}
$$ Show that $f$ is continuous in the interval $[1,5]$.
Ans: If $x=3$, $f(3)=3^2=9$
$\therefore f$ is continuous on $(1,5)$.
If $x=1$, $f(1)=1^2=1$
RHL: $\lim\limits_{ x \to 1^+ }1^2=1$
$\therefore f$ is continuous to the right at $x=1$.
If $x=5$, $f(1)=5^2=25$
RHL: $\lim\limits_{ x \to 5^+ }5^2=35$
$\therefore f$ is continuous to the left at $x=5$.
$\therefore f$ is continuous on $[1,5]$.

**Ex 7b.** $$
\begin{align}
f(x)=\sqrt{ 9 - x^2 } && -3 \leq x \leq 3
\end{align}
$$ Show that $f$ is continuous in the interval $[-3,3]$.
Ans: If $x=0$, $f(0)=\sqrt{ 9 - 0 }=3$
$\therefore f$ is continuous on $(-3,3)$.
If $x=-3$, $f(-3)=\sqrt{ 9-9 }=0$
RHL: $\lim\limits_{ x \to (-3)^+ }\sqrt{ 9-9 }=0$
$\therefore f$ is continuous to the right at $x=-3$.
If $x=3$, $f(3)=\sqrt{ 9-9 }=0$
RHL: $\lim\limits_{ x \to 3^- }\sqrt{ 9-9 }=0$
$\therefore f$ is continuous to the right at $x=-3$.
$\therefore f$ is continuous on $[-3,3]$.

**Ex 8.** $$
f(x)=\begin{cases}
  \frac{\sin^{2}ax}{x^{2}} &\text{if } x \ne 0 \\
  1 &\text{if } x = 0
\end{cases}
$$ If $a=1$, prove that $f$ is continuous at $x=0$.
Ans: if $x=0$, $f(0)=1$
$\therefore f$ is defined.
LHL: $\lim\limits_{ x \to 0^- } \frac{\sin^{2}ax}{x^2}=\lim\limits_{ x \to 0^- } (\frac{\sin ax}{x})^{2}=\lim\limits_{ x \to 0^- } [(\frac{\sin ax}{x})^{2}a^{2}]=a^{2}$
Since $a=1$, LHL$=1^{2}=1$
RHL: $\lim\limits_{ x \to 0^- } \frac{\sin^{2}ax}{x^2}=a^{2}=1$ 
Since LHL$=$RHL, $f$ is continuous at $x=0$.
