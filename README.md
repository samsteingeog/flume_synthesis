# flume_synthesis: Repository for the Flume Synthesis Project

## Developing a Functional Form of Particle Interception in Vegetated Wetlands
## Sam Stein, Laurel Larsen, and Jordan Wingenroth
## Updated on: 11/25/2019


This repository contains code to fit the following formula (from Larsen 2014): 

!["\begin{\eta_{0} \undertilde (\frac{Re_{S}}{\sqrt{(ah)(1-ad)}})^{c1}R^{*c2}(ad)^{c3}P^{c4}}"](C:\Users\samps\OneDrive\Documents\flume_synthesis\eqn_1.png)

This code calls the following variables: 

| Variable | Symbol | Unit |
| ------ | ------ | ----- |
| Collector Reynolds Number | Re_C | N/A |
| Frontal Area per Unit Volume | *a* | cm^-1
| Collector Height | *h* | cm
| Collector Diameter | *d* | cm
| Particle - Collector Radius Ratio | R* | N/A
| Particle - Water Density Ratio | P | N/A
| Contact Efficiency | eta_not (*n*_0)  | N/A

The repo contains the following files: 

* /data:
  + flume_data.csv: raw data files seperated by author and flume run
  + ...
  
* /scripts:
  + function.Rmd: fitting a log transformed linear function of the above eqn
  +...

