**Ex 4a.** Solve $\lim\limits_{ x \to +\infty } \frac{1-e^x}{1+e^x}$.
**Ans:** $\lim\limits_{ x \to +\infty } \frac{\frac{1-e^x}{e^x}}{\frac{1+e^x}{e^x}}=\lim\limits_{ x \to +\infty } \frac{\frac{1}{e^x}-1}{\frac{1}{e^x}+1}=\frac{0-1}{0+1}=-1$

**Ex 4b.** Solve $\lim\limits_{ x \to -\infty } \frac{1-e^x}{1+e^x}$.
**Ans:** $\lim\limits_{ x \to -\infty } \frac{\frac{1-e^x}{e^x}}{\frac{1+e^x}{e^x}}=\lim\limits_{ x \to -\infty } \frac{\frac{1}{e^x}-1}{\frac{1}{e^x}+1}=\frac{1-0}{1+0}=1$

**NOTE:** Since $x \to \infty$, $\frac{1}{e^\infty} \to \frac{1}{\infty} \to 0$

# L'Hopital's Rule (Intermediate form)
If the function isn't in the form of $\frac{0}{0}$ or $\frac{\infty}{\infty}$, then the function must be differentiated until that the specified forms are reached.

$$
\begin{aligned}
  &\lim\limits_{ x \to a } \frac{f(x)}{g(x)} = 
  \lim\limits_{ x \to a } \frac{f'(x)}{g'(x)} \\
  &\text{Here, } \\
  &\lim\limits_{ x \to a } f(x) = 0, \infty \\
  &\lim\limits_{ x \to a } g(x) = 0, \infty \\
\end{aligned}
$$

## Conditions
1. $\lim\limits_{ x \to 0 } \frac{\sin{x}}{x}=1$
2. $\lim\limits_{ x \to \infty } \frac{\sin{x}}{x}=0$
3. $\lim\limits_{ x \to 0 } \frac{\sin{ax}}{ax}=1$
4. $\lim\limits_{ x \to 0 }x\sin{\frac{1}{x}}=0$
5. $\lim\limits_{ x \to 0 }\cos{\frac{1}{x}}=0$
6. $\lim\limits_{ x \to 0 }(1+x)^{\frac{1}{x}}=e$
7. $\lim\limits_{ x \to 0 }(1+ax)^{\frac{1}{ax}}=e$
8. $\lim\limits_{ x \to \infty }(1+x)^{\frac{1}{x}}=e$
9. $\lim\limits_{ x \to \infty }(1+ax)^{\frac{1}{ax}}=e$

## $\frac{0}{0}$ Form
**Ex 5a.** Solve $\lim\limits_{ x \to 0 } \frac{\sin{2x}}{x}$.
**Ans:** $\lim\limits_{ x \to 0 } \frac{2\cos{2x}}{1}=\frac{2}{1}=2$

**Ex 5b.** Solve $\lim\limits_{ x \to 1 } \frac{\ln{x}}{x-1}$.
**Ans:** $\lim\limits_{ x \to 1 } \frac{\frac{1}{x}}{1}=\frac{\frac{1}{1}}{1}=1$

**Ex 5c.** Solve $\lim\limits_{ x \to \pi } \frac{\sin{x}}{x-\pi}$.
**Ans:** $\lim\limits_{ x \to \pi } \frac{\cos{x}}{1}=\frac{-1}{1}=-1$

**Ex 5d.** Solve $\lim\limits_{ x \to 3 } \frac{x-3}{3x^2-13x+12}$.
**Ans:** $\lim\limits_{ x \to 3 } \frac{x-3}{(x-3)(6x-13)}=\lim\limits_{ x \to 3 } \frac{1}{6x-13}=\frac{1}{6.3-13}=\frac{1}{5}$

**Ex 5e.** Solve $\lim\limits_{ x \to 0 } \frac{\sin{2x}}{\sin{5x}}$. (To be solved as H/W)

##  $\frac{\infty}{\infty}$ Form
**Ex 6a.** Solve $\lim\limits_{ x \to \infty } \frac{e^{3x}}{x^{2}}$.
**Ans:** $\lim\limits_{ x \to \infty } \frac{3e^{3x}}{2x}=\lim\limits_{ x \to \infty } \frac{9e^{3x}}{2}=\frac{9e^{\infty}}{2}=\infty$

**Ex 6b.** Solve $\lim\limits_{ x \to \infty } \frac{x}{e^x}$. (To be solved as H/W)

##  $\infty$ Form
**Ex 7.** Solve $\lim\limits_{ x \to \infty }(x-\pi)\cot{x}$.
**Ans:** $\lim\limits_{ x \to \infty } \frac{x-\pi}{\tan{x}}=\lim\limits_{ x \to \infty } \frac{1}{\sec^2{x}}=\lim\limits_{ x \to \infty }\cos^2{x}=1$

