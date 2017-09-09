# cisco-phone-inventory

Utility to extract Cisco IPPhones with registration status and optional serial-number (if webservice on the phone is enabled and reachable!)

## Requires
Node.JS 8.4.0 or higher

## Install
Clone/download this repo  
run this command in the root directory (where package.json is) to install dependancies  
npm install

## Run with serial-number extraction
UCM_HOST=x.x.x.x UCM_USER=administrator UCM_PASS=password UCM_VERSION=11.5 GET_SERIALS=true node index.js  

this generates phones.csv  
name,description,loginuser,dirNumber,status,ipaddress,serial,model

## Run without serial-number extraction
UCM_HOST=x.x.x.x UCM_USER=administrator UCM_PASS=password UCM_VERSION=11.5 node index.js  

this generates phones.csv  
name,description,loginuser,dirNumber,status,ipaddress
