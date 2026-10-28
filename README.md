# fintech-sales-analytics
A beginner-friendly Data Engineering project built on Databricks using SQL, Unity Catalog, data ingestion, validation, transformations, and business analytics.
## Data Engineering Workflow

### 1. Data Ingestion

CSV files are uploaded into a Databricks Unity Catalog Volume and loaded into raw tables.

### 2. Data Validation

Data quality checks are performed including:
- Null value checks
- Duplicate detection
- Record count validation

### 3. Data Transformation

Raw datasets are joined to create a business-friendly analytics table.

### 4. Analytics

Business questions answered include:
- Revenue by province
- Top-selling products
- Highest-spending customers

## Example Analytics Query

```sql
SELECT
    province,
    SUM(sales_value) AS revenue
FROM sales_analytics
GROUP BY province;

Skills Demonstrated
Data Ingestion
Data Validation
SQL Joins
Data Transformation
Aggregations
Analytics Reporting
Databricks Fundamentals
Future Improvements
Implement Bronze, Silver, and Gold layers
Add Delta Tables
Build Databricks Dashboards
Automate ingestion workflows
Deploy infrastructure using Terraform
