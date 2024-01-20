# AzureDataEngineering
AzureDataEngineering || End To End Project
Data Engineering End-To-End project
Reference - https://www.youtube.com/watch?v=pMqnvXgPKlI&t=1963s 
( source - https://www.youtube.com/@learnbydoingit)
Disclaimer : I have followed the video and have been successful in creating the end-to-end Data Engineering project on Pizza-Sales data. I have come across some bottlenecks while implementing the same and hence added references in my document how I resolved the same. I have taken help from other you tube channels and internet resources for the purpose. Hope it helps others anyway.
Thanks to all for putting out these valuable resources online so anyone can learn and implement.
Tools learnt – 
1. SQL server migration 
2. Azure Data Factory 
3. Azure Data Lake Storage Gen2 
4. Azure Databricks 
5. PYSPARK 
6. SPARK SQL 
7. Microsoft Power BI
Installation required –
1.	SQL Server Management Studio 19
2.	Microsoft Integration Runtime
3.	Azure portal (web application, only open with outlook mail with card details for free trial. 2 rupees will be debited for validating credential then MS will credit the same to user. Mark the free trial subscription period. Below is a snapshot to know when your trial ends)
 
4.	Databricks Community edition (web application login, can register without any cloud service linked with your gmail account and giving any ABC company name. If registered with cloud service, it is chargeable so so to use free, should register for community edition. Details shown later.)
5.	Power BI desktop(can install in own device and do stuffs without signing in as it would ask for work domain email. Only thing is without signing in, one will not be able to publish the work in Power BI community however one can download the pbix file and showcase for personal use.)
Issues faced:
1.	SQL server connection issue to Azure – The authentication method should be selected as SQL authentication instead of Microsoft authentication. Follow this video for resolving the issue. - https://youtu.be/AvRUWFq-9ZA?si=RWY86vqIFLX9uIKA
2.	Cluster terminated in Databricks- The cluster created gets terminated due to 60 mins of inactivity. So I cloned the cluster to create a new one and continued to create the workspace and following tasks.
2.a> To track down previously created notebook navigate Workspace>Users>mailed with which workspace created. Snapshots below:
 
 
3.	Databricks Community Login issue– While trying to re-login I got error as my email entered or password invalid even after giving correct credentials. Also the “Forget Password” was not sending reset link in my registered email. There is the catch. While logging in one has to enter the email without any punctuation and all in lowercase characters even though while registering you have entered punctuation or uppercase character. 

