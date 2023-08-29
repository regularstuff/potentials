# proposed

## Start and stop RDS database from lambda 

Use Cognito to make a cell phone verify? Call enpoint and get a ping back  "Are you trying to start Such-and-such cluster"

## Trigger a Snowflake task from an S3 upload

Presumably following tutorial

## CUR wizard

generate AWS cur report setup from a script.... Use boto3 & click library to get Athena worksspace ready
Issue:  after initializing report there is ~24 hour delay before data is written.  The exising
AWS wizard generates cloudformation



##  Snowflake Roles maintenance

Existing projects -- permifrost by gitlab and Thomas Eibner snowflake-provisioning

snowflake-provisioning generates roles based on rules and patterns while
permifrost seems to use explit list -- 

### Example problem

You have two schemas -- Accounting  & Sales.  

Say 5 roles:

ETL Developer -- needs to be able to create/drop tables both of them

ETL Runtime -- needs to be able to populate 

Accounting Report User -- needs query to both schemas

Sales person -- needs query to 1 of them 

Sales intern -- needs query to some subset of one of them 

## API for creating multi-choice quiz 

Support Multiple choice and Fill-in-the blanks (cloze) questions

Question bank only 
	- tags
	- endpoints:
	  - get up to N questions with [list of tags]
	  - get up to N right answers for each questoin in [list of question]
	  - get up to N wrong answers for each questoin in [list of question]

### tech
Fast API, some kind of document database -- dynamodb or mongo?

	  






