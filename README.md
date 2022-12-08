# ACCESS-WOMBAT_01deg_BGC_validation

Repository to share code/notebooks used to validate the WOMBAT ocean BGC output from ACCESS-OM2-01 IAF Cycle 4. 

Overview of diagnostics available: http://cosima.org.au/index.php/2020/07/29/data-available-0-1-1958-2018-access-om2-iaf-run/

Directories of some observational datasets stored on Gadi:
- **OCCCI chl**: `/g/data/ua8/ocean_color/OCCCI/v5-0/8day/chlor_a/`
- **Standard vgpm NPP from MODIS**: `/g/data/ua8/NPP/Standard_VGPM/MODIS/`
- **GEOTRACES (iron)**: `/g/data/ua8/GEOTRACES/idp2021/GEOTRACES_IDP2021_v1/seawater/netcdf/`
- **WOA18** available via cosima cookbook (https://github.com/COSIMA/cosima-recipes/blob/master/Tutorials/COSIMA_CookBook_Tutorial.ipynb)

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
