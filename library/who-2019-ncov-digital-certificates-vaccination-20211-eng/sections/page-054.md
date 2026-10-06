---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-054
section_title: "Page 54"
pages: 54-54
pdf_page: 54
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
37
SECTION 4
Proof of Vaccination scenario
4.2.2.	Operationalizing the Proof of Vaccination use cases
Similar to supporting operationalization of the Continuity of Care use cases, the FHIR implementation 
guide includes implementable specifications for the Proof of Vaccination use cases described in this 
document, (available at https://WorldHealthOrganization.github.io/ddcc). The FHIR implementation 
guide for DDCC:VS contains a standards-compliant specification that explicitly encodes computer-
interoperable logic, including data models, terminologies and logic expressions, in a computable 
language sufficient for implementation of Proof of Vaccination use cases.
4.3.	 Functional requirements for Proof of Vaccination 
scenario
High-level functional requirements for the activities described in Fig. 8 are presented in Table 9 as 
suggested features that any digital solutions that would facilitate DDCC:VS verification may have. 
These are written as guidance requirements only to be used as a starting point for Member States 
or other interested parties that need to develop their own specifications for a digital solution for 
DDCC:VS to take and adapt. 
Given non-functional requirements are common to both scenarios (Continuity of Care and Proof of 
Vaccination) (see Annex 5).
Table 9
Functional requirements for the Proof of Vaccination scenario1
Requirement ID
Functional requirement
UC004 
Manual
UC005 
Offline
UC006 
National
UC007 
International 
 DDCC.FXNREQ.037
Paper cards and the validation markings they bear 
SHOULD be designed to combat fraud and misuse. 
Any process that generates a paper vaccination 
card SHALL include elements on the card that 
support the Verifier in visually checking that the 
card is genuine (e.g. water marks, holographic 
seals etc.) without the use of any digital 
technology. 
 DDCC.FXNREQ.038
Paper vaccination cards SHALL display an HCID.
 DDCC.FXNREQ.039
Where paper cards are used, an authority SHALL 
put in place a process for the replacement of lost 
or damaged cards with the necessary supporting 
technology.
 DDCC.FXNREQ.040
If a paper vaccination card or electronic 
vaccination document bearing a 1D or 2D barcode 
is presented to a Verifier, then it SHALL be 
possible for the Verifier to scan the code and, as a 
minimum, read the HCID encoded in the barcode, 
to visually compare it with the HCID written on 
the paper card, if present.
