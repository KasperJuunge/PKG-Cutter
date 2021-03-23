<img src="https://github.com/KasperJuunge/PKG-Cutter/blob/main/pkg-cutter.png" align="center">

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


