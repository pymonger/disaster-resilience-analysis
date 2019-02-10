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
1. Activate environment:
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
1. To deactivate the environment:
   ```
   conda deactivate
   ```
1. To remove the environment entirely:
   ```
   conda env remove --name cutter
   ```
