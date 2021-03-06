[![Build Status](https://travis-ci.org/andyklimczak/TheReportOfTheWeek-API.svg?branch=master)](https://travis-ci.org/andyklimczak/TheReportOfTheWeek-API)

# The Report Of The Week API

Basic API to provide information on [The Report Of The Week](https://www.youtube.com/user/TheReportOfTheWeek)

### Example Review
```json
{
    "product": "5 Hour Energy Pomegranate",
    "manufacturer": "Living Essentials",
    "category": "Energy Crisis",
    "videoTitle": "Energy Crisis--Energy Drink Review",
    "videoCode": "wyD3nCv_emI",
    "dateReleased": "2011-02-20T00:00:00.000Z",
    "rating": 7
}
```

### Usage

* Check status:
  * [GET /](https://thereportoftheweek-api.herokuapp.com/)
* All reports (sorted by date):
  * [GET /reports](https://thereportoftheweek-api.herokuapp.com/reports)
* Reports by category
  * [GET /reports?category=Energy Crisis](https://thereportoftheweek-api.herokuapp.com/reports?category=Energy%20Crisis)
  * [GET /reports?category=Running On Empty](https://thereportoftheweek-api.herokuapp.com/reports?category=Running%20On%20Empty)
* Reports between certain dates
  * [GET /reports?between=2012-1-1|2013-1-1](https://thereportoftheweek-api.herokuapp.com/reports?between=2012-1-1|2013-1-1)
  
### Example Frontends

* [The Report of the Week Client](https://thereportoftheweek-client.herokuapp.com/) Interactive charts using React, Redux, and Recharts

## Development

0. Install mongodb, node, and npm
1. Clone the repo
2. __npm install__
3. __npm start__ will load the data and start the server
4. __npm test__ will run the tests

### Update data

The json information the server returns is created from seeds/reports.json. Information from new videos needs to be entered manually. Please feel free to update/append new data !
