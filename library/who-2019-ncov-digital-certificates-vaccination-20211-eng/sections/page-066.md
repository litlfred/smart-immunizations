---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-066
section_title: "Page 66"
pages: 66-66
pdf_page: 66
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
49
SECTION 6
PKI for signing and verifying a DDCC:VS
6.2.	 Verifying a DDCC:VS signature
The verification process, shown in in the bottom row of Fig. 13 and further detailed in Fig. 15, reverses 
the signing process to verify content in the signed DDCC:VS.
1.	 A Verifier calculates its own hash (i.e. “calculated hash”) from the information in the DDCC:VS 
using the same hashing algorithm as was used by the document signer. 
2.	 The DDCC:VS’s signed hash is read by a digital solution.
3.	 The document signer’s public key is used to cryptographically transform the signed hash back to 
the document hash. The Verifier can compare the document hash from step 2 to its own calculated 
hash from step 1. If they match, the Verifier is confident that: 
a.	 only someone with access to the DSC’s private key could have signed the document, because the 
public key was able to decrypt the document hash; and
b.	 the data that was signed is the same as the data read from the DDCC:VS, because the calculated 
hash matches the document hash.
4.	 The PHA’s root certificate public key is used to cryptographically verify that the document signer’s 
signature was issued under the responsibility of the PHA. 
Figure 15
How digital signature verification works
public 
key
Matching hash indicates 
valid document
the document contains the 
information that was signed 
with the private key.
Signed 
hash
Document
with digitally 
signed hash 
(the DDCC:VS)
Calculate hash 
from document
Verifier
01100010110
01100010110
01100010110
01100010110
Document Signing
Document Validation
Signer sends digitally signed document and public key to verifier
Document
(vaccination 
data)
Document
hash
Signed 
hash
Document
with digitally 
signed hash 
(the DDCC:VS)
private 
key
Calculate 
hash from 
document
Signer
Add to 
document
01100010110
Digitally 
sign 
hash
01100010110
01100010110
