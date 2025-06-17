<img src="thumbnail.png" alt="thumbnail" width="300"/>

# Saharan Dust Cookbook

[![nightly-build](https://github.com/ProjectPythia/dust-cookbook/actions/workflows/nightly-build.yaml/badge.svg)](https://github.com/ProjectPythia/dust-cookbook/actions/workflows/nightly-build.yaml)
[![Binder](https://binder.projectpythia.org/badge_logo.svg)](https://binder.projectpythia.org/v2/gh/ProjectPythia/dust-cookbook/main?labpath=notebooks)
[![DOI](https://zenodo.org/badge/813731923.svg)](https://zenodo.org/badge/latestdoi/813731923)

This Project Pythia Cookbook explores the relationship between Sharan dust aerosols (Bodèlè source) and meteorological variables using Self-Organizing Maps (SOM), Principal Component Analysis (PCA), and Random Forest Regression (RF).  

## Motivation

Several meteorological and land surface factors have been found to impact Saharan dust emissions and transport. Dust mobilization occurs when surface wind speed of suitable magnitude is above a threshold velocity, often computed based on soil characteristics, vegetation, and solid particles. The purpose of this cookbook is to understand the relationship between dust and some meteorological variables using self-organizing maps ([SOM](ttps://medium.com/machine-learning-researcher/self-organizing-map-som-c296561e2117)), random forest regression ([RF](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)), and principal component analysis (PCA). The question we are really interested in with this cookbook is to know which variables are the most predictive of dust emissions. 

For experimenting purpose, we consider PM10 concentration (PM10), 2m temperature (T2), 2m relative humidity (rh2), planetary boundary layer height (PBLH), 10m wind speed (wind_speed_10m), 925hPa wind speed (wind_speed_925hPa), horizontal wind at 10m (U10), meridional wind at 10m (V10), and convective rainfall (RAINC). This cookbook seeks to establish a clear relationship between the meteorological variables and dust (PM10).

## Authors

[Jacob Tindan](@Jtindan), [Pooja Hari Ambrish](@Pha03), [Altug Karakurt](@altugkarakurt), [Ali Fallah](@alifallahm) Acknowledge primary content authors here_

### Contributors

<a href="https://github.com/ProjectPythia/dust-cookbook/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ProjectPythia/dust-cookbook" />
</a>

## Structure

(State one or more sections that will comprise the notebook. E.g., _This cookbook is broken up into two main sections - "Foundations" and "Example Workflows."_ Then, describe each section below.)

### Section 1 ( Replace with the title of this section, e.g. "Foundations" )

(Add content for this section, e.g., "The foundational content includes ... ")

### Section 2 ( Replace with the title of this section, e.g. "Example workflows" )

(Add content for this section, e.g., "Example workflows include ... ")

## Running the Notebooks

You can either run the notebook using [Binder](https://binder.projectpythia.org/) or on your local machine.

### Running on Binder

The simplest way to interact with a Jupyter Notebook is through
[Binder](https://binder.projectpythia.org/), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) in the cloud. The details of how this works are not
important for now. All you need to know is how to launch a Pythia
Cookbooks chapter via Binder. Simply navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Binder”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

### Running on Your Own Machine

If you are interested in running this material locally on your computer, you will need to follow this workflow:

(Replace "cookbook-example" with the title of your cookbooks)

1. Clone the `https://github.com/ProjectPythia/cookbook-example` repository:

   ```bash
    git clone https://github.com/ProjectPythia/cookbook-example.git
   ```

1. Move into the `cookbook-example` directory
   ```bash
   cd cookbook-example
   ```
1. Create and activate your conda environment from the `environment.yml` file
   ```bash
   conda env create -f environment.yml
   conda activate cookbook-example
   ```
1. Move into the `notebooks` directory and start up Jupyterlab
   ```bash
   cd notebooks/
   jupyter lab
   ```
