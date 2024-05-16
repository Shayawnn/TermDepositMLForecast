# TermDepositMLForecast

## Table of Contents

1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Setup Instructions](#setup-instructions)
4. [Notebook](#notebook)
5. [Results](#results)
6. [License](#license)

## Introduction <a name="introduction"></a>

The project's goal is to predict whether clients of a Portuguese banking institution will subscribe to a term deposit based on data from direct marketing campaigns. This repository contains the analysis, machine learning models, and visualizations used to compare the performance of Logistic Regression, Random Forest, and SVM classifiers.

## Dataset

The dataset used in this project comes from direct marketing campaigns (phone calls) of a Portuguese bank. It includes client demographics, campaign details, and previous interactions, focusing on whether the client subscribed to a term deposit. The dataset is split into multiple files with varying levels of detail and sample sizes to facilitate different computational needs. This data is sourced from [UC Irvine Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing).

## Setup Instructions

### Prerequisites

- Python 3.8 or later. You can download it from [here](https://www.python.org/downloads/).
- pip. It is already installed if you have Python 2 >=2.7.9 or Python 3 >=3.4 downloaded from python.org. If not, you can download it from [here](https://pip.pypa.io/en/stable/installation/).

### Installing

To set up this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/Shayawnn/TermDepositMLForecast.git
   ```
2. Navigate to the project directory:
    ```bash
    cd TermDepositMLForecast
    ```
3. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

## Notebook

The notebook is named `main.ipynb` and can be found in the `notebook` directory. It can be run in Jupyter Notebook or Jupyter Lab. If you're not familiar with these tools, you might find these getting started guides helpful:

- [Jupyter Notebook](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/)
- [Jupyter Lab](https://jupyterlab.readthedocs.io/en/latest/getting_started/overview.html)

You can start the notebook by navigating to the `notebook` directory and executing the command `jupyter notebook` or `jupyter lab`, depending on your setup. This will start a local server and open a tab in your web browser from where you can open `main.ipynb`.

## Results <a name="results"></a>

The analysis revealed that the Random Forest model provided the best performance in terms of accuracy and ROC AUC, indicating its superior capability in handling the complexity of the dataset.

Key findings from our feature importance analysis highlighted that the duration of the last contact, several economic indicators, and the outcome of previous campaigns were critical in influencing clients' decisions. These insights suggest that enhancing client interaction quality and timing could significantly impact subscription rates.

However, the variance in performance metrics, particularly the difference in training and testing accuracy for the Random Forest model, suggests a potential overfitting issue that needs addressing in future model tuning efforts.

## License <a name="license"></a>

This project is licensed under the terms of the [GNU General Public License v3.0](LICENSE).

