### predict okved

goal is to beat baseline=0.12 on f1_weighted generating different features

Structure of data.zip

table Pays - payments between companies:
* hash_inn_kt	- id of senders
* hash_inn_dt	- id of recipients
* week - ordinary week :)
* count -	number of payments per week
* sum -	sum of payments per week

table inn_info_public - info about companies
* hash_inn - id
* okved2 - like industry
* region - region 
* is_public - flag (1 or 0) if object for train or test

It's required for companies with is_public=-1 to predict industry in okved2 of file
