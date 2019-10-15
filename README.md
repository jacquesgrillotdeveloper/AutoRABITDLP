# AutoRABIT Dataloader Pro Data Refresh App
When a Sandbox is refreshed, Product and Pricebook data is included (and conveniently not part of your org limits!).
This app will create AutoRABIT External Id's so that you can populate the Id field before running dataloader pro jobs.

## Dev, Build and Test

## Resources
[Data carried over when a sandbox is refreshed](https://help.salesforce.com/articleView?id=000335966&language=en_US&type=1&mode=1)

## Description of Files and Directories
* AutorabitExtId - external Id field created for Pricebook2, PricebookEntry, and Product2 objects
* AutoRABIT DataLoaderPro Permission Set - access to the External id fields.

## Issues
You are responsible for governance of what is the "source of truth for delta records." In reality, production should be the source. 
For versions of AutoRABIT 4.7 or later you can use an existing External Id field if it exists and populated for all records in the org.