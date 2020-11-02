# flume_synthesis: Repository for the Flume Synthesis Project

### Developing a Functional Form of Particle Interception in Vegetated Wetlands
### Sam Stein, Laurel Larsen, and Jordan Wingenroth
### Updated on: 11/1/2020


This repository contains code to fit the following formula (from Stein et al., *in prep*): 

 $ \ln (\eta) \sim c_{0} + c_{1}\ln \left( \frac{\text{Re}_{c}}{\sqrt{ah(1-ad_{c})}} \right) + c_{2}\ln(ad_{c}) + c_{3}\ln(\text{P}) + c_{4}\ln(\text{R}^{\ast}) $

<a href="https://www.codecogs.com/eqnedit.php?latex=\ln&space;(\eta)&space;\sim&space;c_{0}&space;&plus;&space;c_{1}\ln&space;\left(&space;\frac{\text{Re}_{c}}{\sqrt{ah(1-ad_{c})}}&space;\right)&space;&plus;&space;c_{2}\ln(ad_{c})&space;&plus;&space;c_{3}\ln(\text{P})&space;&plus;&space;c_{4}\ln(\text{R}^{\ast})" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\ln&space;(\eta)&space;\sim&space;c_{0}&space;&plus;&space;c_{1}\ln&space;\left(&space;\frac{\text{Re}_{c}}{\sqrt{ah(1-ad_{c})}}&space;\right)&space;&plus;&space;c_{2}\ln(ad_{c})&space;&plus;&space;c_{3}\ln(\text{P})&space;&plus;&space;c_{4}\ln(\text{R}^{\ast})" title="\ln (\eta) \sim c_{0} + c_{1}\ln \left( \frac{\text{Re}_{c}}{\sqrt{ah(1-ad_{c})}} \right) + c_{2}\ln(ad_{c}) + c_{3}\ln(\text{P}) + c_{4}\ln(\text{R}^{\ast})" /></a>

This code calls the following variables: 

| Variable | Symbol | Unit |
| ------ | ------ | ----- |
| Collector Reynolds Number | Re_c | N/A |
| Frontal Area per Unit Volume | *a* | L^-1
| Collector Height | *h* | L
| Collector Diameter | *d_c* | L
| Particle - Collector Radius Ratio | R* | N/A
| Particle - Water Density Ratio | P | N/A
| Capture Efficiency | eta (*n*)  | N/A

The repo contains the following files: 

* /data:
  + flume_data.csv: raw data files seperated by author and flume run
  + ...
  
* /scripts:
  + function.Rmd: fitting a log transformed linear function of the above eqn
  +...

