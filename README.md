# Super Store Sales-Dashboard

### [1] Dashboard Link :https://app.powerbi.com/links/Wuf-THT80l?ctid=3f66430c-920e-49dc-9dd6-8223afea3b81&pbi_source=linkShare

### [2] Problem Statement

This dashboard helps the Stores Person understand their customers better. It helps the Stores know if their customers are satisfied with their services. Through different ratings, they get to know their improvement area, & thus they can improve their services by identifying these area. It also lets them know the average delivery date & profit,sales. Thus since by using this dashboard they have identified this problem, they can further work on factors responsible for these unwanted issues.

Since,here we can see in this dashboard the profit and sales unit of a super store in which the (profit = 175K) & the (sales = 2M)

Also since average delivery day is 4 days, thus they must try to reduce it.

### [3] Charts used

(a) Card : It was used to display values like sum of 'Profit','Sales','Quantity','Average Delievery Day'.

(b) Slicer : It was used for the branch which was bifurcated as'Region by directions'.

(c) Donut Chart : Used for the 'Sales by segment' ,'Sales by Payment mode', 'Sales by Region'.

(d) Cluster bar Chart : Used to display the 'Sales by sub-category' & 'Sales by category'.

(e) Stacked Column Chart : It was used to show the'Sales by Ship mode'.

(f) Line Chart : Used to display the 'Sum of sales by Order Date'[Yearly] & 'Sum of sales by Order Date'[Quaterly].

(g) Map : It was used to show the Profit & Sales by state.

(h) Stacked Bar Chart : This visual was used to show 'Unit Price' by each product line.
 
### [4] Steps followed 

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : After data preview,select the transform data "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present except column named "AVG Delievery".
- Step 5 : Going through the data and selecting edit query for data cleaning i.e. searching for duplicate values and for each column data type.
- Step 6 : In the report view, under the view tab, theme was selected.
- Step 7 : Since the data contains various data, thus in order to represent profit by months,sales by segment,sales by payment,sales by region a new visual was added.
- Step 8 : Visual filters (Slicers) were added for four fields named "North", "South", "East" & "West".
- Step 9 : Four card visuals were added to the canvas, one representing Profit other representing Sales,followed by the Average Delivery Days & Quantity.
           Using visual level filter from the filters pane, basic filtering was used & null values were unselected for consideration into average calculation.
           
           Although, by default, while calculating average, blank values are ignored.
- Step 10 : Summarization of the columns 'Profit','Quantity' & 'Sales'were done from dataset.
- Step 11 : Datatypes format was changed for the column 'Order Date' & 'Ship Date'.
- Step 12 : Before report view,some parameters were created for some of the columns which includes 'average' & 'sum'.
- Step 13 :All columns were reviewed and verified and the blank dummy columns in the end of dataset's were deleted.
- Step 14 : New measure was created to find average delievery days.
 Step 13 :In 2nd report view, we created a line chart was created which was used to present a yearly and quaterly line graph using sum of sales & Order Date.

Following DAX expression was written for the same,
        
     AVG Delievery = DATEDIFF(Superstore_Sales_Dataset[Order Date],Superstore_Sales_Dataset[Ship Date],DAY)

[DAX Function_snapo](https://github.com/Chandan-Sav/Dashboard---Superstore/assets/121309914/aab319f0-7667-45a4-b2d0-077697cfdef3)

        
 - Step 15 : The report was then published to Power BI Service.
 ![dashboard_snapo](https://github.com/Chandan-Sav/Dashboard---Superstore/assets/121309914/07ce499c-90fb-486b-affc-abd7ed22294d)
 
 


# Snapshot of Dashboard (Power BI Service)

![dashboard_snapo](https://github.com/Chandan-Sav/Dashboard---Superstore/assets/121309914/2c68bcd6-40dd-4da7-8646-4d79e85511a7)

 


 # Report Snapshot (Power BI DESKTOP)

 
![Dashboard_upload](https://github.com/Chandan-Sav/Dashboard---Superstore/assets/121309914/dff42b89-7e9b-455b-86eb-81b2680ebe41)

### [5] Insights

A double page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

#### Card Values

   Profit = 175 K

   Sales = 2 M

   Quantity = 22 K

   Avg Delievery Days = 4 days

           Thus, higher number of sales is there than a  profit.
           
### Snapshot of Cards (Power BI Report)
![dashboard_snapo](https://github.com/Chandan-Sav/Dashboard---Superstore/assets/121309914/3e658f1d-5c6b-4dfc-8dbd-354eed438d5c)
 
 #### Sales
 
 1) Sale By segment :-
     a] Home/Office - 19% 
     b] Consumer    - 48%
     c] Corporate   - 33%
 
 2) Sale By Payment Mode :-
     a] Cards   - 22% 
     b] COD     - 43%
     c] Online  - 35%
 
 3) Sale By Region :-
     a] Central- 22% 
     b] South  - 16%
     c] West   - 33%
     d] East   - 29%
               
             Thus, higher number of sales in segment is by'Consumer' ,in Payment mode by'COD' & in region basis it is 'West'region.
