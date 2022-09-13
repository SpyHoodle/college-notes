# Decomposition
2022-09-12 Mon | [[2.2.2 Computational methods]]

## Problem Decomposition
- **Problem decomposition** -> The process of taking down a large problem and breaking it down into several small problems
	- Smaller problems roughly have the same complexity
	- Smaller problems can then often be broken down further (depending on size and complexity of the problem)
	- Repeat the process until the lowest level ideas represent a singular task, that can then be programmed as a procedure, module, function or method
	- OOP -> methods will be brought back together in classes that will be associated through inheritance, aggregation and composition
	- Procedural Programming -> subroutines organised into modules and a main routine that controls program flow

![[2022-09-12-decomposition-diagram.png]]

## Methods of Decomposition
### Top-down design
1. Look at the problem as a whole and identify its main components
2. Systematically analyse these components until you reach basic building blocks
3. Approach these components as free-standing modules that can be implemented using different methods

### Divide and Conquer
- Very common with searching, sorting and path-finding algorithms
1. Divide or 'unfold' a task into sub-tasks of identical or similar type until an easy-to-solve sub-task (known as the 'base case') is reached
2. Individual sub-tasks are combined or 'folded-back' to provide the solution to the main task