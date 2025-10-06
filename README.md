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
--------------------------------------------------------------------

The links to each part of the project: 

Report: https://github.com/Ank1r0/Report_PowerBI

Data cube: https://github.com/Ank1r0/SSAS_CPD_CRASHES

ETL: https://github.com/Ank1r0/CPD_CRASH_SSIS-ETL-

--------------------------------------------------------------------
Questions: 

1: Impact of Road & Weather Conditions on Crashes(How weather and road conditions affect crashes.) 

2: Hit-and-Run Crash Patterns (How the weather, injuries and crash type affect hit-and-run) 

3: Time-Based Crash Trends(Identify pick crash period and season) 

4: The most severe injury based on maximal speed in crash area 

5: Weather based Crash trends, how weather impact on crash occurance 

6: Weather based injuries, how weather impact on injuries 

7: Road surface and defects impact on crash primary and secondary cause 

8: Severity of injuryries based on crushtype 

9: Weather based crash type 

10: Traffic control device condition on crash type 
 

Extra: 

Heatmap crash location visualisation. 

Streets Ranked by Number of Crash Injuries

--------------------------------------------------------------------
About each column from the original dataset.

CRASH_RECORD_ID 

This number can be used to link to the same crash in the Vehicles and People datasets. This number also serves as a unique ID in this dataset. 

CRASH_DATE_EST_I 

Crash date estimated by desk officer or reporting party (only used in cases where crash is reported at police station days after the crash) 

CRASH_DATE 

Date and time of crash as entered by the reporting officer 

POSTED_SPEED_LIMIT 

Posted speed limit, as determined by reporting officer 

TRAFFIC_CONTROL_DEVICE 

Traffic control device present at crash location, as determined by reporting officer 

DEVICE_CONDITION 

Condition of traffic control device, as determined by reporting officer 

WEATHER_CONDITION 

Weather condition at time of crash, as determined by reporting officer 

LIGHTING_CONDITION 

Light condition at time of crash, as determined by reporting officer 

FIRST_CRASH_TYPE 

Type of first collision in crash 

TRAFFICWAY_TYPE 

Trafficway type, as determined by reporting officer 

LANE_CNT 

Total number of through lanes in either direction, excluding turn lanes, as determined by reporting officer (0 = intersection) 

ALIGNMENT 

Street alignment at crash location, as determined by reporting officer 

ROADWAY_SURFACE_COND 

Road surface condition, as determined by reporting officer 

ROAD_DEFECT 

Road defects, as determined by reporting officer 

REPORT_TYPE 

Administrative report type (at scene, at desk, amended) 

CRASH_TYPE 

A general severity classification for the crash. Can be either Injury and/or Tow Due to Crash or No Injury / Drive Away 

INTERSECTION_RELATED_I 

A field observation by the police officer whether an intersection played a role in the crash. Does not represent whether or not the crash occurred within the intersection. 

Read more 

NOT_RIGHT_OF_WAY_I 

Whether the crash begun or first contact was made outside of the public right-of-way. 

HIT_AND_RUN_I 

Crash did/did not involve a driver who caused the crash and fled the scene without exchanging information and/or rendering aid 

DAMAGE 

A field observation of estimated damage. 

DATE_POLICE_NOTIFIED 

Calendar date on which police were notified of the crash 

PRIM_CONTRIBUTORY_CAUSE 

The factor which was most significant in causing the crash, as determined by officer judgment 

SEC_CONTRIBUTORY_CAUSE 

The factor which was second most significant in causing the crash, as determined by officer judgment 

STREET_NO 

Street address number of crash location, as determined by reporting officer 

STREET_DIRECTION 

Street address direction (N,E,S,W) of crash location, as determined by reporting officer 

STREET_NAME 

Street address name of crash location, as determined by reporting officer 

BEAT_OF_OCCURRENCE 

Chicago Police Department Beat ID. Boundaries available at https://data.cityofchicago.org/d/aerh-rz74 

PHOTOS_TAKEN_I 

Whether the Chicago Police Department took photos at the location of the crash 

STATEMENTS_TAKEN_I 

Whether statements were taken from unit(s) involved in crash 

DOORING_I 

Whether crash involved a motor vehicle occupant opening a door into the travel path of a bicyclist, causing a crash 

WORK_ZONE_I 

Whether the crash occurred in an active work zone 

WORK_ZONE_TYPE 

The type of work zone, if any 

WORKERS_PRESENT_I 

Whether construction workers were present in an active work zone at crash location 

NUM_UNITS 

Number of units involved in the crash. A unit can be a motor vehicle, a pedestrian, a bicyclist, or another non-passenger roadway user. Each unit represents a mode of traffic with an independent trajectory. 

Read more 

MOST_SEVERE_INJURY 

Most severe injury sustained by any person involved in the crash 

INJURIES_TOTAL 

Total persons sustaining fatal, incapacitating, non-incapacitating, and possible injuries as determined by the reporting officer 

INJURIES_FATAL 

Total persons sustaining fatal injuries in the crash 

INJURIES_INCAPACITATING 

Total persons sustaining incapacitating/serious injuries in the crash as determined by the reporting officer. Any injury other than fatal injury, which prevents the injured person from walking, driving, or normally continuing the activities they were capable of performing before the injury occurred. Includes severe lacerations, broken limbs, skull or chest injuries, and abdominal injuries. 

Read more 

INJURIES_NON_INCAPACITATING 

Total persons sustaining non-incapacitating injuries in the crash as determined by the reporting officer. Any injury, other than fatal or incapacitating injury, which is evident to observers at the scene of the crash. Includes lump on head, abrasions, bruises, and minor lacerations. 

Read more 

INJURIES_REPORTED_NOT_EVIDENT 

Total persons sustaining possible injuries in the crash as determined by the reporting officer. Includes momentary unconsciousness, claims of injuries not evident, limping, complaint of pain, nausea, and hysteria. 

Read more 

INJURIES_NO_INDICATION 

Total persons sustaining no injuries in the crash as determined by the reporting officer 

INJURIES_UNKNOWN 

Total persons for whom injuries sustained, if any, are unknown 

CRASH_HOUR 

The hour of the day component of CRASH_DATE. 

CRASH_DAY_OF_WEEK 

The day of the week component of CRASH_DATE. Sunday=1 

CRASH_MONTH 

The month component of CRASH_DATE. 

LATITUDE 

The latitude of the crash location, as determined by reporting officer, as derived from the reported address of crash 

LONGITUDE 

The longitude of the crash location, as determined by reporting officer, as derived from the reported address of crash 

LOCATION 

The crash location, as determined by reporting officer, as derived from the reported address of crash, in a column type that allows for mapping and other geographic analysis in the data portal software 

 

