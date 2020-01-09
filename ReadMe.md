# Readme
## instructions to go from raw imaging data (from CAI) to BIDS

This code will copy the relevant .dcm files as given by CAI to the user's scratch on qriscloud hpc (e.g. awoonga), will convert to BIDS format, and return a compressed copy of the BIDS formatted data back to the original archive folder. 

1. check pathways defined at top of STRWP1_dcm2nii are correctly defined/have been generated where relevant
2. make sure STRWP1_dcm2nii is in your home directory and has been edited to specify the relevant subject and session numbers 
3. this code uses the super useful function dcm2niix - make sure that it and its dependencies are also in the home folder 
4. Upload the log .tsv files to STRIWP1LOGS/ (see the BIDS specification)
5. run file using the command ./STRWP1_dcm2nii (make executable using chmod +x if needed)

### troubleshooting
- dcm2niix can fail if the wildcard search brings up more than 1 file