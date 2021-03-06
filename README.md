# Introduction
Here I provide the code for:  [**IRS County-to-County Migration Data**](https://github.com/mathewhauer/IRS-migration-data/blob/master/manuscript_file.pdf)

### Citation


> Hauer, M.E. *Open Science Framework.* (DOI Forthcoming) (YEAR ACCESSED).



# Abstract

**BACKGROUND**: The Internal Revenue Service's (IRS) county-to-county migration data are an incredible resource for understanding migration in the United States. Produced annually since 1990 in conjunction with the US Census Bureau, the IRS migration data represent 95 to 98 percent of the tax filing universe and their dependents, making the IRS migration data one of the largest sources of migration data. However, any analysis using the IRS migration data must process at least seven legacy formats of these public data across more than 2000 data files -- a serious burden for migration scholars. 

**OBJECTIVE**: To produce a single, flat data file containing complete county-to-county IRS migration flow data and to make the computer code used to process the migration data available. 

**METHODS**: This paper uses R to process more than 2,000 IRS migration files into a single, flat data file for use in migration research. 

**CONTRIBUTION**: To encourage and facilitate the use of this data, we provide a single, standardized, flat data file containing county-to-county migration flows for the period 1990-2010 and provide the full R script to download, process, and flatten the IRS migration data.


# Organization
- `LATEX`  — Contains latex files to reproduce the main manuscript file.
- `R` - Contains the R scripts needed to reproduce the flat IRS migration datafile.
- `MigData`  — Initial data resources, unprocessed.
- `DATA-PROCESSED` — Final, post-processed data.

# Use
- Feel free to create a new branch for further incorporation and analysis. 
- Please properly cite all use of the underlying code or data. Thanks!

# Data

The final IRS migration data can be downloaded at `DATA-PROCESSED/county_migration_data.txt` or reproduced by running the `R/999-master_script.R` file.



# Codebook

`ORIGIN`
- Refers to the 5-digit FIPS code for the origin of the migrants.

`DESTINATION`
- Refers to the two-digit FIPS code associated with each state.

`1990:2010`
- Refers to number of migrants who moved from ORIGIN to DESTINATION in a given year.

- NOTE: there is an additional 5-digit FIPS code in the both the ORIGIN and DESTINATION field. This is coded as 99999 and is in reference to all migration flows containing less than 10 tax filers.

# Correspondence
For any issues with the functionality of these scripts please [create an issue](https://github.com/mathewhauer/IRS-migration-data/issues).

## License
The data collected and presented is licensed under the [Creative Commons Attribution 3.0 license](http://creativecommons.org/licenses/by/3.0/us/deed.en_US), and the underlying code used to format, analyze and display that content is licensed under the [MIT license](http://opensource.org/licenses/mit-license.php).