---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-058
section_title: "Page 58"
pages: 58-58
pdf_page: 58
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
41
SECTION 5
DDCC:VS core data set 
	
→NOT ALL DATA ELEMENTS NEED TO BE IN THE VACCINATION CERTIFICATE. Aligned with the principle of 
capability, flexibility and sustainability, the vaccination certificate is intended to be part of a much 
larger ecosystem of immunization information systems which include:
	»
EIRs (such as OpenSRP [27]);
	»
reporting systems for vaccine coverage monitoring (such as District Health Information Software 2; 
DHIS2 [28]); and
	»
AEFI reporting systems (such as Vigiflow [29]).
To underscore the importance of the ability to implement, the data content model for the DDCC:VS 
core data set has been developed as an HL7 FHIR implementation guide. The DDCC vaccination 
certificate implementation guide1 is based on the widely adopted HL7 FHIR International Patient 
Summary (IPS) health data content model (30). 
International Classification of Diseases (ICD) is the preferred data standard for DDCC:VS. The 11th 
revision of ICD (ICD-11) (31), which comes into effect for recording and reporting in January 2022, is 
recommended as the most suitable and future-proof value set for use in the DDCC:VS data dictionary. 
ICD-11 is:
	
→a global public good that is completely free and available for all to use in its entirety; no payment 
will be required to access any additional parts of the code system; 
	
→kept clinically updated through an open, public and transparent maintenance process; 
	
→able to provide comprehensive content coverage and the granularity required for data fields in 
individual-level systems, including the DDCC:VS; 
	
→easy to integrate into software systems via a public API for use in all settings, without additional 
tooling; this is due to ICD-11’s digital and multilingual structure; and
	
→human-readable and machine-readable. 
For countries with legacy ICD systems (e.g. the 10th revision of ICD, ICD-10), WHO will provide ICD-10- 
based value sets for use in the DDCC:VS data dictionary, as well as mappings to other freely available 
classifications and terminologies (e.g. Anatomical Therapeutic Chemical [ATC], SNOMED CT GPS [32], 
etc.). For guiding principles of the WHO Family of International Classifications (WHO-FIC) and other 
classifications, and terminology mapping in the context of the WHO DDCC:VS, see Annex 3.
1	 The DDCC implementation guide can be found here: https://worldhealthorganization.github.io/ddcc/
