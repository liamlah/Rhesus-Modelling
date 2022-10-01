# A population modelling program for rhesus blood groups.
The program will generate a seed population with a size, average number of offspring and Mendelian allele distribution based on input parameters. 
The program then pairs the individuals in the seed generation and generates offspring that inherit the alleles of their parents in a random manner that closely resembles nature.
The new generation is paired in the same manner and the process continues for the specified number of generations according to the input parameter, or until one allele has been completely eliminated.

Within the generation function is code that attempts to model the sensitisation of a rhesus negative mother to a rhesus positive child, and simulates untreated haemolytic disease of the fetus and newborn in subsequent incompatible offspring. 
A limit on population size can be set (default 10000) to prevent exponential growth in calculation time for each generation. When a population limit is reached, a random shuffle of individuals in the population list occurs, and the list is then truncated back to the set limit. 

The final function generates a graph showing the prevalence of each allele through each generation, additionally the percentage of offspring in a generation that are lost to HDFN is presented.

This code has the potential be adapted to model other mendelian traits in a population.
