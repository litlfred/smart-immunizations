---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-087
section_title: "Page 87"
pages: 87-87
pdf_page: 87
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
70
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
A digital certificate (or public key certificate) is a file that contains a public key along with extra 
information such as the name of the issuer and the validity dates for using the key. A standard such as 
X509 is used to describe the elements in such a file.
HOW DOES A PKI WORK FOR VACCINATION CERTIFICATES?
For the purposes of the DDCC:VS, the PKI is used to establish data provenance, as per example 2 above, 
which works as follows.
A.	 A certificate authority, such as a public health authority, is nominated within a particular country, 
region or jurisdiction, and that certificate authority becomes the “trust anchor” responsible 
for issuing certificates. Trust begins at this point, and this entity has to be a recognized and 
authorized actor. 
B.	 The certificate authority doesn’t sign vaccination documents and data. The signing of vaccination 
documents and data is handled by other agencies, such as public health actors and other 
stakeholders.
C.	 Therefore, the certificate authority issues private–public key pairs to these other actors in the form 
of document signer certificates (DSCs), providing them with the information needed to digitally 
sign documents.
D.	 These different agencies then use the private key in their DSC to perform this signing activity. 
Signing involves encrypting the information using the private key so it is rendered into a format 
that is not human-readable.
E.	 Any electronic information can be signed in this way. The health certificate identifier (HCID) 
could be signed, a representation of the whole vaccination record could be signed, or some other 
combination of information, as determined by the certificate authority, could be signed. 
F.	 An interested party (i.e. a Verifier) who wants to decrypt the encrypted information for the 
vaccination certificate must have two key things. 
	»
The public key corresponding to the private key in the DSC; and
	»
Trust that the public key, from the DSC, came from a certificate authority that the interested party 
trusts.
G.	 To facilitate the two points in (F), a certificate authority usually sets up an online service for this 
purpose. The Verifier can interrogate the service and: 
	»
Ask for the public key if it does not have it. The Verifier can provide the HCID and check that the 
authority has that HCID in its records and that the HCID is linked to a valid public key. This is the 
role of the DDCC:VS Registry Service in this paper.
	»
Once the Verifier has the public key, it can also check with the authority that the public key is valid 
and has not been revoked.
