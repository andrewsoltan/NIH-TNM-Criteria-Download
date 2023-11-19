# NIH-TNM-Criteria-Download
This script uses the SEER API, provided by the NIH National Cancer Institute, to download and save the latest TNM staging criteria (separated by cancer type).

"""
Title: Download TNM Staging Tables by Tumour Type from NIH National Cancer Institute
Date: 19/11/23
Version: 1.0
Author: Andrew Soltan

This script uses the SEER API, provided by the NIH National Cancer Institute, to download and save the latest version of the TNM staging criteria (separated by cancer type) for tumour types of interest.

The full API documentation is available here: https://api.seer.cancer.gov/usage
Instructions to get an API key are available here: https://api.seer.cancer.gov/usage

To get the name of the tumour type for the tumourTypes list:
Review the schema at: https://staging.seer.cancer.gov/tnm/list/2.0/
Select the desired tumour type, and then read the URL https://staging.seer.cancer.gov/tnm/schema/2.0/XXXX - the XXX section is the tumour type to use in the tumourTypes list. Typically this is the tumour type in lower case, e.g. 'colon'

Before running, please set:
1) The tumour types that you would like to download staging criteria for in the "tumourTypes" list
2) The output directory, where TNM staging will be saved (outputFolder). By default, the output directory is: tumourTNMstaging
3) Add your API key

"""