##  $(\infty\pm\infty)$ or $(\frac{1}{\infty}\pm/\frac{1}{\infty})$ Form
**Ex 8.** Solve $\lim\limits_{ x \to 0 }(\frac{1}{x}-\frac{1}{\sin x})$.
**Ans:** $\lim\limits_{ x \to 0 } \frac{\sin x-x}{x\sin x}=\lim\limits_{ x \to 0 } \frac{\cos x-1}{\sin x+(x\sin x+\cos x)}=1$

##  $0^0$, $\infty^0$, $1^{\infty}$ Form
**Ex 9.** Solve $\lim\limits_{ x \to \infty }\left( 1+\frac{1}{x} \right)^x$.
**Ans**: $$ 
\begin{aligned}
	&\text{let } p=\frac{1}{x} 
	\\
	&\therefore x=\frac{1}{p} 
	\\
	&\text{As }  x\to \infty, p\to \frac{1}{\infty} \to 0 
	\\
	&\therefore \lim\limits_{ p \to 0 }(1+p)^{\frac{1}{p}} 
	\\
	&\text{let } y=(1+p)^{\frac{1}{p}} 
	\\
	&\therefore \lim\limits_{ p \to 0 }y=\lim\limits_{ p \to 0 }(1+p)^{\frac{1}{p}} 
	\\
	&\implies \lim\limits_{ p \to 0 }\ln y=\lim\limits_{ p \to 0 }\ln(1+p)^{\frac{1}{p}} 
	\\
	&\implies \lim\limits_{ p \to 0 } \ln y=\lim\limits_{ p \to 0 } \frac{1}{1+p}
	\\
	&\implies \lim\limits_{ p \to 0 } \ln y=1
	\\
	&\implies \lim\limits_{ p \to 0 } y=e
	\\
	&\therefore \lim\limits_{ x \to 0 } (1+\frac{1}{x})^x=e
\end{aligned}
	$$
**Ex 10.** Solve $\lim\limits_{ x \to 0 }(e^x+x)^{\frac{1}{x}}$. (To be solved as H/W)

**Ex 11.** For, $$
f(x) = \begin{cases}
1+2x &\text{if } -1\leq x\leq0 \\
1-2x &\text{if } 0\leq x\leq{\frac{1}{2}} \\
-1+2x &\text{if } x \geq \frac{1}{2}
\end{cases}
$$
Does $f(x)$ have a limit? If so, find the limits for $f(x)$ as $x\to0$ & $x\to \frac{1}{2}$.
**Ans:**

#### For $x\to0$,
LHL: $\lim\limits_{ x \to 0^+ }(1+2x)=1$
RHS: $\lim\limits_{ x \to 0^- }(1-2x)=1$
Since LHL & RHL are same, limit exists.
$\therefore \lim\limits_{ x \to 0 }f(x)=1$

#### For $x\to \frac{1}{2}$,
LHL: $\lim\limits_{ x \to {\frac{1}{2}}^+ }(1-2x)=0$
RHS: $\lim\limits_{ x \to {\frac{1}{2}}^- }(-1+2x)=0$
Since LHL & RHL are same, limit exists.
$\therefore \lim\limits_{ x \to 0 }f(x)=0$

**Ex 12.** For, $$
f(x)=\begin{cases}
(1+2x)^{\frac{1}{x}} &\text{if } x \neq 0 \\
e^2 &\text{if } x=0
\end{cases}
$$
Find $\lim\limits_{ x \to 0 }f(x)$.
**Ans:** 
LHL: $\lim\limits_{ x \to 0^- }(1+2x)^{\frac{1}{x}}=\lim\limits_{ x \to 0^- }[(1+2x)^{\frac{1}{2x}}]^2=e^2$
RHS: $\lim\limits_{ x \to 0^+ }(1+2x)^{\frac{1}{x}}=e^2$
Since LHL & RHL are same, limit exists.
$\therefore \lim\limits_{ x \to 0 }f(x)=e^2$

## For the following form: $$
|x| = \begin{cases}
x &\text{if } x \geq 0 \\
-x &\text{if } x < 0
\end{cases}
$$ 
**Ex 13.** Solve $\lim\limits_{ x \to 0 } \frac{x}{|x|}$ & show that no limits exist.
**Ans:** $$
f(x) = \frac{x}{|x|} = \begin{cases}
\frac{x}{x} &\text{if } x > 0 \\
\frac{x}{-x} &\text{if } x < 0
\end{cases}
$$
LHL: $\lim\limits_{ x \to 0^- }(\frac{x}{-x})=-1$
RHL: $\lim\limits_{ x \to 0^+ }(\frac{x}{x})=1$
Since LHS $\neq$ RHL, no limits exist.

#### H/W (5 in total)
**Ex 14.** Find the limit for $f(x)=\frac{|x|}{x}$ as $x\to0$.
**Ex 15.** $$f(x)=\begin{cases}
2-x &\text{if } x<1 \\
x^{2}+1 &\text{if } x>1
\end{cases}$$ Find $\lim\limits_{ x \to 1 }f(x)$.
**Ex 16.** $$f(x)=\begin{cases}
3x-1 &\text{if } x<1 \\
3-x &\text{if } x>1
\end{cases}$$ Find $\lim\limits_{ x \to 1 }f(x)$.
