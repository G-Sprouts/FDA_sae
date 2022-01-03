# fdata

This tool is meant for the cleaning, creation and storage of custom tables using FDA Adverse Event Reporting System (FAERS) data.

Download whichever [quarterly files](https://fis.fda.gov/extensions/FPD-QDE-FAERS/FPD-QDE-FAERS.html) (ASCII format) you wish to analyze, and utilize these functions to expedite cleaning, organization and database management for your project!

## **Updates**

Database access via psycopg2 and PostgreSQL (last updated 9/23/21)

## **Installation**

Run the following to install:
```
pip install fdata
```
**Note**: If there are empty lists initialized before defining the function, the final output of the function will be attached to these built-in lists. See example below.


## **Usage**
```
import fdata as fd

for drug_file in glob.iglob('file(s)'):
	fd.sorter(drug_file)

	…

	“Check shortened_file and none_list for sorted files”

fd.shortened_file
    (output)
```

See function [documentation](https://github.com/G-Sprouts/FDA_sae/blob/sprout/docs.ipynb) for further explanation

## Dataset creation

Easily create your own dataset using FAERS data for machine learning applications and data visualization tasks! 

![image](https://user-images.githubusercontent.com/66538374/129272912-d6f5af3b-c50d-4c41-84ae-69104c14de6b.png)


See function [documentation](https://github.com/G-Sprouts/FDA_sae/blob/sprout/docs.ipynb) for further explanation
