## Setup

- install conda: https://docs.conda.io/projects/conda/en/latest/user-guide/install/download.html

### iris dataset

- create a conda environment with required packages (in console): `conda create -n ml_workshop scikit-learn matplotlib ipykernel`
- Activate conda environment and start a Jupyter notebook with the right environment:

        conda activate ml_workshop
        python -m ipykernel install --user --name ml_workshop --display-name "ML Workshop"
        jupyter notebook
- Alternative: run in VSCode with Python and Jupyter notebook extensions
- if you don't want to set up a local version, you can try this browser-based notebook: https://jupyter.org/try-jupyter/retro/notebooks/?path=notebooks/Intro.ipynb

### Dogs vs. Cats dataset

Dataset is available on [Kaggle](https://www.kaggle.com/c/dogs-vs-cats) - download and extract the train folder into your working directory.  

- create a conda environment with required packages (in console): `conda create -n ml_workshop2 tensorflow-gpu`
This requires your GPU to be CUDA-enabled - you may have to install additional drivers depending on your hardware.
- alternative: train using CPU (much slower): `conda create -n ml_workshop2 tensorflow`
- Install remaining libraries:

        conda activate ml_workshop2
		conda install keras scikit-learn ipykernel pillow
        python -m ipykernel install --user --name ml_workshop2 --display-name "ML Workshop - cats vs. dogs"
        jupyter notebook
- Alternative: run in VSCode with Python and Jupyter notebook extensions
