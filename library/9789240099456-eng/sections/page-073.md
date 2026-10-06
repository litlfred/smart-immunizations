---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-073
section_title: "Page 73"
pages: 73-73
pdf_page: 73
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
63
Core data elements
personas
indicators
workflows
data
decisions
scenarios
requirements
recommendations
Activity ID. Activity name
Data element ID
Data element name
Description and definition
IMMZ.D21.Generate verifiable digital certificate
IMMZ.D.DE.151
Certificate issuer
The authority or authorized organization that issued the vaccination certificate
IMMZ.D.DE.152
Health Certificate Identifier 
(HCID)
Unique identifier used to associate the immunization event represented in a paper 
vaccination card to its digital representation(s)
IMMZ.D.DE.153
Certificate valid from
Date in which the certificate for an immunization event became valid. No health or 
clinical inferences should be made from this date
IMMZ.D.DE.154
Certificate valid until
Last date in which the certificate for an immunization event is valid. No health or clinical 
inferences should be made from this date
IMMZ.D.DE.155
Certificate schema version
Version of the core data set and HL7 Fast Health Interoperability Resources (FHIR) 
implementation guide that the certificate is using
DE: data element; ID: identification; IMMZ: immunization; N/A: not applicable.
5.2 	 List of calculated data elements
The DAK for immunizations does not have any calculated data elements at this time. Age is not listed as a calculated data element in this DAK as it will be an 
implementation level real-time calculation based on the date of birth and visit date.
5.3 	 Additional considerations for adapting the data dictionary 
Some settings may require the inclusion of additional data elements into the full data set or changes to response options based on contextual differences. 
Additionally, the transition from paper-based forms to digital systems may require some reflection on whether data elements currently on the paper forms should 
be incorporated into the digital system. Furthermore, the following assumptions are made about country’s responsibilities as foundational aspects of implementing 
this DAK: 
	»
It will be up to the country to determine the mechanism for unique ID of the client. It may be based on a national unique ID, biometrics or a system-generated 
unique ID.
	»
It will be up to the country to determine the list of vaccine products available. 
The Annex provides additional guidance for adding data elements to or amending existing data elements in the data dictionary.
