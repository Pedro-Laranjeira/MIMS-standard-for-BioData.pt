# Implementation of MIMS Standard for BioData.pt

This repository contains the code required for the implementation of the MIMS (Minimum Information about a Microarray Experiment) standard for BioData.pt.

## Upload Instructions: 

To upload this code to the server, follow the steps described below:

1. Upload the text file containing the code to the server. The code file should be in TSV (Tab-Separated Values) format.

2. Use the following `curl` command to load the new metadata block:

   ```sh
   curl http://localhost:8080/api/admin/datasetfield/load -H "Content-type: text/tab-separated-values" -X POST --upload-file /tmp/new-metadata-block.tsv

Upload documentation: [https://guides.dataverse.org/en/latest/admin/metadatacustomization.html#id29](https://guides.dataverse.org/en/latest/admin/metadatacustomization.html#id29)
