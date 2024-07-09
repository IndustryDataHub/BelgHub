# BelgHub

### Contents
This GitHub contains an excel-based industrial database for Belgium, providing data on industrial sites, their coordinates, address and activities. For each of these industrial sites, the corresponding data reported in the Emissions Trading System (ETS in short) is mentioned for the year 2022 **(add others?) **as well as the ETS identifier. Also production capacities are listed in the database. Details on the data collection methodology for these columns are shared below.
The database applies TRILATE ids to uniquely identify the different industrial sites and products.

Four sheets are provided:
1) **facilities**\
   Contains detailed information on the different industrial sites. Uniquelly identified by the TRILATE facility id 'TRILATE000'
3) **products**\
   Expands on the industrial sites by adding the different products produced on site.
   A single site can be linked to multiple products, which are now identified by a letter added to the facility id: 'TRILATE000A'
5) **metadata**\
   Contains the references linked to the unique TRILATE product ids.
7) **sources_unique**\
   Contains a unique list of the sources used in this database.
   For datapoints retrieved from the AIDRES or hotmaps database, we refer to these databses as a source itself.
   
### Background and methodology
The database merges data from existing databases, starting from a list of facilities obtained from the [ETS database](url), which was cross-linked with the [IED/E-PRTR database](url) to collect geospatial information on facility-level. The industrial sector scope is limited to energy intensive industries; cement and lime, ceramics, chemicals, fertilisers, food and drinks, glass, non-ferrous metals, paper and pulp, refineries, steel. Next, a desktop study was performed to identify the products produced at each of these facilities and the total production capacities. The authors of this database relied on available, public information and projects with similar scopes like [AIDRES](url) and [Hotmpas](url). 
All possible data from the different sources are combined, providing multiple values for the same datapoint when available. 
The industrial database selects the data based on a ranking of the data sources. 
If a datapoint is not available for a source with priority, the next source in the ranking is selected and so on. 
The main source for the industrial database is the [AIDRES](url) database, launched in the summer of 2023. 
This database focusses on six key sectors or products: steel, chemicals, cement, glass, fertilizers and refineries.
For the production units that are not covered in this data source, a Flemish governmental database on [Integrated Pollution Prevention and Control (IPPC)](url) is used to conduct a manual search. 
As a third data source, the [Hotmaps database](url) is used to complete data gaps, mainly for the products in the pulp & paper and non-ferrous sectors. 
Lastly, further desktop research was performed to fill in remaining crucial data gaps.

### Regionalization Tool
Enya Lenaerts, Negar Namazifard, Nienke Dhondt, Juan Correa Laguna, Pieter Valkering,
The regionalization tool: mapping future Belgian energy needs by coupling a long-term investment planning model with a national industry database.
20th International Conference on European Energy Markets 2024, IEEEXplore. (soon to be published)


### Belgium Hydrogen Network Analysis
Negar Namazifard, Pieter Vingerhoets, Erik Delarue,
Long-term cost optimization of a national low-carbon hydrogen infrastructure for industrial decarbonization,
International Journal of Hydrogen Energy, https://doi.org/10.1016/j.ijhydene.2024.02.324.

### Clustered Based Node Selection for Energy System Modelling
Dhondt, N., Mendez Alva, F., & Van Eetvelde, G. (2024). Introducing industrial clusters in multi-node energy system modelling by the application of the industry–infrastructure quadrant. SUSTAINABILITY, 16(6). https://doi.org/10.3390/su16062585

### Version history
4th of June 2024 - Version 0

### Acknowledgement
This work is supported via the energy transition funds project ‘Trilate’ organized by the FPS economy, S.M.E.s, Self-employed and Energy.
