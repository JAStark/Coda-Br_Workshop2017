# Data Journalism Template for Transparency - Example!
* [Slides](https://jastark.github.io/Coda-Br_Workshop2017Slides/) about why we should make our work transparent, and why this template can help.
* [Interim data](https://drive.google.com/open?id=1pmIDLp84JWxh2buP_1GJFdkzxBMwEao6) where all taxi drop off points were joined with D.C. Shape data in QGIS.
* [Processed data used in Notebook](https://drive.google.com/open?id=1ZXSvP626knV3YBhO99AgCR6JyNYbaJbg) as a csv (too big to store on GitHub (100MB limit)
* [CODA-BR 2017 slides]() "Thinking About Algorithmic Accountability" keynote on algorithmic transparency for tech and for journalism.

## Motivation
To provide a basic example of making data driven journalism (DDJ) transparent to readers, other journalists and government or civic-minded people for my workshop ["How to implement editorial transparency in data journalism"](http://coda.escoladedados.org/#programação) at the 2nd CODA•BR data journalism conference in São Paulo, Brazil 2017.

This example looks at taxi fares in Washington D.C., and filters them based on whether the hails were by app/phone or by street hail; whether the fare was paid for in cash or with a credit card; and looking at differences in meter fare, tip, and total amount.

The example dataset is taxi trips in Washington, D.C. from their [open data portal](http://opendata.dc.gov/datasets?q=taxi).

## Data Dictionary for processed dataset
A strange quirk in QGIS is that column names get truncated when outputting to csv.

* TRIPTYPE: is "DDS" for Digital Dispatch Service, which includes phone dispatch and phone app dispatch; "PSP" for street hail, and "Transport-DC" for Metro Access were filtered out in a previous step.
* METERFARE: Meter fare
* TIP: Tip amount
* TOTALAMOUN: Total amount from meter fare, tip, surcharge, extras, and tolls
* PAYMENTTYP: Payment type (`Cash`, `CreditCard`)
* PAYMENTCAR: Type of card used to pay (e.g. VISA)
* DROPOFFDAT: Drop-off date
* GEOID10: Census tract ID (from shape file)
* NAME10: Block ID (from shape file)
* ALAND10: Area of land in square meters (from shape file)
* GEOID: Census tract ID (from taxi dataset)

## Requirements
Python 3.4.5
Pandas 0.19.2
Matplotlib 1.5.1
Numpy 1.11.3
seaborn 0.7.1

## Installing development requirements
`pip install -r requirements.txt`

# LICENSE
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons Lizenzvertrag" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>

[Coda-Br_Workshop2017](https://github.com/JAStark/Coda-Br_Workshop2017/tree/example) by [Jennifer A. Stark](https://github.com/JAStark) is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
