# stochastic_assignment_3
# Solving Traveling Salesman Problem using Simulated Annealing
The basic TSP is assumed to be known. Here we ask you to try and solve the problem under
the following simplifying assumptions:
- There are paths from all cities to all other cities
- The triangle inequality holds for these paths, i.e. a detour via another city will always
result in a path that is at least as long as the direct path between two cities. The problem is symmetric, i.e. the path from A to B has the same length as that from B to A.

You may also assume that all cities lie in a plane. The quantity to be optimized is the total length of a circuit; the recommended elementary edit is 2-opt where two non-adjacent edges are deleted and the four cities are reconnected so that a new circuit is created. Moving a single city (node) to another location in the circuit can also be effective. Swapping two nodes is not a good idea, in general.
- There are three cities configuration files provided in TSP-Configurations.zip. Test your implementation on the smallest problem, eli51.tsp, then try to address bigger
problems, a280.tsp and pbc442.tsp. Focus your analysis and experiments on a280.tsp
- Few experiments that you could perform are:
  - First of all, you at least need to be able to converge to a good local minimum although the goal is find the global optima or the shortest path.
  - Second, try different cooling schedules and observe their effects on convergence
  - Third, what’s the effects of Markov Chain’s length on the convergence.
