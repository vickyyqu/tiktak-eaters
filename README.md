<img src = https://github.com/vickyyqu/tiktak-eaters/assets/112297073/ff8dc8e8-2668-4262-9c79-71454d6ade17 height=300px >

# TikTok Hackathon Challenge 2023: Team Tiktak Eaters

We are a team of 5 undergraduate students from Singapore Management University participating in the TikTok Hackathon Challenge 2023. We are tackling Problem Statement 1 - Optimize Advertisement Moderation, and this repository showcases our project and solution to the proposed problem.


## Table of Contents
- [Problem Statement](#problem)
- [Introduction](#introduction)
- [Installation](#installation)
- [Additional Notes](#additional)


## Problem Statement

The chosen problem statement for this project revolves around creating a stochastic optimization model to:
1. Dynamically score and prioritise social media advertisements for review
2. Dynamically score the performance of a moderator in moderating ads
3. Match content to be reviewed with the best fitting moderator


## Introduction

To resolve the problem, our team has created a stochastic optimization model that assigns scores to both advertisements and moderators. These scores facilitate the matching of advertisements with moderators, with high-scoring advertisements requiring moderators with similarly strong performance scores. 
The expected outcomes of this projects include:
- General priority score for advertisements
- General performance score for moderators
- Efficient allocation of advertisements to appropriate moderators
  
Through data preprocessing and feature engineering, our aim is not only to assign advertisements based on their scores, but also to consider subregional similarities when there is a shortage of moderators in specific regions.
We then conducted multivariate linear optimization and thereafter a mapping algorithm to best place an advertisement to the most suitable moderator.


## Installation

### To clone this repository:

```bash
$ git clone https://github.com/vickyyqu/tiktak-eaters
$ cd yourproject
$ npm install
```

### To run our project:

1. Run all cells in 'ad_optimisation.ipynb' and 'moderator_optimisation.ipynb' for the ad priority score and moderator performance score optimisation and saved as CSV files stored in 'intermediate' ('ads_data.xlsx' and 'moderators_data.xlsx').
2. Run all cells in 'subregion.ipynb' to generate the mapped markets to subregions and saved as Excel sheets stored in 'intermediate' ('ads_data_final.xlsx' and 'mods_data_final.xlsx').
3. Run all cells in 'mapping.ipynb' to map each ad to a moderator (final output csv stored in 'output' as 'output.csv').


## Additional Notes

- The file size of 'ad_optimisation.ipynb' is too large to be viewed on the GitHub website, to view the notebook and its contents, please clone the repository or download the files.
- 'country_codes.xlsx' in 'data' is an external Excel sheet retrieved from ISO via https://github.com/datasets/country-codes/blob/master/data/country-codes.csv, and used in the mapping of markets to subregions for ads and moderators in 'mapping.ipynb'.
