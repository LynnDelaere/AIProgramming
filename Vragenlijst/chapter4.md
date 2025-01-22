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
* Name 5 parameters to configure a genetic algorithm.
* How does each parameter affect the generation of solutions?
    * Population size: Larger populations allow more diversity but increase computation.
    * Crossover rate: Determines the frequency of combining genes, influencing genetic mix.
    * Mutation rate: Higher rates introduce diversity but may disrupt good solutions.
    * Selection method: Affects which solutions are chosen as parents (e.g., roulette wheel, tournament).
    * Termination condition: Defines when the algorithm should end, affecting convergence time​.


## Fitness function
* What is a fitness function within a genetic algorithm? <br>
A fitness function evaluates how well a solution meets the problem’s criteria, guiding the selection of the best solutions. The fitness function assigns a score to each solution based on its quality.

* Why is the correct choice of the right fitness function crucial for the performance of the algorithm? <br>
The choice of fitness function is crucial because it directly influences the algorithm's direction, focusing on desired outcomes and avoiding misleading solutions​ that may not be optimal.

