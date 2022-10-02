# Quadratic Equation Solver
2022-09-25 | [[Computer Science/2.2 Problem Solving and Programming/2.2 Problem Solving and Programming]]
- Understand the problem
	$ax^2 + bx + c = 0$

	$x_1 x_2 = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$
	
	$\text{Let } d = b^2 - 4ac$
	$x_1 x_2 = \frac{-b \pm \sqrt{d}}{2a}$

	$d = 0$
	$x_1 = -\frac{b}{2a}$
	$x_2 = x_1$

	$d > 0$
	$x_1 = \frac{-b+\sqrt{d}}{2a}$
	$x_2 = \frac{-b-\sqrt{d}}{2a}$

	$d < 0$
	$\therefore \text{No real solutions}$
- Use test data to check the problem
- Draw a flowchart for the program
- Write the pseudo-code for the program
- Write the actual code

```python
a = float(input("Enter a: "))
b = float(input("Enter b: "))
c = float(input("Enter c: "))
d = b*b - 4*a*c

if d == 0:
    xl = -b/(2*a)
    x2 = x1
    print (x1, x2)
elif d > 0:
    x1 = (-b + d**0.5)/(2*a)
    x2 = (-b - d**0.5)/(2*a)
    print(x1, x2)
else:
    print("There is no real solution")
```
