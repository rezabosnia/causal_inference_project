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
* `pandas`, `numpy`, `scikit-learn`
* `causalml` for uplift modeling and evaluation
* `econml` and `DoubleML` for ATE/HTE estimation
* `networkx` and `graphviz` for DAG visualization
* AWS SageMaker (for deployment pipeline)

## Requirements

* Python 3.8+
* pip or conda environment
* Jupyter Notebook or compatible IDE
* Credentials for AWS (if using SageMaker for scoring pipeline)

## Installation Instructions

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/causal-inference-project.git
   cd causal-inference-project
   ```

2. Create virtual environment (optional):

   ```bash
   python -m venv env
   source env/bin/activate  # or .\env\Scripts\activate on Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage Instructions

* Run `notebooks/` for step-by-step exploration:

  * `01_dag_analysis.ipynb`: Build and analyze causal DAGs
  * `02_ate_estimation.ipynb`: Estimate ATE using DoubleML and OLS
  * `03_mediation_analysis.ipynb`: Decompose direct vs indirect effects
  * `04_hte_analysis.ipynb`: Explore treatment heterogeneity
  * `05_uplift_modeling.ipynb`: Train and evaluate uplift models

* Pre-trained uplift model can be loaded with:

  ```python
  with open('uplift_rf_model.pkl', 'rb') as f:
      uplift_rf_loaded = pickle.load(f)
  ```

## Documentation

See `docs/` for full methodology explanations, assumptions, and interpretation guidelines. Key methods include:

* Causal DAG construction
* DoubleML for ATE under confounding
* Uplift modeling for ITE estimation
* AUUC and Qini metrics for evaluation

## Visuals

* DAG diagrams (experiment and mediation setup)
* Uplift gain curve visualizations
* Feature importance plots from trained uplift model

## Support Information

For questions or collaboration:

* **Author**: Muhammad Reza Tribosnia
* **Email**: \[[your-email@example.com](mailto:your-email@example.com)]
* UCL MSc Business Analytics, Class of 2025

## Project Roadmap

* [x] Apply causal inference methods to real A/B test data
* [x] Evaluate ATE, HTE, ITE, and mediation
* [x] Deploy monthly uplift scoring pipeline to AWS SageMaker
* [ ] Validate uplift predictions with future experiments
* [ ] Expand dataset coverage to improve generalization

## Project Status

**Completed (Internship phase finished – August 2025)**
Deployment-ready uplift model developed and evaluated. Future iterations will focus on validation and scaled deployment.

## Contribution Guidelines

This project is currently closed for contributions during the dissertation period. Future collaboration may be opened post-submission.

## License

MIT License (or specify your own if different)

## Useful Links

* [CausalML Documentation](https://causalml.readthedocs.io/)
* [DoubleML GitHub](https://github.com/DoubleML/doubleml-for-py)
* [Econometrics & Machine Learning Notes](https://www.econml.ai/)
