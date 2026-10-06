---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-046
section_title: "Page 46"
pages: 46-46
pdf_page: 46
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
29
SECTION 4
Proof of Vaccination scenario
4.2.	 Proof of Vaccination workflows and use cases 
In order to sign a digital document, PKI technology is required. Each Member State would be 
responsible for managing its own PKI through its PHA or another national delegated authority. PKI is 
described in further detail in section 6 and Annex 4. This document assumes that a PKI has already 
been deployed or is available within a country to support the DDCC:VS workflows described in this 
section. This PKI supports the sharing of public keys that correspond to the private keys that have 
been used to cryptographically sign DDCC:VS and may support the sharing of public keys from trusted 
International PHAs so that signed DDCC:VS issued by these parties may be cryptographically verified.
Figure 7
The relationships between digital services for Proof of Vaccination 
Digital 
Health 
Solution
DDCC:VS 
Generation 
Service
DDCC:VS 
Repository
(optional)
DDCC:VS 
Registry 
Service
Status 
Checking 
Application 
(optional)
Submit vaccination 
event
HCID provided by existing National System or 
issued by DDCC:VS Generation Service 
Return 
DDCC:VS
Store DDCC:VS 
(optional)
Online 
status 
check
 (optional)
Register 
DDCC:VS
Online verification DDCC:VS 
(optional)
The digital services for Proof of Vaccination and the relationships between them are shown in Fig. 7.
Note the use of the HCID throughout these services. As the unique identifier included in a DDCC:VS, it can be provided by an existing 
national system, generated at the point of care or issued by DDCC:VS Generation Service (as illustrated in Figure 7). Subsequent vaccinations 
may also be added to the digital record associated to the HCID. HCID can allow verifiers to search for, and retrieve a DDCC:VS for the purposes 
of verification.
