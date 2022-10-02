# Signed Numbers
2022-09-29 Thu | [[1.4.1 Data Types]]

## Sign and Magnitude
- **Sign** -> +/-
- **Magnitude** -> 255
- The most important bit becomes the sign 
	- Most important bit means the one which will have the biggest effect if it's lost i.e. 128 if lost would change the number a lot but loosing 1 wouldn't
	- 0 -> +
	- 1 -> -
- This does not work for calculations

## Two's Compliment
- Used for calculations
- The most important bit becomes negative
	- 128 -> -128
- $\text{2s compliment} = \text{1s compliment} + 1$
	- Flip all the bits, add one and then you have the negative number