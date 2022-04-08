# Load Testing  
## Resource
https://k6.io/blog/load-testing-with-postman-collections/  
  
Load testing with 500 user at ./summary.html visible at:  
https://htmlpreview.github.io/?https://github.com/TourifyDevelopment/organization/blob/main/backend/load-testing/summary.html  

## Postman export
Export postman collection:  
* Import openapi file in postman  
* Export collection (right click on collection -> export to json file)  
* Run postman-to-k6 with collection.json file  

## Commands:
```
# convert postman collection to k6 test
$ postman-to-k6 collection.json \
    -o k6-script.js

# run load test
$ k6 run \
    --vus 100 \
    --duration 5m \
    k6-script.js
```