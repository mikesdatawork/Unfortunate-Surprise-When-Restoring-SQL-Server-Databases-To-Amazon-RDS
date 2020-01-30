![MIKES DATA WORK GIT REPO](https://raw.githubusercontent.com/mikesdatawork/images/master/git_mikes_data_work_banner_01.png "Mikes Data Work")        

# Unfortunate Surprise When Restoring SQL Server Databases To Amazon RDS
**Post Date: May 1, 2015**        



## Contents    
- [About Process](##About-Process)  
- [Author](#Author)        

## About-Process

<p>Amazon RDS is an excellent solution if you are starting with an Amazon RDS SQL Instance, and you're immediately using it directly. In other words installing applications, and pointing them to your RDS instance so it can create it's databases. If you are developing custom database solutions, and start building out databases directly in Amazon RDS; then you should also be fine. However; you will find the task extremely complicated when importing/restoring databases, or data sets from any former non-RDS SQL database environments. It has severe limitations that are outside all industry import/migration norms. Additionally; any automated database processes that were created on the source database environments, or any replication schemes across the enterprise will not be supported. I'm confident in the future; Amazon RDS will evolve this product to include wide scale support of all kinds of import & restore operations including database automations however; right now this is not the case. This caught me by surprise.
Database migrations are possible, but it needs to be a complete custom 'manual' solution by which you would target each and every database, table, and subsequent objects individually. This is full ETL development for ETL. SQL logic will need to be written and the ETL process will most likely be managed via Integration Services (SSIS). Remember; this is done per database, per object. Once the schema, and data have been properly moved some objects will need to be recreated at the destination.</p>

![Importing Data To Amazon RDS]( https://mikesdatawork.files.wordpress.com/2015/05/image001.jpg "Unfortunate Surprise With SQL Import Limitations To Amazon RDS")
 
See the Amazon Docs directly here: http://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/SQLServer.Procedural.Importing.html


[![WorksEveryTime](https://forthebadge.com/images/badges/60-percent-of-the-time-works-every-time.svg)](https://shitday.de/)


## Author

[![Gist](https://img.shields.io/badge/Gist-MikesDataWork-<COLOR>.svg)](https://gist.github.com/mikesdatawork)
[![Twitter](https://img.shields.io/badge/Twitter-MikesDataWork-<COLOR>.svg)](https://twitter.com/mikesdatawork)
[![Wordpress](https://img.shields.io/badge/Wordpress-MikesDataWork-<COLOR>.svg)](https://mikesdatawork.wordpress.com/)

 
![Mikes Data Work](https://raw.githubusercontent.com/mikesdatawork/images/master/git_mikes_data_work_banner_02.png "Mikes Data Work")

