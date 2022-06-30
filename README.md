# EDS 232: Machine Learning in Environmental Science (Winter Quarter 2022) - Species Distribution Models  
## [Course website](https://bbest.github.io/eds232-ml/)
## Instructor: Ben Best
## Student author: Mia Forsline 
### Due 2022-01-19

## Motivation and project goal
This assignment is designed to teach the fundamentals of building, calibrating, and evaluating a species distribution model (SDM) using a variety of methods such as regressions and decision trees. Specifically, I am interested in the distribution of the common mudpuppy salamander, *Necturus maculosus*. To build the model, I am using species observation data points from the [Global Biodiversity Information Facility (GBIF)](https://www.gbif.org/). 

## Intended purpose and important concepts
This project is intended for educational purposes, and the student author practiced the following:
- fetching species observation data from GBIF using an API 
- fetching environmental data from [WorldClim](https://worldclim.org/) and [ENVIREM](https://envirem.github.io/) to build a raster and define the environmental relationship for the SDM 
- generate pseudo-absence data
- use pair plots to visualize correlation between environmental variables and minimize multicollinearity issues
- explore a variety of logistic regression techniques to understand why Maxent (Maximum Entropy) is such a powerful and commonly used tool
  - linear model 
  - generalized linear model 
  - generalized additive model
  - Maxent
- explore how decision trees and random forests can be used to classify categorical presence/absence data 
- calibrate and evaluate the model 

## Future research
Future research aims to inform policy regarding renewable wind energy in the United States and abroad. Additionally, further research could explore different scenarios, other than the two housing scenarios included in this study.

## Installation
The following packages were utilized during this analysis:
- `sqlalchemy`
- `psycopg2`
- `geopandas`
- `math`

## Data
Data for this analysis is NOT hosted in the repository because the source code directly pulls all data from [WorldClim](https://worldclim.org/) and [ENVIREM](https://envirem.github.io/). Data was incorporated using following file structure.

- eds232-species (_repository_)
    - README.md
    - .gitignore
    - eds232-species.Rproj
    - obs.geojson
    - javac
    - RMD files
    - HTML files
    - JPEG files
    - /data (_data_)
      - /env

## Assignment overview: 
1. [Explore the data](https://bbest.github.io/eds232-ml/lab1a_sdm-explore.html)
2. [Logistic regression](https://bbest.github.io/eds232-ml/lab1b_sdm-regress.html)
3. [Decision trees and random forests](https://bbest.github.io/eds232-ml/lab1b_sdm-regress.html)
4. [Evaluate](https://bbest.github.io/eds232-ml/lab1d_sdm-evaluate.html)
