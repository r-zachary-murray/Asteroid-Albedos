[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7778016.svg)](https://doi.org/10.5281/zenodo.7796840)

 

# Predicting Asteroid Albedos using Neural Networks

This repository contains supplementary information from the paper [Using neural networks to model Main Belt Asteroid albedos as a function of their proper orbital elements](https://arxiv.org/abs/2305.16392).  It consists of two parts.  

1) A catalog of over 500,000 asteroids with albedos inferred from their proper elements.  This is useful if one desires a quick lookup of a previously known asteroid.

2) The weights used by the Neural Network ensemble to generate these predictions.  These are useful if one desires to make a prediction about a newly discovered body whose proper orbital elements have yet to be computed.  It also contains an example notebook demonstrating how to unzip, load, and make predictions using the weights. 

## The catalog includes the following columns.  Their definitions are as follows:  
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

<p align="center"><em>Note that, for context, the catalog several columns for context that are taken from the <a href="http://asteroids.matf.bg.ac.rs/fam/">AFP</a> and   
  <a href="https://sbn.psi.edu/pds/resource/neowisediam.html">NEOWISE</a>.  This catalog, as a csv file is available in this repository as 'albedos_murray_2023.csv'. </em></p>


## The weights themselves can also be used to make predictions. 

These weights are saved as HDF5 files and no special package needs to be installed to use them.  However, Tensorflow and Keras must be installed to load and interact with these files.  Both packages can be installed at once by using pip. 

    pip install tensorflow

Once these packages are installed, copy the appropriate weights ("vis_ensemble" for visible albedos) into your working directory along with "scaler.pkl" and the "Example.ipynb" notebook. The notebook contains helper functions and a fully worked example showing how to make a prediction.  

If all else fails, feel free to raise an issue via Github or reach out to the author directly: 

* Zachary Murray, Center for Astrophysics | Harvard & Smithsonian, <zachary.murray@cfa.harvard.edu>
















































