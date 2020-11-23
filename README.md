# flume_synthesis: Repository for the Flume Synthesis Project

### A Functional Form for Particle Interception in Vegetated Environments 
### Sam Stein, Laurel Larsen, and Jordan Wingenroth
### Updated on: 11/1/2020


This repository contains code to fit the following formula (from Stein et al., *in prep*): 
<a href="https://www.codecogs.com/eqnedit.php?latex=\ln&space;(\eta)&space;\sim&space;c_{0}&space;&plus;&space;c_{1}\ln&space;\left(&space;\frac{\text{Re}_{c}}{\sqrt{ah(1-ad_{c})}}&space;\right)&space;&plus;&space;c_{2}\ln(ad_{c})&space;&plus;&space;c_{3}\ln(\text{P})&space;&plus;&space;c_{4}\ln(\text{R}^{\ast})" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\ln&space;(\eta)&space;\sim&space;c_{0}&space;&plus;&space;c_{1}\ln&space;\left(&space;\frac{\text{Re}_{c}}{\sqrt{ah(1-ad_{c})}}&space;\right)&space;&plus;&space;c_{2}\ln(ad_{c})&space;&plus;&space;c_{3}\ln(\text{P})&space;&plus;&space;c_{4}\ln(\text{R}^{\ast})" title="\ln (\eta) \sim c_{0} + c_{1}\ln \left( \frac{\text{Re}_{c}}{\sqrt{ah(1-ad_{c})}} \right) + c_{2}\ln(ad_{c}) + c_{3}\ln(\text{P}) + c_{4}\ln(\text{R}^{\ast})" /></a>

which calls the following variables: 

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
  + flume_review_data.csv: experimental flume data for fitting the model
  + mudd_data.csv: data set to recreate Mudd et al., 2010 Figure 5 using our new functional form for particle capture
  + data_40.csv: data set of typical marsh flow and vegetation conditions w/ 40um sized particles 
  
* /scripts:
  + flume_model.Rmd: markdown file to fit the above eqn and integrate it into the model for marsh elevation change presented in Mudd et al., 2010. 

References:

Mudd, S.M.;  D’Alpaos, A.;  Morris, J.T.   How does vegetation affect sedimentation on tidal marshes? Investigating particle capture and hydrodynamic controls on biologically mediated sedimentation. *Journal of Geophysical Research: Earth Surface* 2010, *115*, 1–14.  doi:10.1029/2009JF001566.
