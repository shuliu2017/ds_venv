# ds_venv
This repository provides instructions for creating a Python virtual environment for data scientists.

# Install a virtual environment

Suppose we want to create a Python virtual environment called test_environment on Desktop

- `cd` to your working directory
- run `python -m venv test_environment`
- activate your virtual environment
  - on windows `C:\Users\{username}\Desktop\test_environment\Scripts\activate`
  - on mac `C:\Users\{username}\Desktop\test_environment\Scripts\activate`
- install required package by running `pip install -r requirements.txt`

# Install a ipython kernel

If we want to installa kernel called TestKernel for jupyter notebook, we can use the following code

- python -m ipykernel install --user --name test_environment --display-name "TestKernel"
  - --user: specify the kernel should be installed only for the current user
  - --name test_environment: kernel name, usually chosen as the name of the virtual environment, can be different
  - --display-name "TestKernel": name what will appear in the jupyter notebook
- jupyter kernelspec list
