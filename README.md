# StochasticReliability

## File contents

### Input files

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

* *SmartMeter*: smart meter number
* *Timestamp*: Timestamp of the data
* *A+*: Active energy produced
* *A-*: Active energy consumed
* *R+*: Reactive energy produced
* *A-*: Reactive energy consumed
* *Overload*: overload indicator (1 overloaded, 0 normal)
* *Curtailment*: curtailment indicator (1 curtailed, 0 normal)

### Output files

#### Stochastic results

[FirstMethod-Output.csv](FirstMethod-Output.csv)

Contains the first method results of each scenario

The layout of the file is on the following form:

* *Scenario*: scenario number
* *Experiment*: Instance number
* *Deterministic_CPU_Time(s)*: CPU time for the deterministic part
* *Solution_Number*: number of solution (1-5)
* *Deterministic_obj1*: Smart meters serviced
* *Deterministic_obj2*: Cabinet changes
* *Deterministic_obj3*: Fuses changes
* *UOI*: Unified Overload Index
* *UOI_std*: Unified Overload Index standard deviation
* *Error(%)*: Percentage of error
* *LB*: Lower bound
* *UB*: Upper bound
* *N*: number of simulations
* *R*: efficiency index
* *SAOFI*: SAOFI index
* *SAODI*: SAODI index
* *CAODI*: CAODI index
* *CBLSAOFI*: CBLSAOFI index
* *CBLODI*: CBLODI index
* *ASOFI*: ASOFI index
* *ASODI*: ASODI index
* *CPU_Time(ms): Total CPU time 

[SecondMethod3dec-Output.csv](SecondMethod3dec-Output.csv)

Contains the second method with 3 decimal places precision results of each scenario

[SecondMethod4dec-Output.csv](SecondMethod4dec-Output.csv)

Contains the second method with 4 decimal places precision results of each scenario

The layout of the two above files is on the following form:

* *Scenario*: scenario number
* *Experiment*: Instance number
* *Independent_run*: number of best independent run
* *Solution*: number of solution (0-4)
* *Initial_UOI* : Unified Overload Index of the input state
* *Final_UOI*: Expected UOI
* *UOI_std*: Unified Overload Index standard deviation
* *Gap(%)*: Percentage of error
* *LB*: Lower bound
* *LB_std*: Lower bound standard deviation
* *UB*: Upper bound
* *UB_std*: Upper bound standard deviation
* *SAOFI*: SAOFI index
* *SAODI*: SAODI index
* *CAODI*: CAODI index
* *CBLSAOFI*: CBLSAOFI index
* *CBLODI*: CBLODI index
* *ASOFI*: ASOFI index
* *ASODI*: ASODI index
* *Actions*: number of fuses changes
* *CPU_Time(ms): Total CPU time 

[FirstMethod-ActionPlan.csv](FirstMethod-ActionPlan.csv)

Contains the first method action plan of each scenario

* *Scenario*: scenario number
* *Experiment*: Instance number
* *Solution_Number*: number of solution (1-5)
* *obj1*: Smart meters serviced
* *obj2*: Cabinet changes
* *obj3*: Fuses changes
* *load_init_(1-31)*: initial load on cable 1-31
* *load_after_(1-31)*: load after applying the plan on cable 1-31
* *reachable_(1-31)*: reachability index after applying the plan on cable 1-31 (1 reachable, 0 unreachable) 
* *total_sm_(1-31)*: number of smart meters on cable 1-31
* *overload_init_(1-31)*: overload index (1 overload, 0 normal) 
* *curtailed_after_(1-31)*: curtailment index (1 curtailement applied, 0 no action taken)
* *startFuse_init_(1-31)*: initial start fuse state (1 close, 0 open)
* *startFuse_after_(1-31)*: start fuse state after applying the plan (1 close, 0 open)
* *endFuse_init_(1-31)*: initial end fuse state (1 close, 0 open)
* *endFuse_after_(1-31)*: end fuse state after applying the plan (1 close, 0 open)

[SecondMethod3dec-ActionPlan.csv](SecondMethod3dec-ActionPlan.csv)

Contains the second method with 3 decimal places precision action plan of each scenario

[SecondMethod4dec-ActionPlan.csv](SecondMethod4dec-ActionPlan.csv)

Contains the second method with 4 decimal places precision action plan of each scenario

The layout of the two above files is on the following form:

* *Scenario*: scenario number
* *Experiment*: Instance number
* *Solution_Number*: independent_run * 10 + number of solution (0-4)
* *obj1*: Expected Unified Overload Index
* *obj2*: Fuses changes
* *obj3*: Initial UOI
* *load_init_(1-31)*: initial load on cable 1-31
* *load_after_(1-31)*: load after applying the plan on cable 1-31
* *reachable_(1-31)*: reachability index after applying the plan on cable 1-31 (1 reachable, 0 unreachable) 
* *total_sm_(1-31)*: number of smart meters on cable 1-31
* *overload_init_(1-31)*: overload index (1 overload, 0 normal) 
* *curtailed_after_(1-31)*: curtailment index (1 curtailement applied, 0 no action taken)
* *startFuse_init_(1-31)*: initial start fuse state (1 close, 0 open)
* *startFuse_after_(1-31)*: start fuse state after applying the plan (1 close, 0 open)
* *endFuse_init_(1-31)*: initial end fuse state (1 close, 0 open)
* *endFuse_after_(1-31)*: end fuse state after applying the plan (1 close, 0 open)


## Author

* **Nikolaos Antoniadis** - [nikosantoniadis](https://github.com/nikosantoniadis) 

## License

[![Creative Commons License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc-sa/4.0/)  
This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).


