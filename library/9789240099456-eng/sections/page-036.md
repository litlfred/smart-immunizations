---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-036
section_title: "Page 36"
pages: 36-36
pdf_page: 36
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
26
personas
indicators
workflows
data
decisions
scenarios
requirements
recommendations
Digital adaptation kit for immunizations
4
Generic business processes 
and workflows
Component
A business process is a set of related activities or tasks performed together to achieve the objectives of the health programme, such as registration, counselling or 
referrals (13,23). Workflows are a visual representation of the progression of activities (tasks, events, interactions) that are performed within the business process 
(23). The workflow provides a “story” for the business process being diagrammed and is used to aid communication and collaboration among users, stakeholders 
and engineers.
This DAK focuses on key business processes that are part of routine immunization programmes and mass immunization campaigns (see Table 8). The significant 
difference between routine immunizations and mass immunization campaigns is in the planning phase (see process B. Plan service delivery). The remaining 
business processes, most importantly process D. Administer vaccine (which drives most of the decision logic of whether to vaccinate or not), are the same 
regardless of whether they are part of the routine immunization programme or a mass immunization campaign. The workflows of the identified processes use 
standard notation for business process mapping. Table 9 provides an overview of this notation. For each process type, the corresponding business processes, data 
elements and decision support needs are detailed in the subsequent sections of this document. 
Table 8. Overview of business processes
# 
Process 
Process ID 
Personas 
Objectives 
Task set 
 
Title 
ID used to reference 
this process 
throughout the DAK
Individuals 
interacting to conduct 
the process 
What the process seeks to achieve 
The general set of activities performed within the process 
A
Vaccination 
location 
registration 
IMMZ.A
System 
administrator
All vaccination locations (including private 
sector facilities, government centres and/
or other entities involved in public health 
efforts) able to administer vaccines must be 
registered and uniquely identified to enable 
appropriate tracking of vaccine coverage 
and stock. In the case of a health-care 
facility with multiple vaccination locations, 
only the facility will be registered.
Starting point: System administrator registers new vaccination location or update 
information about existing vaccination location. 
	» Validate against the National Master Facility List (NMFL)
	» Notify NMFL team of changes/updates
	» Request and submit additional information
	» Create and update vaccination location record
	» Generate unique identifier for vaccination location 
	» Send vaccination location registration notification
