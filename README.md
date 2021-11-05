# pvs-atrophy
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/willtack/pvs-data.git/main)

Scripts for running neuroprint on NACC subjects for periventricular spaces project.

In order:
1) create_collection.ipynb - create the Flywheel collection and populate with sessions from NACC-SC enumerated by PVS_subjects.csv
2) check_and_run_ants.ipynb - check which sessions have already been analyzed with ANTs-CT (expensive to run)
3) run_wscore_pvs.ipynb - run Neuroprint on the sessions recently analyzed with ANTs
4) download_wscore_csvs - download the raw results data from Flywheel to local directory
4) calcSchaeferVolumes.sh - calculate the volume of each Schaefer label for weighting in next step
5) aggregate_data - combine all the individual w-score csvs into one; weight w-scores by volume