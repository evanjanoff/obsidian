---
note-type: class-note
tags:
related-concepts: "[[Math]]"
course-name: "[[Calculus 1]]"
---
## Intro to Integrals
- ### Area
	- Areas on a graph can be described by functions and determined by applying geometric formulas: [[geometric-formulas.pdf]]
- ### Sigma Notation
	- The sum (or summation) of many numbers can be written using sigma notation
		- $\sum_{k=1}^{n}a_{k}$ where:
			- $\Sigma$ represent a sum
			- $k$ is the index of summation (or counter) and shows the starting value, in this case 1
			- $n$ is the ending value
			- $a_k$ represents the expression being used to determine the numbers being added in the sum (aka the summand)
	- *The Summation of a Constant*
		- If $C$ is a constant and the starting value is 1, $\sum_{k=1}^{n}C=C\cdot n$
	- *Summations of Powers of Consecutive Numbers*
		- $\sum_{k=1}^{n}k=1+2+\cdots+n=\frac{n\left(n+1\right)}{2}$
		- $\sum_{k=1}^{n}k^2=1^2+2^2+\cdots+n^2=\frac{n\left(n+1\right)\left(2n+1\right)}{6}$
		- $\sum_{k=1}^{n}k^3=1^3+2^3+\cdots+n^3=\frac{n^2\left(n+1\right)^2}{4}$
		- $\sum_{k=1}^{n}k^4=1^4+2^4+\cdots+n^4=\frac{n\left(n+1\right)\left(2n+1\right)\left(3n^2+3n-1\right)}{30}$
		- note: these formulas only work if starting value $k=1$
	- *Summation of a Constant Multiple*
		- $\sum_{k=1}^{n}C\cdot a_{k}=C\cdot\sum_{k=1}^{n}a_{k}$
	- *Summation of a Sum of Difference*
		- $\sum_{k=1}^{n}\left(a_{k}\pm b_{k}\right)=\sum_{k=1}^{n}a_{k}\pm\sum_{k=1}^{n}b_{k}$
- ### Area Under a Curve - Riemann Sums
	- When approximating the area between a non-negative function $y=f(x)$ and the x-axis by using $n$ rectangles:
		- The summation $\sum_{k=1}^{n}f\left(x_{k}\right)\cdot\Delta x$ is called the Reimann Sum
		- where: $x_k$ is a value of $x$ in the $k^{th}$ subinterval and $\Delta x$ is the width of that subinterval
## Definite Integrals
- ### Definition
	- The definite integral of a continuous function $f$ over the interval $[a,b]$ is the limit of a Riemann sum as the number of subintervals approaches infinity.
	- This is the net change in $f(x)$ over the interval $[a,b]$ and will be seen graphically as the  area between the curve and the x-axis. Positive values are above the axis and negative below.
	- This equality is shown in integral notation and sigma notation as:
		- $\int_{a}^{b}f\left(x\right)\mathrm{d}x=\lim_{n\to\infty}\sum_{k=1}^{n}f\left(x_{k}\right)\cdot\Delta x$
		- where: $\Delta x=\frac{b-a}{n}$ and $x_{k}=a+\Delta x\cdot k$
- ### Definite Integrals and Reimann Sums
	- Converting integral notation to limit of Reimann sum
		- Find $\Delta x$
		- Use $\Delta x$ to find $x_k$
		- Sub both into sigma notation formula
	- Converting limit of Reimann sum to integral notation
		- Parse the formula to find $\Delta x$ and $f(x_k)$
		- Use those values and the formulas above to find $a$ and $b$.
- ### Properties of the Definite Integral
| Property                                                              | Formula                                                                                                                | In Words                                                                                                          |
| --------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Definite integral when lower and upper bounds are equal               | $\int_{a}^{a}f\left(x\right)\mathrm{d}x=0$                                                                             | When limits of integration are equal, the value of the definite integral is 0.                                    |
| Definite integral when upper and lower bounds are interchanged        | $\int_{b}^{a}f\left(x\right)\mathrm{d}x=-\int_{a}^{b}f\left(x\right)\mathrm{d}x$                                       | When the order of the limits of integration are interchanged, the values of the definite integrals are opposites. |
| Definite integral of a constant function                              | $\int_{a}^{b}kdx=k\left(b-a\right)$                                                                                    | The definite integral of a constant is equal to the constant multiplied by the width of the interval $(b-a)$.     |
| Definite integral of a constant multiple function                     | $\int_{a}^{b}k\cdot f\left(x\right)\mathrm{d}x=k\int_{a}^{b}f\left(x\right)\mathrm{d}x$                                | The constant $k$ can be moved outside, and the definite integral of $f(x)$ is multiplied by $k$.                  |
| Definite integral over a partition of an interval, with $a\le b\le c$ | $\int_{a}^{b}f\left(x\right)\mathrm{d}x+\int_{b}^{c}f\left(x\right)\mathrm{d}x=\int_{a}^{c}f\left(x\right)\mathrm{d}x$ | Adding areas.                                                                                                     |
- ### Properties of Definite Integrals of Combined Functions

