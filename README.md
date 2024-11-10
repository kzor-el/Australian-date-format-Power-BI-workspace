# Display Australian date format on Power BI workspace

When publishing Power BI reports with Australian date format from Power BI Desktop to Power BI Workspace, the date format may default to the US date format i.e. from DD/MM/YYYY to MM/DD/YYYY.

To resolve this insert the Caldendar table into PowerBI desktop and create a relationship between the Existing Power BI table Date column the new Calendar Date column.

1. Open Power BI in Desktop
2, Select Get Data
3. Select Blank Query
4. Under Query Settings select Advanced Editor
5. Paste the Calendar table code from:
6. Select Home
7. Select Close and Apply - the new table will generate.
8. Create the Relationship between table date fields:
  i. Go to tables
  ii. Select Manage Realtionship
  iii. in the first table field select your orginal data source table and highlight the applicable date column
  iv. in the second table field select the new calendar table and the first date column
  v. Select Cardinality > Many to one
  vi. Selct Cross filer > Single
  vii. Select ok.
9. Repeat steps 2-8 for each additional date column that requires filtering/visability in the report.
10. Republish your report to the workspace and dates will now appear in the correct format.
