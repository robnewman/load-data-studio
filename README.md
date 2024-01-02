# load-data-studio-conda
Test repo for loading a Data Studio directly from a Github repo

# Install miniconda

1. Use [Homebrew](https://brew.sh/) to install [miniconda](https://formulae.brew.sh/cask/miniconda): `brew install --cask miniconda`
2. Initialize: `conda init "$(basename "${SHELL}")"`
3. Config to use [Conda-Forge](https://conda-forge.org/):

  ```
  conda config --add channels conda-forge
  conda config --set channel_priority strict
  ```

# Steps to generate a conda environment file

1. Create a conda environment (with specific packages): `conda create --name myjupyterenv python jupyter jupyterlab`
2. Activate the environment: `conda activate myjupyterenv`
3. Generate a YAML file of the environment: `conda env export > environment.yml`
4. Add to the repo: `git add environment.yml`
