# Aws-Rds-Db-Connection-to-mysql-workbench-locally
hostname:- endpoint past here
port no :- past here 3306

aws =>rsd=>database=>name_mysql_db => Connectivity & security ==>Security=>VPC security groups=>editinbound rule =>add portno anywhere 0.0.0.0
admin

password:-Mypassword.1

Q2)aws rds mssql database to local sql workbench

C:\bigdata\Workbench-Build130\JDBCDrivers\mssql-jdbc-12.6.3.jre8.jar

download connector its depency 12.6.3.jre8.jar must little old version

C:\bigdata\Workbench-Build130\JDBCDrivers\mysql-connector-java-8.0.28.jar

jdbc:sqlserver://serverName[\instanceName][:portNumber];property=value;property=value
jdbc:sqlserver://mssqldb2.cx0m0s8648g4.us-east-1.rds.amazonaws.com:1433;trustServerCertificate=true;databaseName=mydb
aws =>rsd=>database=>name_mysql_db => Connectivity & security ==>Security=>VPC security groups=>editinbound rule =>add portno anywhere 0.0.0.0

hostname:- endpoint past here
port no :- past here 1433
databasename :- Configuration

aws =>rsd=>database=>name_mssql_db => Connectivity & security ==> Endpoint coppy then past
admin

password:-Mypassword.1
trustServerCertificate=true;databaseName=mydb one more step
