---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-035
section_title: "Page 35"
pages: 35-35
pdf_page: 35
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
18
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Continuity of Care scenario
SECTION 3
3.2.	 Continuity of Care workflows and use cases
The Continuity of Care scenario is summarized in Fig. 3. The workflow’s actors and settings, and its 
related high-level requirements, may be described as follows.
1.	 A Subject of Care presents at a care site. The identity of the Subject of Care is established as per 
Member State processes and norms. The Subject of Care MAY present an existing DDCC:VS card to 
inform the care delivery process. The Vaccinator MAY retrieve existing health history data about 
the Subject of Care if authorized to do so.
2.	 A Vaccinator administers a COVID-19 vaccination.
3.	 Elements of the DDCC:VS core data set content SHALL be entered onto the DDCC:VS paper card, 
which SHALL have an HCID. The DDCC:VS paper card SHALL be provided to the DDCC:VS Holder at 
Point A. The HCID SHALL be used to establish a globally unique identifier (ID) for the DDCC:VS or to 
reference the ID of a previously established DDCC:VS.
4.	 The care site MAY have a local Digital Health Solution with data entered at the point of care. If so, 
the Vaccinator and/or Data Entry Personnel directly record details of the vaccination event, which 
SHALL be persisted based on the DDCC:VS core data set.
5.	 The care site MAY have a local Digital Health Solution with data entered after the vaccine 
administration event. If so, Data Entry Personnel can record details of the vaccination event, which 
SHALL be persisted according to the DDCC:VS core data set.
If a Digital Health Solution does not exist at the care site, details of the vaccination event SHALL be 
recorded and persisted in a paper record (e.g. immunization registry book), according to the required 
DDCC:VS core data set. Details of the vaccination event can then be electronically recorded into a 
Digital Health Solution available at another site, by Data Entry Personnel. 
Health data captured during the vaccination event SHALL be recorded as coded content using the FHIR 
standard. If the data represent a subsequent vaccination event (e.g. second dose), this content SHALL 
be added as another event to the Subject of Care’s existing FHIR composition. 
Once the DDCC:VS content is digitally recorded and persisted, either by the Vaccinator or Data Entry 
Personnel at the point of care or after the vaccination has been administered, and the DDCC:VS has 
been digitally signed using PKI technology and created by the DDCC Generation Service, the record of 
the vaccination event is available in a digital format, as a DDCC:VS, to the DDCC:VS Holder at Point B.
