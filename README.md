## Mortgage Data Map

As part of a retrospective event on the 10-year anniversary of the 2008 financial crisis, the Economic Studies program at the Brookings Institution produced a number of pieces looking into the causes of the crisis. 

I created an interactive map using **D3.js** and **AngularJS** to accompany one such piece. The [map shows](https://www.brookings.edu/blog/up-front/2018/09/10/mapping-the-boom-in-nonbank-mortgage-lending-and-understanding-the-risks/) where the share of *nonbank mortgages* are greatest in the U.S. 

On hover over a county, a tool tip displays both the percentage of all mortgages as well as the county name. Example of data structure used below: 

| name | id | rate |
| ---- | -- | ---- |
| county name | FIPs code | rate | 

The interactive uses [FIPs code](https://en.wikipedia.org/wiki/FIPS_county_code) which provides unique identifiers for U.S. counties to match data with shape files. The data is then displayed as a heat map where shares of these mortgages are highest. 

If a user scrolls over a county without any data, no information is displayed. 
