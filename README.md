## Human Development Report Office Statistical Data API

**1. Overview**
The Human Development Report Office (HDRO) offers this REST API for the developers to query human development-related data in JSON format. The data can be queried by indicator id(s), year(s) and country code(s) and grouped by any order. 

**Documentation:** https://hdr.undp.org/en/data (identify relevant indicators)
<br/>

**2. Developers Page** 
The Human Development Report Office (HDRO) offers these REST API endpoints for the developers to query human development related data in JSON format. The data can be queried by indicator id, year, and country ISO code.

**Link:** hdrosystem-env.eba-zbgtnp54.us-east-1.elasticbeanstalk.com/swagger/

```php
https://api.hdrdata.org/CountryIndicators/gbr/2020
```
 
**3. Using the API**

  1. `country_code` e.g. country_code = 'LSO, ZAF, GBR'
  2. `indicator_id` e.g.  indicator_code='690706'
     - 169706-Expected years of schooling (years)
  3. `year` e.g. year = '2020, 2019, 2017,2018' `not specified in query used for this context`

**3.1 Commonwealth member countries sample call**
```php
https://api.hdrdata.org/CountryIndicator/ATG,AUS,BGD,BHS,BLZ,BRB,BRN,BWA,CAN,CMR,CYP,DMA,FJI,GBR,GHA,GMB,GRD,GUY,IND,JAM,KEN,KIR,KNA,LCA,LKA,LSO,MDV,MLT,MOZ,MUS,MWI,MYS,NAM,NGA,NRU,NZL,PAK,PNG,RWA,SGP,SLB,SLE,SWZ,SYC,TON,TTO,TUV,TZA,UGA,VCT,VUT,WSM,ZAF,ZMB,TGO,GAB
```

**3.2 Sample Queries**
**Base URL:** https://api.hdrdata.org/
```php
Primary Endpoints:
- /CountryIndicators/{country}/{year}
- /CountryIndicators/pagination
- /CountryIndicators/filter


```
