# COMP30850 Assignment — Spring 2025/26

**Deadline: Sunday 8th March 2026**

## Overview

Analysing bike rental data can offer valuable insight into how people move around urban spaces, revealing patterns of everyday travel. This assignment involves applying **network analysis and visualisation** techniques to a Dublin bike rental dataset to identify hub stations, frequent routes between bike stations, and temporal trends.

The assignment should be implemented as a **single Jupyter Notebook** (not a script). Your notebook should be clearly documented, using comments and Markdown cells to explain the code and interpret the results of your analysis.

The data for the assignment is available at: http://mlg.ucd.ie/modules/COMP30850/bike-data.zip

This data contains two separate files:

1. **stations.csv** — Information about individual bike rental stations, one station per row with a unique identifier.
2. **rentals.csv** — List of bike rentals, one row per trip, including the identifiers of the start and end stations.

---

## Tasks

### Task 1 — Static Network Construction

a) To analyse the station-to-station movement, create an appropriate network representation from the raw data with the following properties:

- Each **node** represents a unique station, identified by a unique identifier. It should also have attributes containing the station's name and area.
- Each **edge** indicates one or more trips from an origin station to a different destination station.

### Task 2 — Static Network Characterisation

a) Apply a range of different methods to characterise the **structure and connectivity** of the bike-trip network created in Task 1.

b) Apply several different **centrality measures** to identify hub stations in the bike-trip network. Discuss how the centrality scores might be interpreted in each case.

c) Identify any stations with significant **positive net flow** (more arrivals than departures) and significant **negative net flow** (more departures than arrivals).

### Task 3 — Static Network Visualisation

a) Extract a subgraph containing only the stations located in the **'Northside' area** of Dublin. Export this subgraph as a **GEXF file**.

b) Load the GEXF file in **Gephi**. Use Gephi's layout functionality to create several useful visualisations of the subgraph highlighting different aspects such as overall connectivity structure. Export the final visualisations as **PNG files**.

### Task 4 — Dynamic Network Analysis

a) Using the dates associated with each trip, construct a set of **daily time networks** representing station-to-station movement on each day.

b) Apply various methods to characterise the **global structure and connectivity** of the daily networks. Compare these network-level metrics across different days and discuss any temporal patterns you observe.

c) By analysing station-level activity over time, identify stations where **capacity should be increased** by the bike rental operator.

---

## Use of Generative AI

You may use generative AI tools (e.g., ChatGPT, Copilot, Gemini), provided you disclose their use. At the beginning of your notebook, include an **"AI Use Statement"** in a Markdown cell — this is required even if you do not use any AI tools. **Penalties will apply** if this statement is missing or inaccurate.

---

## Guidelines

- The assignment must be completed **individually**. All submissions will be subject to plagiarism checking. Any evidence of plagiarism can result in a **0 grade**.
- The grade awarded will be based on the complexity and appropriateness of the analysis and the level of detail.
- Submit via **Brightspace** as a single ZIP file containing your `.ipynb` notebook, the GEXF file, and the Gephi PNG visualisations.
- **Late submission penalties:**
    - 1–5 calendar days late: 1 grade point deduction (e.g. B → B-)
    - 6–10 calendar days late: 2 grade point deduction (e.g. B → C+)
    - Assignments will **not be accepted** beyond 10 calendar days without formally approved Extenuating Circumstances.