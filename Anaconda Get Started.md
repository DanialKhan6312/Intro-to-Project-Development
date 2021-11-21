# Anaconda 


Anaconda is a distribution of the Python for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment.

Anaconda enables us to manage enviroments and dependencies using simple command line arguments. 


# Anaconda Installation 

## Options:

[Anaconda Navigator](https://www.anaconda.com/products/individual)

Predownloads fundemental moduels as well as Data Science specific IDEs and software. 

Provides a nice interface for software and enviroment managment

[Miniconda](https://docs.conda.io/en/latest/miniconda.html)

Minimal instalation for Anaconda. Installs conda shell but not predefined packages


[Miniforge](https://github.com/conda-forge/miniforge)

Same as Miniconda but specifically useful for M1 Macs


# Simple conda commands


## Create enviroment: 
``` conda create --name myenv python=3.10.0```

Why create different enviroment and not just isntall everything onto a single location? 

** Conflicting dependencies management 

** Execution on varying clusters

** Minimal migration onto other machines 

** Define version of python to run on

## Activate enviroment
``` conda activate myenv```

## List existing conda installations 

```conda list```

Should be empty 


```conda install numpy ```

```conda list```
Should be filled with numpy and all its dependencies 

## Specify version to install 
```conda install pandas=1.3.4```


## Create requirment file 

````conda list -e > requirements.txt```

## Create new enviroment with requirment file(different machine or same machine)


```conda create --name myenv2 --file requirements.txt```

## New enviroment should have all packages and dependencies matching old one! 
``` conda activate myenv2 ```

```conda list ```

## We can now serialize our envorments across multiple machines with matching versions and dependencies making deployement A LOT easier




