#Monte Carlo simulation to estimate pi


##Introduction

The Monte Carlo simulation is an algorithm that uses a large number of repeated random sampling and produces summary statistics based on the sum of outcomes. The Monte Carlo simulation will define a domain of possible inputs, generate inputs randomly over the domain, perform a deterministic computation on the random inputs, and then aggregate the results.

##Using Monte Carlo to estimate the value of pi

A circle that can fit in the square with domain [-1,1] has a radius of 1 and area π. The area of the square is 4. The ratio of the area of the circle to the square is π/4. 

To approximate the value of π using Monte Carlo, draw a circle of radius 1 in the 2x2 square. By randomly scattering a large number N points in the square, the number of points within the circle divided by N and multiplied by 4 is an approximation of π by the ratio of the areas of the circle and square. 

By drawing random numbers between -1 and 1 for x and y positions of the points and using Pythagoras' theorem to check if the point is within the circle, this procedure can be simulated by using the NumPy package.
