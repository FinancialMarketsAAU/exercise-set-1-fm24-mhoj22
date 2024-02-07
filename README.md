# Exercise Set 1 for the Financial Markets Course

$\textbf{Exercise 1}$

Proving the first that strictly preffered denoted $succ$ is both irreflexive and transitive if $\succsim$ is rational. 

Using the strong preference relation we have $x\succ x \Leftrightarrow x\succsim x$ but not $x\succsim x$, which is a direct contradiction.


Now to the transitive part let the following be given: $x\succ y$ andd $y \succ z$. Thus giving the relations:

$x \succ y \Leftrightarrow x \succsim y$ but not $y \succsim x$


$y \succ z \Leftrightarrow y \succsim z$ but not $z \succsim y$


Thus we must have $x\succsim y \succsim z$ but not $z \succsim y \succsim x$ implying the transitivity that: $(x\succ y$ and $y \succ z) \Leftrightarrow$ $x\succ y \succ z$.


Now it needs to be shown that $\sim$ is reflexive that is $x\sim x \forall x \in X$. This happens since: $\forall x \in X: x\sim x \Leftrightarrow x\succsim x and x \succsim x$ which holds for all given $x$ thus the indifference relation is reflexive.

It is also transitive since $y\sim x$ and $x\sim z$ gives:

$y \sim x \Leftrightarrow y \succsim x$ and $x\succsim y$
$x \sim z \Leftrightarrow x \succsim z$ and $z\succsim x$


Which if $\succsim$ is rational would imply that: $z\succsim x \succsim y$ and $y\succsim x \succsim z$ which in turn would imply: $z\succsim y$ and $y\succsim z$ and thus:

$y\sim x$ and $x \sim z \Leftrightarrow y \sim z$.

Obviously $\sim$ is also symmetric since $y\sim x \Leftrightarrow y \succsim x$ and $x \succsim y \Leftrightarrow x \succsim y$ and $y \succsim x \Leftrightarrow x \sim y.$



Part three of the proof is to show that if $x \succ y \succsim z$ then $x\succ z$. Since $x \succ y \Leftrightarrow x \succsim y$ and not $y\succsim x$.

And since we dont have $y\succsim x$ and we have $y\succsim z$ this implies that we can not have $z\succsim x$. The other way we also must have $x \succsim y \succsim z$ implying $x \succ z$.



$\textbf{Exercise 2}$

The lexicographic preference relation $\succsim$ over $R^2$ is defined by $(x_1,x_2)\succsim (y_1,y_2)$ if $x_1>y_1$ or $x_1=y_1$ and $x_2 \geq y_2$.


To show that this relation is transitive assume that: $(x_1,x_2) \succsim (y_1,y_2)$ and $(y_1,y_2) \succsim (z_1,z_2)$:

This gives:

$(x_1,x_2)\succsim (y_1,y_2) \Leftrightarrow$ $x_1>y_1$ or $x_1=y_1$ and $x_2 \geq y_2$.

$(y_1,y_2)\succsim (z_1,z_2) \Leftrightarrow$ $y_1>z_1$ or $y_1=z_1$ and $y_2 \geq z_2$.


If it is the case that $x_1>y_1$ we must also have that $x_1>y_1>z_1$. If $x_1=y_1$ and $x_2 \geq y_2$ and that $x_2\geq y_2\geq z_2$ if we also had that $x_1=y_1=z_1$. Thus we can combine the cases to see that $\succsim$ is transitive for all cases i.e. $x_1=y_1=z_1$, $x_1>y_1=z_1$, $x_1>y_1>z_1$, $x_1=y_1>z_1$.




To show that the lexicogrpahic preference relation is not continuous consider the sequence:

$(x_1^n,x_2^n)=(1-1/n,1)$ and $(y_1,y_2)=(1,0)$. Since we have that $(1-1/n,1)\precsim (1,0)$ for all $n$ we should have that $x\precsim y$, but since $x=\lim_{n\rightarrow \infty} (x_1^n,x_2^n)=(1,1)$ we have that $x=(1,1) \succsim y=(0,1)$ and thus the preference relation is not continuous.



