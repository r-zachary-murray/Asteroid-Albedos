# Asteroid-Albedos

This repository contains the ensenble of weights and catalog described in the paper "Using Neural Networks to Model Main Belt Albedos as a function of Proper Orbital Elements".  It also contains an example notebook demonstrating how to unzip, load and make predictions using the weights. 


### The catalog several columns for context that are taken from the [AFP](http://asteroids.matf.bg.ac.rs/fam/) and [NEOWISE](https://sbn.psi.edu/pds/resource/neowisediam.html) datasets. These columns are documented below.

<div align="center">
  <table>
    <tr>
      <th>Row</th>
      <th>Definition</th>
    </tr>
    <tr>
      <td>number</td>
      <td>MPC number</td>
    </tr>
    <tr>
      <td>a</td>
      <td>Proper semi-major axis</td>
    </tr>
    <tr>
      <td>ecc</td>
      <td>Proper eccentricity</td>
    </tr>
    <tr>
      <td>sinI</td>
      <td>Sin of the proper inclination</td>
    </tr>
    <tr>
      <td>V albedo</td>
      <td>Visible albedo</td>
    </tr>
    <tr>
      <td>V albedo error</td>
      <td>Error in the visible albedo</td>
    </tr>
    <tr>
      <td>IR albedo</td>
      <td>Infrared albedo</td>
    </tr>
    <tr>
      <td>IR albedo error</td>
      <td>Error in the infrared albedo</td>
    </tr>
    <tr>
      <td>Diameter</td>
      <td>Asteroid Diameter</td>
    </tr>
    <tr>
      <td>Diameter err</td>
      <td>Error in Asteroid Diameter</td>
    </tr>
    <tr>
      <td>family</td>
      <td>Integer corresponding to the asteroid family</td>
    </tr>
    <tr>
      <td>sigma_pred_vis</td>
      <td>Error due to measurement uncertainty on $log_{10}(p_V)$</td>
    </tr>
    <tr>
      <td>pred_vis</td>
      <td>Predicted visible albedo</td>
    </tr>
    <tr>
      <td>sigma_belt_vis</td>
      <td>Error due to belt stochasticity on $log_{10}(p_V)$</td>
    </tr>
    <tr>
      <td>sigma_pred_ir</td>
      <td>Error due to measurement uncertainty on $log_{10}(p_{IR})$</td>
    </tr>
    <tr>
      <td>pred_ir</td>
      <td>Predicted infrared albedo</td>
    </tr>
    <tr>
      <td>sigma_belt_ir</td>
      <td>Error due to belt stochasticity on $log_{10}(p_{IR})$</td>
    </tr>
  </table>
</div>

