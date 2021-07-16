# test-repo
This is a test repository
While doing session on Composite Models with Aggregations many people asked me how and where you got the demo data and how did you build it.
So, I have tried to bring together all the steps I took to build the demo on Composite Models with aggregations. This demo would be good showcase on Azure Synapse + Power BI integration story as well as some key best practices explained through demo (Result Set Caching, Row level security implementation etc.). One can use this for their own learning as well. 
For this Demo I used the WWI database that is provided as Sample Database for Synapse and is publicly available to use. For simplicity and reuse, I am providing all the scripts I used in each step for preparing / setting up this demo. 
Folder “WWIDemoDBPrepCreate_WWISynapseDW” contains these scripts together with numbered steps. You can use it in the same order to build it quicker. In the last script (05_faster_ExtrapolateandPopulateFactSales.sql) I have prepared three versions of fact table 145 million rows, 1 billion rows and 1 million rows. Depending on how big the source table you want you can use the respective version by renaming one of those tables.  
Folder “PowerBICompositeWithAggsDemo” contains the actual demo files. It contains set of Power BI template files one for simple demo and another for more advanced RLS demo. The SQL script files should be used in conjunction with these demos. For example “DW02_Create&PopulateRLSTable.sql” is a pre-requisite to demo RLS and should be performed as a part of demo set up. 
