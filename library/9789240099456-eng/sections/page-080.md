---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-080
section_title: "Page 80"
pages: 80-80
pdf_page: 80
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
70
personas
indicators
workflows
data
decisions
scenarios
requirements
recommendations
Digital adaptation kit for immunizations
6.2 	 Decision-support tables
Each of the decision logics listed in the overview table (see Table 11) is elaborated in the decision-support implementation tool found here. These decision-support 
tables comprise the components described in Table 12. 
It is important to note that the decision-support logic here is translated directly from the WHO guidelines and guidance documents and has been reviewed by 
the panel of experts who have created those guidelines documents. We do not anticipate the decision-support logic to change much as the logic was created and 
reviewed by clinical experts. However, some level of adaptation may be needed depending on changes to the workflow and/or changes to the data dictionary. 
Any changes to the decision-support logic should be considered carefully, as an embedded decision-support system can greatly affect the quality of care at the 
point of care. As helpful as decision-support logic can be to the health worker, incorrect decision-support logic can also be detrimental. Thus, any new decision-
support logic should be carefully reviewed and agreed upon by in-country clinical experts and tested with a standard set of cases to ensure consistency.
Table 12. Components of the decision-support tables
Decision ID
The name of the “decision” describing which algorithm or logic is represented (e.g. whether a client needs to be vaccinated for mumps). The 
Decision ID should correspond to the number in the overview table on “overview” tab
Business rule
The description of the decision that needs to be made based on IF/THEN statements with the appropriate data element name for the variables. 
The rule should demonstrate the relationship between the input variables and the expected outputs and actions within the decision-support 
logic (e.g. IF client has not been vaccinated against mumps THEN give mumps vaccine)
Trigger
The event that would indicate when this decision-support logic should appear within the workflow, such as the activity that would trigger this 
decision to be made
Inputs
Output
Guidance displayed to 
health worker
Annotations
Reference(s)
These are the variables or 
conditions that need to be 
considered to determine 
the consequent actions or 
outputs.
If there are multiple 
input entries on the 
same row (such as here), 
these different inputs are 
considered as “AND” – 
conditions that need to be 
in place at the same time.
The decision support that the 
system must recommend as action 
to be taken given the criteria are 
met. The software will refer to the 
contents here to make relevant 
automated decision support. Action 
will trigger the system to perform a 
decision-support outcome.
Pop-up alert messages 
for the health worker; it 
should include the written 
content that will appear 
in the pop-up messages 
notifying the health 
worker of the appropriate 
next steps.
This column should be used for any other notes, 
annotations or communication messages 
within the team. This should include any 
additional information that does not fit into 
the other columns. Note that this message 
WILL NOT appear as a pop-up message. While 
noting down the annotations, please note the 
correct audience for the annotation (who is this 
message for?).
A reference to 
this decision 
rule
Inputs placed on different 
rows are considered as 
“OR” conditions that can be 
considered independently of 
the inputs on other rows.
