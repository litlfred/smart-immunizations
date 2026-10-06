---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-068
section_title: "Page 68"
pages: 68-68
pdf_page: 68
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
51
SECTION 7
National governance considerations
SECTION
National 
governance 
considerations 
7 
Governance in the health sector is “a wide range of steering and 
rule-making related functions carried out by governments/decisions 
makers as they seek to achieve national health policy objectives that 
are conducive to universal health coverage” (33). A national framework 
to govern the complex and dynamic health policy for implementing 
DDCC:VS should be tailored to meet the Member State’s needs, which 
vary. This section provides an overview of some key governance 
considerations for Member States implementing DDCC:VS solutions. 
However, it will be the responsibility of the Member State to determine 
the most appropriate governance mechanisms for its context. 
Fundamentally, trust in the system should derive from the security-by-design of a PKI and the 
governance rules put in place by the Member State to operate it. The Proof of Vaccination scenario of 
use requires governance to be established at two levels: 1. the PHA; and 2. the Member State. At PHA 
level, at least one DSC needs to be utilized to sign the DDCC:VS. At Member State level, an authorized 
DSC-sharing mechanism needs to be established to indicate which DSCs are currently permitted to 
sign the DDCC:VS. There are two recommended approaches.
1.	 ROOT CERTIFICATE AUTHORITY: The Member State establishes a root certificate authority, which 
holds a root certificate for the DDCC:VS. The private key of the Root Certificate managed by the 
Member State may be used by the Member State to sign a PHA’s DSC that has been authorized for 
use. The public key of the root certificate can be used to validate that the DSC is authorized. Note 
that the term “root” does not imply hierarchy or that the root certificate authority is at the top of 
that hierarchy. Rather, it is used to denote that a root certificate authority may be trusted directly 
(34). 
2.	 MASTER LIST: The Member State establishes a mechanism to manage and distribute, as appropriate, 
a master list of DSCs that have been authorized for PHAs to use to sign the DDCC:VS.
Member States can leverage an existing PKI or create a new one specifically for DDCC:VS. Regardless, 
depending on how a Member State’s health systems are organized, there are several PKI options that the 
national-level ministry of health could consider, depending on the governance context in the Member State.
