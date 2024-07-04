# BelgHub

### Contents
This GitHub contains an excel-based industrial database for Belgium, providing data on (among other) ondustrial sites, their activities and production capacities.
The database applies TRILATE ids to uniquely identify the different industrial sites and products.

Four sheets are provided:
1) **facilities**
   Contains detailed information on the different industrial sites. Uniquelly identified by the TRILATE facility id 'TRILATE000'
3) **products**
   Expands on the industrial sites by adding the different products that ar eproduced on site.
   A single site can be linked to multiple products, which are now identified by a letter added to the facility id: 'TRILATE000A'
5) **metadata**
   Contains the references linked to the unique TRILATE product ids.
7) **sources_unique**
   Contians a unique list of the sources used in this database.
   For datapoints provided by the AidRES or hotmaps database, we refer to these databses as a source itself.
   
### Background
The database merges data from existing databases, starting from a list of facilities obtained from the ETS database [1], which was cross-linked with the IED/E-PRTR database [2] to collect geospatial information on facility-level. 
All possible data from the different sources are then combined, providing multiple values for the same datapoint when available. 
The industrial database selects the data based on a ranking of the data sources. 
If a datapoint is not available for a source with priority, the next source in the ranking is selected and so on. 
The main source for the industrial database is the AidRES database [3], launched in the summer of 2023. 
This database focusses on six key sectors or products: steel, chemicals, cement, glass, fertilizers and refineries.
For the production units that are not covered in this data source, a Flemish governmental database on Integrated Pollution Prevention and Control (IPPC) [4] is used to conduct a manual search. 
As a third data source, the Hotmaps database [5] is used to complete data gaps, mainly for the products in the pulp & paper and non-ferrous sectors. 
Lastly, desktop research was performed to fill in remaining crucial data gaps.

### Version history
4th of June 2024 - Version 0

### Acknowledgement
This work is supported via the energy transition funds project ‘Trilate’ organized by the FPS economy, S.M.E.s, Self-employed and Energy.

### Citation
[1] ETS database
[2] IED/E-PRTR database
[3] AidRES
[4] Flemish governmental database on Integrated Pollution Prevention and Control (IPPC)
[5] Hotmaps
