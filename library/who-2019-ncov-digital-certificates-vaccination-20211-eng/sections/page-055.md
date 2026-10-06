---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-055
section_title: "Page 55"
pages: 55-55
pdf_page: 55
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
38
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Proof of Vaccination scenario
SECTION 4
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
 DDCC.FXNREQ.041
If a paper vaccination card or electronic 
vaccination document bears a QR code and that 
2D barcode includes a digital signature, then 
it MAY be possible for the Verifier to check the 
signature, using information downloaded from a 
DDCC:VS Registry Service, to ensure it is genuine.
 DDCC.FXNREQ.042
It MAY be possible to log all offline verification 
operations so that, at a later stage, when an online 
connection is available, verification decisions 
can be reviewed and reconfirmed against data 
provided by the online DDCC:VS Registry Service. 
For example, this may be done to confirm that a 
certificate checked offline in the morning using 
public key and revocation data downloaded from 
the DDCC:VS Registry Service the day before has 
not been added to a public key revocation list 
issued that same day.
 DDCC.FXNREQ.043
It SHALL always be possible to perform some form of 
offline verification of vaccination cards; any solution 
should be designed so that a loss of connectivity to 
online components of the solution cannot force the 
verification work to stop.
 DDCC.FXNREQ.044
If, at the time of verification, a Verifier has online 
access/connectivity to a DDCC:VS Registry Service 
managed by a National PHA, then it SHALL be 
possible to query whether the HCID present in the 
barcode (and the public key, if also present) of the 
paper vaccination card are currently valid.
 DDCC.FXNREQ.045
When making the verification check, any solution 
SHALL send only the minimum information 
required for the verification to complete. The 
minimum information comprises the metadata 
(see section 5.2) and signature of the DDCC:VS.
 DDCC.FXNREQ.046
When receiving a request for validation, a 
National PHA SHALL consult its DDCC:VS Registry 
Service and respond with a status to indicate that 
the signing key has not been revoked, that the key 
was issued by a certified authority, and that the 
DDCC has not otherwise been revoked.
 DDCC.FXNREQ.047
A PHA servicing a validation request MAY respond 
with basic details of the vaccination card holder 
(name, date of birth, sex, etc.), in accordance with 
PHA policies, so the Verifier can confirm that the 
vaccination card corresponds to the DDCC:VS 
Holder who has presented himself or herself for 
validation.
 DDCC.FXNREQ.048
A PHA SHALL maintain a PKI to underpin the signing 
and verification process. Lists of valid public keys 
and revocation lists will be held in such a system 
and be linked to the DDCC:VS Generation Service to 
associate public keys with HCIDs.
 DDCC.FXNREQ.049
A PHA MAY log the requests it receives for 
verification (even if rendered anonymous), so 
that it has a searchable history for the purposes 
of audit and fighting fraud, provided that such 
logging respects data protection principles.
