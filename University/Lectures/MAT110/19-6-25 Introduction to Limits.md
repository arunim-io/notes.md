# Limits
**Definition:** If the values of $f(x)$ become arbitrarily close to a single number $l$ as the values of a variable approach to $a$ from both sides of $a$ (left or right), then $l$ is called the limit of $f(x)$.

**Denoted by:** $\lim\limits_{x->a}f(x)=l$

## Right-hand Limits (RHLs)
**Definition:** If the values of $f(x)$ become arbitrarily close to a single number $l$ as the values of a variable approach to $a$ from the right side of $a$, then $l$ is called the right-hand limit (RHL) of $f(x)$.

**Denoted by:** $\lim\limits_{x->a^+}f(x)=l$

## Left-hand Limits (LHLs)
**Definition:** If the values of $f(x)$ become arbitrarily close to a single number $l$ as the values of a variable approach to $a$ from the left side of $a$, then $l$ is called the left-hand limit (LHL) of $f(x)$.

**Denoted by:** $\lim\limits_{x->a^-}f(x)=l$

## Condition for a limit to exist
$$
\lim\limits_{x->a^+}f(x)=\lim\limits_{x->a^-}f(x)=\lim\limits_{x->a}f(x)
$$

**Ex 1a.** Solve $\lim\limits_{x\to_{5}}x^2-4x+3$.
**Ans:** $5^2 - 4.5 + 3 = 8$

**Ex 1b.** Solve $\lim\limits_{ x \to -4 }\frac{{2x + 8}}{x^2 + x -12}$.
**Ans:** $\lim\limits_{ x \to -4 } \frac{{2(x + 4)}}{(x + 4)(X - 3)}=\lim\limits_{ x \to -4 } \frac{2}{x-3}=\frac{2}{-4-3}=-\frac{2}{7}$

## Limits in Infinity
If the values of $f(x)$ eventually gets as close as we like to a number $L$ as $x$ increases without bound, then we can write:
$$
\begin{align}
  \lim\limits_{ x \to +\infty } f(x) = L
  \\
  \text{OR}
  \\
  f(x) \to L &\text{ as } x \to +\infty
\end{align}
$$
Similarly, if the values of $f(x)$ eventually gets as close as we like to a number $L$ as $x$ decreases without bound, then we can write:
$$
\begin{align}
  &\lim\limits_{ x \to -\infty } f(x) = L 
	\\
  &f(x) \to L &\text{ as } x \to -\infty
\end{align}
$$
So, to summarize:
$$
\begin{aligned}
  &\lim\limits_{ x \to +\infty }f(x)=l
  \\
  &\lim\limits_{ x \to -\infty }f(x)=l
  \\
  &\text{Given that } R = (-\infty,+\infty)
\end{aligned}
$$

### Conditions
1. $\lim\limits_{ x \to +\infty }(1+\frac{1}{x})^x=e$
2. $\lim\limits_{ x \to -\infty }(1+\frac{1}{x})^x=e$
3. $\lim\limits_{ x \to \pm \infty }{f(x)}^n={(\lim_{ x \to \pm \infty }f(x))}^n$
4. $\lim\limits_{ x \to \pm \infty }kf(x)=k\lim\limits_{ x \to \pm \infty }f(x)$
5. $\lim\limits_{ x \to \pm \infty }k=k$

**NOTE:** Since $k$ is a constant, the specified limit doesn't have any effect on it.

### Infinite Limits at Infinity
If the values of $f(x)$ increases without bound as $x \to +\infty$ or $x \to \infty$, then we can write:
$$
\begin{aligned}
  &\lim\limits_{ x \to +\infty }f(x)=\pm\infty
  &\lim\limits_{ x \to -\infty }f(x)=\pm\infty
\end{aligned}
$$

**Ex 2.** Solve $\lim\limits_{ x \to +\infty }\left( 1+\frac{1}{2x} \right)^x$.
**Ans:** $\lim\limits_{ x \to +\infty }\left[ \left( 1+\frac{1}{2x} \right)^{2x} \right]^\frac{1}{2}=\sqrt{e}$

**Ex 3.** Solve $\lim\limits_{ x \to -\infty } \frac{{4x^{2}-x}}{2x^3-5}$.
**Ans:** $\lim\limits_{ x \to -\infty } \frac{\frac{4x^2-x}{x^3}}{\frac{2x^3-5}{x^3}}=\lim\limits_{ x \to -\infty } \frac{\frac{4}{x}-\frac{1}{x^2}}{2-\frac{5}{x^3}}=0$
