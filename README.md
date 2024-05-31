# Minimal Example of Tutorial in Jupyter Notebook running GPT2

[![Binder](https://mybinder.org/badge_logo.svg)](https://notebooks.gesis.org/binder/v2/gh/GESIS-Methods-Hub/minimal-example-ipynb-python-gpt2/HEAD?labpath=index.ipynb)

This repository is a minimal example of a Jupyter Notebook running GPT2 (and two other language models).
The notebook is located in the `index.ipynb` file.

## Usage

To run the notebook in the cloud using Binder, click on the Binder badge above, or use this [link](https://notebooks.gesis.org/binder/v2/gh/GESIS-Methods-Hub/minimal-example-ipynb-python-gpt2/HEAD?labpath=index.ipynb).
This will open the notebook in a new tab in your browser.

To run the notebook locally, install the required libraries with `conda` by running the following command in the terminal.
Note: The `environment.yml` file lists all Python libraries on which your notebooks depends.
Remove `cpuonly` from the `environment.yml` file if you use a GPU.

```bash
conda env create -f environment.yml
```

Then, activate the environment:

```bash
conda activate example-environment
```

In addition, download the pre-trained GPT2 model by running the following command:

```bash
./download_models.py
```

Finally, start the Jupyter Notebook server:

```bash
jupyter-notebook index.ipynb
```
