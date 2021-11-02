# ChemRxiv_API
A python wrapper for making API call to the ChemRxiv (https://chemrxiv.org/engage/chemrxiv/public-dashboard) server. Please refer to the code documentation for query parameters.

## Pre-requisites
Run the following command to install the required packages.
```
pip install -r requirements.txt
```

## Example use:
```
from chemrxiv_wrapper import *
response = chemrxiv_api(
    term = 'composites',
    skip = 10,
    limit = 20,
    sort = 'VIEWS_COUNT_DESC',
    searchDateFrom = format_time('2020/02/29'),
    searchDateTo = format_time('2021/03/01')
    )
```
