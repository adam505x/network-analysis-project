## Movement Networks

- Movement networks represent how people move through urban spaces, with locations (like bike stations) as nodes and trips between them as connecting edges.
    
    ![](attachment:9d52fdbd-c791-49b1-989a-5c6f6c61c7a7:imageseb458bef-7453-456e-9901-ef146a500d7c-01_1222_1604_761_693.jpg)
    

## COMP30850 Assignment

## Summary:

Analysing bike rental data can offer valuable insight into how people move around urban spaces, revealing patterns of everyday travel. This assignment involves applying network analysis and visualisation techniques to a Dublin bike rental dataset to identify hub stations, frequent routes between bike stations, and temporal trends.

## Dataset:

The data for the assignment is available at the link below.

## http://mlg.ucd.ie/modules/COMP30850/bike-data.zip

## Deadline: Sunday 8th March 2026

## COMP30850 Assignment - Data

- The data contains two separate CSV files:
1. stations.csv: Information about individual bike rental stations, one station per row with a unique identifier.
2. rentals.csv: List of bike rentals, one row per trip, including the identifiers of the start and end stations.

```
station_id,name,capacity,area
ST_0001,Smithfield North,42,Northside
ST_0002,Parnell Square North,45,Northside
ST_0003,Clonmel Street,40,Southside
ST_0004,Avondale Road,40,Northside
ST_0005,Mount Street Lower,38,Southside
ST_0006,Christchurch Place,43,Southside
ST_0007,Grantham Street,39,Southside
ST_0008,Pearse Street,43,Southside
ST_0009,York Street East,41,Southside
ST_0010,Excise Walk,42,Northside
```

```
year,month,day,hour,start_station_id,end_station_id
2026,1,27,19,ST_0018,ST_0057
2026,1,26,16,ST_0028,ST_0041
2026,1,31,7,ST_0013,ST_0060
2026,1,28,10,ST_0064,ST_0095
2026,1,26,12,ST_0020,ST_0042
2026,1,28,7,ST_0089,ST_0108
2026,1,26,17,ST_0018,ST_0066
2026,1,28,10,ST_0102,ST_0002
2026,1,29,14,ST_0068,ST_0063
2026,1,31,15,ST_0083,ST_0064
```

## COMP30850 Assignment - Tasks

- Task 1: Static Network Construction
- To analyse the station-to-station movement, create an appropriate network representation from the raw data with the following properties:
- Each node represents a unique station, identified by a unique identifier. It should also have attributes containing the station’s name and area.
- Each edge indicates one or more trips from an origin station to a different destination station.

## COMP30850 Assignment - Tasks

- Task 2: Static Network Characterisation
- Apply a range of different methods to characterise the structure and connectivity of the bike-trip network created in Task 1.
- Apply several different centrality measures to identify hub stations in the bike-trip network. Discuss how the centrality scores might be interpreted in each case.
- Identify any stations with significant positive net flow (more arrivals than departures) and significant negative net flow (more departures than arrivals).

## COMP30850 Assignment - Tasks

- Task 3: Static Network Visualisation
- Extract a subgraph from the bike-trip network created in Task 1 containing only the stations located in the ‘Northside’ area of Dublin. Export this subgraph as a GEXF file.
- Load the GEXF file in Gephi. Use Gephi’s layout functionality to create several useful visualisations of the subgraph. Your visualisations should highlight different aspects such as the network’s overall connectivity structure. Export the final visualisations as PNG files.

## COMP30850 Assignment - Tasks

- Task 4: Dynamic Network Analysis
- Using the dates associated with each trip, construct a set of daily time networks representing station-to-station movement on each day.
- Apply various methods to characterise the global structure and connectivity of the daily networks. Compare these network-level metrics across different days and discuss any temporal patterns you observe.
- By analysing station-level activity over time, identify stations where capacity should be increased by the bike rental operator.

## COMP30850 Assignment - Rubric

| Task | Component | Mark |
| --- | --- | --- |
| Task 1 | Static Network Construction  - Data loading and parsing  - Construction of an appropriate static network | 15 |
| Task 2 | Static Network Characterisation  - Characterisation of the static network  - Centrality analysis of the static network  - Identify any stations with significant positive net flow and significant negative net flow | 30 |
| Task 3 | Static Network Visualisation  - Creation and export of the required subgraph  - Visualisations of the subgraph using Gephi | 20 |
| Task 4 | Dynamic Network Analysis  - Creation of time window networks  - Analysis of the time window networks using global measures  - Identify stations where capacity should be increased | 25 |
| General | - Al Use Statement  - Python code quality and notebook structure  - Use of Markdown cells for interpretation and explanation | 10 |

## COMP30850 Assignment - Guidelines

- You may use generative AI tools for this assignment (e.g., ChatGPT, Copilot, Gemini), provided you disclose their use as described below.
- At the beginning of your notebook, you must include an “AI Use Statement” in a Markdown cell.
- This is required even if you did not use any generative AI tools.
- If you do use generative AI, list the tool (and model, if known) and describe how it was used (e.g., understanding data, debugging or generating code).
- Penalties will apply if this statement is missing or inaccurate.

## COMP30850 Assignment - Guidelines

- The assignment should be completed individually. All submissions will be subject to plagiarism checking. Any evidence of plagiarism can result in a 0 grade.
- The grade awarded will be based on the complexity and appropriateness of the analysis and the level of detail.
- Submit your assignment via Brightspace. Your submission should be in the form of a single ZIP file containing your notebook file (.IPYNB), the GEXF file exported in Task 3, and the PNG files for the visualisations created in Gephi.
- Due by end of Sunday 8th March. This is a hard deadline, penalties apply for late submission. Assignments will not be accepted any later than 10 calendar days without Extenuating Circumstance.

## COMP30850 Assignment - Guidelines

- Assignment is worth $40 \%$ of overall module grade.
- See the assignment PDF on Brightspace for full details.

## COMP30850 Assignment - Spring 2025/26

Deadline: Sunday 8th March 2026

## Overview

Analysing bike rental data can offer valuable insight into how people move around urban spaces, revealing patterns of everyday travel. This assignment involves applying network analysis and visualisation techniques to a Dublin bike rental dataset to identify hub stations, frequent routes between bike stations, and temporal trends.

The assignment should be implemented as a single Jupyter Notebook (not a script). Your notebook should be clearly documented, using comments and Markdown cells to explain the code and interpret the results of your analysis.

The data for the assignment is available at the link below.
http://mlg.ucd.ie/modules/COMP30850/bike-data.zip