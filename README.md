# The Traveling Skier Problem
Public Repository for DSCI 478 Final Project: The Traveling Skier Problem

## Authors: 

D'Andre Tafoya, Jillian Cook, Lauren Bair

## Project Description:

This repository encompasses the entirety of our code for the DSCI 478 capstone final project at Colorado State University. For this project we decided to optimize a Traveling Salesperson Problem (TSP) for the 2013 Vail Resorts Lifetime Epic Pass challenge. 26 resorts were on the pass at the time, and the goal was to visit every resort in a single season. The goal was to find the most cost optimal path to all 26 resorts to see how valuable the lifetime Epic Pass truly was given the price of the pass per year. We further extended our research by utilizing the Google Maps and Amadeus APIs to pull real time travel and cost data and also explored various methods and algorithms that are commonly used when tackling the TSP. We hope this analysis provides an interesting and educational perspective on an enaging real-world scenario.

## File Structure:

cost_optimization.ipynb - 

cost_paths.ipynb - This file holds the base TSP model and basic cost optimization methods including the Held-Karp and OR-Tools methods utilizing a fixed cost model.

Multimodal_Travel_Planner.ipynb -

OpenTSP_paths.ipynb - This file provides another look at the TSP, but without the constraint of being required to start and end at the same location. We wanted to explore a more realistic cost model based on the competition, where winning the competition only took reaching the last resort (not the return trip home), and an Open TSP approach provided that.

paths.ipynb - This file has the base path of the optimized TSP entirely dependent on distance, not cost. This provided a baseline as to how different methods would be used when introducing prices of travel into the problem.