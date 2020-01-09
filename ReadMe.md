# Readme
## instructions to go from raw imaging data (from CAI) to BIDS
1. edit code STRWP1_dcm2nii with relevant subject and session numbers
2. ssh into awoonga and sync updated STRWP1_dcm2nii with home directory
3. Make sure that the raw data is named according to the naming convention (see STRWP1_dcm2nii)
4. Upload the log .tsv files to STRIWP1LOGS/
5. run file using ./STRWP1_dcm2nii
6. zip resulting subject folders and make a copy in the CAI directory (rawloc) -    zip -r output_file.zip file1

### troubleshooting
- dcm2niix can fail if the wildcard search brings up more than 1 file