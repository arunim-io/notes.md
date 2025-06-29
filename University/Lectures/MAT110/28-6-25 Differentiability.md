We know that for $y=f(x)$,
$$
\begin{align}
 \frac{dy}{dx}=\frac{d}{dx}f(x) \\
 \implies y' = f'(x)
\end{align}
$$
So, the derivative of $f(x)$ is:
$$f'(x)=\lim\limits_{ h \to 0 } \frac{f(x+h)-f(h)}{h}$$

# Derivative of $f(x)$ at $x=a$

Let the function $f(x)$ be defined at $x=a$, so that $f'(a)=\lim\limits_{ h \to 0 } \frac{f(a+h)-f(h)}{h}$ can be called the **derivative** of $f(x)$ at $x=a$, provided that the limit exists.
![[diffrentiability-graph.drawio.svg]]
## Left-hand Derivative (LHD)

$$Lf'(a)=\lim\limits_{ h \to 0^- } \frac{f(a+h)-f(h)}{h}$$

## Right-hand Derivative (RHD)

$$Rf'(a)=\lim\limits_{ h \to 0^+ } \frac{f(a+h)-f(h)}{h}$$

# Differentiable function

A function is said to be differentiable at $x=a$ if the derivative exists, such that:
1. $f(x)$ is continuous.
2. LHD = RHD.

**NOTE:** In questions regarding differentiable functions, you will need to check the function's continuity to find out its differentiability.

**Ex 1.** Find the derivative of $f(x)=\sin x$ using limit definition (or 1st principle of derivative forms).
**Ans:** $$
\begin{align}
 f'(x)
 & = \lim\limits_{ h \to 0 } \frac{\sin(x+h)-\sin x}{h} \\
 & = \lim\limits_{ h \to 0 } \left[ \frac{1}{h}.2\cos\left( \frac{x+h+x}{2} \right)\sin\left( \frac{x+h-x}{2} \right) \right] \\
 & = \lim\limits_{ h \to 0 } \left[ 2\cos\left( x+\frac{h}{2} \right). \frac{1}{h}\sin\left( \frac{h}{2} \right) \right] \\
 & = \lim\limits_{ h \to 0 } 2\cos\left( x+\frac{h}{2} \right). \lim\limits_{ h \to 0 } \left[ \frac{1}{h}\sin \frac{h}{2} \right] \\
 & = 2\cos x . \frac{1}{2}\lim\limits_{ h \to 0 }\left[ \frac{\sin \frac{h}{2}}{\frac{h}{2}} \right] \\
 & = 2\cos x. \frac{1}{2}.1 \\
 & = \cos x
\end{align}
$$

**Ex 2.** Find the derivative of $f(x)=\cot x$ using limit definition.

$$
f'(x)\begin{align}
 & = \lim\limits_{ h \to 0 } \frac{\cot (x + h) - \cot x}{h} \\
 & = \lim\limits_{ h \to 0 } \left[ \frac{1}{h}\left( \frac{\cos (x+h)}{\sin(x+h)}-\frac{\cos x}{\sin x} \right) \right] \\
 & = \lim\limits_{ h \to 0 } \left[ \frac{1}{h}\left( \frac{\sin x \cos(x+h)-\cos x\sin(x+h)}{\sin x\sin(x+h)} \right) \right] \\
 & = \lim\limits_{ h \to 0 } \left[ \frac{-\sin h}{h\sin x\sin(x+h)} \right] \\
 & = -\lim\limits_{ h \to 0 } \frac{\sin h}{h} . \lim\limits_{ h \to 0 } \frac{1}{\sin x\sin(x+h)} \\
 & = -1. \frac{1}{\sin ^{2}x} \\
 & = -\csc^2 x
\end{align}
$$

**Ex 3.** In $f(x)=x^{2}+2$, is $f(x)$ continuous & differentiable at $x=2$?

**Ans:** $$
\begin{align}
 & f(1)=1^2+2 = 3 \\
 & LHL=\lim\limits_{ x \to 1^- } f(1)=3 \\
 & RHL=\lim\limits_{ x \to 1^+ } f(1)=3 \\
 & \therefore f \text{ is continuous \& defined.} \\
 & LHD=Lf'(1)=\lim\limits_{ h \to 0^- } \frac{f(h+1-f(1))}{h} \\
 & = \lim\limits_{ h \to 0^- } \frac{(h+1)^2+2-3}{h} \\
 & = \lim\limits_{ h \to 0^- } h+2 \\
 & = 3 \\
 & RHD=Rf'(1)=3 \\
 & \text{Since } LHD=RHD, f(x) \text{ is differentiable at} x=1.
\end{align}
$$

**Ex 4.** For, $$
f(x)=\begin{cases}
  x^2\sin(\frac{1}{x}) &\text{if } x \neq 0 \\
  0 &\text{if } x=0
\end{cases}
$$ Test its continuity at $x=0$.

**Ex 5.** $$
f(x) = \begin{cases}
x^2 & \text{if } x \leq 1 \\
\sqrt x  & x > 1
\end{cases}
$$ Is it differentiable at $x=1$?

**Ex 6.** Check the differentiability of the function, $f(x)=|x-1|+|x+3|$, at (1) $x=1$ & (2) $x=-3$.

**Ans:**  
1. $$
\begin{align}
 & f(1)=2+2=4 \\
 & LHL = 4 \\
 & RHL = 2+2=4 \\
 & LHD = \lim\limits_{ h \to o^- } \frac{4-4}{h}=0 \\
 & RHD = \lim\limits_{ h \to 0^+ } \frac{2(h+1)+2-4}{h}=2 \\
 & \text{Since } LHD \neq RHD, f(x) \text{ isn't differentiable at } x=1. 
\end{align}
$$
2. $$
\begin{align}
 & f(-3)=-2(-3)-2=4 \\
 & LHL = 4 \\
 & RHL = 4 \\
 & LHD = \lim\limits_{ h \to o^- } \frac{-2(h-3)-2-4}{h}=-2 \\
 & RHD = \lim\limits_{ h \to 0^+ } \frac{4-4}{h}=0 \\
 & \text{Since } LHD \neq RHD, f(x) \text{ isn't differentiable at } x=-3. 
\end{align}
$$