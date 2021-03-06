# Metal Price APIs

## Overview
Application provides API to retrieve metal prices.  
Initial data is loaded when application starts.  
Scheduler is configured to retrieve the latest data once a day. 


## APIs
API to get all available metals  
http://localhost:9095/api/metals

API to get latest prices for all available metals  
http://localhost:9095/api/prices

API to get history prices for the given metal   
(default days to retrieve is 15 days)  
http://localhost:9095/api/prices?metalID=2

API to get history prices for the given metal,  
"size" parameter is to provide number of days to retrieve  
http://localhost:9095/api/prices?metalID=2&size=3

## Run
### Prerequisites
Java, Maven, Git and Docker Compose need to be installed.

### Commands
> git clone https://github.com/05021991/metalprice.git  
> cd metalprice  
> mvn package  
> docker-compose up