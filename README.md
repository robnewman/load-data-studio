# load-data-studio
Test repo for loading a Data Studio directly from a Github repo

# Steps to generate a conda environment file

1. Create a conda environment (with specific packages): `conda create --name myjupyterenv python jupyter jupyterlab`
2. Activate the environment: `conda activate myjupyterenv`
3. Generate a YAML file of the environment: `conda env export > environment.yml`
4. Add to the repo: `git add environment.yml`
