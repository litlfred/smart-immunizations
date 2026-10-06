---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-049
section_title: "Page 49"
pages: 49-49
pdf_page: 49
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
32
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Proof of Vaccination scenario
SECTION 4
Table 8
Proof of Vaccination use cases
Use case ID
UC004
UC005
UC006
UC007 
Use case name
Manual Verification
Offline Cryptographic 
Verification
Online Status Check 
(National DDCC:VS)
Online Status Check (International 
DDCC:VS)
Figure
Figure 9
Figure 10
Figure 11
Figure 12
Use case 
description
A Verifier verifies 
a DDCC:VS using 
purely visual means, 
based on his or 
her subjective 
judgement, as is 
currently done 
with International 
Certificate of 
Vaccination or 
Prophylaxis. This 
type of check is 
currently well 
accepted, is quick 
and easy to do, and 
requires no digital 
technology.
A Verifier verifies 
a DDCC:VS using 
digital cryptographic 
processes in an offline 
mode.
This pathway is used 
when the DDCC:VS is 
being verified in the same 
jurisdiction as it was 
issued. A Verifier verifies 
a DDCC:VS using digital 
cryptographic processes 
in an online mode that 
includes a status check 
against the PHA’s DDCC:VS 
Registry Service and, 
optionally, the DDCC:VS 
Repository.
This pathway is used when the 
DDCC:VS is being verified in a 
foreign jurisdiction to where it 
was issued. A Verifier verifies an 
internationally issued DDCC:VS 
using digital cryptographic 
processes in an online mode that 
includes a status check against the 
National PHA’s DDCC:VS Registry 
Service, which in turn accesses 
an International PHA’s DDCC:VS 
Registry and DDCC:VS Repository, if 
such services exist and such access 
is authorized by the issuing PHA. 
It is assumed in this workflow that 
a Verifier does not directly access 
an International PHA’s DDCC:VS 
Registry or Repository Service. 
Connectivity 
required
Offline
Offline
Online
Online
Level of 
verification
	
→Verification 
is visually 
performed by 
the Verifier. As 
judgement can 
be subjective, it 
relies on policies 
to protect against 
discrimination.
	
→Can confirm that the 
HCID barcode on the 
paper card is valid 
and has not been 
altered. 
	
→Can confirm whether 
the DDCC:VS has 
been issued by an 
authorized PHA. 
	
→Can confirm that 
the hash of any 
signed 2D barcodes 
matches the health 
content represented 
therein.
	
→Can confirm that the 
HCID barcode on the 
paper card is valid and 
has not been altered.
	
→Can confirm whether the 
DDCC:VS has been issued 
by an authorized PHA. 
	
→If authorized to do so, 
can confirm that the 
content on a DDCC:VS 
paper card matches the 
DDCC:VS digital content.
	
→Can confirm that the 
hash of any signed 
2D barcodes matches 
the health content 
represented therein.
	
→Can check whether 
signed 2D barcodes 
containing DDCC:VS 
content have been 
revoked or updated.
	
→Can confirm that the HCID 
barcode on the paper card is valid 
and has not been altered. 
	
→Can confirm whether the DDCC:VS 
has been issued by an authorized 
International PHA. 
	
→If authorized to do so, can confirm 
that the content on a DDCC:VS 
paper card matches the DDCC:VS 
digital content.
	
→Can confirm that the hash of 
any signed 2D barcodes matches 
the health content represented 
therein.
	
→Can check whether signed 2D 
barcodes containing DDCC:VS 
content have been revoked or 
updated.
Verify whether 
the DDCC:VS 
has been 
revoked?
Not possible
Possible if a cache of 
revoked certificates 
is maintained by the 
Verifier
Possible
Possible 
DDCC:VS 
Registry 
Service
Not required
Required
Required
Required
DDCC:VS 
Repository
Optional
Optional
Required
Required
DDCC:VS: Digital Documentation of COVID-19 Certificates: Vaccination Status; HCID: health certificate identifier; ID: identifier; PHA: public 
health authority.
