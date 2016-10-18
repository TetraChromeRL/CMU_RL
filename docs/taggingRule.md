# Data Tagging Guidelines (Standardization) for Logbook ATA Chapters

## Overview   
This page outlines a set of rules to use when annotating data for Condition, Component, Location, Result, and Action entities for use within Tetrachrome and the overall Information Exraction project (CMU and Boeing). This document attempts to make clear rules which should be applied given ambiguous tagging situations.


### Entity Descriptions
**Component:** A part of the airplane.  
**Location:** A location within the airplane, specific enough to generally get you within arm's length of a Condition or Component. Also, directional information which disambiguates one Component from another or helps to identify it(them) specifically.     
**Condition:** A specific situation which has occurred or is occurring with regards to a Component or Location.
**Action:** A task which is/was carried out to attempt to resolve the Condition present in the record.  
**Result:** The outcome of an Action.  


### Intuition

Example:   
![Intuition Example](IMG/Intuition.png)   
The above example can be thought of in two main ways and occurs frequently.   
SUBJECT TEXT: "LEADING EDGESTANDBY SHUTOFF VALVE ELECTRICAL CONNECTOR"    
 
Component: "LEADING EDGESTANDBY SHUTOFF VALVE ELECTRICAL CONNECTOR"    
Location: ""   


Example:   
![Intuition Example 2](IMG/Intuition2.png)     
SUBJECT TEXT: "RH WING LEADING EDGESTANDBY SHUTOFF VALVE ELECTRICAL CONNECTOR"   
 
Component: "LEADING EDGESTANDBY SHUTOFF VALVE ELECTRICAL CONNECTOR"    
Location: "RH WING"   
 

### Examples   

#### DISC_CMPLNT_TX (Logbook complaint text entries)  
![ATA 25 Number 1](IMG/Complaint/Logbook1.png)  
Application of Guideline 7. RH, RRH, and LH are not tagged as they are considered sub-Compoent level location information. 25J is annotated as Location in application of Guideline  6, 3, and 4.
![ATA 25 Number 2](IMG/Complaint/Logbook2.png)  
Location information preceding a Component.
![ATA 25 Number 4](IMG/Complaint/Logbook4.png)  
Multiple individual SEAT Locations.
![ATA 24 Number 1](IMG/Complaint/Logbook5.png)  
M19 is not sufficient data to locate the Circuit Breaker being referenced so is annotated as Component.
![ATA 24 Number 4](IMG/Complaint/Logbook8.png)  
P320 is the location of a specific Panel, J10 and L3 are the locational information of the sub-Component CIRCUIT BREAKER so is annotated as Component.
  
#### MAINT_ACT_TX (Logbook maintenance action text entries)  
![ATA 24 Number 1](IMG/Action/Logbook9.png)  
![ATA 24 Number 2](IMG/Action/Logbook10.png)  
![ATA 24 Number 4](IMG/Action/Logbook12.png)  
![ATA 24 Number 1](IMG/Action/Logbook13.png)  
![ATA 24 Number 2](IMG/Action/Logbook14.png)  
![ATA 24 Number 3](IMG/Action/Logbook15.png)  
