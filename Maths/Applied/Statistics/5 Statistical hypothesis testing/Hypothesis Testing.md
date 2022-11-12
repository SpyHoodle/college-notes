# Hypothesis Testing
2022-11-11 | [[5 Statistical hypothesis testing]]

## The Idea
- A method or a statement to determine if the probability of something happening is actually different to what it should be
	- E.g. Is this coin biased? Has this change in design made parts fail less? etc.
- **Null Hypothesis** $H_0$ -> What you assume would happen normally, what you think is or should be the current case 
	- e.g. the probability of a head when you flip a coin is 0.5 if the coin is fair
- **Alternative Hypothesis** $H_1$ -> The other probability we are thinking about, we think that this may actually be the case
	- e.g. the probability of a head is greater than 0.5 as we think it may be bias towards heads
- **Significance Level** -> The arbitrarily set probability of incorrectly rejecting the null hypothesis
	- **Critical Region** -> The region of data created or inside the significance level
		- If we collect data within this region, we are saying that this result was significant
			- E.g. the number of heads was 9 out of 10 coin flips, is in the significance level, therefore an extreme value
			- Therefore have evidence to suggest that the null hypothesis can be rejected and could be incorrect
		- **Critical Value** -> The value at the start of the critical region
	- **The Actual Significance Level** -> In a binomial distribution, it's the probability of the first value in the critical region (defined by the predefined significance level) onward
- **Tail** -> One end of the distribution 

## One-tail
- $H_0: p = 0.6$
	- Historically the probability of this event is 0.6
- $H_1: p < 0.6$
	- However we believe that the probability of our event is less than 0.6
	- If the significance level is 10%, then we'd be looking at 10% of the data at the bottom
- $H_1: p > 0.6$
	- However we believe that the probability of our event is greater than 0.6
	- If the significance level is 10%, then we'd be looking at 10% of the data at the top

## Two-tail
- $H_0: p = 0.3$ 
	- Historically the probability of this event is 0.3
- $H_1: p \neq 0.3$
	- However we believe that the probability is not 0.3
	- Therefore it could be greater than 0.3 or less than 0.3
	- If the significance level is 10%, then we'd be looking at 5% of the data at either ends (two tails)
		- This is because the 10% significance level is split over two regions
		- Therefore the significance level is halved
	- When we're doing a question, we decide which tail to look at by calculating the expected value (by multiplying the probability by the number of trials) and then see if the value that was found is above or below
		- If it's above, we'll look at the top tail as that is the only way it could be extreme
		- If it's below, we'll look at the bottom tail

## Finding the Critical Region
- As we cannot find X (the collected data) from the probability, we must use a ready made table or generate one on the calculator
- [This video explains how to do it perfectly](https://youtu.be/xwlkpT4LLmg)

## Examples
![[2022-11-11-hypothesis-testing-example-1.png]]
> Example 1: One-tail, Less than, Failed to reject $H_0$

![[2022-11-11-hypothesis-testing-example-2.png]]
> Example 2: One-tail, More than, Rejected $H_0$

![[2022-11-11-hypothesis-testing-example-3.png]]
> Example 3: Two-tail, More than (as 29 is greater than the expected value), Rejected $H_0$
> TLMaths: https://youtu.be/Eb7r4eYLUXc
