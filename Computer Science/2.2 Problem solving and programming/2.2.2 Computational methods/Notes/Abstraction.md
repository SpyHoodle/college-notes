# The Nature of Abstraction
2022-09-12 Mon

### Abstraction
- **Abstraction** -> Removing unnecessary detail from a problem.
	- Widely used to simplify things that may be complex
	- Must ensure that you include the minimum amount of detail necessary to solve the given problem
	- Designing computer systems often uses:
		- Icons
		- Symbols
		- Legends
		- Colour-coding

- **Representational abstraction** -> What remains when unnecessary detail has been removed
	- A simpler version directed at solving a specific problem

- **Generalising** -> Grouping things in terms of a set of common characteristics
	- Fundamental technique used in OOP
	- Code can be developed and shared between objects
	- Generalisation can also be applied to the problem itself
		- Often helpful to identify a problem as an example of a more general set of problems

### Information Hiding
- A core concept of all computer systems
- Impossible to comprehend their working without layers of abstraction

- **Interface** -> Provides an abstraction of what lies behind it
	- E.g. operating systems use a graphical user interface to make it easier for users to interact with the computer
	- Operating systems have a common interface across machines
	- Upgrading the machine would improve performance but wouldn't affect the interface

- A class encapsulates all of its private attributes and methods -> only exposed through it's interface
- Clear interfaces allow changes to be made without disrupting anything else


### Procedural Abstraction
- **Procedural abstraction** -> Abstracting the actual values used in a particular computation as a part of a computation pattern or method - a procedure
	- E.g. 1 + 2 = 3 -> a + b = c 

### Functional Abstraction
- **Functional abstraction** -> The implementation detail of the computational method is hidden (like a black box) 
	- E.g. functions in Python
	- Receive input(s) -> process it -> return it
	- The transformation of the input(s) is hidden from the user

### Data Abstraction
- **Data Abstraction** -> A technique that separates the way that a compound data structure is used from the details of how it is implemented or constructed
	- Higher level languages include abstract data types that are a logical description of how the data is viewed and the operations that can be performed on it
		- E.g. a queue, elements can only be added from the rear and removed from the front, but the programmer is only concerned with functions like `AddToQueue()` and `RemoveFromQueue()`
	- Prevents you from getting caught up in how the data type is constructed
		- Especially with more complex data structures

### Problem Abstraction
- **Problem Abstraction** -> The process of generalising or reducing a problem to one that has already been solved
	- Identifying what type of problem it is -> abstracting to leave a generalisation -> applying it to an existing solution such as an algorithm

#### Example
Consider the following problem:
> The Alpaca Soap Company is going to launch a new product range: Lemon and Lime. The organic range includes soap and a body cream. The cream needs to be stored carefully so that it does not deteriorate. The company has advance orders for the next year and must produce 300 batches in the next quarter, then 250, 100, and 350 in successive quarters. There are fixed costs of £10,000 per quarter and each batch costs £300 to produce. If needed, the cost of storage is £500 per batch per quarter. The company wants to produce a production plan that allows its advance orders to be satisfied and minimises its total cost.

This problem should be reduced to a shortest path problem, and then applied to a suitable shortest path algorithm e.g. [Dijkstra's shortest path algorithm](https://isaaccomputerscience.org/concepts/dsa_search_dijkstra)

## References
- [Isaac Computer Science - Abstraction](https://isaaccomputerscience.org/concepts/dsa_ctm_abstraction?examBoard=all&stage=all)

#TODO: Change Dijkstra's shortest path algorithm to my own note
#TODO: Ask Abid about procedural abstraction