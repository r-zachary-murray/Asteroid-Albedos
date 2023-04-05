# Asteroid-Albedos

This repository contains the ensenble of weights and catalog described in the paper "Using Neural Networks to Model Main Belt Albedos as a function of Proper Orbital Elements".  It also contains an example notebook demonstrating how to unzip, load and make predictions using the weights. 


The catalog several columns for context that are taken from the [AFP](http://asteroids.matf.bg.ac.rs/fam/) and [NEOWISE](https://sbn.psi.edu/pds/resource/neowisediam.html) datasets. 

number: MPC number

a: proper semi major axis

ecc: proper eccentricity

sinI: sin of the proper inclination

V albedo: visible albedo

V albedo error:  error in the visible albedo

IR albedo: infrared albedo

IR albedo error:  error in the infrared albedo

Diameter: Asteroid Diameter

Diameter err: Error in AsteroidDiameter

family: Integer corresponding to the asteroid family

sigma_pred_vis: error due to measurment uncertainty on $log_{10}(p_V)$

pred_vis: predicted visible abledo

sigma_belt_vis: error due to belt stocastisity on $log_{10}(p_V)$

sigma_pred_ir: error due to measurment uncertainty on $log_{10}(p_{IR})$

pred_ir: predicted infrared abledo

sigma_belt_ir: error due to belt stocastisity on $log_{10}(p_{IR})$
