# TASK-2

Step 1: Load Data from Excel
Open Power BI Desktop.

Click Get Data and select Excel Workbook.

Choose your Excel file, select the table or worksheet containing data, and click Load.

Verify that the Excel data appears in the Fields pane.

Step 2: Load Data from SQL Server
Click Get Data and select SQL Server Database.

Enter the Server Name and Database Name.

Choose either:

Import mode to load data directly into Power BI.

DirectQuery mode to retrieve data on-demand for large datasets.

Select the table or query you want to use and click Load.

Step 3: Transform and Clean Data
Click Transform Data to open Power Query Editor.

For both Excel and SQL data:

Filter unnecessary rows by using column filters.

Rename columns for consistency (e.g., "Prod_Name" to "Product Name").

Remove duplicates where necessary using Remove Duplicates.

Set appropriate data types (e.g., "Number" for sales, "Date" for order dates).

Merge data from the two sources:

Use Merge Queries to join datasets on a common field (e.g., OrderID, ProductID).

Alternatively, use Append Queries if you need to stack datasets vertically.

Step 4: Create Relationships
Switch to Model View by clicking the third icon on the left-hand pane.

Drag and drop fields to create relationships between tables:

For instance, connect OrderID in the SQL Server table with OrderID in the Excel table.

Verify the relationships:

Ensure cardinality matches the data (e.g., One-to-Many if each order in SQL links to multiple rows in Excel).

Check cross-filter direction (usually set to single direction).

Step 5: Build Visualizations
Switch to Report View.

Add the following visuals as shown in the dashboard:

A Map visualization to display sales by country (e.g., Canada, France, Germany).

Pie Chart for showing discounts and gross sales by product (e.g., Paseo, Velo).

Bar Chart for sales, profit, and units sold by segment (e.g., Government, Midmarket).

Drag relevant fields into the visualization well:

For the map, use Country and Sales.

For the pie chart, use Product Name, Discounts, and Gross Sales.

For the bar chart, use Segment and Profit.

Step 6: Customize and Enhance
Apply formatting to make the report user-friendly:

Add titles and adjust color schemes for clarity.

Enable data labels and tooltips for all visuals.

Use slicers for interactivity:

Add slicers to filter by Date, Product, or Region.

Step 7: Finalize and Share
Save your report as a .pbix file.

Click Publish in the Home ribbon to upload the report to Power BI Service.

Share the report with stakeholders or embed it in applications.

![Image](https://github.com/user-attachments/assets/5b870f7e-9e43-4269-9eee-0f674540a821)
