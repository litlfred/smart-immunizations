---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-041
section_title: "Page 41"
pages: 41-41
pdf_page: 41
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
24
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Continuity of Care scenario
SECTION 3
3.2.2.	Operationalizing the Continuity of Care use cases
In order to operationalize the Continuity of Care use cases, as the specification is intended to 
be implementable, an HL7 FHIR implementation guide has been created (available at:
https://WorldHealthOrganization.github.io/ddcc). HL7 FHIR is a free and open data exchange 
standard that can be used to establish interoperability across systems. The implementation guide 
is to ensure that data for the DDCC:VS is captured in a consistent and interoperable way. The HL7 
FHIR implementation guide for DDCC:VS contains a standards-compliant specification that explicitly 
encodes computer-interoperable logic, including data models, terminologies and logic expressions, in a 
computable language sufficient for implementation of the Continuity of Care use cases. 
3.3.	 Functional requirements for Continuity of Care 
scenario
High-level functional requirements for the elements described in Fig. 3 are presented in Table 5 as 
suggested features that any digital solutions that would facilitate DDCC:VS issue or usage may have. 
These are written as guidance requirements only, to be used as a starting point for Member States or 
other interested parties who need to develop their own specifications for a DDCC:VS to take and adapt.
Non-functional requirements are applicable to both scenarios of use (Continuity of Care and Proof of 
Vaccination) and are included in Annex 5.
Table 5
Functional requirements for the Continuity of Care scenario1 
Requirement ID
Functional requirement
UC001
Paper First
UC002
Offline Digital
UC003 
Online Digital
 DDCC.FXNREQ.001
It SHALL be possible for the Vaccinator to identify the 
Subject of Care as per the norms and policies of the PHA 
under whose authority the vaccination is administered.
 DDCC.FXNREQ.002
It SHOULD be possible to verify the identity of the Subject 
of Care against existing records, if such a check is mandated 
by local procedures, and to retrieve any pertinent health 
history.
 DDCC.FXNREQ.003
It SHALL be possible to register a new Subject of Care if the 
person is presenting for the first time.
 DDCC.FXNREQ.004
It SHALL be possible to issue a new paper card to the 
Subject of Care for the purpose of recording the vaccination.
 DDCC.FXNREQ.005
It SHALL be possible to update an existing paper card held 
by the Subject of Care if the card is presented during the 
vaccination and there is space available on the card.
 DDCC.FXNREQ.006
Where paper cards are used, a PHA SHALL put in place a 
process to replace lost or damaged cards with the necessary 
supporting technology.
 DDCC.FXNREQ.007
It SHALL be possible to associate a globally unique HCID 
with a paper vaccination card recording each vaccination 
administered to the Subject of Care.
