# The Traveling Skier Problem
Public Repository for DSCI 478 Final Project: The Traveling Skier Problem

## Authors: 

D'Andre Tafoya, Jillian Cook, Lauren Bair, Garrett Hayden

## Project Description:

This repository encompasses the entirety of our code for the DSCI 478 capstone final project at Colorado State University. For this project we decided to optimize a Traveling Salesperson Problem (TSP) for the 2013 Vail Resorts Lifetime Epic Pass challenge. 26 resorts were on the pass at the time, and the goal was to visit every resort in a single season. The goal was to find the most cost optimal path to all 26 resorts to see how valuable the lifetime Epic Pass truly was given the price of the pass per year. We further extended our research by utilizing the Google Maps and Amadeus APIs to pull real time travel and cost data and also explored various methods and algorithms that are commonly used when tackling the TSP. We hope this analysis provides an interesting and educational perspective on an enaging real-world scenario.

## File Structure:

Multimodal_Cost_Optimization.ipynb - This file contains the main multi-modal TSP planner which uses both APIs and finds the optimal route, optimal cost, and provides a trip summary. It pulls real-world driving distances and flight fares and compares the cost of driving vs. flying for every leg.

Base_TSP_COST.ipynb - This file holds the base TSP model and basic cost optimization methods including the Held-Karp and OR-Tools methods utilizing a fixed cost model.

Multimodal_Travel_Planner.ipynb - This file extends the cost_optimization.ipynb file by taking the optimal TSP route and creating a full multi-modal itinerary by establishing driving vs. flying rules, calculating costs and distances, and printing the itinerary. It also includes an annotated map that shows the airports and resorts used in the calculation, as well as the route taken.

Open_TSP.ipynb - This file provides another look at the TSP, but without the constraint of being required to start and end at the same location. We wanted to explore a more realistic cost model based on the competition, where winning the competition only took reaching the last resort (not the return trip home), and an Open TSP approach provided that.

Base_TSP_Distance.ipynb - This file has the base path of the optimized TSP entirely dependent on distance, not cost. This provided a baseline as to how different methods would be used when introducing prices of travel into the problem.

## Sources

### Scholarly Journals

Lian, Kai Q., and Gareth A. Tribello. “An Elementary Approach to the Vehicle Routing Problem via   Python and Google API.” American Journal of Operations Research, vol. 14, no. 6, 29 Nov. 2024, Art. no. 146009, https://doi.org/10.4236/ajor.2024.146009

Maria, Eny, et al. “Measure Distance Locating Nearest Public Facilities Using Haversine and Euclidean Methods.” Journal of Physics: Conference Series, vol. 1450, no. 1, Feb. 2020, Art. no. 012080, https://doi.org/10.1088/1742-6596/1450/1/012080.

Ono, Daryl, Jose Rincón, and Althea Thomas. “A Criteria-Based Approach to the Traveling Salesman Problem (TSP).” Western Decision Science Journal, 2020. LMU Digital Commons, https://digitalcommons.lmu.edu/librarian_pubs/143

### Other Sources

“Common Routing Tasks  |  Or-Tools  |  Google for Developers.” Google, Google, https://developers.google.com/optimization/routing/routing_tasks

Custer, Charlie. “How to Use an API in Python.” Dataquest, 25 Mar. 2025, https://www.dataquest.io/blog/api-in-python/

“Getting Started!” FlightAPI, FlightAPI, https://docs.flightapi.io/

“Held–Karp Algorithm.” Rosetta Code, 13 April 2025, https://rosettacode.org/wiki/Held%E2%80%93Karp_algorithm

Liang, David. “Intro - Python Algorithms: Traveling Salesman Problem.” Medium, Medium, 19 July 2024, https://medium.com/@davidlfliang/intro-python-algorithms-traveling-salesman-problem-ffa61f0bd47b

Prewitt, Nate, and Seth M Larson. “HTTP for HumansTM¶.” Requests, https://requests.readthedocs.io/en/latest/

“The Directions API Demo.” Google, Google, https://developers.google.com/maps/documentation/directions/start

“Travelling Salesman Problem Using Dynamic Programming.” GeeksforGeeks, GeeksforGeeks, 26 Nov. 2024, https://www.geeksforgeeks.org/travelling-salesman-problem-using-dynamic-programming/

“Traveling Salesperson Problem  |  OR-Tools  |  Google for Developers.” Google, Google, https://developers.google.com/optimization/routing/tsp

“What is an API (Application Programming Interface)?” Amazon Web Services, Amazon Web Services, Inc., https://aws.amazon.com/what-is/api/
