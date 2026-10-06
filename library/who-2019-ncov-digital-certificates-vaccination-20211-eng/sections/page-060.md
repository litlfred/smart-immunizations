---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-060
section_title: "Page 60"
pages: 60-60
pdf_page: 60
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
43
SECTION 5
DDCC:VS core data set 
The data elements for each vaccination event section outlines data that need to have been collected 
for each vaccination the vaccinated person received (see Table 11). For each dose, all the data 
elements in Table 11 are required to have been recorded. In paper form, this is equivalent to a separate 
row on a vaccination certificate that is then repeated for each vaccination received. 
Table 11
Data for each vaccination event, with preferred code system	
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
Vaccine or 
prophylaxis
Generic description of the 
vaccine or vaccine sub-type 
(e.g. COVID-19 mRNA vaccine, 
HPV vaccine).
Coding
ICD-11
Required 
Required 
Vaccine brand
The brand or trade name 
used to refer to the vaccine 
received.
Coding
As defined by 
Member State
Required 
Required 
Vaccine 
manufacturer
Name of the manufacturer 
of the vaccine received (e.g. 
Serum Institute of India, 
AstraZeneca). If vaccine 
manufacturer is unknown, 
market authorization holder 
is REQUIRED.
Coding
As defined by 
Member State
Required – 
conditional
Required – 
conditional
Vaccine market 
authorization holder
Name of the market 
authorization holder of 
the vaccine received. If 
market authorization 
holder is unknown, vaccine 
manufacturer is REQUIRED.
Coding
As defined by 
Member State
Required – 
conditional
Required – 
conditional
Vaccine batch 
number 
Batch number or lot number 
of the vaccine.
String
Not applicable
Required 
Required 
Date of vaccination
Date on which the vaccine 
was provided.
Date
Complete date, 
following ISO 8601 
Required 
Required 
Vaccination 
valid from
Date upon which provided 
vaccination is considered 
valid
This data should only be 
considered valid at the time 
of issuance, as guidance is 
likely to evolve with further 
scientific evidence.  Any 
user of this data (Vaccinator, 
Verifier) should validate 
this date according to their 
national policy.  
In the case of repeated 
doses, the data field for a 
subsequent dose should 
override the data field for a 
predecessor dose.
Date
Complete date, 
following ISO 8601
Optional
Optional
Dose number
Vaccine dose number.
Quantity
Not applicable
Required 
Required
