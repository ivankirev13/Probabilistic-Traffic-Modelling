# Probabilistic-Traffic-Modelling

Summer project at Technische Universität München

This is a project done at TUM in the summer of 2022 as part of the TUM PREP program.

In many cities there are counters at a number of intersections, which count the number of vehicles passing at that location. The data is discrete, i.e for a given counter we have the number of cars that have passed within each hour. 

The objective of the first project is to create a mathematical model describing the traffic of a given counter. We are using data from an arbitrary counter in Strassbourgh during a single week in 2016. We then fit ARIMA model on a training set and create a forecast which is then compared with the true data.

The second part of the project creates a probabilistic model for traffic flow. We assume that a car travels from counter A to counter B, given that the distance between them is known. Supposing that some cars travel faster than the normal speed and others drive slower, we model that a given car at point A arrives at point B in time X, which follows a normal distribution with mean the average time a car travels the given distance. Using this, we predict the number of cars at counter B at each time. If we are given the true data from counter B, we make other predictions including the number of cars parked somewhere in between the two counters or the number of cars taking a turn at an intersection.
