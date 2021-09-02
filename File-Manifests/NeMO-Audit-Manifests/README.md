# NeMO Audit File Manifests

Directory for File Manifests and Specimen Inventories for the data
collections included in the NeMO file audit recieved August 5, 2021. 
For each project, CSVs were generated for:

1. A Specimen Inventory of samples in the BCDC inventory that have
files at NeMO, with an added column of 'Files per Sample'

2. A File Manifest generated for all matched files in the NeMO audit
list, including associated Sample ID, NeMO ID, and File URI at NeMO, 
as well as checksums provided by NeMO when available

3. A Specimen Inventory of samples in the BCDC inventory that
had **no** matched files in the NeMO audit


Additional notes:

* These File Manifests are **not** final versions - there are still
unlabelled entries in the current audit that could be matched on
file name or with additional information from NeMO. These manifests
are intended as an initial audit, and uploading missing files should not
proceed without first consulting with NeMO to see if files identified
as missing can yet be recovered at the archive.

* There is one set of csvs per "project", and each csv may
  have multiple data collections included. The data collection
  association is provided in column Q of the Sample Inventory csvs,
  and column E of the File Manifest.

* Controlled vocabulary for 'Filetype' in the File Manifest is still
  under review, so the terms shown in that column are provisional,
  based on file extension.






