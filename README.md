# ACCESS-WOMBAT_01deg_BGC_validation

Repository to share code/notebooks used to validate the WOMBAT ocean BGC output from ACCESS-OM2-01 IAF Cycle 4. 

Overview of diagnostics available: http://cosima.org.au/index.php/2020/07/29/data-available-0-1-1958-2018-access-om2-iaf-run/

Directories of some observational datasets stored on Gadi:
- **OCCCI chl**: `/g/data/ua8/ocean_color/OCCCI/v5-0/8day/chlor_a/`
- **Standard vgpm NPP from MODIS**: `/g/data/ua8/NPP/Standard_VGPM/MODIS/`
- **GEOTRACES (iron)**: `/g/data/ua8/GEOTRACES/idp2021/GEOTRACES_IDP2021_v1/seawater/netcdf/`
- **WOA18** interpolated to 0.1 deg grid: `/g/data/ik11/observations/woa18_bgc/woa_bgc_10/`
- **GLODAPv2.2022** (bottle data, not gridded I believe): `/g/data/ua8/GLODAP/`

.    
.  

## Suggested Workflow
To clone this repo run: `git clone https://github.com/hrsdawson/ACCESS-WOMBAT_01deg_BGC_validation.git` or, if you have ssh keys set up, `git clone git@github.com:hrsdawson/ACCESS-WOMBAT_01deg_BGC_validation.git`

### Create your branch (to work)

`git checkout -b "your_name"`

Before working, verify that you are on your own branch. Once you are done working, add and commit the files (only the files you want to push), and push your branch to the repo:

`git push origin "your_name"`

On the github repository you should now see that a branch has pushed changes, and create a pull request to merge with the main branch.

### Sync your local branch to main

`git checkout main`  
`git pull origin main`  
`git checkout "your_name"`  
`git merge origin/main`

## NCI Jupyter Notebook

To launch a jupyter notebook from Gadi you can use NCI Australian Research Environment (ARE).

1. Login to [https://are.nci.org.au](https://are.nci.org.au)
2. Start a JupyterLab instance
3. Adjust session walltime, queue, compute size (might need Large or X-Large), project, storage (e.g., gdata/hh5+gdata/e14+gdata/ik11+gdata/ua8+gdata/cj50)
4. Under Advanced options add:
  * **Module directories**: `/g/data/hh5/public/modules`
  * **Modules**: `conda/analysis3-unstable`
5. Click launch
6. Wait for queue to finish then click Open JupyterLab
7. Create a new notebook or open an existing notebook from a directory (via left column).
