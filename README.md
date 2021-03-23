<img src="https://raw.githubusercontent.com/KasperJuunge/mlcutter/main/mlcutter-color.png" align="center">

## What is it?
Minimalistic package templates should be a no-brainer to create. This cookiecutter template helps you with that! 💪📦



## How to create a ML-Cutter template?
[Cookiecutter](https://github.com/cookiecutter/cookiecutter) is used to generate the template. So first install cookiecutter with pip:

``` bash
pip install cookiecutter
```
Generate the template:
``` bash
python -m cookiecutter https://github.com/KasperJuunge/PKG-Cutter
```



## The Project Structure You'll Get

```
├── LICENSE
├── README.md                           <- The top-level README for developers using this project.
│
├── notebooks                           <- Jupyter notebooks.
│
├── references                          <- Data dictionaries, manuals, and all other explanatory materials.
│
├── src                                 <- Source code for use in this project.
│   └── package_name
│       │
│       ├── __init__.py                 
│       │        
│       ├── package_name.py             <- Main class in package that ties functions from all the submodules together <3
│
├── requirements.txt                    <- The requirements file for reproducing the analysis environment. 
│                                       
└── setup.py                            <- makes project pip installable (pip install -e .) so src can be imported.
```



## Workflow

When the template is initialized it creates a blank project structure, ready for developing your very own model package 📦

My typical workflow using this project structure is the following:

#### 1. Get Raw Data
First, get the data. Write the get_model_data() function to get the raw data for modeling. Place the raw data in ~/data_storage/raw/

#### 2. Exploratory Data Analysis
Now we need to get our hands dirty! Explore the data, analyze the problem, make some plots, remove outliers and try to come up with some input features. This process is carried out using Jupyter Notebooks which should be placed in ~/notebooks/

#### 3. Build Features
Now write the build_features() function which turns the raw data into juicy features. The function should also split the dataset in train, validation and test set and place it in ~/data_storage/dataset/

#### 4. Train Model
Now we're ready to train the model. Write the train_model() function in the model module. The hyperparameters can be imported from the hyperparams_dict in the config module. Save state_dicts in /trained_models/

#### 5. Measure performance
Write the measure_performance() function that calculates relevant metrics for a trained model on the test dataset.

#### 6. Write prediction function
Write the predict() function to make it as easy as possible to make predictions using a trained model.

#### 7. Create model class
some text here..

### Credits

This template is inspired by the [DrivenData Data Science Template](https://github.com/drivendata/cookiecutter-data-science). Thanks!