| Property                                           | Formula                                                                                                                                                          | In Words                                                                                                            |
| -------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| Definite integral of a sum of two functions        | $\int_{a}^{b}\left\lbrack f\left(x\right)+g\left(x\right)\right\rbrack\mathrm{d}x=\int_{a}^{b}f\left(x\right)\mathrm{d}x+\int_{a}^{b}g\left(x\right)\mathrm{d}x$ | The definite integral of a sum of two functions is the sum of the definite integral of the functions.               |
| Definite integral of a difference of two functions | $\int_{a}^{b}\left\lbrack f\left(x\right)-g\left(x\right)\right\rbrack\mathrm{d}x=\int_{a}^{b}f\left(x\right)\mathrm{d}x-\int_{a}^{b}g\left(x\right)\mathrm{d}x$ | The definite integral of a difference of two functions is the difference of the definite integral of the functions. |
- ### Comparison Properties
	- *Comparing Two Functions*
		- If $f(x)\le g(x)$ on $[a,b]$ then $\int_{a}^{b}f\left(x\right)\mathrm{d}x\le\int_{a}^{b}g\left(x\right)\mathrm{d}x$.
	- *Bounds on the Value of a Definite Integral*
		- If $m=$ the min value of $f(x)$ on $[a,b]$
		- And, $M=$ the max value of $f(x)$ on $[a,b]$.
		- Then, $m\le f(x) \le M$ for every value $f(x)$ on the interval $[a,b]$.
		- Therefore $m\left(b-a\right)\le\int_{a}^{b}f\left(x\right)\mathrm{d}x\le M\left(b-a\right)$.
## Antiderivatives
- $F(x)$ is an antiderivative of $f(x)$ if $F'(x)=f(x)$.
- ### The 1st Fundamental Theorem of Calculus
	- Let $F(x)$ be an antiderivative of $f(x)$, meaning $F'(x)=f(x)$.
	- Then, $\int_{a}^{b}f\left(x\right)\mathrm{d}x=F\left(b\right)-F\left(a\right)$, which means we evaluate the antiderivative at the endpoints, then subtract.
	- This can be shown with the notation $F\left(x\right)\vert_{a}^{b}=F\left(b\right)-F\left(a\right)$.
- ### The 2nd Fundamental Theorem of Calculus
	- Let $f(x)$ be a continuous function on the closed interval $[a,b]$ with $a\le x \le b$.
	- Let $F\left(x\right)=\int_{a}^{x}f\left(t\right)\mathrm{d}t$. Then , $F^{\prime}\left(x\right)=\frac{d}{\mathrm{d}x}\int_{a}^{x}f\left(t\right)\mathrm{d}t=f\left(x\right)$.
- ### Indefinite Integrals
	- Another name for an antiderivative.
	- The indefinite integral of a function $f(x)$ is the collection of functions whose derivatives are equal to $f(x)$.
	- *Notation*
		- If $F'(x)=f(x)$, then we write $\int f\left(x\right)\mathrm{d}x=F\left(x\right)+C$, where $C$ is an arbitrary constant (usually 0?).
		- Notice, same symbol as a definite integral with out starting and ending values.
- ### The Power Rule
	- *Power Rule for Antiderivatives*
		- $\int x^{n}dx=\frac{1}{n+1}\cdot x^{n+1}+C,n\ne-1$
			- Note: if $n=-1$ use natural logarithm rule below.
	- *Antiderivative of a Constant*
		- $\int kdx=kx+C$
	- *Natural Logarithm Rule*
		- $\int\frac{1}{x}\mathrm{d}x=\ln\left|x\right|+C, x\ne0$
- ### Properties of Antiderivatives
	- *Antiderivative of a Constant Multiple of a Function*
		- $\int k\cdot f\left(x\right)\mathrm{d}x=k\cdot\int f\left(x\right)\mathrm{d}x$
	- *Antiderivative of a Sum of Functions*
		- $\int\left\lbrack f\left(x\right)+g\left(x\right)\right\rbrack\mathrm{d}x=\int f\left(x\right)\mathrm{d}x+\int g\left(x\right)\mathrm{d}x$
	- *Antiderivative of a Difference of Functions*
		- $\int\left\lbrack f\left(x\right)-g\left(x\right)\right\rbrack\mathrm{d}x=\int f\left(x\right)\mathrm{d}x-\int g\left(x\right)\mathrm{d}x$
	- Note: It is helpful to rewrite radicals and powers in exponential form to make them easier to work with (i.e. $x^{-1}$ and $x^{\frac{1}{2}}$).
