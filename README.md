# Business Case:

The Accounts Department of the Company maintains the invoice level details of all vendors for each part procured. The Business Planner receives invoice data from the Accounts Department for each vendor and collects the supplier and part level information separately from the Purchase Department. The Business Planner has to study the relevant data and identify the Procurement trends, Supplier limitations, Product based supplier consolidation and minimize cost impact to company.


## Problem Statement

As the collected Data is of different years for multiple Plants grouped by different Business Units. The parts are either made of Aluminum or Ferrous of different raw material grade alloys, with the source being either Tier 1 supplier or Tier 2 supplier. Considering all these factors, create a dashboard which is insightful on all these factors and can help the Procurement Department make better supply chain strategic decisions.


## Data Sources

The dataset used for this analysis is the "Report_Master.xlsx", "Material_weights_and_source.xlsx" & "Supplier_data.xlsx"


## Tools
- Excel
- Power BI
	- Data cleaning
	- Data Filtering
	- Assigning Data Types
	- Data analysis
	- Graphical representation


## Data Cleaning preparation

In the initial data preparation stage, following task were performed:
	- Data Extraction, Loading & Transforming
	- Handling errors & null values
	- Data types as per description


- Non-MSME suppliers are basically the ones which have a Turnover > 100cr, Lower than this will be classified into different types of MSME category.


### Exploratory Data Analysis

SCENARIO 1:
	- Our task is to build a dashboard page and name it as “Supplier Overview”, which gives us a supplier status and its capabilities. Also, categorizing them as per the data provided in the data set. This will help the responsible Purchase Group (Buyer) get a focused quick insight for the suppliers.


SCENARIO 2:
  - We would need another dashboard page and name it as “Volume Movement” to help analyze the Purchase volume movement throughout different years for past comparisons and business planning upcoming demands. We would need multiple filtering options as per business units, purchasing groups, Manufacturing plants, Part Family, supplier names, and raw materials.
  - As we have different report files for different years, create a master table combining the table Report 2019 and Report 2020 files into one. And establish a relationship between the newly created Master Report table and Material weight and source.
    - Now lets plot some charts to visualize the data for further analysis
      - Invoicevalue vs Supplier Name, name it as “Supplier Purchase Volume”
      - Invoicevalue by Part Family, name it as “Part Family Purchase Volume”
      - Invoicevalue by month distributed by Years, name it as “Purchase Volume by Month and Year”
      - Invoicevalue by Business Unit, name it as “BU Purchase Volume”

### Data Analysis
Utilized Custom columns, merging of column, append queries, measures, Bar chart, Column chart, Area chart, Donut chart, Pie chart, chiclet slicers, maps, etc


### Results/Findings:

SCENARIO 1:
  - We have total 35 suppliers out of which 16 are Ferrous suppliers & 19 are Non-Ferrous supplier
  - Overall 17 are Small MSME Suppliers, 6 are Medium MSME Suppliers & 12 are Non-MSME Suppliers
  - As per strategy status 14 are No-Go suppliers & 21 are Go suppliers
  - Suppliers are mainly located in South & Centre of India & small presence in North India
  - Top supplier in terms of Volume is "AM&ACP" which is present in Bangalore who has both Casting & Machining with payment terms upto 90 days

SCENARIO 2:
  - Supplier Purchase Volume for Non-Ferrous is from "AM&ACP" which is 1.407M & for Ferrous is from "BIPL" - 202M, "SSI" - 200M & "APPPL" 192M
  -  Part Family Purchase Volume is highest for "In-Line Pump Housing" which is 1385.15M (28.24%)
  -  Purchase Volume by Month and Year:
        - During 2019 the maximum purchase volume was in July - 270M & lowest in November 181M
        - During 2020 the maximum purchase volume was in December - 303M & lowest in April 3M
  - Petrol System Business Unit generates the Highest purchase Volume of 3798M


### Recommendations:

Based on analysis, following recommendations can be utilized:
  - AM&ACP Supplier is found to be most reliable & most liked supplier, buyers can prefer this supplier for Non-Ferrous materials
  - BIPL, SSI & APPPL generates high volume for Ferrous material, Buyers can prefer BIPL & APPPL. SSI Supplier falls in No-Go strategy
  - Electronics Division & Automotive Engineering sector to be focused on improvement to generate revenue



 
