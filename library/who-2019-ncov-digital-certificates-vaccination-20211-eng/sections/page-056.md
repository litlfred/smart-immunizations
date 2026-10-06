---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-056
section_title: "Page 56"
pages: 56-56
pdf_page: 56
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
39
SECTION 4
Proof of Vaccination scenario
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
 DDCC.FXNREQ.051
A PHA SHALL be able to return a verification 
status, as defined by the implementer, to a 
requester, based on the information provided.
 DDCC.FXNREQ.052
A PHA MAY be able to service individual 
verification requests (i.e. details relating to 
one vaccination certificate) or requests sent in 
bulk (details of multiple certificates sent in one 
request).
 DDCC.FXNREQ.053
A PHA SHOULD be able to validate that the 
requestor making a verification request is an 
authorized agent, but MAY also allow anonymous 
verification requests.
 DDCC.FXNREQ.054
The certificate authority (or authorities) in each 
country SHALL maintain records of the DSCs 
issued for the purpose of signing vaccination 
certificates and expose any service(s) that allow a 
public key to be looked up and checked against its 
records to check for validity.
 DDCC.FXNREQ.055
Any communication between a Verifier and a 
DDCC:VS Registry Service or other data service 
managed by a PHA SHALL be secured to prevent 
interference with the data in transit and at rest.
 DDCC.FXNREQ.056
SMS-based verification of alphanumeric HCIDs 
MAY be provided by a PHA as a means of sending a 
verification request or receiving a response with a 
status code.
 DDCC.FXNREQ.057
If a verification request is made in country A 
for a certificate that was issued by country B 
or a supranational entity, then country A’s PHA 
SHOULD have a means of transferring the request/
querying the data held by that authority.
 DDCC.FXNREQ.058
A Member State SHOULD put in place bilateral or 
multilateral agreements with other countries or 
with a supranational entity or regional body for 
access to those entities’ vaccination certificate 
data and digital signatures.
 DDCC.FXNREQ.059
Communications between one country’s and 
another’s PHA or a supranational DDCC:VS Registry 
Service SHALL be secure and prevent interference 
with the data in transit and at rest.
 DDCC.FXNREQ.060
It SHALL be the ultimate responsibility of the 
country where verification is taking place to 
decide whether a vaccination claim is valid or not.
 DDCC.FXNREQ.061
There SHOULD be a mechanism for country A 
to notify country B if a suspected fraudulent 
certificate from country B’s jurisdiction comes to 
the attention of country A.
1D: one-dimensional; 2D: two-dimensional; DDCC: Digital Documentation of COVID-19 Certificates; DDCC:VS: Digital Documentation of 
COVID-19 Certificates: Vaccination Status; DSC: document signer certificate; HCID: health certificate identifier; ID: identifier; PHA: public 
health authority.
1	 The use case(s) to which each functional requirement applies are indicated with a 
.
