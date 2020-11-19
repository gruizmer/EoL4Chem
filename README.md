# EoL4Chem

EoL4Chem is a code written in Python to track chemicals across different location in the United States of America, using publicly-available databases.

<sup>[1](#myfootnote1)</sup>

<p align="center">
  <img src=https://github.com/jodhernandezbe/EoL4Chem/blob/main/EoL4Chem.svg width="80%">
</p>

# Requirements:

This code was written using Python 3.x, Anaconda 3, and operating system Ubuntu 18.04. The following Python libraries are required for running the code:

1. [chardet](https://anaconda.org/anaconda/chardet)
2. [pandas](https://anaconda.org/anaconda/pandas)
3. [numpy](https://anaconda.org/conda-forge/numpy)
4. [pyyaml](https://anaconda.org/anaconda/pyyaml/)
5. [selenium](https://anaconda.org/conda-forge/selenium)
6. [webdriver-manager](https://pypi.org/project/webdriver-manager/)
7. [regex](https://anaconda.org/conda-forge/regex)
8. [beautifulsoup](https://anaconda.org/anaconda/beautifulsoup4)
9. [requests](https://anaconda.org/anaconda/requests)
10. [argparse](https://anaconda.org/conda-forge/argparse)
11. [fake-useragent](https://anaconda.org/auto/fake-useragent)
12. [nltk](https://anaconda.org/anaconda/nltk)
13. [plotly](https://anaconda.org/plotly/plotly)
14. [plotly-orca](https://anaconda.org/plotly/plotly-orca)
15. [psutil](https://pypi.org/project/psutil/)
16. [holoviews](https://anaconda.org/conda-forge/holoviews)
17. [matplotlib](https://anaconda.org/conda-forge/matplotlib)
18. [seaborn](https://anaconda.org/anaconda/seaborn)

# EoL dataset structure

| Feature name | Type | Feature name | Type |
| ------------- | ------------- | ------------- | ------------- |
| REPORTING YEAR |	Integer | RECEIVER TRIFID	| Alphanumeric |
| GENERATOR TRIFID	| Alphanumeric | RECEIVER RCRAInfo ID	| Alphanumeric |
| GENERATOR NAME |	Alphanumeric | RECEIVER NAME	| Alphanumeric |
| GENERATOR STREET |	Alphanumeric | RECEIVER STREET	| Alphanumeric |
| GENERATOR CITY |	Alphanumeric | RECEIVER CITY	| Alphanumeric |
| GENERATOR COUNTY |	Alphanumeric | RECEIVER COUNTY	| Alphanumeric |
| GENERATOR STATE |	Alphanumeric | RECEIVER STATE	| Alphanumeric |
| GENERATOR ZIP |	Integer | RECEIVER ZIP	| Integer |
| GENERATOR LATITUDE |	Float | RECEIVER LATITUDE	| Float |
| GENERATOR LONGITUDE |	Float | RECEIVER LONGITUDE | Float |
| GENERATOR TRI PRIMARY NAICS CODE | Integer | PATHWAY RELATIVE IMPORTANCE | Float |
| GENERATOR TRI PRIMARY NAICS TITLE | Alphanumeric | NUMBER OF BROKERS | Integer |
| SRS CHEMICAL ID | Integer | MAXIMUM POSSIBLE FLOW FOLLOWING PATHWAY | Float |
| TRI CHEMICAL ID NUMBER | Alphanumeric | RELIABILITY OF MAXIMUM POSSIBLE FLOW FOLLOWING PATHWAY | Integer |
| RCRAInfo CHEMICAL ID NUMBER | Alphanumeric | TEMPORAL CORRELATION OF MAXIMUM POSSIBLE FLOW FOLLOWING PATHWAY | Integer |
| CAS NUMBER | Alphanumeric | RETDF FRS ID | Integer |
| TRI CHEMICAL NAME | Alphanumeric | RETDF TRIFID | Alphanumeric |
| TRI CLASSIFICATION | Alphanumeric | RETDF NAME | Alphanumeric |
| METAL INDICATOR | Alphanumeric | RETDF STREET | Alphanumeric |
| CAA HAP? | Alphanumeric | RETDF CITY | Alphanumeric |
| CWA BIOSOLIDS? | Alphanumeric | RETDF COUNTY | Alphanumeric |
| CWA PRIORITY? | Alphanumeric | RETDF STATE | Alphanumeric |
| SDWA CANDIDATE? | Alphanumeric | RETDF ZIP | Integer |
| SDWA NPDWR? | Alphanumeric | RETDF LATITUDE | Float |
| TSCA NC INVENTORY? | Alphanumeric | RETDF LONGITUDE | Float |
| SMILES | Alphanumeric | RETDF PRIMARY NAICS CODE | Integer |
| CHEMICAL CATEGORY 1 | Alphanumeric | RETDF PRIMARY NAICS TITLE | Alphanumeric |
| CHEMICAL CATEGORY 2 | Alphanumeric | RETDF REPORTING YEAR | Integer |
| CHEMICAL CATEGORY 3 | Alphanumeric | MAXIMUM AMOUNT PRESENT AT RETDF | Integer |
| GENERATOR CONDITION OF USE | Alphanumeric | TOTAL WASTE GENERATED BY RETDF | Float |
| UNIT | Alphanumeric | RELIABILITY OF TOTAL WASTE GENERATED BY RETDF | Integer |
| QUANTITY TRANSFER OFF-SITE | Float | COMPARTMENT | Alphanumeric |
| RELIABILITY OF OFF-SITE TRANSFER | Integer | FLOW TO COMPARTMENT FROM RETDF | Float |
| WASTE MANAGEMENT UNDER TRI | Alphanumeric | RELIABILITY OF FLOW TO COMPARTMENT FROM RETDF | Integer |
| WASTE MANAGEMENT UNDER EPA WMH | Alphanumeric | TOTAL RELEASE FROM RETDF | Float |
| RECEIVER FRS ID	| Integer | RELIABILITY OF TOTAL RELEASE FROM RETDF | Integer |


# Disclaimer

The views expressed in this article are those of the authors and do not necessarily represent the views or policies of
the U.S. Environmental Protection Agency. Any mention of trade names, products, or services does not imply an endorsement by the U.S.
Government or the U.S. Environmental Protection Agency. The U.S. Environmental Protection Agency does not endorse any commercial products, service, or enterprises.

# Acknowledgement

This research was supported in by an appointment for Jose D. Hernandez-Betancur to the Research Participation
Program at the Center for Environmental Solutions and Emergency Response, Office of Research and Development,
U.S. Environmental Protection Agency, administered by the Oak Ridge Institute for Science and Education through an Interagency Agreement No. DW-89-92433001 between the U.S. Department of Energy and the U.S. Environmental Protection Agency.

-----------------------------------------------------------------------------------------------------------------------------

<a name="myfootnote1">1</a>: - Recycling, energy recovery, treatment & disposal facility (RETDF).
                             - Pollution abatement unit (PAU).
