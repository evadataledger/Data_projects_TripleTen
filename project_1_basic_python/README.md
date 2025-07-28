# Project 1: Basic Python - IMDb Raing Analysis - IMDb Golden Age Analysis

This project explores the following assumption: 

> **Do highly-rated TV shows from the "Golden Age of Television" (1999-present) also receive the most IMDb votes?**

Originally developed during the **TripleTen Data Science Bootcamp**, this project has been expanded to include two versions: 
- A guided project based on TripleTen's curriculum
- An independent extension using a public IMDb dataset

## Project Versions

### `Project_1_Basic_TripleTen.ipynb`
- Follows the original TripleTen project structure (Stage 1-3)
- Assumption: Highly-rated **TV shows** also receive the most votes
- Pubic IMDb dataset is used to simulate the original closed dataset

### `Project_IMDB_Top1000.ipynb`
- Independent extension using the **IMDb Top 1000** dataset from Kaggle
- Focuses on movies from 1999 onward
- Broader EDA with correlation analysis, visualizations, and insights

## Objective 
Analyze whether highly-rated movies and TV shows released from 1999 onward also received the most IMDb votes. 
The assumption is that popularity and quality are directly related - this project test that theory. 

## Tools Used
- Python (`pandas`, `matplotlib`)
- Jupyter Notebook

## Key Insights
- A **moderate correlation** (r=0.45) was observed between ratings and vote counts.
- Some highly-rated shows/movies had few votes - popularity and quality don't always align.
- Logarithmic scaling was useful to visualize skewed vote counts.
- Critical review scores (`meta_score`) had wider variance than user ratings.

## Data
This version uses the public [IMDb Top 1000 dataset](https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows) from Kaggle.
For data paths and details, see:  '/data/README.md'

## What I learned
- Clean and explore real-world datasets.
- Handle missing data with imputation or omission
- Normalize messy column names programmiatically
- Use scatterplots, `corr()`, and log scales for skewed data
- Test and interpret assumptions with EDA 

## Structure 
The `requirements.txt` file lists all Python libraries needed to run this project.  
It can be used to install dependencies with:

```bash
pip install -r requirements.txt

project_1_basic_python/
├── notebooks/
│   ├── Project_1_Basic_TripleTen.ipynb
│   └── Project_1_IMDB_Top1000.ipynb
├── requirements.txt   # dependencies used in this project
├── README.md

