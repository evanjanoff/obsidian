---
note-type: class-note
tags:
related-concepts: "[[Math]]"
course-name: "[[Calculus 1]]"
---
## Intro to Derivatives
- ### Definition of The Derivative
	- The slope of the tangent line at a point on the function, often noted as $m_{tan}$, is equal to the derivative of the function at that point. The instantaneous rate of change of the punction at a point.
- ### Limit Definition of the Derivative
	- $f^{\prime}\left(x\right)=\lim_{h\to0}\frac{f\left(x+h\right)-f\left(x\right)}{h}$
	- There are many common derivative notations:
		- $f^{\prime}(x)$ - most common, "f prime of x"
		- $D[f(x)]$, $\frac{d}{dx}[f(x)]$, $\frac{df}{dx}$, $\frac{dy}{df}$ and $y^{\prime}$ are other common notations
- ### Basic Derivative Rules
	- Power Rule - $\frac{d}{\mathrm{d}x}\left\lbrack x^{n}\right\rbrack=n\cdot x^{n-1}$
	- Derivative of Sine - $\frac{d}{\mathrm{d}x}\left\lbrack\sin x\right\rbrack=\cos x$
	- Derivative of Cosine - $\frac{d}{\mathrm{d}x}\left\lbrack\cos x\right\rbrack=-\sin x$
- ### Tangent Line Equations
	- $y=f\left(a_{}\right)+f^{\prime}\left(a\right)\left(x-a\right)$
## Properties and Formulas
- ### Differentiability
	- A function $f(a)$ is said to be differentiable at $x=a$ if $f(x)$ is continuous at $x=a$ and $f'(a)$ is defined
		- If a function is not continuous at a point (e.g. point discontinuity or vertical asymptote) it is not differentiable
		- Some functions are continuous but not differentiable
			- For instance if $f'(x)$ would result in a vertical tangent (divide by 0) at $x=a$, the function is not differentiable there
		- Graphically, if there are discontinuities or sharp corners, the function is not differentiable
- ### Derivative of a Constant
	- $D\left\lbrack k\right\rbrack=0$
		- Any constant $k=k\cdot x^0$ therefore $D\left\lbrack k\right\rbrack=\frac{0\cdot k}{x}=0$
- ### Derivative of Constant Multiple
	- $D\left\lbrack k\cdot f\left(x\right)\right\rbrack=k\cdot D\left\lbrack f\left(x\right)\right\rbrack$
- ### Derivative of a Sum
	- $D\left\lbrack f\left(x\right)+g\left(x\right)\right\rbrack=D\left\lbrack f\left(x\right)\right\rbrack+D\left\lbrack g\left(x\right)\right\rbrack$
- ### Derivative of a Difference
	- $D\left\lbrack f\left(x\right)-g\left(x\right)\right\rbrack=D\left\lbrack f\left(x\right)\right\rbrack-D\left\lbrack g\left(x\right)\right\rbrack$
- ### The Product Rule
	- $D\left\lbrack f\left(x\right)\cdot g\left(x\right)\right\rbrack=D\left\lbrack f\left(x\right)\right\rbrack\cdot g\left(x\right)+f\left(x\right)\cdot D\left\lbrack g\left(x\right)\right\rbrack$
- ### The Quotient Rule
	- $\frac{d}{\mathrm{d}x}\left\lbrack\frac{f\left(x\right)}{g\left(x\right)}\right\rbrack=\frac{g\left(x\right)f^{\prime}\left(x\right)-f\left(x\right)g^{\prime}\left(x\right)}{\left\lbrack g\left(x\right)\right\rbrack^2}$
- ### The Power Rule
	- $D\left\lbrack\left\lbrack f\left(x\right)\right\rbrack^{n}\right\rbrack=n\cdot\left\lbrack f\left(x\right)\right\rbrack^{n-1}\cdot f^{\prime}\left(x\right)$
