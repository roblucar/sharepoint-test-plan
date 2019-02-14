# 2.1 Test no data deletion during recrawl of Sharepoint sites that are offline

## summary

Verify that no indexed data is removed during recrawl of Sharepoint sites that are not accessible due to complete outage  

## steps

* create a site collection sc1
* create a site s1
* create a list l1_s1 within s1 
* create a list item li1_l1_sc1 within l1_sc1
* enable "delete dead URIs" and set "fetch failure allowance" to 1 on the datasource  
* crawl sc1

## prelimiary assertion

verify that site s1 content was indexed. 

## additional steps

* shutdown sharepoint instance hosting site s1
* perform incremental crawl on site sc1

## assertion

verify that the crawl has stopped 

verify that the site s1 indexed content is still present
