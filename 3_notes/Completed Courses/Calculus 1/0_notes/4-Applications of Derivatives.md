---
note-type: class-note
tags:
related-concepts: "[[Math]]"
course-name: "[[Calculus 1]]"
---
## Maximums and Minimums
- **Critical Numbers**
	- A value of $c$ in the domain of $f(x)$ for which $f'(c)=0$ or is undefined, provided that $f(c)$ is defined
	- May indicate a local or global min or max value
	- Workflow:
		- Find domain of $f(x)$
		- Take derivative of $f(x)$
		- Determine where $f'(x)$ is undefined, if $f(x)$ is defined at that value, it is a critical number
		- Solve $f'(x)=0$, if $f(x)$ is defined at that value, it is critical number
- **Finding Maximums and Minimums of a Function**
	- Workflow:
		- Find the critical numbers as per above
		- Substitute critical numbers into original formula to check for extraneous solutions and find coordinates of possible max/min on graph
- **Extreme Value Theorem**
	- If a function is continuous on a closed interval $[a,b]$, it will have global max and min values on that interval
## Mean Value Theorem
- **Rolle's Theorem**
	- Let $f(x)$ be continuous on the closed interval $[a,b]$ with $f(a)=f(b)$, and differentiable on the open interval $(a,b)$.
	- Then, there is at least one value of $c$ between $a$ and $b$ for which $f'(c)=0$.
	- Workflow:
		- Determine if function $f(x)$ is continuous over interval $[a,b]$
		- Determine if function $f(x)$ is differentiable over interval $(a,b)$
		- Determine if $f(a)=f(b)$
		- Solve $f'(x)=0$, only answers on interval $(a,b)$ are correct
- **Mean Value Theorem for Derivatives**
	- Let $f(x)$ be continuous on the closed interval $[a,b]$, and differentiable on the open interval $(a,b)$.
	- Then, there is at least one value of $c$ between $a$ and $b$ for which $f^{\prime}\left(c\right)=\frac{f\left(b\right)-f\left(a\right)}{b-a}$
	- Workflow:
		- Determine if function $f(x)$ is continuous over interval $[a,b]$
		- Determine if function $f(x)$ is differentiable over interval $(a,b)$
		- Solve MVT formula above to find $f'(c)$
		- Find derivative $f'(x)$, set $f'(x)=f'(c)$ and solve for $x$
## The Shape of Derivatives
- Sketching $f'(x)$ from values of $f(x)$
	- if $f(x)$ is increasing at $x=a$, then $f^{\prime}\left(a\right)>0$
	- if $f(x)$ is decreasing at $x=a$, then $f^{\prime}\left(a\right)<0$
- Sketching $f(x)$ from values of $f'(x)$
	- If $f'(x)>0$ on an interval, then $f(x)$ is increasing on that same interval.
	- If $f'(x)<0$ on an interval, then $f(x)$ is decreasing on that same interval.
	- If $f'(x)$ changes directions at a point where $f'(x)=0$ there is a local min or max there.
- Concavity
	- If $f''(x)>0$ on an interval, then the graph of $f(x)$ is concave up on the same interval.
	- If $f''(x)<0$ on an interval, then the graph of $f(x)$ is concave down on the same interval.
	- **Inflection Points**
		- Points where function shifts between concave up and down, found at points where $f''(x)=0$ or is undefined as long as $f(x)$ is defined at that point.
- **Second Derivative Test**
	- Suppose $f'(c)=0$ (definition of Critical Numbers), which means $f(x)$ has a horizontal tangent at $x=c$
		- If $f''(c)<0$, $f(x)$ is concave down around $c$, there is a local max
		- If $f''(c)>0$, $f(x)$ is concave up around $c$, there is a local min
		- If $f''(c)=0$, the test is inconclusive
	- Workflow:
		- Find solve $f'(x)$ to find critical numbers.
		- Substitute into $f''(x)$ to determine if convex up (min) or down (max).
		- Sub back into $f(x)$ to find values.
## Asymptotic Behavior of Functions
- Behavior of limits as they approach $\pm\infty$
	- [[limit-cheatsheet.pdf]]
- Horizontal Asymptotes and Limits
	- The graph of $f(x)$ has a horizontal asymptote $y=c$ if either $\lim_{x\to\infty}f\left(x\right)=c$ or $\lim_{x\to-\infty}f\left(x\right)=c$
- Vertical Asymptotes and Limits
	- The graph of $f(x)$ has a vertical asymptote $x=a$ if either $\lim_{x\to a^{-}}f\left(x\right)=\pm\infty$ or $\lim_{x\to a^{+}}f\left(x\right)=\pm\infty$
	- Refer to [[finding-limit-flowchart.jpg]] for steps to find limit
- Other Asymptotes
	- Asymptotes can also exist as Slant (Oblique) or non-linear styles
		- Find by polynomial long division
- **Graphing a Function Workflow**
	- Given a function $f(x)$
		- Find $f'(x)$ and $f''(x)$
		- From the original function:
			- Find the domain of the function
			- Determine if there are any asymptotes
			- Find x and y intercepts
		- Find all critical numbers of $f'(x)$, i.e. values of $x$ within the domain of $f(x)$ where $f'(x)=0$ or is undefined.
		- Find all values where $f''(x)=0$ or is undefined.
		- Form a combined sign graph for $f'(x)$ and $f''(x)$ to determine where the graph is increasing (intervals where $f'(x)$ is positive), decreasing (intervals where $f'(x)$ is negative), concave up (intervals where $f''(x)$ is positive), concave down (intervals where $f'(x)$ is negative).
		- Identify local extreme points (points where $f'(x)$ changes between positive and negative) and inflection points (points where $f''(x)$ changes between positive and negative).
		- Graph the function.
## L'Hopital's Rule
- If $\lim_{x\to a}\frac{f\left(x\right)}{g\left(x\right)}$ is indeterminate in the form $\frac{0}{0}$ or $\frac{\infty}{\infty}$:
	- Then you can find the limit by taking the derivatives of both $f(x)$ and $g(x)$