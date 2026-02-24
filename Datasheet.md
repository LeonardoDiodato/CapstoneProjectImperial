# Datasheet
### Motivation
The dataset used has been created to collect all the datapoints available for each of the functions of this Capstone project.

The dataset is to support the Capstone Project, which is a Black Box Optimization challenge

### Composition
The dataset is composed of all the observed points for each of the eight functions.
#### Size
Each function has a different number of features:
- function one has 2 features
- function two has 2 features
- function three has 3 features
- function four has 4 features
- function five has 4 features
- function six has 5 features
- function seven has 6 features
- function eight has 8 features
#### Format
All the values are expressed in real numbers with a decimal or exponential notation when too small.
Each decimal value has a maximum precision of 8 digits after the decimal point.

For each function:
- the inputs are represented in a matrix with dimensions defined by number of features of the function times the number of observed points.
- the outputs are defined in a one dimensional array of values which represents the collection of values of the function in each observed points.

#### Gaps
Being that these data are coming from a Black Box Optimization challenge, these represent the explored points over the domain space for each of the functions, so inherently presents many gaps over the domain space.


### Collection Process
#### Time frame
The time frame of the competition has been of 13 weeks, during which a new point has been queried for each week.

#### Strategy Used and Queries generation
The strategy I've relied on to through this competition has been based on a Bayesian Optimization approach. 
This approach has been divided in two steps: for the first half of the available time, I've tried to explore the domain space for each of the function so to use a more exploratory behavior.
For the second half of the available time, I've tuned the model to use a more exploitative behaviour, based on the previous results.

For some of the functions, this approach failed for some of the weeks, meaning that the new suggested point to query was a point already known.
Unfortunately I was not able to catch this issue immediately, so some of the queries might present the same values queried over different weeks.
When this was found, this issue has been fixed by using an artificial neural network approach to generate the query point for the following week instead of using the point suggested by the Bayesian Optimization approach.

### Preprocessing and uses
No preprocessing or transformation has been done on the data used in the dataset for this competition.
This dataset is intended to be used only in the context of this Capstone challenge.

### Distribution and maintenance
This dataset is publicly available within the current repository at the address: https://github.com/LeonardoDiodato/CapstoneProjectImperial
This dataset is free to use, please note that the intended use is limited to the context of this Capstone challenge.
This dataset is not maintained, and will not be updated. 


