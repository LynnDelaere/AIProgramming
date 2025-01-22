# Advanced evolutionary approaches

## Selection mechanisms
Briefly discuss the principle of following selection mechanisms in the evolutionary algorithm and discuss the advantages and disadvantages of each selection mechanism:
* **Roulette wheel selection**
    Roulette wheel selection is a selection mechanism that selects individuals based on their fitness. The probability of an individual being selected is proportional to its fitness. The selection process is done by spinning a roulette wheel, where the size of the wheel is proportional to the fitness of the individual.
    *Advantages*: easy to implement and allows weaker individuals to be selected.
    *Disadvantages*: biased towards higher fitness values, which reduces the diversity.
* **Rank selection**
    Rank selection is a selection mechanism that selects individuals based on their rank in the population. The individuals are sorted based on their fitness and assigned a rank. The probability of an individual being selected is proportional to its rank.
    *Advantages*: less biased towards higher fitness values, which increases the diversity.
    *Disadvantages*: slower convergence because strong individuals are not selected as often.
* **Tournament selection**
    Tournament selection is a selection mechanism that selects individuals by comparing them in a tournament. A random subset of the population is selected and the fittest individual in the subset is selected. 
    *Advantages*: balances exploration and exploitation, effective with fewer high-fitness individuals. 
    *Disadvantages*: requires a tournament size parameter, which can be difficult to determine. 
* **Elitism selection**
    Elitism selection is a selection mechanism that selects the best individuals from the population and carries them over to the next generation. 
    *Advantages*: preserves the best individuals in the population.
    *Disadvantages*: the population may converge prematurely to a local optimum.

## Mutation mechanisms
Briefly discuss the principle of following mutation mechanisms in the evolutionary algorithm:
* **Boundary mutation**
    In boundary mutation, a gene randomly selected from a real-value encoded chromosome is set randomly to a lower bound value or upper bound value. The minimum and maximum can be the same for all indexes or set uniquely for each index
* **Arithmetic mutation**
     Arithmetic mutation is a mutation mechanism that selects a gene in an individual and mutates it by adding or subtracting a small value. The mutation operator selects a random gene and adds or subtracts a small value to its current value. 

## Tree encoding and tree crossover
Briefly discuss the principle of:
* **Tree encoding**
    Tree encoding represents a chromosome as a tree of elements. Tree encoding is versatile for representing complex solutions where the hierarchical structure is important. Each node in the tree represents a function or terminal value, and the tree is evaluated recursively to produce the final solution.
* **Tree crossover**
    Tree crossover is similar to single-point crossover in that a single point in the tree structure is selected and then the parts are exchanged and combined with copies of the parent individuals to create an offspring individual. The resulting children must be verified to be valid solutions that obey the constraints of the problem. 