# snowflake_proj13_monitoring

## TASK 1 : Snowflake History and Warehouse Usage
**Category:** Snowflake Monitoring  
**Title:** Monitoring Query and Warehouse Usage in Snowflake  

### Instruction  
Understand and practice using Snowflake's Account Usage views to monitor query history and warehouse usage.  

### Tasks  
- **Query History**: Retrieve recent queries executed within your Snowflake environment and display details.  
- **Analyze Warehouse Usage**: Check the average credits used by each warehouse in the last 24 hours to optimize warehouse sizing.  

### Hint  
- Use `SNOWFLAKE.ACCOUNT_USAGE.QUERY_HISTORY` to view executed queries.  
- Use `SNOWFLAKE.ACCOUNT_USAGE.WAREHOUSE_METERING_HISTORY` to monitor warehouse resource usage and credits.  

---

## TASK 2 : Snowflake Query Activity and Query Execution Details
**Category:** Snowflake Monitoring  
**Title:** Monitoring Query Activity by User and Query Execution Details  

### Instruction  
Learn to use Snowflake’s Account Usage views to analyze query activity per user and examine details of successful queries.  

### Tasks  
- **Query Count per User**: Retrieve the number of queries executed by each user in the past 24 hours, ordered by highest count.  
- **Successful Query Details**: Get details of the most recent successful queries (user, warehouse, execution status, time, rows produced).  

### Hint  
- Use `SNOWFLAKE.ACCOUNT_USAGE.QUERY_HISTORY`.  
- Use `CURRENT_TIMESTAMP` and `DATEADD` to filter queries for the past 24 hours.  

---

## TASK 3 : Snowflake Failed Queries and Warehouse Credits Usage
**Category:** Snowflake Monitoring  
**Title:** Analyzing Failed Queries and Warehouse Credits Usage  

### Instruction  
Use Snowflake’s Account Usage views to identify failed queries and monitor warehouse credits usage.  

### Tasks  
- **Failed Queries**: Retrieve details of failed queries (query ID, user, warehouse, error message).  
- **Credits Usage Analysis**: Explore credits consumed by each warehouse to optimize cost.  

### Hint  
- Failed queries info is in `SNOWFLAKE.ACCOUNT_USAGE.QUERY_HISTORY`.  
- Credits usage is in `SNOWFLAKE.ACCOUNT_USAGE.WAREHOUSE_METERING_HISTORY`.  

---

## TASK 4 : Snowflake Warehouse Load and Database Storage Usage
**Category:** Snowflake Monitoring  
**Title:** Monitoring Warehouse Load and Database Storage Usage  

### Instruction  
Use Snowflake Account Usage views to track warehouse queuing times and database storage consumption.  

### Tasks  
- **Warehouse Queuing Analysis**: Query `WAREHOUSE_LOAD_HISTORY` for avg provisioning and load queuing times in last 24 hrs.  
- **Database Storage Usage**: Review storage usage across databases.  

### Hint  
- `SNOWFLAKE.ACCOUNT_USAGE.WAREHOUSE_LOAD_HISTORY` for queue analysis.  
- `SNOWFLAKE.ACCOUNT_USAGE.DATABASE_STORAGE_USAGE_HISTORY` for storage usage.  

---

## TASK 5 : Snowflake Query Execution Time and Role Grants
**Category:** Snowflake Monitoring  
**Title:** Analyzing Query Execution Time and Role Grants  

### Instruction  
Use Account Usage views to analyze query performance and audit user role grants.  

### Tasks  
- **Average Query Execution Time by User**: Find average execution time per user in last 24 hrs.  
- **User Role Grants**: Review roles granted to users for access auditing.  

### Hint  
- Use `SNOWFLAKE.ACCOUNT_USAGE.QUERY_HISTORY` for execution details.  
- Use `SNOWFLAKE.ACCOUNT_USAGE.GRANTS_TO_USERS` to check user roles.  