- ### Trig Derivatives
	- $D\left\lbrack\sin x\right\rbrack=\cos x$
	- $D\left\lbrack\cos x\right\rbrack=-\sin x$
	- $D\left\lbrack\tan x\right\rbrack=\sec^2x$
	- $D\left\lbrack\sec x\right\rbrack=\sec x\tan x$
	- $D\left\lbrack\csc x\right\rbrack=-\csc x\cot x$
	- $D\left\lbrack\cot x\right\rbrack=-\csc^2x$
### Higher Order Derivative

| Level          | y-notation | d-notation          | f-notation   | D-notation  |
| -------------- | ---------- | ------------------- | ------------ | ----------- |
| 1st Derivative | $y'$       | $\frac{dy}{dx}$     | $f'(x)$      | $D[f(x)]$   |
| 2nd Derivative | $y''$      | $\frac{d^2y}{dx^2}$ | $f''(x)$     | $D^2[f(x)]$ |
| 3rd Derivative | $y'''$     | $\frac{d^3y}{dx^3}$ | $f'''(x)$    | $D^3[f(x)]$ |
| 4th Derivative | $y^{(4)}$  | $\frac{d^4y}{dx^4}$ | $f^{(4)}(x)$ | $D^4[f(x)]$ |
| nth Derivative | $y^{(n)}$  | $\frac{d^ny}{dx^n}$ | $f^{(n)}(x)$ | $D^n[f(x)]$ |
## The Chain Rule
- ### Basic Functions
	- If: $y=f(u)$ is a composite function where $u$ is a function of $x$
	- Then: $\frac{\mathrm{d}y}{\mathrm{d}x}=\frac{df}{du}\cdot\frac{du}{\mathrm{d}x}$
		- Can also be written as: $y^{\prime}=f^{\prime}\left(u\right)\cdot u^{\prime}$ or $D\left\lbrack y\right\rbrack=f^{\prime}\left(u\right)\cdot D\left\lbrack u\right\rbrack$
- ### Derivative of Exponential Functions
	- The derivative of $e^x$
		- $D[e^x] = e^x$
	- The derivative of $e^u$ if $u$ is a function of $x$
		- $D\left\lbrack e^{u}\right\rbrack=e^{u}\cdot u^{\prime}$
	- The derivative of $a^x$
		- $D\left\lbrack a^{x}\right\rbrack=a^{x}\cdot\ln a$
	- The derivative of $a^u$
		- $D\left\lbrack a^{u}\right\rbrack=a^{u}\ln a\cdot u^{\prime}$
			- where: $u$ is a function of $x$
- ### Derivative of Logarithmic Functions
	- The derivative of $\ln x$
		- $D\left\lbrack\ln x\right\rbrack=\frac{1}{x}$
	- The derivative of $\ln u$
		- $D\left\lbrack\ln u\right\rbrack=\frac{1}{u}\cdot u^{\prime}$
			- where $u$ is a function of $x$
	- The derivative of logarithmic function
		- $D\left\lbrack\log_{a}x\right\rbrack=\frac{1}{x\cdot\ln a}$
			- where: $a\ne1$
	- The derivative of a composite logarithmic function
		- $D\left\lbrack\log_{a}u\right\rbrack=\frac{u^{\prime}}{u\cdot\ln a}$
			- where: $a\ne1$ and $u$ is a function of $x$
- ### Application of Derivatives
	- Vertical Motion
		- if: the function $h(t)$ models the height of a object
		- then: $v(t)=h'(t)$ is the velocity of the object
		- and: $a(t)=h''(t)$ is the acceleration of the object
	- Growth and Decay
		- $f\left(t\right)=Ae^{kt}$ models exponential growth or decay
			- if: $k>0$ the function models growth
			- if: $k<0$ the function models decay
		- therefore: $f'(t)$ measures the instantaneous rate of change at a specific $t$
	- Total and Marginal Costs
		- if: the function $C(x)$ models the total cost of $x$ items
			- the cost of the $n^{th}$ item can be found by subtracting $C(n)-C(n-1)$
			- this marginal cost can also be estimated using $C'(n-1)$
		- $AC\left(x\right)=\frac{C\left(x\right)}{x}$ models the average cost/item for $x$ items
			- therefore: $AC^{\prime}\left(x\right)$ models the rate at which the average cost is changing at a specific item