- ### Antiderivatives of Trig Functions
	- $\int\sin xdx=-\cos x+C$
	- $\int\cos xdx=\sin x+C$
	- $\int\sec^2xdx=\tan x+C$
	- $\int\csc^2xdx=-\cot x+C$
	- $\int\sec x\tan xdx=\sec x+C$
	- $\int\csc x\cot xdx=-\csc x+C$
- ### Antiderivatives of Exponential Functions
	- $\int e^{x}dx=e^{x}+C$
	- $\int a^{x}dx=\frac{a^{x}}{\ln a}+C$
	- $\int e^{kx}dx=\frac{1}{k}e^{kx}+C$ where $k$ is a constant
- ### Using u-Substitution to Reverse the Chain Rule
	- Used to find the antiderivative of a composite function.
- ### Differential Equations
	- An equation that relates to one or more function and their derivatives.
	- To solve a differential equation in the form $y'=f(x)$, find the antiderivative of $f(x)$, which can be written as $F\left(x\right)=\int f\left(x\right)\mathrm{d}x$.
	- The **general solution** is $y=F(x)+C$.
	- The **particular solution** is one that doesn't contain a general constant. Instead a point on the function is passed to the solution to solve for $C$.
## The Fundamental Theorem of Calculus
- To find the exact area under a function over a given interval $[a,b]$:
	- First, evaluate the indefinite integral of the function.
	- Then, apply the 1st Fundamental Theorem over the given interval.
- ### The Area Between 2 Curves That Don't Intertwine
	- If you have 2 curves, $y=f(x)$ and $y=g(x)$, and $f(x) \ge g(x)$ on the interval $[a,b]$
	- Then, the area between the 2 curves can be found with:
		- $Area=\int_{a}^{b}\left\lbrack f\left(x\right)-g\left(x\right)\right\rbrack\mathrm{d}x$
- ### The Area Between 2 Curves Using Horizontal Subrectangles
	- In some cases it makes more sense to calculate the area between 2 curves horizontally rather than vertically.
	- If you have 2 curves, $x=h(y)$ and $x=k(y)$, and $h(y) \ge k(y)$ on the interval $[c,d]$
	- The, the area between the 2 curves can be found with:
		- $Area=\int_{c}^{d}\left\lbrack h\left(y\right)-k\left(y\right)\right\rbrack\mathrm{d}y$
- ### Average Value of a Function
	- If $f(x)$ is continuous on the interval $[a,b]$, then the average value of the function is:
		- $\frac{1}{b-a}\int_{a}^{b}f\left(x\right)\mathrm{d}x$
- ### The Mean Value Theorem for Integrals
	- If $f(x)$ is continuous on interval $[a,b]$ there is at least one value $c$ such that:
		- $f\left(c\right)=\frac{1}{b-a}\int_{a}^{b}f\left(x\right)\mathrm{d}x$
- ### Table of Integrals
	- A broader selection of antiderivatives can be found here:
		- [[table-of-integrals.pdf]]
- ### Approximating Definite Integrals
	- *Trapezoidal Rule*
		- $\int_{a}^{b}f\left(x\right)\mathrm{d}x$ can be approximated by the sum:
			- $\frac{\Delta x}{2}\left\lbrack f\left(x_0)+2f\left(x_1\right)+2f\left(x_2\right)+\cdots+2f\left(x_{n-1}\right)+f\left(x_{n}\right)\right\rbrack\right.$
		- where $\Delta x=\frac{b-a}{n}$ and each $x$ is an endpoint of an evenly space subinterval between $a$ and $b$.
	- *Simpson's Rule*
		- The value of $\int_{a}^{b}f\left(x\right)\mathrm{d}x$ is approximated by:
			- $\frac{\Delta x}{3}\left\lbrack f\left(x_0)+4f\left(x_1\right)+2f\left(x_2\right)+4f\left(x_3\right)+2f\left(x_4\right)+\cdots+2f\left(x_{n-2}\right)+4f\left(x_{n-1}\right)+f\left(x_{n}\right)\right\rbrack\right.$
			- where $\Delta x=\frac{b-a}{n}$ and each $x$ is an endpoint of an evenly space subinterval between $a$ and $b$.
			- Note: $n$ must be even.