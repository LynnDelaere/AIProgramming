# Evolutionary Algorithms

## Genetic Algorithms: life cycle
* Briefly explain the life cycle of a genetic algorithm. <br>
The life cycle of a genetic algorithm consists of the following steps:
    * Initialization: Create a population of random solutions.
    * Evaluation: Evaluate the fitness of each solution in the population.
    * Selection: Select the best solutions for the next generation.
    * Crossover: Create new solutions by combining the genes of two parents.
    * Mutation: Introduce random changes in the genes of the new solutions.
    * Termination: Stop the algorithm when a stopping criterion is met.

## Enter diversity
* Genetic algorithms use crossover and mutation as principles to ensure the diversity of the next generations.
    * Explain this principle. <br>
    Crossover and mutation are used to introduce new genetic material into the population, which helps to maintain diversity and explore new regions of the search space.
    * Give some examples of crossover and mutation.
        * Single point crossover: A single point is selected in the parent chromosomes, and the genes are swapped to create new offspring.
        * Uniform crossover: Genes are randomly selected from the parents to create new offspring.
        * Bit flip mutation: Random bits in the chromosome are flipped to introduce new genetic material.
        * Swap mutation: Two genes in the chromosome are swapped to create a new solution.

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

