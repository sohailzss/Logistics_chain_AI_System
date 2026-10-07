docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=LogisticsAIPass123!" ^
   -p 1433:1433 --name legacy-mssql ^
   -d mcr.microsoft.com/mssql/server:2022-latest


 - python scripts\ingest_legacy_data.py