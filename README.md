# Project Name

#### -- Project Status: [Active, On-Hold, Completed]

## Project Intro/Objective
The purpose of this project is ________. (Describe the main goals of the project and potential civic impact. Limit to a short paragraph, 3-6 Sentences)

### Collaborators
|Name     |  Github Page   |  Personal Website  |
|---------|-----------------|--------------------|
|Misha Berrien | [mishaberrien](https://github.com/mishaberrien)| [www.mishaberrien.com](https://mishaberrien.com/)  |

### Methods Used
* Inferential Statistics
* Machine Learning
* Data Visualization
* Predictive Modeling
* etc.

### Technologies
* R
* Python
* D3
* PostGres, MySql
* Pandas, jupyter
* HTML
* JavaScript
* etc.

## Project Description
(Provide more detailed overview of the project.  Talk a bit about your data sources and what questions and hypothesis you are exploring. What specific data analysis/visualization and modelling work are you using to solve the problem? What blockers and challenges are you facing?  Feel free to number or bullet point things here)


## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](Repo folder containing raw data) within this repo.
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...
5. Follow setup [instructions](Link to file)

## Featured Notebooks/Analysis/Deliverables
* [Notebook/Markdown/Slide Deck Title](#)
* [Notebook/Markdown/Slide DeckTitle](#)
* [Blog Post](#)

---

This file structure is based on the [DSSG machine learning pipeline](https://github.com/dssg/hitchhikers-guide/tree/master/sources/curriculum/0_before_you_start/pipelines-and-project-workflow).

## Content and Structure

		├── README.md          <- The top-level README for developers.
		├── conf               <- Space for credentials
		│
		├── data
		│   ├── 01_raw         <- Immutable input data
		│   ├── 02_intermediate<- Cleaned version of raw
		│   ├── 03_processed   <- Data used to develop models
		│   ├── 04_models      <- trained models
		│   ├── 05_model_output<- model output
		│   └── 06_reporting   <- Reports and input to frontend
		│
		├── docs               <- Space for Sphinx documentation
		│
		├── notebooks          <- Jupyter notebooks. Naming convention is
		|                         date YYYYMMDD (for ordering),
		│                         the creator's initials, and a short `-` 
		|                         delimited description.
		│
		├── references         <- Data dictionaries, manuals, etc. 
		│
		├── results            <- Final analysis docs.
		│
		├── requirements.txt   <- The requirements file for reproducing the 
		|                         analysis environment.
		│
		├── .gitignore         <- Avoids uploading data, credentials, 
		|                         outputs, system files etc
		│
		└── src                <- Source code for use in this project.
		    ├── __init__.py    <- Makes src a Python module
		    │
		    ├── d00_utils      <- Functions used across the project
		    │   └── remove_accents.py
		    │
		    ├── d01_data       <- Scripts to reading and writing data etc
		    │   └── load_data.py
		    │
		    ├── d02_intermediate<- Scripts to transform data from raw to 
		    |   |                  intermediate
		    │   └── create_int_payment_data.py
		    │
		    ├── d03_processing <- Scripts to turn intermediate data into 
		    |   |                 modelling input
		    │   └── create_master_table.py
		    │
		    ├── d04_modelling  <- Scripts to train models and then use 
		    |   |                  trained models to make predictions. 
		    │   └── train_model.py
		    │
		    ├── d05_model_evaluation<- Scripts that analyse model 
		    |   |                      performance and model selection.
		    │   └── calculate_performance_metrics.py
		    │    
		    ├── d06_reporting  <- Scripts to produce reporting tables
		    │   └── create_rpt_payment_summary.py
		    │
		    └── d07_visualisation<- Scripts to create frequently used plots
			└── visualise_patient_journey.py


