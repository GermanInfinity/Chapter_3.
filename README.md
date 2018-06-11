# Chapter_3.
This chapter delves deeper into the parts of an Evolutionary Algorithm. 

Stage 1 - Encoding and Operators

i) Binary Code: Multiple-point Crossover, Uniform Crossover

ii) Real Code: Without preference(Arithmetic crossover, Blend crossover, Simplex crossover), With preference(Simulated binary crossover, Unimodal normal distribution crossover), Mutation without direction(Uniform mutation, Boundary mutation, Nonuniform mutation, Normal mutation, Cauchy mutation, Polynomial mutation), Mutaton with direction(DE)

Note: 
Crossover tends to be important because it enables search on the global level of the solution space. It is a way of exploration before arriving at a local optima. 
Mutation tends to be important because it enables search in local optima or basin, to search for the best solution. It is a way of exploitation. 
So the process starts with cross over which searches over a large space, before it is fine-tuned for convergence to occur during mutation.


Stage 2 - Selection Methods

iii) Selection Methods: Proportional selection(RWS and SUS), Fitness scaling and transferral(Linear scaling, Sigma truncation, Power law scaling, Boltzmann scaling)

Note:
Selection methods address issues like the randomness in selecting individuals when close to the optimal basin(random walk), sticking with and increasing the number of highly fit individuals but instead creating a diverse population, selecting individuals when it is difficult to calculate their fitness, and genetic drift. 
Fitness scaling is scaling the fitness of individuals to control how "super-individuals" are handled in the population and chosen for the mating pool. 

iv) Ranking: Linear ranking, Nonlinear ranking

Note:
Ranking is to rank the individuals initally, then use these ranks to determine probability of being selected. It is important in the case we cannot get the fitness of individuals in the population but we can get a rank or we want to adjust selective pressures among individuals. 

v) Tournament Selection

Note:
Tournament selection is different from selection methods in (iii) because it is used primarily for selecting individuals in local basins. It is more of a local search method, and is very easy to implement. It involves picking k number of individuals in the population and competing their fitnesses against each other to determine the best for a mating pool. So it only takes a subset of individuals from the global population. 


Stage 3 - Replacement and Stop Criteria

vi) Replacement: Boltzmann selection replacement, Fitness-based replacement rule, Random-based replacement rule, Age-based replacement rule, Elitism technique, Conservative way, Competition between parents and offspring, Replacement happens with probability, Species adaptation genetic algorithm

Note: 
no. of offspring < no. of parents, no. of offspring > no. of parents, no. of offspring == no. of parents.
SAGA has no variation operators, it is a way of randomly selecting, competing, and changin(replacing) individuals in a population; it is usually adopted for large-scale operation domain searching. Boltzmann selection is definetly replacement, because it is a competition between the parent and the child to see who stays in the population. 
The techniques are for adjusting replacement rules. 

vii) Stop Criteria: Stop with fitness value, top with fitness change, Stop with time


Stage 4 - Parameter Control
viii) Parameter control: Deterministic strategy, Adaptive strategy, Self-adaptive strategy -- Variation Operator Control, popsize Control, 

Note: 
Elements affecting optimization are local factors and global factors. Local factors are for individuals thus are affected by cross-over and mutation operators. Global factors are on the population thus are affected by selection methods, population size and stop criteria. Both these factors need to have their parameters tweaked for a specific problem. In EA's we intially would like to search over a wide area of solutions, before converging to a desired location. This is really only possible by following a strategy that guides the control of the parameters for variation operators, population size, over time. 


References
Rationale for designing a good real code crossover operator.[2-3]

Credit--
Xinjue Yu, Mitsuo Gen. <chapter 2.> Introduction to Evolutionary Algorithms
