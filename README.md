# Traveling_Salesman-AI
This code implements an Ant Colony Optimization (ACO) algorithm to solve the Traveling Salesman Problem (TSP). The TSP is a classic combinatorial optimization problem where the objective is to find the shortest possible route that visits a list of cities and returns to the origin city.

### Key Classes and Functions
- **City Class**: Represents a city using x and y coordinates and calculates the Euclidean distance between cities.
- **Ant Class**: Represents an ant, which:
  - Visits cities in a specific order.
  - Chooses the next city based on pheromone and distance data.
  - Deposits pheromones to reinforce shorter paths.
- **TravelingSalesmanProblemACO Class**: Manages the ACO simulation, including:
  - **Initialization of Cities**: Randomly generates city coordinates.
  - **Pheromone Matrix**: Maintains and updates pheromone levels.
  - **Ant Generation and Tour Simulation**: Spawns ants for each generation to find shorter paths iteratively.
  - **Evaporation and Pheromone Reinforcement**: Prevents stagnation by reducing pheromone levels over time, encouraging exploration.

### Algorithm Flow
1. **City Initialization**: Generates random cities within a defined coordinate range.
2. **Pheromone Initialization**: Sets initial pheromone levels across all city pairs.
3. **Ant Simulation**: Each ant begins at a random city and completes a full tour by selecting cities based on pheromone levels and distances.
4. **Pheromone Evaporation**: Reduces pheromone levels to encourage diversity and avoid overemphasis on suboptimal paths.
5. **Route Visualization**: After all generations, the best path discovered is plotted for visual inspection.

### AI Concepts Utilized
This algorithm utilizes ACO, an AI approach based on swarm intelligence and probabilistic optimization. The collective learning from pheromone deposition and following enables the artificial colony to adaptively seek the shortest path over multiple generations.
