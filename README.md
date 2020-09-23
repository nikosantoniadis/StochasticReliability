# StochasticReliability

## File contents

[Cabinets_public.csv](Cabinets_public.csv)

Contains the data for the cabinets of the smart grid

The layout is on the following form:

* *Cabinet*: cabinet number
* *Latitude*: latitude of the cabinet<sup>*</sup>
* *Longitude*: longitude of the cabinet<sup>*</sup>
* *Substation*: substation indicator (1 substation, 0 normal cabinet)

<sup>*</sup> For privacy purposes, we substituted the coordinates to the easternmost Greek territory, the uninhabited island Strongyli. 

[Smartmeters_public.csv](Smartmeters_public.csv)

Contains the data for the smart meters of the smart grid

The layout is on the following form:

* *SmartMeter*: smart meter number
* *Latitude*: latitude of the smart meter<sup>*</sup>
* *Longitude*: longitude of the smart meter<sup>*</sup>
* *Cable*: connection cable number of the smart meter 

<sup>*</sup> For privacy purposes, we substituted the coordinates to the easternmost Greek territory, the uninhabited island Strongyli. 

[Cables_original.csv](Cables_original.csv)

Contains the data for the cables of the smart grid

The layout is on the following form:

* *Cable*: cable number
* *MaxLoad*: maximum load of the cable
* *Start_Fuse*: start fuse number of the cable
* *End_Fuse*: end fuse number of the cable

[Fuses_original.csv](Fuses_original.csv)

Contains the data for the fuses of the smart grid

The layout is on the following form:

* *Fuse*: fuse number
* *Cabinet*: cabinet number of the fuse

(Consumption_X_Y.csv)

Contains the consumption data of the X scenario, Y instance

SmartMeter,Timestamp,A+,A-,R+,R-,Overload,Curtailment
* *SmartMeter*: smart meter number
* *Timestamp*: Timestamp of the data
* *A+*: Active energy produced
* *A-*: Active energy consumed
* *R+*: Reactive energy produced
* *A-*: Reactive energy consumed
* *Overload*: overload indicator (1 overloaded, 0 normal)
* *Curtailment*: curtailment indicator (1 curtailed, 0 normal)

[obj3.csv](obj3.csv)

Contains the results of the third objective (percentage of changed fuses) of each scenario

The layout of the (obj1.csv),(obj2.csv), and (obj3.csv) is on the following form:

* *Scenario*: scenario number
* *Average*: the arithmetic mean of the experiments 
* *CI-L*: Lower bound of the 99% confidence interval 
* *CI-H*: Upper bound of the 99% confidence interval



## Author

* **Nikolaos Antoniadis** - [nikosantoniadis](https://github.com/nikosantoniadis) 

## License

[![Creative Commons License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc-sa/4.0/)  
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).


