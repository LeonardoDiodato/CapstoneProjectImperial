# Capstone Project Imperial
Capstone Project created as part of the Professional Certificate in Machine Learning and Artificial Intelligence (Imperial College London).

## Section 1 - Project Overview
This project involves a Black Box optimization problem.<br>
The goal of this challenge is to find the global maximum for each of the 8 functions provided as black boxes.<br>
This is relevant in ML as many problems can be framed as BBO, where the problem can be modeled with an underlying undisclosed function of which we need to find the global maximum or minimum values.<br>
So practicing on this challenge is very useful to gain some hands-on experience in data science.<br>

## Section 2 - Inputs and Outputs
Inputs for these functions are given by rational numbers with 6 decimals precision.<br>
Each function takes one of these numbers for each dimension<br>
Dimensions for these functions and sample inputs for each are defined as follows:<br>

- Function 1: 2 dimensions - 0.000000-0.000000
- Function 2: 2 dimensions - 0.000000-0.000000
- Function 3: 3 dimensions - 0.000000-0.000000-0.000000
- Function 4: 4 dimensions - 0.000000-0.000000-0.000000-0.000000
- Function 5: 4 dimensions - 0.000000-0.000000-0.000000-0.000000
- Function 6: 5 dimensions - 0.000000-0.000000-0.000000-0.000000-0.000000
- Function 7: 6 dimensions - 0.000000-0.000000-0.000000-0.000000-0.000000-0.000000
- Function 8: 8 dimensions - 0.000000-0.000000-0.000000-0.000000-0.000000-0.000000-0.000000-0.000000

The input space is between the values 0 and 1 for each of the functions dimensions

The output for each function is a single rational number with 6 decimals precision representing the function value in that point of the domain space eg. 0.000000

## Section 3 - Challenge Objectives
The objective of the challenge is to find the global maximum for each of the 8 functions<br>
The major constraint of the challenge is the limited amount of observations available for these functions<br>
For each of these functions an initial set of 10 inputs and outputs was provided, and each week a new coordinates set can be provided as input, so to query the underlying function, and the result is provided back.<br>
For each week there is a limitation of just 1 input for each function.
Being that the challenge is designed to last 13 weeks, a total of 23 points observed will be a available for each function at the end of the challenge.<br>
The other factor that is limiting the most this challenge is the fact that each of these functions has an unknown structure.<br>
So no assumption can be made a priori about the behavior of the function. But various data analysis techniques can be applied to the dataset of each function to disclose any correlation of the input features over the function domain.


## Section 4 - Technical Approach
The technical approach I'm following of this challenge is relying on Bayesian Optimisation.<br>
I've decided to use an explorative approach on the first half of the challenge, and I will focus on exploitation on the second half.<br>
This is to ensure a wider coverage of the domain space in the first half of the challenge before focusing on any specific area of the domain, so not to miss any global maximum by focusing on a local maximum.<br>
I will also try during the course of this challenge to use other ML methods, were possible.

## Datasheet
https://github.com/LeonardoDiodato/CapstoneProjectImperial/blob/main/Datasheet.md

## Model Card
https://github.com/LeonardoDiodato/CapstoneProjectImperial/blob/main/Model%20card.md