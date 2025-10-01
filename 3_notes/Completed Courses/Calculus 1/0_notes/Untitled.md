---
note-type: class-note
tags:
related-concepts: "[[Math]]"
course-name: "[[Calculus 1]]"
---
- ## Average Rate of Change
		- The slope of a line tells us the average rate of change of that line
		- Given function $y=f(x)$ and an interval $[a,b]$ the average rate of change over the interval is the **Secant Line** between those points
			- $\frac{\Delta f\left(x\right)}{\Delta x}=\frac{f\left(b\right)-f\left(a\right)}{b-a}$
- ## Instantaneous Rate of Change
		- The slope of the tangent line shows the rate of change at a specific point which can be inferred from applying the ((67ed78f7-8050-4266-8be0-a2c294444c91)) over a very small interval.
	- ### Limits
		- When attempting to find $\lim_{x\to a}f(x)$ follow this ((67f9568b-b672-452a-98a7-fa926f1af969))
		- **Limit Properties**
			- Some important limit properties can be seen here:
				- ((681bebb5-4d01-4947-8b69-03ddf0172dab))
			- **Squeeze Theorem**
				- Suppose $g\left(x\right)\le f\left(x\right)\le h\left(x\right)$ for $x$ values near $x=a$
					- if $\lim_{x\to a}g\left(x\right)=\lim_{x\to a}h\left(x\right)=L$
					- then $\lim_{x\to a}f\left(x\right)=L$
		- **Formal Definition of a Limit**
			- $\lim_{x\to a}f\left(x\right)=L$ means that for every given $\epsilon>0$ there exists $\delta>0$ such that:
				- if $x$ is within $\delta$ units of $a$ (and $x\ne a$), then $f(x)$ is within $\epsilon$ units of $L$
				- Meaning $|f(x)-L|<\epsilon$ whenever $0<|x-a|<\delta$
					- Recall: $|x|<a$ is equivalent to $-a<x<a$ for any positive value of $a$
	- ### Continuous Functions
		- **Definition**
			- A function $f(x)$ is continuous at $x=a$ if $f(a)$ is defined and $\lim_{x\to a}f\left(x\right)=f\left(a\right)$
		- **Intermediate Value Theorem**
			- Suppose $f(x)$ is a continuous function on the closed interval $[a,b]$. Let $V$ be a value between $f(a)$ and $f(b)$. Then, there is at least one value of $c$ between $a$ and $b$ such that $f(c)=V$.
-