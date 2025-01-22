# Chapter 7 Swarm intelligence: particles

## Particle swarm intelligence: bird flocks

### What do the following terms mean for simulating the movement of individual birds in relation to bird flocks?

* **Alignment**:
    An individual should steer in the average heading of its neighbors to ensure that the group travels in a similar direction.
* **Cohesion**:
    An individual should move toward the average position of its neighbors to maintain the formation of the group.
* **Separation**:
    An individual should avoid crowding or colliding with its neighbors to ensure that individuals do not collide, disrupting the group.

![ExapleRelations](image-19.png)

## Particle swarm optimization algorithm

### Discuss the different steps in the particle swarm optimization life cycle algorithm.

* **Initialize the population of particles:** Determine the number of particles to be used, and initialize each particle to a random position in the search space.
* **Calculate the fitness of each particle:** Given the position of each particle, determine the fitness of that particle at that position.
* **Update the position of each particle:** Repetitively update the position of all the particles, using principles of swarm intelligence. Particles will explore the search space and then converge to good solutions.
* **Determine the stopping criteria:** Determine when the particles stop updating and the algorithm stops.

### Discuss how the position of the particles is updated.
The position of the particles is updated based on their velocity. The speed of a particle is influenced by three components:
* **Inertia:** This is the tendency of a particle to maintain its current speed.
* **Cognitive component:** This is the tendency of a particle to move back to its own best position that it has found so far.
* **Social component:** This is the tendency of a particle to move to the best position found by the entire swarm.

The new speed is calculated by combining the current speed, the cognitive factor and the social factor. The position of a particle is then updated by adding the calculated speed to the current position.
The formula for updating the position is: new position = current position + new speed

![VisualRepresentation](image-20.png)

### How is the best solution ultimately determined?

The best solution is determined by the fitness function. The fitness of each particle is calculated based on its current position, and the particles with the best fitness (the lowest value at minimization, or the highest value at maximization) are tracked. In each iteration, the best fitness of the particles is updated. The best position found by the swarm is considered the final solution. The particle with the best position and value can be chosen at the end of the process.

### What criteria can be used to stop the algorithm?
* **Maximum number of iterations:** The algorithm stops after a predefined number of iterations.
* **Stagnation:** The algorithm is stopped if the best solution in the swarm no longer improves significantly. This means that the swarm may have converged to a local optimum or that further iterations will no longer lead to better results.

## Particle swarm optimization algorithm
### Explain the following relation:<br>New velocity = inertia component + cognitive component + social component <br>What is the function of?

The formula describes how the the velocity of a particle is updated in the PSO algorithm. By combining the three components, the movement of each particle is dynamically adjusted, balancing exploration and using the search space to find an optimal solution.
* **The inertia component** 
    The inertia component represents the resistance to movement or change in direction for a specific particle that influences its velocity. The inertia component consists of two values: the inertia magnitude and the current velocity of the particle. The inertia value is a number between 0 and 1.
* **The cognitive component**
    The cognitive component represents the internal cognitive ability of a specific particle. The cognitive ability is a sense of a particle knowing its best position and using that position to influence its movement. The cognitive constant is a number greater than 0 and less than 2. A greater cognitive constant means more exploitation by the particles.
* **The social component**
    The social component represents the ability of a particle to interact with the swarm. A particle knows the best position in the swarm and uses this information to influence its movement. Social acceleration is determined by using a constant and scaling it with a random number. The social constant remains the same for the lifetime of the algorithm, and the random factor encourages diversity in favoring the social factor.