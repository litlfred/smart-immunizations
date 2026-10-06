---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-064
section_title: "Page 64"
pages: 64-64
pdf_page: 64
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
47
SECTION 6
PKI for signing and verifying a DDCC:VS
Member States will need to establish or utilize a domestic PKI that can be leveraged to issue and to 
verify DDCC:VS. An existing PKI framework may be used, provided it meets the requirements outlined 
in this document. This document assumes that a PKI has already been deployed or is available within 
a country to support the DDCC:VS workflows described in sections 3 and 4. The PKI can be maintained 
and managed by another government entity (e.g. ministry of ICT, ministry of interior, ministry of 
foreign affairs) or by a contractor that the PHA has selected. Regardless, PHAs will have the signing 
authority. The two key steps for establishing a PKI framework are: 
1.	 The PHA will need to generate at least one document signer certificate (DSC) – a private–public 
key pair that can be used by the trusted agents of the PHA to sign the DDCC:VS. 
2.	 The Member State will need to establish a mechanism to assert that a DSC from a PHA has been 
authorized to sign health documents. Two approaches are outlined in section 7.
There are many ways in which a PKI can be implemented. An example implementation of digital 
signing is provided in the implementation guide available at: https://WorldHealthOrganization.github.
io/ddcc. The precise algorithms used for the implementation – for example, for hashing and for 
signature generation – are at the discretion of the Member State.
Figure 13
The chain of trust
CSCA
country signing 
certificate authority
DSC
document signer 
certificate
DDCC
Digital 
Documentation 
of COVID-19 
Certificate
public
private
public
private
Signing and Issuing a DDCC
Verifying a DDCC
1
3
3
1
2
2
