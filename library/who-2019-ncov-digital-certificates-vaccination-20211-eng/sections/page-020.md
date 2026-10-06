---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-020
section_title: "Page 20"
pages: 20-20
pdf_page: 20
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
3
SECTION 1
Introduction
1.3.2.	Out of scope
Aspects that are considered out of the scope of this work are: 
	
→digital documentation of COVID-19 laboratory test results (which will be covered in a separate 
guidance document);
	
→digital documentation of history of SARS-CoV-2 infection (which will be covered in a separate 
guidance document);
	
→digital documentation of COVID-19 recovery status because of the uncertainty around any 
immunity status arising from recovery;
	
→any governance, judgement or decision based on the information provided in a DDCC:VS for any 
purpose (e.g. its use as a vaccine passport);
	
→recording and handling of adverse event reporting;
	
→considerations for monitoring and evaluation of DDCC:VS roll-out and use;
	
→the choice of algorithm for generating any two-dimensional (2D) barcodes, which is at the 
discretion of the Member State. A Member State may augment the core data set with additional 
information (e.g. a passport number) to provide a stronger identity binding than is presumed in 
this document, for use cases that require it under existing Member State policies and regulations. 
Identity binding would enable utilization of existing 2D barcode algorithms such as those set out 
by the International Civil Aviation Organization (ICAO) and the European Union. The HL7 FHIR 
implementation guide (at https://WorldHealthOrganization.github.io/ddcc) provides an algorithm 
for generating 2D barcodes that may be used in the absence of identifying information beyond that 
found within the core data set; and
	
→technical functionality to support selective disclosure of information contained in DDCC:VS.
1.4.	 Assumptions
The technological specification for a DDCC:VS is intended to be flexible and adaptable for each Member 
State to meet its diverse public health needs as well as the diverse needs of individuals around the 
world. It is assumed that there is no one-size-fits-all solution, and so the specification must remain 
flexible and software-agnostic, while minimizing the amount of digital infrastructure required. 
The requirements outlined are intended to allow for DDCC:VS solutions to meet the needs of a 
country’s holistic public health preparedness and response plan, while still being usable in other 
national and local contexts. An overarching assumption is that multiple digital health products and 
solutions will be implemented to operationalize the requirements described in this document. This 
allows for support of local and sustainable development so that Member States have a broad choice of 
appropriate solutions without excluding compliant products from any source.
The following assumptions are made about Member States’ responsibilities as foundational aspects of 
setting up and running a DDCC:VS solution. 
	
→Member States will be responsible for implementing the policies necessary to support the 
DDCC:VS workflows, complying with their legal obligations under national and international 
law, including any applicable obligations related to respecting human rights and data protection 
policies.
