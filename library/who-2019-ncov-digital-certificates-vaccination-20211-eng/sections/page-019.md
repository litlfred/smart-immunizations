---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-019
section_title: "Page 19"
pages: 19-19
pdf_page: 19
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
2
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Introduction
SECTION 1
As Member States are increasingly looking to adopt digital solutions for a vaccination certificate for 
COVID-19, this document provides a baseline set of requirements for a compliant DDCC:VS solution that 
is interoperable with other standards-based solutions. With the baseline requirements met, it is also 
anticipated that Member States will further adapt and extend these specifications to suit their needs, most 
likely working with a local technology partner of their choice to implement a digital solution. 
This document is therefore software-agnostic and provides a starting point for Member States 
to design, develop and deploy a DDCC:VS solution for national use in whichever format best suits 
their needs (e.g. a paper card with a one-dimensional [1D] barcode or QR code stickers, or a fully 
functioning smartphone application developed internationally or locally). 
1.2.	 Target audience
The primary target audience of this document is national authorities tasked with creating or 
overseeing the development of a digital vaccination certificate solution for COVID-19. The document 
may also be useful to government partners such as local businesses, international organizations, non-
governmental organizations and trade associations, that may be required to support Member States in 
developing or deploying a DDCC:VS solution. 
1.3.	 Scope 
1.3.1.	In scope
This document specifically focuses on how to digitally document COVID-19 vaccination status and 
attest that an individual has received a vaccine (i.e. how to provide a signed digital vaccination 
certificate). Two priority scenarios are described in Table 1: Continuity of Care and Proof of 
Vaccination. This document describes a specification for a signed digital vaccination certificate, 
including:
	
→ethical and legal considerations, and privacy and data protection principles for the design, 
implementation and use of a DDCC:VS;
	
→use cases arising from the two scenarios for the operation of a DDCC:VS, including the sequence of 
steps involved in executing the scenarios;
	
→a core data set with the data elements that must be handled for a DDCC:VS describing vaccination 
status, as described in the use cases;
	
→a Health Level Seven (HL7) Fast Healthcare Interoperability Resources (FHIR) implementation 
guide based on the content outlined in this guidance document, to support the adoption of open 
standards for interoperability; and 
	
→approaches for implementing a DDCC:VS, including considerations for setting up a national trust 
framework to enable digital signing of a vaccination certificate.
