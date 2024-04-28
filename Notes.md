## DBT
1. Run a full refresh from command
   `dbt run — select tag:incremental_model --full-fresh`
2. Use soureces, create source.yml file and use that instead of table name/ref
3. Add source reshness to sources yml file
4. Add generic tests (unique, not_null, accepted_values, relationships)
5. Make single tests for specific models
7. Learn doc blocks for dbt documentation
8. How is View different then ephimeral

## Other

1. Use a service account for creds ?