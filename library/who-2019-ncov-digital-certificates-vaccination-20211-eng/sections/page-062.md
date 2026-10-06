---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-062
section_title: "Page 62"
pages: 62-62
pdf_page: 62
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
45
SECTION 5
DDCC:VS core data set 
The vaccination certificate metadata contain data elements that are not typically visible to the 
user, but that are required to be linked to the certificate itself (see Table 12). It is anticipated that 
additional metadata elements will be added by Member States at the time of certificate generation to 
support specific use case implementations.
Table 12
Vaccination certificate metadata
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
Certificate issuer
The authority or authorized 
organization that issued the 
vaccination certificate.
String
Not applicable
Required
Required
Health certificate 
identifier (HCID)
Unique ID used to associate 
the vaccination status 
represented in a paper 
vaccination card to its digital 
representation(s).
ID
Not applicable
Required
Required
Certificate 
valid from
Date in which the certificate 
for a vaccination event 
became valid. No health or 
clinical inferences should be 
made from this date.
Date
Complete date, 
following ISO 8601 
Optional 
Optional 
Certificate valid 
until
Last date in which the 
certificate for a vaccination 
event is valid. No health or 
clinical inferences should be 
made from this date.
Date
Complete date, 
following ISO 8601 
Optional 
Optional 
Certificate schema 
version
Version of the core 
data set and HL7 FHIR 
implementation guide that 
the certificate is using.
String
Not applicable
Required
Required
FHIR: Fast Healthcare Interoperability Resources; HL7: Health Level Seven; ID: identifier; ISO: International Organization for Standardization.