$\textbf{Exercise 3}$

The utility function known as the constant elasticity of substitution utility function is given by 

$$U(x)=[\alpha_1x_1^\rho+\alpha_2x_2^\rho]^{1/\rho}$$

in a two-commodity world.


i) First it will be shown that when $\rho=1$
 the indifference curves become linear:

 The utility function then takes the form:

$$U(x)=[\alpha_1x_1+\alpha_2x_2]$$

For a given level of utility $k$ this becomes:

$$k=\alpha_1x_1+\alpha_2x_2.$$

Solving for $x_2$ we get: $x_2=\frac{k}{\alpha_2}-\frac{\alpha_1}{\alpha_2}x_1$. Thus for $\rho=1$ we get linear indifference curves at a given level of utility $k$ where the slope of the indifference curve is $-\frac{\alpha_1}{\alpha_2}$.



ii) Showing that as $\rho \rightarrow 0$ the utility function comes to represent the same preferences as the Cobb-Douglas function: $U(x)=x_1^{\alpha_1}+x_2^{\alpha_2}$.


We apply a monotonic tranformation $\ln(x)$ thus getting $\ln(U(x))=\frac{\ln([\alpha_1x_1^\rho+\alpha_2x_2^\rho])}{p}$$

We now use L'hopital as $n\rightarrow \infty$: $\lim_{n\rightarrow \infty}\frac{\alpha_1x_1^\rho \ln(x_1)+\alpha_2x_2^\rho \ln(x_2)}{\alpha_1x_1^\rho+\alpha_2x_2^\rho}=\frac{\alpha_1 \ln(x_1)+\alpha_2 \ln(x_2)}{\alpha_1+\alpha_2}=\frac{\ln(x_1^{\alpha_1}x_2^{\alpha_2})}{\alpha_1+\alpha_2}$

Using the monotonic transformation $e^x$ we see that $e^{\frac{1}{\alpha_1+\alpha_2}}x_1^{\alpha_1}x_2^{\alpha_2}$ is of the same form as the cobb-douglas utility function and we could even devide by the positive number $e^{1/(\alpha_1+\alpha_2)}$ to get exactly the form above, since this would also be a monotonic transformation.


iii) Now to plot the lower contour set for 

$$U(x)=[\alpha_1x_1^\rho+\alpha_2x_2^\rho]^{1/\rho}$$

When $U(x)=1$ and $\rho=1/2$ and $\alpha_1=\alpha_2=1$:

$$1=[x_1^{1/2}+x_2^{1/2}]^{2}$$

$$(1-x_1^{1/2})^2=x_2$$

Using this the following Julia code should produce the lower contour set:

#Julia code
using Plots
X = 0.1:0.005:0.35     
α = 0.5

f(x) = (1-x^(1/2))^2

y=[f(x) for x in X]

plot(X,y, fillrange = zeros(size(X,1),1), 
fillalpha = 0.3, label="{y∈R²:y≺x}")

plot!(X,y,line = :dash, color = :red, 
linewidth = 3, label="{y∈R²:y~x}")


iv)

Here are indifference curves for $k=0.4,0.5$ and $0.6$: $\rho=1/2$ and $\alpha_1=\alpha_2=1$:

#Julia code
using Plots
X = 0.1:0.005:0.35
K = 0.4:0.1:0.6
α = 1/2

f(x,k) = (k^α-x^α)^(1/α)

y=[f(x,k) for x in X, k in K]

plot(X, y, label=["K=0.4" "K=0.5" "K=0.6"])


Now it will be plotted for $\rho=2$:

#Julia code
using Plots
X = 0.1:0.005:0.35
K = 0.4:0.1:0.6
α = 2

f(x,k) = (k^α-x^α)^(1/α)

y=[f(x,k) for x in X, k in K]

plot(X, y, label=["K=0.4" "K=0.5" "K=0.6"])











