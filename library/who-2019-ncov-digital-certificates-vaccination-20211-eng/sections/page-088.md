---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-088
section_title: "Page 88"
pages: 88-88
pdf_page: 88
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
71
H.	 Finally, now that the Verifier knows that the public key came from a trusted source, the Verifier can 
decrypt whatever information has been provided for the vaccination certificate. If the decryption 
reveals the data, the Verifier can be confident that:
	»
the information could only have been encrypted by someone with the private key, therefore it must 
have come from someone in possession of the DSC;
	»
the information has not been altered or tampered with after it was signed, otherwise the decryption 
would not work; and
	»
the information can be trusted, because the Verifier trusts the certificate authority, and trusts the 
certificate authority to have issued the DSC, which must have been used to encrypt the information.
I.	 If the public key decrypts the encrypted information so that it looks identical to the unencrypted 
version provided, the Verifier can be confident that only the entity in possession of the private key 
sent these data, and that it has not been altered since by any other party. 
	»
For the vaccination certificates, the HCID must resolve back to a digital record that is digitally signed 
in the manner described.
	»
Optionally, the DDCC:VS core data set could also be encoded into a barcode to enable the Verifier to 
perform an offline check, but the Verifier would still need to be able to validate that the public key 
was a valid one.
A PKI is only as secure as the IT infrastructure on which it is implemented; although PKI gives a high 
degree of trust, care must be taken to design and run the system in a manner that maintains security.
