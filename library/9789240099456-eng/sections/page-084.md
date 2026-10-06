---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-084
section_title: "Page 84"
pages: 84-84
pdf_page: 84
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
74
personas
indicators
workflows
data
decisions
scenarios
requirements
recommendations
Digital adaptation kit for immunizations
6.3 	 Scheduling-logic overview
In addition to specific decision-support logic that needs to be detailed, there is also scheduling logic to facilitate the digital tracking of clients and ensure that 
appropriate services are provided in a timely manner according to clinical protocols. For example, it will be important for the health worker to know when the 
client’s next polio vaccination is due based on the recommended vaccination schedule for polio as per WHO recommendations. In the case of immunization, 
decision-support logic is derived from scheduling logic. Table 11 provides an overview of the different scheduling-logic tables included in this DAK. The details 
within each scheduling logic are elaborated here. Table 15 provides an example scheduling-logic table for measles vaccination.
Table 15. Example scheduling-logic table for measles vaccination schedule in countries with ongoing transmission in which the risk of measles mortality remains 
high
Schedule 
ID
IMMZ.D18.S.Measles.Ongoing transmission schedule
IMMZ.D Administer vaccine
Service 
name 
Service 
description 
Trigger 
event
Trigger 
date
Create 
condition
Due date
Overdue 
Expiration 
Completion
Comments Reference(s)
The name of 
the service 
for which 
the schedule 
is relevant
Description 
of the 
service (to 
provide 
clarity)
What event 
signals the 
start of 
the service 
schedule?
What is the 
date of the 
signalling 
event that 
will be 
used to 
determine 
a service’s 
due date?
Are there 
any 
conditions 
that specify 
when a 
service 
should be 
given?
How is the 
due date of 
the service 
calculated?
When does the service 
become overdue?
When does the service 
expire?
How does the health 
worker complete the 
service?
 
 
Schedule for countries with ongoing transmission in which the risk of measles mortality remains high
MCV dose 1 
(MCV1)
Provision of 
MCV1 from 
the primary 
series
Child’s birth
“Date of 
birth”
The client 
is due for 
MCV1 if the 
client is 
at least 9 
months of 
age.
“Date of 
birth” + 9 
months
To be determined 
by Member States; 
however, there is no 
recommended overdue 
date and individuals 
are always eligible to be 
vaccinated.
To be determined 
by Member States; 
however, there is 
no recommended 
expiration date 
and individuals are 
always eligible to be 
vaccinated.
MCV1 was 
administered
Count of vaccines 
administered (where 
“Vaccine type” = 
“Measles-containing 
vaccines” and “Type 
of dose” = “Primary 
series”) = 1
–
WHO recommendations 
for routine 
immunization 
– summary 
tables (March 
2023) (28)
