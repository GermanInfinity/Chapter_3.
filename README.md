# Chapter_3.
This chapter delves deeper into the parts of an Evolutionary Algorithm. 
Stage 1 - Encoding and Operators

i) Binary Code: Multiple-point Crossover, Uniform Crossover

ii) Real Code: Without preference(Arithmetic crossover, Blend crossover, Simplex crossover), With preference(Simulated binary crossover, Unimodal normal distribution crossover), Mutation without direction(Uniform mutation, Boundary mutation, Nonuniform mutation, Normal mutation, Cauchy mutation, Polynomial mutation), Mutaton with direction(DE)

Note: 
Crossover tends to be important because it enables search on the global level of the solution space. It is a way of exploration before arrive at a local optima. 
Mutation tends to be important because it enables search in local optima or basin, searching for the best solution. It is a way of exploitation. 
So the process starts with cross over which searches over a large space, before it is fine-tuned for convergence to occur while mutation.

iii) Selection Methods: Proportional selection(RWS and SUS), Fitness scaling and transferral(Linear scaling, Sigma truncation, Power law scaling, Boltzmann scaling)
Selection methods address issues like the randomness in selecting individuals when close to the optimal basin(random walk), sticking and increasing the amount of a highly fit individual but to create diversity in the population, selecting individuals when it is difficult to calculate their fitness, and genetic drift. 
Fitness scaling is for scaling the fitness of individuals to control how "super-individuals" are handled in the population and chosen for the mating pool. 

(iv) Ranking 

References
Rationale for designing a good real code crossover operator.[2-3]

Credit--
Xinjue Yu, Mitsuo Gen. <chapter 2.> Introduction to Evolutionary Algorithms
