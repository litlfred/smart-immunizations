---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-044
section_title: "Page 44"
pages: 44-44
pdf_page: 44
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
27
SECTION 4
Proof of Vaccination scenario
SECTION
Proof of 
Vaccination 
scenario 
4 
This section describes the use cases and actors involved in using a 
DDCC:VS for Proof of Vaccination, as well as functional requirements 
for a digital solution. The Proof of Vaccination scenario relies on the 
PHA having access to a trusted means of digitally signing an HL7 FHIR 
document, which represents the core data set for the DDCC:VS. It will 
be up to Member States to define the purposes for which this scenario 
is applied and adapted to their own contexts and levels of digital 
maturity, in compliance with their legal and policy frameworks.
4.1.	 Key settings, personas and digital services
For the Proof of Vaccination scenario, there is one additional setting to consider: the verification 
site, where it is necessary for people to prove their COVID-19 vaccination status (such as a care site, a 
school, or an airport). How, when, where, and by whom the DDCC:VS can be verified should be defined 
by the Member State. The relevant policies, including data protection policies, should be put in place 
accordingly. 
These key personas (see Table 6) are anticipated to interact with digital services (see Table 7). Not 
all of these digital services will have a user interface that the key personas directly interact with, but 
they are still critical building blocks of the reference architecture.
