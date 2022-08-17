# ohw22-proj-gcmfilters
## Mapping eddy flow structures using GCM-Filters

### Important links: 

- [Pangeo Data Catalog](https://catalog.pangeo.io/browse/master/ocean/)
- [GCM-filters documentation](https://gcm-filters.readthedocs.io/en/latest/index.html)

Below we have our plan for the week!

### Goals for Tuesday:
  - Make sure everyone can open and is comfortable with jupyterhub - ok
  - Run some examples of GCM-Filters on the Hub 
  - Decide what data set to use from the Pangeo Data Catalog - ok (NCAR CESM Global High Resolution Ocean Model Fields)

### Goals for Wednesday: 
- Run the example "Filtering on CPUs vs GPUs" from GCM-Filters; 
- Explore the data set, examine regions of interest and try to apply the GCM-Filters using the examples;
 - Update the code for using Laplacians to filter vector fields in the NCAR CESM POP model.

## Instructions for running a `GCM-filters` environment

- Make sure you have pulled (`git pull`) the updated version of this repo so that you have the file `gcm-filters_env.yaml` in your JupyterHub. You can take a look at the `.yaml` file and see the packages listed that we will have access to within our soon-to-be created environment.
- Open a Terminal on your Hub.
- In terminal, type:

```
conda env create -f gcm-filters_env.yaml
```
This creates a new environment from the file (hence the `-f`) named gcm-filters_env.yaml.
- You will have to wait several minutes while the environment is created.
- At the end, you should see something like the following:

```
Preparing transaction: done
Verifying transaction: done
Executing transaction: done
#
# To activate this environment, use
#
#     $ conda activate gcm-filters-env
#
# To deactivate an active environment, use
#
#     $ conda deactivate
```
You do not need to do anything else at the command line if you get to this stage. (That is, you do not need to activate the environment, though are welcome to if you'd like.)
- Optional: In case we are missing a package, we can add it to the `gcm-filters_env.yaml` file later and then type
```
conda env update --file gcm-filters_env.yaml --prune
```
- The last step is to start a new notebook with the new environment we just created! To do this, you will need to open a new landing page (click the "+" in the upper left of the Hub). You should see an option to open a notebook in the top row with the new environment called "gcm-filters-env". NOTE: it may take a couple minutes for the environment to appear.


