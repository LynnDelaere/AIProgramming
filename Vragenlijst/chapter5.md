# Advanced evolutionary approaches

## Selection mechanisms
* Briefly discuss the principle of following selection mechanisms in the evolutionary algorithm and discuss the advantages and disadvantages of each selection mechanism:
    * Roulette wheel selection <br>
        Roulette wheel selection is a selection mechanism that selects individuals based on their fitness. The probability of an individual being selected is proportional to its fitness. The selection process is done by spinning a roulette wheel, where the size of the wheel is proportional to the fitness of the individual. The wheel is spun and the individual that the wheel stops at is selected. <br>
        *Advantages*: easy to implement and allows weaker individuals to be selected. <br>
        *Disadvantages*: biased towards higher fitness values, which reduces the diversity. <br>
    * Rank selection <br>
        Rank selection is a selection mechanism that selects individuals based on their rank in the population. The individuals are sorted based on their fitness and assigned a rank. The probability of an individual being selected is proportional to its rank. <br>
        *Advantages*: less biased towards higher fitness values, which increases the diversity. <br>
        *Disadvantages*: slower convergence because strong individuals are not selected as often. <br>
    * Tournament selection <br>
        Tournament selection is a selection mechanism that selects individuals by comparing them in a tournament. A random subset of the population is selected and the fittest individual in the subset is selected. <br>
        *Advantages*: balances exploration and exploitation, effective with fewer high-fitness individuals. <br>
        *Disadvantages*: requires a tournament size parameter, which can be difficult to determine. <br>
    * Elitism selection <br>
        Elitism selection is a selection mechanism that selects the best individuals from the population and carries them over to the next generation. <br>
        *Advantages*: preserves the best individuals in the population. <br>
        *Disadvantages*: can lead to premature convergence if the best individuals dominate the population. <br>

## Mutation mechanisms
* Briefly discuss the principle of following mutation mechanisms in the evolutionary algorithm:
    * Boundary mutation <br>
        Boundary mutation is a mutation mechanism that selects a gene in an individual and mutates it to the boundary value of the gene's domain. The mutation operator selects a random gene and sets its value to the minimum or maximum value of the gene's domain. <br>
    * Arithmetic mutation <br>
        Arithmetic mutation is a mutation mechanism that selects a gene in an individual and mutates it by adding or subtracting a small value. The mutation operator selects a random gene and adds or subtracts a small value to its current value. <br>

## Tree encoding and tree crossover
* Briefly discuss the principle of:
    * Tree encoding
        Tree encoding is a method of representing a solution as a tree structure. Each node in the tree represents a function or terminal value, and the tree is evaluated recursively to produce the final solution. <br>
    * Tree crossover
        Tree crossover is a crossover operator that combines two parent trees to produce offspring trees. The crossover operator selects a random subtree from each parent tree and swaps them to create two new offspring trees. <br>