## Linear Approximation and Differential
- ### Linear Approximation
	- The equation for the tangent line of a function $f(x)$ near $x=a$ is:
		- $L\left(x\right)=f\left(a\right)+f^{\prime}\left(a\right)\left(x-a\right)$
			- After finding this formula, substituting a value of $x$ near $a$ into the formula lets you estimate a value for $f(x)$
- ### Linear Approximation Error
	- $Err=\vert f\left(x_{}\right)-L\left(x\right)\vert$
- ### Differentials
	- The differential of $f$
		- an estimation in the change in a function $f$ with a change in $x$
		- $df=f^{\prime}\left(x\right)\mathrm{d}x$ or $dy=f^{\prime}\left(x\right)\mathrm{d}x$
			- where: $dy$ is an approximation of $\Delta y$ and $dx$ is $\Delta x$
	- Estimating measurement errors
		- $df=f^{\prime}\left(x\right)\mathrm{d}x$
			- where: $da$ is the differential of the function for the measurement, $f'(x)$ is the derivative of the function, and $dx$ is the possible error
- ### Newton's Method
	- The x-intercept of a function $y=f(x)$ can be determined by taking successively closer tangent lines of the function
	- the formula for the next guess is $x_{n+1}=x_{n}-\frac{f\left(x_{n}\right)}{f^{\prime}\left(x_{n}\right)}$
- ### Implicit Differentiation
	- technique for finding the derivative of a dependent variable (like y) with respect to an independent variable (like x) when the variables are intertwined in an equation that's difficult or impossible to solve for y in terms of x.
	- ex: the equation of a circle such as, $x^2+y^2=9$
		- **Differentiate both sides:** Apply the derivative operator d/dx to every term on both sides of the equation. 
			logseq.order-list-type:: number
		- **Apply the Chain Rule to y terms:** Whenever you differentiate a term containing y, you must multiply its derivative by dy/dx (or y'). 
			logseq.order-list-type:: number
		- **Isolate dy/dx:** Rearrange the resulting equation to solve for dy/dx.
			logseq.order-list-type:: number
- ### Logarithmic Differentiation
	- when finding derivative of a function $y=f(x)$ where there are multiple layers of exponents, quotients and products you can simplify the process by taking the natural logarithm of both sides
		- ex: $y=x^x$, take natural log: $lny=xlnx$, find derivative
- ### Derivatives of Inverse Trig Functions
	- $D\left\lbrack\sin^{-1}x\right\rbrack=\frac{1}{\sqrt{1-x^2}}$
	- $D\left\lbrack\sin^{-1}u\right\rbrack=\frac{u'}{\sqrt{1-u^2}}$
	- $D\left\lbrack\cos^{-1}x\right\rbrack=\frac{-1}{\sqrt{1-x^2}}$
	- $D\left\lbrack\cos^{-1}u\right\rbrack=\frac{-u'}{\sqrt{1-u^2}}$
	- $D\left\lbrack\tan^{-1}x\right\rbrack=\frac{1}{1+x^2}$
	- $D\left\lbrack\tan^{-1}u\right\rbrack=\frac{u'}{1+u^2}$
	- $D\left\lbrack\cot^{-1}x\right\rbrack=\frac{-1}{1+x^2}$
	- $D\left\lbrack\cot^{-1}u\right\rbrack=\frac{-u'}{1+u^2}$
	- $D\left\lbrack\sec^{-1}x\right\rbrack=\frac{1}{\left|x\right|\sqrt{x^2-1}}$
	- $D\left\lbrack\sec^{-1}u\right\rbrack=\frac{u'}{\left|u\right|\sqrt{u^2-1}}$
	- $D\left\lbrack\csc^{-1}x\right\rbrack=\frac{-1}{\left|x\right|\sqrt{x^2-1}}$
	- $D\left\lbrack\csc^{-1}u\right\rbrack=\frac{-u'}{\left|u\right|\sqrt{u^2-1}}$
- ### Related Rates in Geometric Situations
	- Implicit differentiation applied to geometric formulas lets us determine to rates of change on the elements of those objects.
	- Can be applied to any geometric formula:
		- [[geometric-formulas.pdf]]