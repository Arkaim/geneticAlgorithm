# Genetic Algorithm Report for Basics of Computer Simulation


## Description 
Genetic Algorithm to find roots of equation with 4 variables
**2x+3y+5z+4q=20**

Roots of an equation are in the range of [0;20]

We take 5 random values of a,b,c,d

We have 5 randomed generations
1. (22,12,11,7)
2. (8,29,12,1)
3. (12,26,4,15)
4. (3,9,10,23)
5. (13,17,26,6) 

Then we have to calculate the fittness coefficient by calculating distance from needed value to 20.

The nearest values to 20 are more desired.

Next, we will choose five pairs of parents, who will have exactly one child. We will give the will to the case exactly five times, each time the chance to become a parent will be the same and will equal the chance of survival. (We use "crossover" here)

---

## Pseudocode

```python
FOR each C do{
	find start node
	REPEAT
		FOR (i=0; i < (N)/2; i++) {
			select five parents from population
			generate five offsprings by crossover operation between two parent
			insert five offsprings to the new generation
			if (new_offspring satisfy the coverage) {
				add offsping to new population
				break
			}
		}
		mutate some offsprings in new generation list
	do until satisfy
}
```
