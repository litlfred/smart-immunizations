---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-017
section_title: "Page 17"
pages: 17-17
pdf_page: 17
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
xv
The minimum requirements for a DDCC:VS are as follows.
	
→The potential benefits, risks and costs of implementing a DDCC:VS solution should be assessed 
before introducing a DDCC:VS system and its associated infrastructure. This includes an impact 
assessment of the ethical and privacy implications and potential risks that may arise with the 
implementation of a DDCC:VS.
	
→Member States must establish the appropriate policies for appropriate use, data protection and 
governance of the DDCC:VS to reduce the potential harms, while achieving the public health 
benefits involved in deploying such a solution. 
	
→A digitally signed electronic version of the data about a vaccination event, called a DDCC:VS, must 
exist. As a minimum, both the required data elements in the core data set and the metadata should 
be recorded, as described in section 5.2.
	
→An individual who has received a vaccination should have access to proof of this – either as a 
traditional paper card or a version of the electronic DDCC:VS.
	
→Where a paper vaccination card is used, it should be associated with a health certificate identifier 
(HCID). A DDCC:VS should be associated, as a digital representation, with the paper vaccination 
card via the HCID. Multiple forms of digital representations of the DDCC:VS may be associated with 
the paper vaccination card via the HCID.
	
→The HCID should appear on any paper card in both a human-readable and a machine-readable 
format (i.e. alphanumeric characters that are printed, as well as rendered as a 1D or 2D barcode).
	
→A DDCC:VS Generation Service should exist. The DDCC:VS Generation Service is responsible for 
taking data about a vaccination event, converting it to use the FHIR standard, and then digitally 
signing the FHIR document and returning it to the DDCC:VS Holder. This signed FHIR document is 
the DDCC:VS.
	
→A DDCC:VS Registry Service should exist. The DDCC:VS Registry Service is responsible for storing 
an index that associates an HCID with metadata about the DDCC:VS. As a minimum, the Registry 
Service stores the core metadata described in section 5.2. One or more DDCC:VS Repository 
Service(s) may exist, which can be used to retrieve a DDCC:VS; in which case the location of the 
DDCC:VS may also be included in the metadata within the DDCC:VS Registry Service. 
The different services are discussed in more detail in sections 3 and 4, and are shown in Fig. 7.
These components are minimum requirements; Member States may adopt and develop additional 
components for their deployed DDCC:VS system.
