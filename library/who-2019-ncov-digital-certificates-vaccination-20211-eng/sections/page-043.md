---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-043
section_title: "Page 43"
pages: 43-43
pdf_page: 43
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
26
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Continuity of Care scenario
SECTION 3
Requirement ID
Functional requirement
UC001
Paper First
UC002
Offline Digital
UC003 
Online Digital
 DDCC.FXNREQ.024
If an offline Digital Health Solution for vaccination 
registration is available, then it MAY be responsible for 
outputting the vaccination data using the FHIR standard.
 DDCC.FXNREQ.025
If an offline Digital Health Solution for vaccine registration 
is available, and is part of the national PKI trust framework, 
and is authorized by the PHA to sign vaccination content as 
a DDCC:VS, then it SHALL register the DDCC:VS through the 
DDCC:VS Registry Service. 
 DDCC.FXNREQ.026
For each care delivery session, the facility, organization 
and care delivery health worker context of the vaccine 
administration event SHALL be established.
 DDCC.FXNREQ.027
If an online/connected public health DDCC:VS Generation 
Service is available at the time of vaccination, then it SHALL 
be possible to register the vaccination as soon as possible 
after it is administered.
 DDCC.FXNREQ.028
The DDCC:VS Generation Service involved in the vaccination 
SHALL ensure encryption of data, in transit and at rest, to 
provide end-to-end security of personal data.
 DDCC.FXNREQ.029
The DDCC:VS Generation Service MAY be the agent 
responsible for issuing the HCID, provided that the HCID can 
be associated at the time of vaccination in a timely manner. 
If the DDCC:VS Generation Service is responsible for issuing 
HCIDs, it SHALL only issue unique HCIDs, i.e. the same HCID 
should never appear on two different paper vaccination 
cards. 
 DDCC.FXNREQ.030
If pre-generated HCIDs and pre-printed vaccination 
cards are used, the generation of the HCIDs, along with 
any supporting technology to ensure HCIDs will not be 
duplicated within or across care sites, SHALL be managed by 
PHA policy. 
 DDCC.FXNREQ.031
It SHALL be possible for the DDCC:VS Generation Service to 
accept data from an authorized, connected point-of-care 
system, where such a system exists, i.e. to be able to accept 
data transferred from local data stores at sites where 
vaccinations are administered.
 DDCC.FXNREQ.032
It SHALL be possible for the DDCC:VS Generation Service to 
represent vaccination data using the FHIR format.
 DDCC.FXNREQ.033
It SHALL be possible for the DDCC:VS Generation Service to 
perform digital signing of vaccination data.
 DDCC.FXNREQ.034
It MAY be possible for the solution to generate a machine-
readable 2D barcode that, in addition to the HCID, contains 
further useful technical information, such as a web end--
point for validating the HCID, or a public key. 
 DDCC.FXNREQ.035
It MAY be possible for the DDCC:VS Generation Service 
to generate a 2D barcode that includes the unencrypted 
minimum core data set content (in FHIR standard) of the 
vaccination, thus providing a machine-readable version of 
the vaccination certificate.
DDCC.FXNREQ.036
The DDCC:VS Generation Service SHALL maintain a connection 
between an HCID, the vaccination data associated with it in 
a DDCC:VS, any 2D barcode generated from the data, and the 
private/public key used to sign the data.
 1D: one-dimensional; 2D: two-dimensional; DDCC: Digital Documentation of COVID-19 Certificates; DDCC:VS: Digital Documentation of 
COVID-19 Certificates: Vaccination Status; HCID: health certificate identifier; ID: identifier; PHA: public health authority.
1 The use case(s) to which each functional requirement applies are indicated with a 
.
