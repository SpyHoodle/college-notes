# Fixed & Floating Point
2022-09-30 Fri | [[1.4.1 Data Types]]

## Fixed Point
- Written in Two's Compliment
- Decimal columns are written as fractions

### Example
| -16 | 8   | 4   | 2   | 1   | .   | $\frac{1}{2}$ | $\frac{1}{4}$ | $\frac{1}{8}$ | $\frac{1}{16}$ |
| --- | --- | --- | --- | --- | --- | ------------- | ------------- | ------------- | -------------- |
| 1   | 1   | 0   | 1   | 1   | .   | 1             | 1             | 1             | 0              |
|     |     |     |     |     |     |               |               |               |                |
- $-16 + (8 + 2 + 1 + \frac{1}{2} + \frac{1}{4} + \frac{1}{8}) = -5\frac{1}{8}$
- A common mistake would be to try and make $+ \frac{1}{8}$ instead of $+ \frac{7}{8}$

## Floating Point
- $\text{Mantissa} \cdot \text{Base}^{\text{Exponent}}$
	- Effectively standard form
	- Store large numbers in less memory
	- The mantissa is a fixed point in Two's Compliment
	- The base would be 2 for binary
	- The exponent is an integer in Two's Compliment