# Aws-Rds-Db-Connection-to-mysql-workbench-locally
```markdown
# AWS RDS Database Connection Instructions

### MySQL Database
**Hostname:** endpoint past here  
**Port No:** past here 3306  

**Steps:**
1. Navigate to: `aws => rsd => database => name_mysql_db => Connectivity & security => Security => VPC security groups`
2. Edit inbound rule: Add port no anywhere `0.0.0.0`

**Admin Credentials:**  
**Username:** admin  
**Password:** Mypassword.1  

---

### AWS RDS MSSQL Database to Local SQL Workbench

**Required Files:**
- `C:\bigdata\Workbench-Build130\JDBCDrivers\mssql-jdbc-12.6.3.jre8.jar`
- Dependency: `12.6.3.jre8.jar` (must be a slightly older version)
- `C:\bigdata\Workbench-Build130\JDBCDrivers\mysql-connector-java-8.0.28.jar`

**JDBC Connection String Format:**
```
jdbc:sqlserver://serverName[\instanceName][:portNumber];property=value;property=value
```

**Example:**
```
jdbc:sqlserver://mssqldb2.cx0m0s8648g4.us-east-1.rds.amazonaws.com:1433;trustServerCertificate=true;databaseName=mydb
```

**Steps:**
1. Navigate to: `aws => rsd => database => name_mysql_db => Connectivity & security => Security => VPC security groups`
2. Edit inbound rule: Add port no anywhere `0.0.0.0`

**Hostname:** endpoint past here  
**Port No:** past here 1433  
**Database Name:** Configuration  

**MSSQL Database:**  
1. Navigate to: `aws => rsd => database => name_mssql_db => Connectivity & security`
2. Copy the Endpoint and paste it.

**Admin Credentials:**  
**Username:** admin  
**Password:** Mypassword.1  

Additional Step:  
Ensure `trustServerCertificate=true;databaseName=mydb` is included in the connection string.
```
