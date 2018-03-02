CREATE external TABLE IF NOT EXISTS company(cid int, cname string, cloc string, empid int)
    row format delimited                                                     
    FIELDS terminated BY '\t'  
    LINES terminated BY ‘\n’
stored AS textfile location '/hive_external_table_company';


 ROW FORMAT SERDE 
 
   LINES terminated BY ‘\n’ or any char but the default is '\001'.
   
   STORED AS--TEXTFILE-
   -STORED AS--+-SEQUENCEFILE-------------------------------------------------------------------------------------+-'   
                +-RCFILE-------------------------------------------------------------------------------------------+     
                +-BINARY SEQUENCEFILE-
                
                --AS--select_statement-
                
                Derby is the build in embedded database in hive for development environment.
