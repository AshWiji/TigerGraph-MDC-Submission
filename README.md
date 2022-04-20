# TigerGraph-MDC-Submission
Anti-Mafia Network Analytics Platform


# Anti-Mafia Network Analytics Platform
**Contributers and Contact Information**

Sebastian Coles sebastiancoles@kubrickgroup.com
William McCreery williammccreery@kubrickgroup.com
Gilson Aquino gilsonaquino@kubrickgroup.com
Katie Pegrum katiepegrum@kubrickgroup.com
Ashley Wijesuriya ashleywijesuriya@kubrickgroup.com


**Problem Statement**

Criminal organisations are responsible for various illicit activities, which inevitably result in a reduced safety to the general public, as well as costing the government billions in damages every year. Unfortunately, the members, structure and overall reach of such organisations are very difficult to identify, a problem which is further exacerbated by the fact that many members of these organisations have been infiltrated within law enforcement agencies with the goal of facilitating their endeavours.

As it stands it would seem that law enforcement agencies are having a tough time keeping up with the task of eradicating these criminal entities, especially given that these criminal individuals can rather quickly reorganise themselves within a new organisation upon the dissolution of the previous. On the other hand, allowing these organisations to remain uncheck will result in the continuing proliferation of drugs and violent crimes, this is a problem we as a society need to correct.

**Description**: 

Serious and organised crime is estimated to cost the UK economy at least £37 billion a year, hence the public funds which would be freed up as a result of identify and disrupting members of these organisations can be repurposed towards projects that can improve quality of life and infrastructure.

A major activity undertaken by these criminal organisations  is drug trafficking, this inevitably leads to thousands of people succumbing to addiction. As such, reducing the illegal import of drugs would inevitably result in an increase in public health, as well as increased workforce participation from individuals who might have otherwise become addicts. Furthermore, reduction in the occurrence of violent crimes would make for a safer environment for the general public.

Therefore, it is clear to see that the identification and subsequent disruption of these criminal organisations would greatly improve society both socially and financially. On the other hand, this use case of graph technology could drastically reduce the time taken for the structure of a crime organisation to be uncovered, and hence lead to faster and more plentiful abolition of such organisations. As well as a cleaner and more dedicated law enforcement agency.

Our project pushes the boundaries of what it means to be connected. We draw connections between individuals on a multitude of categories with varying importance, the connections generated go beyond what could be feasible with the naked eye.
Our schema encompasses data pertaining to members of the public, law enforcement agencies and criminal organisations. Ideally every citizen would be represented on this graph, thus allowing us to see how people link to one another, may it be through family ties, a transaction made regularly or once a few years ago, a message sent, or even a call received. The network generated from all these links would allow no connection to go unseen. 
Imagine a police force where all corrupt agents can be easily identified and perhaps even used without their knowledge to reach the criminals, imagine being able to determine all individuals belonging to these organisations and their structure, imagine the ability to determine location hotspots for criminal recruiting, and subsequently being able to implement government programmes to pacify such regions, in essence cutting these organisations from their supply of henchmen.
Implementing such a tool could allow a drastic reduction in the number of illicit activities and thus lead to a safer and more righteous society.


## Dependencies

This project requires the schema to be setup and mapped to the correct CSV files. More details are explained below.

## Installation

Please follow the steps below to access and run our project.

1. Clone repository to your local machine
2. Look inside the "Export_Schema_And_Mapping" folder. Import the "Schema_Data_Mapping_And_Queries_Mapping_The_Mafia.gz" file into Graph Studio to get our Graph Schema and Data Mapping
3. Map the data file CSV's located in the "Data" folder to the Nodes and Edges
4. Copy and Paste the GSQL queries in the GSQL folder into the Tiger Graph query editor and run them.
5. Alternatively, Web_Link: "https://modeling-the-mafia.i.tgcloud.io/#/home"

## Query Details:

1) Avg_Bank_Transaction_Mafia_Boss: This query returns the Banks that Mafia Bosses use and the average transfer made at each bank

2) Avg_Bank_Transaction_Mafia_Member: This query returns the Banks that Mafia Members use and the average transfer made at each bank

3) Corruption_By_City: This query returns the Locations and the normalised corruption rating of each city (Counts of corruption in the city / max city corruption count)

4) Crime_Count_By_Location: This query returns the count of instances of crime for each

5) Crime_Type_By_City: This query returns returns key value pairs detailing the number of each crime type per city

6) Mafia_Boss_Per_Bank: This query returns a count of the Mafia Bosses using each bank respectively

7) Police_Transactions_Sum_Over_All_Time: This query returns the sum of bank transactions each member of the polcie have made. Police with significantly high transactions are more likely to be involved in the Mafia

8) Police_With_Failed_Raids_Linked_To_Mafia: This query returns the police officers who have contacted individuals in the Mafia and have failed one or more police raids (of Mafia premises)

9) Police_With_One_Or_More_Failed_Raid: This query returns the police officers who have failed one or more police raids (of Mafia premises)

10) Sum_Of_Police_Transactions_With_Mafia_Connections: This query returns the sum of bank transactions of police officers who have bene in contact with individuals in the mafia

## Known Issues and Future Improvements

The synthetic data was randomised and as a result it was difficult to show insights for everything. Future improvements include having access to real organised crime data. 
