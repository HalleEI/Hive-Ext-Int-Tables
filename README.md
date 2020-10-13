# Hive-Ext-Int-Tables
RDBMS, CSV file Import To HDFS Plus External, Internal Tables
3 RDBMS’s = MySQL, MsSQL, and Postgresql
MySQL tables imported to HDFS in the directory /user/input/mysqltables
MsSQL tables imported to HDFS in the directory /user/input/mssqltables
Postgresql tables imported to HDFS in the directory /user/input/clubpo
Used SFTP to transfer csv file to GCP. using the put command
Csv files imported to HDFS in the directory /user/input/csvtables 

To transfer file from remote(GCP instance) to my lfs (Documents directory), used the get command
halle@halle-VirtualBox:~/Documents$ sftp 34.122.255.12
Connected to 34.122.255.12.
sftp> get facilities_202010101920.csv
Fetching /home/halle/facilities_202010101920.csv to facilities_202010101920.csv
/home/halle/facilities_202010101920.csv                                                                     100%  342     4.4KB/s   00:00    
sftp> lls
facilities_202010101920.csv
sftp> 
  
In hive	 -     Created DB called extfitness.
-	Created 3 external tables with schema for my 3 csv files and loaded data into the tables
        -     Created DB called fitness.
-	Created 3 internal tables with schema for my 3 csv files and loaded data into the tables
