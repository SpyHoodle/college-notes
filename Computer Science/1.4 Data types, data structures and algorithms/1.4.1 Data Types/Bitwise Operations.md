# Bitwise Operations
2022-11-03 | [[1.4.3 Boolean Algebra]]
> **Note:** everything in brackets is the Python bitwise operator for the logic gate.

- *AND* (&) -> Perform and on each of the digits
- *OR* (|) -> Perform or on each of the digits
- *XOR* (^) -> Find the difference (subtraction)
	- You can check if two things are the same by *XOR* and the result will be 0, if not, it will have a value as there is a difference between them
	- XOR can be used to swap two variables without a temp variable
		- X = 1010 (10), Y = 0011 (3)
		- X = X *XOR* Y = 1001 (9)
		- Y = X *XOR* Y = 1010 (10)
		- X = X *XOR* Y = 0011 (3)
		- X = 0011 (3), Y = 1010 (10)
- *NOT* (~)-> Gets you the 1s compliment
	- Add 1, you get the 2s compliment
- **Right shift** (>>) -> Divides by two for every shift
	- Shifts all the digits a number of places to the right
- **Left shift** (<<) -> Multiplies by two for every shift
	- Shifts all the digits a number of places to the left