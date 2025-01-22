# Evolutionary Algorithms

## Genetic Algorithms: life cycle
Briefly explain the life cycle of a genetic algorithm.

The life cycle of a genetic algorithm consists of the following steps:
* Creating a population: Creating a random population of potential solutions.
* Measuring the fitness of individuals in the population: Determining how good a specific solution is. This task is accomplished by using a fitness function that scores solutions to determine how good they are.
* Selecting parents based on their fitness: Selecting pairs of parents that will reproduce offspring.
* Reproducing individuals from parents: Creating offspring from their parents by mixing genetic information and applying slight mutations to the offspring.
* Populating the next generation: Selecting individuals and offspring from the population that will survive to the next generation.

## Enter diversity
Genetic algorithms use crossover and mutation as principles to ensure the diversity of the next generations.
Explain this principle.
Give some examples of crossover and mutation.

* Crossover: Combining the first part of one parent with the second part of another parent to create a new offspring.
    * Single point crossover: One point in the chromosome is selected, the fist part of the chromosome is taken from the first parent, and the second part is taken from the second parent. These two parts are then combined to create a new offspring.
    * Two-point crossover: Two points in the chromosome are selected, referencing the two parents, parts are chosen in an alternating manner to make a new offspring.
    * Uniform crossover: A mask is created to determine which genes are taken from which parent. The mask is randomly generated, and the genes are selected based on the mask.
        
* Mutation: Randomly changing the offsprings slightly to create variation in the population>
    * Bit-string mutation: A gene is randomly selected, and its value is flipped.
    * Flip-bit mutation: All genes in a chromosome are inverted to the opposite value.

## Genetic Algorithm parameters
Name 5 parameters to configure a genetic algorithm.
How does each parameter affect the generation of solutions?

* Chromosome encoding: The chromosome encoding method requires thought to ensure that it is applicable to the problem and that the potential solutions strive for global maxima. The encoding scheme is at the heart of the success of the algorithm.
* Population initialization: Although the individuals in a population are initialized randomly, ensuring that the solutions are valid is important for optimizing the computation of the genetic algorithm and initializing individuals with the right constraints.
* Number of offspring: The number of offspring created in each generation can be configured. Given that after reproduction, part of the population is killed off to ensure that the population size is fixed, more offspring means more diversity, but there is a risk that good solutions will be killed off to accommodate those offspring.
* Parent selection method: The selection method used to choose parents can be configured. The selection method must be based on the problem and the desired explorability versus exploitability.
* Stopping condition: The stopping condition for the algorithm must make sense based on the problem and desired outcome. Computational complexity and time are the main concerns for the stopping condition.


## Fitness function
What is a fitness function within a genetic algorithm? 

The fitness function determines the quality of an individual solution in the population. It measures how well a candidate solution achieves it's intended goal. The fitness function assigns a score to each possible solution. This score is used to determine which individuals are selected for reproduction and which individuals survive to the next generation. A fitness function is like a heuristic that guides the algorithm in finding the best solution.

Why is the correct choice of the right fitness function crucial for the performance of the algorithm?

The choice of fitness function is crucial because it directly influences the algorithm's direction. If the fitness function is not well designed, the algorithm may not converge to the optimal solution. A good fitness function should accurately reflect the desired characteristics of the optimal solution and be able to distinguish 'good' solutions from 'bad' ones.  A wrong fitness function can lead to a poorly performing algorithm that is unable to find useful solutions.

