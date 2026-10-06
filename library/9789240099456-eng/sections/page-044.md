---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-044
section_title: "Page 44"
pages: 44-44
pdf_page: 44
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
34
personas
indicators
workflows
data
decisions
scenarios
requirements
recommendations
Digital adaptation kit for immunizations
A. VACCINATION LOCATION REGISTRATION BUSINESS PROCESS NOTES AND ANNOTATIONS
1.	
Obtain vaccination location information  
	»
Vaccination location information may be obtained from multiple 
sources (e.g. from a vaccination location list, an NMFL, a service within 
the national HMIS, etc.) and is ideally standardized across the country/
region. Information can be received manually or automatically. In the 
case of temporary clinics, satellite or remote clinics, the vaccination 
location may be an organizing entity such as a public health unit. It is 
important to note that there will be two separate lists, one for the EIR and 
a separate NMFL. Not all facilities provide immunization services, and in 
some cases (such as temporary clinics), they may not be included in the 
NMFL. This will be dictated by local policy.
2.	
Validate against the NMFL
	»
The vaccination location information is validated against the NMFL 
to determine if there is a match (indicating this new registration is a 
duplicate). This step may be automated.
3.	
Does vaccination location information match?   
	»
The system validates whether the new vaccination location exists in the 
NMFL to determine if it is a new vaccination location or a match/update 
to an existing record. 
	»
If the vaccination location exists in the NMFL, system administrator will 
verify that the information is complete. If the new vaccination location 
does not exist in the NMFL, the system administrator will add/update the 
vaccination location in the PCPOSS or flag for correction/validation. This 
step, or portions of this step, may be automated.
4.	
Allowed to add/update vaccination location information?  
	»
In some circumstances, all vaccination location data are owned and 
updated solely by the NMFL and then shared with other systems. It will 
also depend on the type of information. For example, the name of the 
vaccination location may be “owned” by the NMFL, but other data, such 
as the type of fridge, may be managed by the PCPOSS.
5.	
Notify NMFL team of change/update  
	»
The NMFL team will make appropriate changes.
6.	
Update/add new vaccination location
	»
If all required information is complete, a new vaccination location record 
is created in the PCPOSS.
	»
There may be cases where a health-care facility has multiple vaccination 
locations across the region. In this case, only the facility will be 
registered.
7.	
Generate unique location identifier
	»
PCPOSS will generate a unique ID number to assign to the vaccination 
location or entity that is permitted to deliver vaccines. This only applies 
to new facilities.
8.	
Verify information for additional data  
	»
System administrator reviews the vaccination location information to 
determine if any updated information or additional information was 
provided to the PCPOSS that was not available in the NMFL. This step 
may be automated.
9.	
Information complete?  
	»
System administrator reviews completeness of the information required 
to register the vaccination location. This step may be automated.
10.	 Request additional information  
	»
System administrator requests necessary additional information 
needed to register the vaccination location. This may be requested 
from the vaccination location directly or the most appropriate source 
(e.g. a district information officer, a cold chain officer, NMFL staff, etc.) 
depending on the data needed.
