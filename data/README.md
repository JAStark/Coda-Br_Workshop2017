# DATA
Data is from Washington D.C.'s [open data portal](http://opendata.dc.gov/datasets?q=taxi) for January 2017.

## raw
Contains the unzipped file downloaded from above.
Data was provided along with `README_DC_Taxicab_trip.txt` explaining the data, with data dictionary, row counts etc.

## external
Contains shape files for D.C. census tracts which were used to join the point locations in the taxi data to tract-level data.

## interim
Contains shape files of the taxi point location data and the D.C. census tract data. The dataset used in this notebook consisting of point locations of taxi drop-offs within D.C., regardless of whether they with picked up within D.C. or not.

Data were also filtered for pickups in D.C., but this set was not used in analysis.

Taxi data was joined with D.C. shape data using QGIS software via the GUI.

## processed
Contains the csv file output of the join of taxi point data for drop-offs in D.C.

## Notebooks
This directory contains just one python Jupyter Notebook with some data exploration and simple visualisations, in addition to means and medians.

**Data Dictionary**
Truncated titles seems to be a quirk of QGIS, as the column headers were not truncated in the original datasets.

For Drop-offs:
* TRIPTYPE: is "DDS" for Digital Dispatch Service, which includes phone dispatch and phone app dispatch; "PSP" for street hail, and "Transport-DC" for Metro Access were filtered out in a previous step.
* METERFARE: Meter fare
* TIP: Tip amount.
* TOTALAMOUN: Total amount from meter fare, tip, surcharge, extras, and tolls.
* PAYMENTTYP: Payment type (`Cash`, `CreditCard`)
* PAYMENTCAR: Type of card used to pay (e.g. VISA).
* DROPOFFDAT: Drop-off date.
* GEOID10: Census tract ID (from shape file)
* NAME10: Block ID (from shape file)
* ALAND10: Area of land in square meters (from shape file)
* GEOID: Census tract ID (from taxi dataset)

## Requirements
These are the versions used in this project, but older or newer versions might still be ok.

Python 3.4.5
Pandas 0.19.2
Matplotlib 1.5.1
Numpy 1.11.3
Seaborn 0.7.1

## LICENSE

This project is licensed under
