---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-085
section_title: "Page 85"
pages: 85-85
pdf_page: 85
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
68
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Annex 4
What is public key infrastructure (PKI)? 
The solution discussed in this document involves applying digital signatures to information to provide 
a guarantee that the information has been validated by an accredited authority. The proposed method 
is to employ a digital certificate using a private–public key pair, a common mathematical approach 
for encryption and digital trust. The processes, systems, software and rules around the management 
of these certificates form a PKI – essentially, all the components that need to be in place for a trusted 
solution to work.
WHY IS A PKI NEEDED?
Various individuals and organizations, when presented with a vaccination certificate, will need to be 
able to verify that the certificate has come from an approved authority, and that what the document 
purports to be is indeed true. 
For paper-based records, verification has been achieved historically by means of signatures and 
unique seals (e.g. stamps, holographic images, special paper), but these can be copied or forged. The 
electronic equivalent, making use of technology, is a digital certificate. At its simplest, the electronic 
equivalent can be a pair of keys: a private key and a public key. Either key can be used to digitally 
encrypt information in such a way that it can only be decrypted by its twin key. The private key is kept 
secret and protected, as the name suggests, but the public key is widely disseminated.
WHAT IS A PKI?
A system is needed to distribute public keys and to reassure the recipient that the public key has come 
from an accredited source (i.e. the certificate authority). This is one job of a PKI, which is a mechanism 
for disseminating the public keys and for following up with any revocation notices if a public key is 
found to be compromised. Revocation may happen, for example, if the private key is obtained by an 
unintended party.
In essence, the PKI binds a certificate to the identity of a particular individual or organization, so 
that a recipient can trust that the public key provided does reliably resolve back to the individual or 
organization in question.
HOW IS A PKI USED?
This property of the pair of keys for encryption or decryption (based on a one-way mathematical 
operation involving the factorization of large numbers) has many useful applications. Examples are:
Example 1:	
If I want to send a confidential message to a friend, then I can encrypt the message with 
his or her public key and send it out confident that only the person with the private key 
(my friend) will be able to read it.
Example 2:	
Likewise, if I want to send a message to the same friend and give him or her confidence 
that it could only have come from me, I can encrypt it with my private key, and my 
friend can then decrypt it with my public key, knowing that only someone with the 
private key (i.e. me) could have written it.
