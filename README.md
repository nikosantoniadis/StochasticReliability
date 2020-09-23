# StochasticReliability

## File contents

[Cabinets_public.csv](Cabinets_public.csv)

Contains the data for the cabinets of the smart grid

The layout is on the following form:
Cabinet,Latitude,Longitude,Substation

* *Cabinet*: cabinet number
* *Latitude*: latitude of the cabine<sup>*</sup>
* *Longitude*: longitude of the cabinet<sup>*</sup>
* *Substation*: substation indicator (1 substation, 0 normal cabinet)


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


