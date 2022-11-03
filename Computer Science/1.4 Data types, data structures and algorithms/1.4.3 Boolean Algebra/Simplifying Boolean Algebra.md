# Simplifying Boolean Algebra
2022-11-03 | [[1.4.3 Boolean Algebra]]

## De Morgan's Law
- Either logical function *AND* or *OR* may be replaced by the other given certain changes to the expression
- Allows statements to be simplified so that they only use *NAND* or *NOR* gates
	- Makes it easier to build microprocessors
	- e.g. Solid-state drives are made up of only *NAND* gates 
- e.g. *NOT* A *AND* *NOT* B is *NOT*(A *OR* B)
- Steps are as follows:
	- Change *OR* to *AND* (or vice versa)
	- *NOT* the terms on either side of the operator
	- *NOT* everything that has changed
	- Remove double negation (any multiple of two *NOT* gates next to each other)

### Diagram Example
![[2022-11-03-de-morgans-law-example.png]]

## Association
- Allows us to remove brackets from an expression to regroup the variables
- A *OR* (B *OR* C) = (A *OR* B) *OR* C = A *OR* B *OR* C
- A *AND* (B *AND* C) = (A *AND* B) *AND* C = A *AND* B *AND* C

## Commutation
- The order of applications of two separate terms is not important
- A *OR* B = B *AND* A
- A *AND* B = B *AND* A

## Distribution
- Allows us to multiply or factor out an expression
- A *AND* (B *OR* C) = (A *AND* B) *OR* (A *AND* C)
- A *OR* (B *AND* C) = (A *OR* B) *AND* (A *OR* C)

## Absorption
- Where the rule applies, the second term inside the bracket can be eliminated and absorbed by the term outside the bracket
- A *OR* (A *AND* B) = A
	- As A has to be True for the logic to end as True, as if it wasn't neither condition would be met
- A *AND* (A *OR* B) = A
	- As if A wasn't True, the *AND* would never succeed as it contains A by itself, so the conditions are only met when A is True, which is the same as saying A