# Housing-Element-Analysis

This repository contains notebooks demonstrating the data analysis process for the Sites Inventory documents in California Housing Elements. I use San Diego and South Pasadena as example municipalities to walk through some of the unique problems that arise when working with these datasets. By joining a municipality's list of sites identified for housing development during the 2021-2019 (6th) Housing Element cycle with geocoded parcel data and block-group level household income data from the Census, we can visualize the spatial distribution of potential future housing production and conduct a basic analysis of how a given jurisdiction intends to distribute low-income housing over its various neighborhoods. Dr. Paavo Monkkonen of UCLA Urban Planning developed a process to apply a Gini coefficient methodology to compare the actual distribution of low-income housing sites with a perfectly equal distribution of sites throughout the city, as one measure of the city's fulfillment of California affirmatively furthering fair housing (AFFH) requirements. In brief, the steps are as follows:
1. Download the municipality's Sites Inventory document
2. Extract the table data from the PDF
3. Clean the extracted data (in Excel or Python)
4. Download land parcel data
5. Download median household income Census data
6. Join the Sites Inventory and parcel datasets to produce a geocoded Sites Inventory dataset
7. Join the geocoded Sites Inventory with Census data
8. Apply the Gini methodology to the final dataset to calculate an AFFH score
