# Housing-Purchase-or-Rent
This project explores which housing choice is more affordable, purchasing or renting, at the zip code level throughout the United States of America.

Tools Used: Python, SQL, JavaScript, Plotly, APIs, Leaflet.

This project's objective is to visualize housing market data within the entire US.

First, Jupyter Notebook is used to write Python code to run an API query through the US Census Bureau site to get the most recent American Community Survey (2018) census data available at that time. The Python code creates a CSV file that is saved, and then that same CSV file is used to populate a database that was created by writing SQL code, and this created a SQL server to store the housing data at the zip code level.

To run this code, you will first need to set up a PostgreSQL server named Project_2. Then set your user account as admin2 with password: 12345 or update the code with your own superuser ID and password. Use the Table_creator code to make the column headings needed. Finally import the census_data_2018 CSV file.

This will set up the server so that the app.py can make the proper connections with the data.

Subsequently, I started on the JavaScript and created multiple functions to create and display the data. The user can enter a zip code for anywhere in the US and find the data that was pulled.

An API call is made to Zillow in real time to obtain market data on the Home Value Index by zipcode and the Rental index to visualize what areas may be better to buy in vs rent in. This was displayed using Plotly as bar graphs.

The area selected by the user is displayed in a Leaflet map automatically and changes whenever a new zipcode is entered.

At the same time a call is made to the SQL server based on the zipcode entered to display key market data for the area to display in the Market Highlights box as well as generate a pie chart below the map to show the number of houses built in that zip code in various year ranges.

Lastly to comply with Zillow's terms of using their API, a button with jQuery was created that when clicked, routes you to the Zillow website.
