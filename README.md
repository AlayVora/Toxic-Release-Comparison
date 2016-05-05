##Toxic Release Comparison for USA between years (2005 & 2006)

##Steps to run the project:
1. Install WAMP server
2. extract the contents of "Semantic Project UI source code.zip" into the "www" directory of WAMP server directory.
3. Access the homepage of the project with the following URL: http://localhost/Semantic/

##Introduction:
+ The project focuses on using Semantic web approach to integrate two RDF datasets from Data.gov website using SPARQL queries. The integration happens with the help of a common predicate.
+ The datasets being used for the project are been hosted on Jena Fuseki Server on an Amazon EC2 instance.
+ Using the Google Visualization API’s, the required results are rendered to the webpage using JavaScript and HTML.
+ Geo Map, Data Table and Column Chart are the three Google Visualizations used for displaying the results.
+ Geo Map shows the map of the United States which change in Air Emissions between the years 2005 and 2006 for each State which can be seen while hovering the mouse to the respective State region.
+ On clicking the State region in the Geo Map we can see a bar chart comparing the change of all toxics released (Land, Underground and Air) by the state into the environment.


##Target Audience:

+ This project can be useful to the Environmental Protection Agency of USA for studying the growth of toxic release across the years and to take corrective measures in this area. 
+ The categorized analysis can also be used to regulate environmental taxes in the respective state, where the toxic growth has dramatically increased.

##Description of Data Sources:

+ Dataset 191: 2005 Toxics Release Inventory National data file of all US States and Territories
+ The Toxics Release Inventory (TRI) is a publicly available EPA database that contains information on toxic chemical releases and waste management activities reported annually by certain industries as well as federal facilities.  

+ Dataset 249: 2006 Toxics Release Inventory National data file of all US States and Territories
+ The Toxics Release Inventory (TRI) is a publicly available EPA database that contains information on toxic chemical releases and waste management activities reported annually by certain industries as well as federal facilities.

##Number of Triples:
+ Dataset 191 – 9,973,192
+ Dataset 249 – 10,040,889


##Data Integration:
+ The two datasets are being integrated in the website using a common predicate from both datasets having predicate name as ‘state’.
+ The SPARQL query used for getting the required results contained aggregate functions like SUM.
+ Jena Fuseki Server supports all the required aggregate functions and thus we used Fuseki’s custom SPARQL endpoint for hosting the two Datasets. 
+ The Fuseki server can be accessed in the following server: http://52.207.219.191:3030/

    
    
