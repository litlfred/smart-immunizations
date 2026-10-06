---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-047
section_title: "Page 47"
pages: 47-47
pdf_page: 47
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
30
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Proof of Vaccination scenario
SECTION 4
The verification of a claim of vaccination is illustrated in Fig. 8. The workflow’s actors and settings, 
and its related high-level requirements, may be described as follows.
1.	 A DDCC:VS Holder presents a DDCC:VS to a Verifier in support of a claim of vaccination status.
2.	 To verify the COVID-19 vaccination claim of a verifiable DDCC:VS Holder, there are four separate 
pathways (Manual Verification, Offline Cryptographic Verification, Online Status Check [national 
DDCC:VS] and Online Status Check [international DDCC:VS]) that a Verifier could take to check the 
COVID-19 vaccination claim at Point C, elaborated as Proof of Vaccination use cases in Table 8. A 
Verifier may visually verify a DDCC:VS, or scan a machine-readable version of the DDCC:VS’s HCID 
and use that when accessing a verification service or verify using a digitally signed, machine-
readable representation of the core data set content (e.g. as a 2D barcode). 
Note that, regardless of the use case, a DDCC:VS Generation Service is required. The DDCC:VS Registry 
Service is also required. However, the DDCC:VS Repository Service is optional depending on which 
use case is being implemented, but it is required for the online verification use cases. See Table 7 
for descriptions of the DDCC:VS services noted; the DDCC:VS Registry Service is not equivalent to a 
registry.
4.2.1.	Proof of Vaccination use cases
Navigating through the workflow diagram shown in Fig. 8, there are four possible verification 
pathways (illustrated separately in Fig. 9, Fig. 10, Fig. 11 and Fig. 12), which are the use cases of the 
Proof of Vaccination scenario listed in Table 8.
