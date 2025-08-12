# causal-inference-project

## Description

This project applies modern **causal inference methods** to improve A/B test analysis beyond average treatment effects (ATE) to uncover **how**, **why**, and **for whom** an intervention works. Conducted as part of a UCL MSc Business Analytics project in collaboration with **The Economist**, the study integrates DAGs, DoubleML, mediation analysis, HTE, and uplift modeling to drive more precise and personalized experimentation strategies.

## Table of Contents

* [Technologies Used](#technologies-used)
* [Requirements](#requirements)
* [Installation Instructions](#installation-instructions)
* [Usage Instructions](#usage-instructions)
* [Documentation](#documentation)
* [Visuals](#visuals)
* [Support Information](#support-information)
* [Project Roadmap](#project-roadmap)
* [Project Status](#project-status)
* [Contribution Guidelines](#contribution-guidelines)
* [License](#license)
* [Useful Links](#useful-links)

## Technologies Used

* Python 3.x
* `pandas`, `numpy`, `scikit-learn`, `statsmodels`
* `causalml` for uplift modeling and evaluation
* `econml` and `DoubleML` for ATE/HTE estimation

## Requirements

* Python== 3.12.9
* numpy==2.2.5


## Usage Instructions

* Run `notebooks/` for step-by-step exploration:

  * `causal_inference_code.ipynb`: Download and Preprocess A/B Test Data, Decompose Treatment Effects
  * `uplift_modeling.ipynb`: Estimate ITE using Uplift Modeling
  * `outsample_prediction_uplift_modeling.ipynb`: Uplift Modeling Prediction on Unseen Data

## Documentation

See `docs/` for full methodology explanations, assumptions, and interpretation guidelines. 

## Support Information

For questions or collaboration:
* **Author**: Muhammad Reza Tribosnia
* **Email**: \[[rezabosnia@gmail.com](mailto:rezabosnia@gmail.com)]

