Step 1 - Open Power BI report

Step 2 - Import dataset in Power BI report.From webiste(https://ourworldindata.org/coronavirus)
To import dataset, go to Home -> Get data -> Select dataset - Trasform data --  For rows and columns to select the best appropriate data for Data Virtulization in Power BI.

Step 3 - Creating some calculated measures(fields).
To create calculated measures -> Right click on dataset in Fields section -> Select New measure -> Enter the following formulas one by one:


skillnation.in took o help from 2 Day Live Workshop - Power Bi Domination Workshop -- How to create query in Power BI query

*Active cases = SUM('CoronaVirus Data'[Confirmed Daily])-SUM('CoronaVirus Data'[Deaths Daily])-SUM('CoronaVirus Data'[Recovered Daily])
*Average Confirm daily = SUM('CoronaVirus Data'[Confirmed Daily]) / DISTINCTCOUNT('CoronaVirus Data'[Date])
*Average Death daily = SUM('CoronaVirus Data'[Deaths Daily]) / DISTINCTCOUNT('CoronaVirus Data'[Date])
*Average Recovered daily = SUM('CoronaVirus Data'[Recovered Daily]) / DISTINCTCOUNT('CoronaVirus Data'[Date])
*Mortality Rate = SUM('CoronaVirus Data'[Deaths Daily])/SUM('CoronaVirus Data'[Confirmed Daily])
*Recovery Rate = SUM('CoronaVirus Data'[Recovered Daily])/SUM('CoronaVirus Data'[Confirmed Daily])

Step 4 - Designing dashboard.

Add 'Title' in Power BI report.
To add 'Title', go to Insert -> Select 'Text box' from Elements section -> Enter title as 'Covid-19 Global Analysis'.
Add 'Card' for Mortality Rate in Power BI report.
To add 'Card', go to Visualization pane -> Drag and drop 'Card' visual in Power BI report.
Add fields into the 'Card' visual
Put 'Mortality Rate' in 'Fields'.
Similarly, create cards for 'Mortality Rate', 'Recovery Rate', 'Average confirmed cases per day', 'Average recovered cases per day', and 'Average deaths per day'.
Add 'Guage' for Total Cases in the Power BI report.
To add 'Guage', go to Visualization pane -> Drag and drop 'Guage' visual in Power BI report.
Put 'Confirmed Daily' in the 'Value' and 'Maximum value' fields.
Add 'Guage' for Active Cases in the Power BI report.
To add 'Guage', go to Visualization pane -> Drag and drop 'Guage' visual in Power BI report.
Put 'Active Cases' in 'Value' and 'Confirmed Daily' in the 'Maximum value' field.
Add 'Guage' for Deaths in the Power BI report.
To add 'Guage', go to Visualization pane -> Drag and drop 'Guage' visual in Power BI report.
Put 'Deaths Daily' in 'Value' and 'Confirmed Daily' in the 'Maximum value' field.
Add 'Guage' for Recovered in Power BI report.
To add 'Guage', go to Visualization pane -> Drag and drop 'Guage' visual in Power BI report.
Put 'Recovered Daily' in 'Value' and 'Confirmed Daily' in the 'Maximum value' field.
Add 'Slicer' for Month-year in Power BI report.
To add 'Slicer', go to Visualization pane -> Drag and drop 'Slicer' visual in Power BI report.
Put 'Month-Year' in 'Field'.
Add 'Slicer' for Date in the Power BI report.
To add 'Slicer', go to Visualization pane -> Drag and drop 'Slicer' visual in Power BI report.
Put 'Date' in 'Field'.
Add 'Slicer' for Country/Region in the Power BI report.
To add 'Slicer', go to Visualization pane -> Drag and drop 'Slicer' visual in Power BI report.
Put 'Country/Region' in 'Field'.
Add 'Map' for Covid-19 confirmed cases in the Power BI report.
To add 'Map', go to Visualization pane -> Drag and drop 'Map' visual in Power BI report.
Put 'Country/Region' in the 'Location' field and 'Confirmed Daily' in the 'Size' field.
Add 'Clustered bar chart' for Confirmed Cases by Country/Region in Power BI report.
To add 'Clustered bar chart', go to Visualization pane -> Drag and drop 'Clustered bar chart' visual in Power BI report.
Put 'Country/Region' in the 'Axis' field and 'Confirmed Daily' in the 'Values' field.
Add 'Line and Clustered column chart' for Cumulative Confirmed, Deaths, Recovered by Date in Power BI report.
To add 'Line and Clustered column chart', go to Visualization pane -> Drag and drop 'Line and Clustered column chart' visual in Power BI report.
Put 'Date' in the 'Shared axis' field, 'Deaths' in 'Column values' field, 'Confirmed' and 'Recovered' in the 'Line values' field.
Add 'Table' in the Power BI report.
To add 'Table', go to Visualization pane -> Drag and drop 'Table' visual in Power BI report.
Put 'Country/Region', 'Confirmed Daily, 'Recovered Daily', 'Deaths Daily', 'Average Confirm daily', 'Average Recovered daily', 'Average Deaths daily', 'Recovery Rate' and 'Mortality Rate' in 'Values' field.
To apply conditional formatting on Table -> Go to Format -> Conditional formatting -> Select column -> Turn on Data bar.

