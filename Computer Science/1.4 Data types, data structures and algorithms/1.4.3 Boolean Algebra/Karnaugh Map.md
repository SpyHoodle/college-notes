# Karnaugh Maps
2022-11-03 | [[1.4.3 Boolean Algebra]]

- Allows you to visualise and understand a logical expression easier
- Used to illustrate an expression as seen below (A *OR* *NOT* B)![[2022-11-04-karnaugh-map-diagram.jpeg]]
- Can be used to simplify a very long and complex expression involving many variables
	- E.g. four variables, A, B, C and D
		- Write out all the combinations of A and B, and C and D in the grid sides
		- Make sure only one variable changes each time -> i.e. 00, 01, 11, 10
		- Put a 1 where all the expressions joined by or are valid
		- Group all 1s together
			- The total 1s in the groups must be a multiple of 2
			- Maximise the total 1s in the groups and minimise the amount of groups
			- Groups can be joined from opposite sides of the Karnaugh Map
			- Groups cannot be diagonal
		- Then, construct each expression for each group by adding together the individual logic functions, then *OR* them all together