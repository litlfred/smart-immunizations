---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-059
section_title: "Page 59"
pages: 59-59
pdf_page: 59
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
42
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
DDCC:VS core data set
SECTION 5
5.2.	 Core data elements
The three key sections of the core data set are: 
1.	
the header 
2.	
data elements for each vaccination event 
3.	
vaccination certificate metadata.
The header section data elements include the Subject of Care’s ID information (see Table 10). The 
header section is intended to capture information about the vaccinated individual to allow for 
information on the vaccination event to be linked to a specific person. This data should remain the 
same regardless of which vaccination a person has received; thus, it should only be collected once. 
Table 10
Header section of the DDCC:VS with preferred code system
Data element label
Description
Data type
Preferred code 
system
Requirement status 
for Continuity of 
Care
Requirement 
status for Proof of 
Vaccination
Name
The full name of the 
vaccinated person.
String
Not applicable
Required
Required
Date of birth 
The vaccinated person’s date 
of birth (DOB), if known. If 
unknown, use assigned DOB 
for administrative purposes. 
Date
Complete date, 
following ISO 8601 
(YYYYMMDD or 
YYYY-MM-DD)
Required 
Required 
Unique identifier
Unique ID for the vaccinated 
person, according to the 
policies applicable to each 
country. There can be more 
than one unique ID used to 
link records (e.g. national 
ID, health ID, immunization 
information system ID, 
medical record ID).
ID
Not applicable
Optional –
recommended
Optional –
recommended
Sex
Documentation of a specific 
instance of sex information 
for the vaccinated person.
Coding1
As defined by 
Member State
Optional –
recommended
Not needed 
ID: identifier; ISO: International Organization for Standardization.
1 	 Coding data elements are multiple choice and the input options, or values, are data elements taken from a set of predefined options (e.g. 
sex, vaccine or prophylaxis, vaccine brand).
