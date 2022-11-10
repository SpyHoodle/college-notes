# Useful Circuits
2022-11-08 | [[1.4.3 Boolean Algebra]]

## Binary equivalence tester
- If two inputs are exactly the same, the circuit should output a 1
- This can be represented with a *NOT XOR* gate
![[2022-11-08-binary-equivalence-circuit.png]]
### Truth table
| A   | B   | Q   |
| --- | --- | --- |
| 0   | 0   | 1   |
| 0   | 1   | 0   |
| 1   | 0   | 0   |
| 1   | 1   | 1   |

## Binary half adder
- Can add two single bit binary numbers together
- The sum is formed by an *XOR*, and the carry is formed from an *AND*
![[2022-11-08-binary-half-adder-circuit.png]]

### Truth table
| A   | B   | C   | S   |
| --- | --- | --- | --- |
| 0   | 0   | 0   | 0   |
| 0   | 1   | 0   | 1   |
| 1   | 0   | 0   | 1   |
| 1   | 1   | 1   | 0   |

## Binary full adder
- For multiple digit addition, multiple carry's may be needed
- To reliably add two single-bit digits in any position, three inputs are needed
	- These are the values for the two bits and the carry from the previous calculation (or column when you do binary column addition)
- This circuit is built from two half adders
	- Use the first half adder to calculate A + B
	- Use the second half adder to add the result of the first half adder and the carry from the previous calculation (or column) to get the final sum)
	- If one of the half adders have remaining a carry of 1, set the final carry ($C_{out}$) to be zero by using *OR* on the carry's of both the calf adders
![[2022-11-08-binary-full-adder-circuit.png]]
### Truth Table
| $A$ | $B$ | $C_{in}$ | $C_{out}$ | $S$ (sum) |
| --- | --- | -------- | --------- | --------- |
| 0   | 0   | 0        | 0         | 0         |
| 0   | 0   | 1        | 0         | 1         |
| 0   | 1   | 0        | 0         | 1         |
| 0   | 1   | 1        | 1         | 0         |
| 1   | 0   | 0        | 0         | 1         |
| 1   | 0   | 1        | 1         | 0         |
| 1   | 1   | 0        | 1         | 0         |
| 1   | 1   | 1        | 1         | 1          |

## Four-bit binary adder
- Not needed in the exam, but useful for understanding adders
- Full adders can be chained together
- At the start of the chain is a half adder, because there is no digit to carry in
![[2022-11-08-binary-four-bit-binary-adder.png]]

## Sequential circuits
- Outputs depend not only on the current inputs but also on the sequence of past events
- **Flip-flop** -> Allows a previous output value to be stored, and thus acts as a simple memory device
	- Outputs are always opposite
	- These memory units are volatile
	- Can be asynchronous, where the inputs will be processed as they arrive
	- Can be synchronous, meaning the operations are controlled by a clocks

- **RS flip-flop** -> Stores the value of a single binary digit from two inputs
	- Can be done with *NAND* or *NOR* gates, but effectively flips around the flip-flop
- **D-type flip-flop** -> A synchronous sequential circuit that can be used to store the value of a single binary digit
	- $D$ is the data signal
	- $Clk$ is the clock signal
	- It has an internal loop which allows the previous output value to be stored
	- When the clock signal is low (0) changes at D make no difference to the outputs
	- When the clock signal is high (1) the value of input D will appear at output Q. *NOT* Q is always the inverse of Q.
	- If there are changes in the data during the period when the clock signal is high, the output at Q,Q will change in line with D,D. 
		- This may not be a desirable feature of the circuit. 
		- An edge-triggered D-type flip flop will deal with this problem
![[2022-11-08-d-type-flip-flop.png]]

### Truth table
| Clock | D   | Q                   | *NOT* Q                   |
| ----- | --- | ------------------- | ----------------------- |
| 0     | 0   | Previous value of Q | Previous value of *NOT* Q |
| 0     | 1   | Previous value of Q | Previous value of *NOT* Q |
| 1     | 0   | 0                   | 1                       |
| 1     | 1   | 1                   | 0                       |
