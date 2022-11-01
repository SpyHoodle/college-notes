# Normalised Floating Point
2022-10-04 | [[1.4.1 Data Types]]

- **Normalised** -> Optimised form
	- Maximised range
		- Affected by exponent
	- Maximised precision
		- Affected by mantissa
	- More precise numbers can be represented by a bigger mantissa and a smaller exponent
	- Most signifiant bit and second significant bit of the mantissa must be different
		- $0.1010$ and $1.0110$ are valid but $1.1101$ is not valid