# Asteroid-Albedos

This repository contains the ensenble of weights and catalog described in the paper "Using Neural Networks to Model Main Belt Albedos as a function of Proper Orbital Elements".  It also contains an example notebook demonstrating how to unzip, load and make predictions using the weights. 


### The catalog several columns for context that are taken from the [AFP](http://asteroids.matf.bg.ac.rs/fam/) and [NEOWISE](https://sbn.psi.edu/pds/resource/neowisediam.html) datasets. These columns are documented below.

| Row             | Definition                                  |
|-----------------|---------------------------------------------|
| number          | MPC number                                  |
| a               | Proper semi-major axis                      |
| ecc             | Proper eccentricity                         |
| sinI            | Sin of the proper inclination               |
| V albedo        | Visible albedo                             |
| V albedo error  | Error in the visible albedo                |
| IR albedo       | Infrared albedo                            |
| IR albedo error | Error in the infrared albedo               |
| Diameter        | Asteroid Diameter                          |
| Diameter err    | Error in Asteroid Diameter                 |
| family          | Integer corresponding to the asteroid family |
| sigma_pred_vis  | Error due to measurement uncertainty on $log_{10}(p_V)$ |
| pred_vis        | Predicted visible albedo                   |
| sigma_belt_vis  | Error due to belt stochasticity on $log_{10}(p_V)$    |
| sigma_pred_ir   | Error due to measurement uncertainty on $log_{10}(p_{IR})$ |
| pred_ir         | Predicted infrared albedo                  |
| sigma_belt_ir   | Error due to belt stochasticity on $log_{10}(p_{IR})$  |
