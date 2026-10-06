---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-096
section_title: "Page 96"
pages: 96-96
pdf_page: 96
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
79
The registries and repositories defined in the OpenHIE architecture (see Fig. A6.1) may play a role in 
providing data that are part of the DDCC:VS core data set defined in section ‎5. These registries and 
repositories include the following: 
TERMINOLOGY SERVICES: A registry service used to manage clinical and health system terminologies, 
which health applications can use for mapping to other standard or non-standard code systems 
to support semantic interoperability. For example, a terminology service can be used to manage 
terminology mappings of existing code systems to the International Classification of Diseases, 11th 
revision (ICD-11). 
CLIENT REGISTRY: Also referred to as a patient registry, a demographic database that contains 
definitive information about each Subject of Care. This database can include a Subject of Care’s 
name, date of birth, sex, address, phone number, email address, as well as other person-specific 
information such as parent–child relationships, caregiver relationships, family–clinician relationships 
and consent directives. It is also in the client registry that the list of unique identifiers (IDs; e.g. 
national ID, national health ID, health insurance ID) for a particular Subject of Care can be found. The 
data elements in the DDCC:VS core data set that may be populated with data from the client registry 
include:
	
→name 
	
→date of birth 
	
→sex 
	
→unique IDs. 
FACILITY REGISTRY: A database of facility information, including data such as the facility name, a Public 
Health Authority (PHA)-issued unique ID, the organization under whose responsibility the facility 
operates, location (by address and/or Global Positioning System [GPS] coordinates), facility type, 
hours of operation, and the health services offered. The data elements in the DDCC:VS core data set 
that may be populated with data from the facility registry include:
	
→administering centre: facility name or unique ID can be used to represent this
	
→country of vaccination. 
HEALTH WORKER REGISTRY: A database of health worker information that contains information such 
as name, date of birth, and qualifications of health workers (including cadre, accreditations and 
authorizations of practice). The health worker registry also references unique health worker IDs that 
may have been issued by a PHA, care delivery organizations or individual health facilities. The data 
element in the DDCC:VS core data set that may be provided with information from the health worker 
registry is:
	
→health worker ID.
