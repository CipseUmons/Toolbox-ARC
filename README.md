# Toolbox-ARC
A toolbox to process neural data

# Anaconda
Anaconda is an environment manager for Python. We use it to set environments which contain all the needed libraries. This is how to use it:

## 1. Installation
Download Anaconda for the last Python version (3.X) using [THIS LINK](https://www.anaconda.com/distribution/).
Follow the instructions of the .exe file.

## 2. Create environment
### a) From scratch
- Open "Anaconda Prompt"

- Create your environment with the last Python version:
```
conda create -n myenv python=3.X
````
Note: replace "myenv" by the name of your environment (whatever you want) and "X" by the corresponding Python version.

- Activate your environment:
```
conda activate myenv
```
Note: the text (myenv) should appear at the beginning of the new command line.

- Add the libraries you need by typing the corresponding command found in [Anaconda Cloud](https://anaconda.org/anaconda/repo).

Tips: Choose "Anaconda/" option when available.

Example with [scipy](https://anaconda.org/anaconda/scipy):
```
conda install -c anaconda scipy
```

### b) From Yaml file
- Download the Yaml file of the desired environment (desired_env.yml).

- In the Anaconda Prompt, go to the corresponding location
```
cd PATH_TO_YAML_FILE
```
Note, replace PATH_TO_YAML_FILE with the absolute path of the folder where the desired file is stored.

- Import the environment:
```
conda env create -f desired_env.yml
```
Note: replace "desired_env" by the corresponding environment name.

- Activate your environment:
```
conda activate myenv
```
Note: the text (myenv) should appear at the beginning of the new command line.

## 3. Launch Jupyter Notebook
A Jupyter Notebook is a notebook allowing you to write and run Python code easily using your conda environment.

While your environment activated, launch a new notebook:
```
jupyter notebook
```
A Chrome tab will open, choose the folder where you what your notebook to stand and create a new Python 3 notebook:

![Example image](docs/new_notebook.png)
