# Report_PowerBI
Project: Chicago Traffic Crash Data Analytics Pipeline
Description: Developed a comprehensive, end-to-end data analytics solution to process and analyze over 1.5 million records from the Chicago Police Department's public traffic crash database. The project transformed raw, inconsistent CSV data into interactive, actionable business intelligence to uncover critical insights into crash causality, severity, and patterns.

Technical Stack: SQL Server (T-SQL), SQL Server Integration Services (SSIS), SQL Server Analysis Services (SSAS), Power BI, DAX, MDX

Key Responsibilities & Achievements:

Data Engineering (ETL):

Designed and built a robust, scalable SSIS package to extract, clean, and validate data from multiple large-scale CSV sources (Crashes, Vehicles, People).

Engineered a custom data cleansing pipeline to handle incomplete fields, inconsistent entries, and data quality issues inherent in the public dataset.

Loaded transformed and conformed data into a SQL Server data warehouse with a optimized star-schema for analytical performance.

Data Modeling & OLAP:

Architected a multi-dimensional data cube using SSAS to enable complex, multi-faceted analysis across dimensions of time, location, weather, and road conditions.

Defined calculated members and Key Performance Indicators (KPIs) within the cube to measure crash frequency, injury severity, and hit-and-run rates.

Data Visualization & Analysis:

Developed an interactive Power BI report featuring drill-down capabilities and dynamic filtering to explore the 10+ key analytical questions.

Synthesized complex data into clear visualizations, including time-series trends, heatmaps of crash locations, and ranked comparisons.

Core Analytical Insights Delivered:

Quantified the impact of adverse weather and poor road surface conditions on crash frequency and injury severity.

Identified temporal patterns and peak periods for crashes to inform resource allocation.

Uncovered characteristics and contributing factors prevalent in hit-and-run incidents.

Analyzed the relationship between posted speed limits and the severity of resulting injuries.

Ranked streets and intersections by crash and injury count to prioritize safety improvements.

The links to each part of the project: 

Report: https://github.com/Ank1r0/Report_PowerBI

Data cube: https://github.com/Ank1r0/SSAS_CPD_CRASHES

ETL: https://github.com/Ank1r0/CPD_CRASH_SSIS-ETL-



