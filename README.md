# cutter

## Requirements
1. Install anaconda3 (https://www.continuum.io/downloads)
1. Install GEOS Framework (http://www.kyngchaos.com/software:frameworks). On Mac, install using http://www.kyngchaos.com/files/software/frameworks/GEOS_Framework-3.6.1-1.dmg.
1. Clone repository:
   ```
   git clone https://github.iu.edu/INFODER/cutter.git
   cd cutter
   ```
1. Create environment:
   ```
   conda env create
   ```
   This will create an conda environment as specified by the `environment.yml` config file.
1. Export environment variable for GDAL. Add the following line to your shell profile (e.g. `~/.bash_profile`):
   ```
   export GDAL_DATA=$(gdal-config --datadir)
   ```

## Working with the anaconda environment
* To activate the environment:
   ```
   source activate cutter
   ```
   If you run into this error:
   ```
   CommandNotFoundError: Your shell has not been properly configured to use 'conda activate'.
   ```
   Initialize your shell first then activate your environment:
   ```
   conda init $(basename $SHELL)
   source activate cutter
   ```
* To deactivate the environment:
   ```
   conda deactivate
   ```
* To remove the environment entirely:
   ```
   conda env remove --name cutter
   ```

## Getting Started
1. Activate the environment:
   ```
   source activate cutter
   ```
1. Run jupyter:
   ```
   jupyter notebook
   ```
1. A browser will open up showing the contents of this repository. Click on the `01-Getting_Started.ipynb` notebook and run through it.
1. Next, run through the `02-Community_Case_Studies.ipynb` notebook.
1. Finally, run through the `03-Indicator_Relationships.ipynb` notebook.
1. Review previous contributions under [history](history).
