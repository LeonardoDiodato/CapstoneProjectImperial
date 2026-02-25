# Model Card
### Overview
The models used in this Capstone Project are:
- Bayesian Optimization
- Neural Networks

### Intended Use
These two models have been tuned to be used in this Capstone Project only.
Any other use case should be avoided.

### Details
In the 'code' folder contains the code used week by week for the time of this competition.<br>
Inside each week folder you can find the approaches used for that week.
Here is a detailed breakdown:
- Week 1:
  Neither Bayesian Optimization or Neural Networks have been used in the first week. The first query for each of the functions was chosen to be in the middle of the domain space (all the values for each of the features were set to 0.5)
- Week 2:
Bayesian Optimization has been used for all the functions
- Week 3:
Bayesian Optimization has been used for all the functions
- Week 4:
Bayesian Optimization has been used for all the functions
- Week 5:
Bayesian Optimization has been used for all the functions
- Week 6:
Bayesian Optimization has been used for all the functions. <br>Neural Networks were used for functions 5 and 8
- Week 7:
Bayesian Optimization has been used for all the functions <br>Neural Networks were used for functions 5 and 8
- Week 8:
Bayesian Optimization has been used for all the functions <br>Neural Networks were used for functions 7 and 8
- Week 9:
Bayesian Optimization has been used for all the functions <br>a Neural Network has been used for function 7
- Week 10:
Bayesian Optimization has been used for all the functions <br>a Neural Network has been used for function 8
- Week 11:
Bayesian Optimization has been used for all the functions <br>Neural Networks were used for functions 5 and 8
- Week 12:
Bayesian Optimization has been used for all the functions
- Week 13:
Bayesian Optimization has been used for all the functions

#### Approach Evolution
I've tried to rely on Bayesian Optimization focusing on exploration from week 1 to week 7, and exploitation from week 8 to week 13.
When this approach failed (see Limitations below) I've used the Neural Network Approach

### Performance
The performance of the Bayesian Optimization approach has been tracked to ensure that the new queried points were different for each week.
This has been done after the limitation of that model has been found, as described below.
The performance of the Neural Networks used have been measured by ensuring the most accurate training possible on he existing data points, when this method was used.

### Assumptions and Limitations
I've assumed that the Bayesian Optimization approach would have been sufficient throughout the whole competition.
I've found this not to be true when I've realized that this approach was keeping to suggest query points already known.
Unfortunately I was not able to catch this issue immediately so some of the queries have been similar over different weeks.
When this was noticed, I've used a Neural Network approach for the functions which the Bayesian Optimization approach was failing for each week.

### Ethical considerations
This models is easily replicable as all the code and parameters used are available, so it can be easily adapted to any real-world application
