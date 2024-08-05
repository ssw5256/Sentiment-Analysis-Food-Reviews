
# Sentiment Analysis on Amazon Reviews

This repository contains a Jupyter Notebook that performs sentiment analysis on Amazon Fine Food Reviews using two techniques: the VADER lexicon-based approach and the RoBERTa pretrained model from Hugging Face.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Dataset](#dataset)
- [Usage](#usage)
- [Notebook Overview](#notebook-overview)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Overview

The goal of this project is to analyze the sentiment of Amazon Fine Food Reviews using two different sentiment analysis methods:

1. **VADER (Valence Aware Dictionary and sEntiment Reasoner)**: A lexicon and rule-based sentiment analysis tool specifically attuned to sentiments expressed in social media.
2. **RoBERTa (Robustly optimized BERT approach)**: A transformer model trained on a large corpus of text data to understand and predict sentiment.

## Installation

To run the notebook, you'll need to have Python installed along with several packages. The following instructions will help you set up the environment.

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/sentiment-analysis-amazon-reviews.git
   cd sentiment-analysis-amazon-reviews
   ```

2. **Install dependencies**:
   You can install the required packages using `pip`:
   ```bash
   pip install -r requirements.txt
   ```
   Alternatively, if you prefer using conda:
   ```bash
   conda create --name sentiment-analysis python=3.8
   conda activate sentiment-analysis
   pip install -r requirements.txt
   ```

## Dataset

The dataset used in this notebook is the Amazon Fine Food Reviews dataset. It can be downloaded from [Kaggle](https://www.kaggle.com/snap/amazon-fine-food-reviews). The dataset should be placed in a directory path `$[systemfolder]/$(pathToRepo)` or you can modify the path in the notebook to match your local setup.

## Usage

Once you have the repository cloned and the dependencies installed, you can run the Jupyter Notebook to reproduce the analysis.

1. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
2. **Open the notebook**: 
   - Navigate to the notebook file in your Jupyter Notebook interface and open it.
   - Run the cells sequentially to perform the analysis.

## Notebook Overview

The notebook is divided into the following sections:

1. **Import Libraries**: Importing necessary libraries such as Pandas, NumPy, NLTK, and Transformers.
2. **Data Loading**: Reading the Amazon Reviews dataset and performing an initial exploration.
3. **VADER Sentiment Analysis**: Applying VADER to perform sentiment analysis on the reviews.
4. **Visualizing VADER Results**: Plotting the distribution of sentiment scores and visualizing results with Seaborn.
5. **RoBERTa Sentiment Analysis**: Using a pre-trained RoBERTa model to perform sentiment analysis.
6. **Combining Results**: Merging VADER and RoBERTa results and analyzing correlations.
7. **Visualizing Combined Results**: Visualizing the combined sentiment analysis results.
8. **Examples**: Exploring specific reviews with strong positive or negative sentiment as predicted by both models.

## Results

The sentiment analysis provides insights into how customers feel about products based on their reviews. The combined use of VADER and RoBERTa allows for a robust analysis, showcasing the strength of each model in capturing nuances in sentiment.

- **Visualizations**: The notebook includes several visualizations such as bar plots and pair plots to compare sentiment scores.
- **Sentiment Predictions**: The final section compares predictions from both models for various reviews, highlighting differences in sentiment interpretation.




## Acknowledgements

- The **Amazon Fine Food Reviews** dataset was used for this analysis.
- **VADER** and **Hugging Face Transformers** were utilized for sentiment analysis.
- Special thanks to the open-source community for providing the tools and datasets that made this project possible.