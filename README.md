# StochasticReliability

# Preventing Overloading Incidents on Smart Grids: A Multiobjective Combinatorial Optimization Approach
Results and the presentation of the paper *Preventing Overloading Incidents on Smart Grids: A Multiobjective Combinatorial Optimization Approach* that will be presented on the 3rd International Conference on Optimization and Learning (OLA2020), Cadiz, Spain, 17-19 February 2020. 

## Presentation

[OLA_Presentation_19_Feb_2020-Final.pdf](OLA_Presentation_19_Feb_2020-Final.pdf)

The slides of the presentation on the 3rd International Conference on Optimization and Learning (OLA2020), Cadiz, Spain, 17-19 February 2020.

## File contents

[scenarios.csv](scenarios.csv)

Contains the information of the 216 scenarios we used in our experiments

The layout is on the following form:
* *Scenario*: scenario number
* *ProdOv*: percentage of overloaded producers 
* *ConsOv*: percentage of overloaded consumers 
* *ProdCur*: percentage of curtailed producers
* *ConsCur*: percentage of curtailed consumers

[obj1.csv](obj1.csv)

Contains the results of the first objective (percentage of connected users) of each scenario

[obj2.csv](obj2.csv)

Contains the results of the second objective (percentage of visiting cabinets) of each scenario

[obj3.csv](obj3.csv)

Contains the results of the third objective (percentage of changed fuses) of each scenario

The layout of the (obj1.csv),(obj2.csv), and (obj3.csv) is on the following form:

* *Scenario*: scenario number
* *Average*: the arithmetic mean of the experiments 
* *CI-L*: Lower bound of the 99% confidence interval 
* *CI-H*: Upper bound of the 99% confidence interval

[timings.csv](timings.csv)

Contains the running time for each experiment

* *ID*: experiment number
* *Scenario*: scenario number
* *Time*: running time of the experiment (in msec) 


## Author

* **Nikolaos Antoniadis** - [nikosantoniadis](https://github.com/nikosantoniadis) 

## License

[![Creative Commons License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc-sa/4.0/)  
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).


