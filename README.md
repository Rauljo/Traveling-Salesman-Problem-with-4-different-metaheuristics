# Traveling-Salesman-Problem-with-4-different-metaheuristics

In this repository, 4 different metaheuristics (Simulated Annealing, Tabu Search, Genetic Algorithm, Ant Colony) have been implemented to solve the travelling salesman problem. 

Each of the jupyer notebooks describes the process followed to study the data, implement the solutions and test different configurations until the final results are obtained. 

At the end of each notebook a reflection on the results obtained is written in ‘REPORT’. 

In the last notebook: Colonies. A comparison of the results obtained with the four algorithms is made. This conclusion is shown below:

# Comparison:

Finally, throughout the practical part of the course we have seen 4 different metaheuristics, each one with its strengths and weaknesses. Let's comment on them, and determine which one will be better for which situations. In general, a table that summarises the results obtained is the following:

| Algorithm             | Fast Solution | Time       | Slow Solution | Time            |
|-----------------------|---------------|------------|---------------|-----------------|
| Simulated Annealing   | 29000        | 2 seconds  | 26463        | 100 seconds     |
| Tabu Search           |         | | 23343           | 323 seconds             |
| Genetic Algorithm     | 40000   | 4 seconds | 29835 | 1 hour and 13 minutes    |
| Ant Colony | 25230 | 4 seconds | 22459 | 448 seconds|
| Greedy Algorithm | 27033 | 0.006 seconds | | |


In general, the metaheuristics have given very different results with different runtimes. We have added the Voracious Algorithm (which was used in Tabu List and Ant Colony) because it may be interesting to consider it when deciding which algorithm to use.

In all these algorithms the execution time increases as the size of the problem (the number of cities to visit) increases, preventing us from reaching the optimal solution and only getting close to it in most cases. Although in all cases the time increases, it does not do so to the same extent: in Tabu Search, Genetic Algorithm and Ant Colony, the three algorithms would multiply their execution times by 4 or 5 when doubling the size of the problem. The Voracious algorithm would still result in a very small runtime. The Simulated Temple algorithm scales less than its competitors (multiplying by 1.x depending on the run).

The Tabu Search and Genetic Algorithm algorithms would not be beneficial in any case, because of their time constraints and the solutions they find. The Voracious Search algorithm could be recommended in certain situations where we want a fixed result, in a very short time, and as long as it turns out that the algorithm works well for the particular problem; as this need not always be the case. The main problem with the Simulated Temple and Ant Colony algorithms is the variability of their results in short run times. However, they return results very close to the optimum (especially Ant Colony, since they start from a voracious solution). For longer runs, Ant Colony is highly recommended, as long as the problem is not excessively large.


