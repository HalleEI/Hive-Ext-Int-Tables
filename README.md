# Hive-Ext-Int-Tables
RDBMS, CSV file Import To HDFS Plus External, Internal Tables
3 RDBMS’s = MySQL, MsSQL, and Postgresql
MySQL tables imported to HDFS in the directory /user/input/mysqltables
MsSQL tables imported to HDFS in the directory /user/input/mssqltables
Postgresql tables imported to HDFS in the directory /user/input/clubpo
Used SFTP to transfer csv file to HDFS.
Csv files imported to HDFS in the directory /user/input/csvtables 
  
In hive	 -     Created DB called fitness.
-	Created 3 external tables with schema for my 3 csv files and loaded data into the tables
-	Created 3 internal tables with schema for my 3 csv files and loaded data into the tables
