# mal-activity-reporting
This repo consists of crawling, data-crunching, and analysis script of a ASIACCS'19 submission

The Final Dataset is hosted at [Google Drive](https://drive.google.com/open?id=1kxlk7Y16SI8OZ_yyE46fqJfCSwbd4bnJ)

Python 2.7
Packages: pandas, matplotlib, numpy, tqdm

To run the scripts, extract the downloaded Data files such that your directory reflects the structure below
```
|mal-activity-reporting/
|	|Datastore/
|	|	|XX_reports.csv
|	|	|YY_reports_NN.csv
|	|Unlabelled_predictions/
|	|Characterization/
|	|	|Affinity/
|	|	|Dataset Summary/
|	|	|Proportions/
|	|	|Tops/
|	|Churn/
|	|Specialization/
```


The Datastore contains multiple .csv files each containing mal-activity specific reports.
These files follow a common structure:
```
IP,
Country Code (CC),
Autonomous System Number (ASN),
Second level domain (2LD) [If avaliable],
AS Organization Name,
Day,
Month,
Year,
Blacklist Source [:VT is appended if extended from Virus Total, e.g. mdl:VT]
```
The Unlabelled_predictions contains multiple .csv files each containing a prediction for its corresponding mal-activity reports.
