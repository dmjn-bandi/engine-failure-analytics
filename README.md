# Engine Failure Analytics

### Files:
- `data_preprocessing.ipynb` - Jupyter Notebook
- `analytics.lvdash.json` - Databricks Dashboard

### Executing Steps:
1. Upload the source data to a volume and configure the path to it in the notebook under the `# source data file path` comment.
2. By default, the notebook uses the `default` database. However, the database name can be changed if necessary. If a database with the specified name does not already exist, the script will automatically create it.
3. Execute all cells in the notebook. Once the execution is complete, it will generate four tables: `bronze_data`, `silver_data`, and `gold_data`, plus an additional `mi_matrix` table for the dashboard.
4. If necessary, change the catalog and database names in the dashboard dataset queries to match the ones used during the notebook execution. The dashboard uses two datasets: the `gold_data` and the `mi_matrix` tables.