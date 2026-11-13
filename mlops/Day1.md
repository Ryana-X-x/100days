### The Problem: 
The xFusionCorp Industries data science team requires a standardized Python environment for their new machine learning project. Set up a virtual environment on the `controlplane` host that includes all necessary ML libraries.

  

The work is done on the `controlplane` host under `/root/code/`.

The end state must satisfy the following:

- a Python virtual environment named `ml-env` exists under `/root/code/`;
- the environment has `numpy`, `pandas`, `scikit-learn`, and `matplotlib` installed;
- a `requirements.txt` capturing the installed packages is saved at `/root/code/requirements.txt`.

-------------------------------
- first we check python and pip versions
- python3 --version, pip3 --version
-------------
- then we setup the venv
- python3 -m venv ml-env
- source /root/code/ml-env/activate
------------------------
- pip install `numpy`, `pandas`, `scikit-learn`, `matplotlib` 
- pip freeze > /root/code/requirements.txt
----------------------------
- python -c "import numpy, pandas, sklearn, matplotlib; print('All ML libraries imported successfully')"