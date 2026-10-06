---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-081
section_title: "Page 81"
pages: 81-81
pdf_page: 81
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
71
Decision-support logic
personas
indicators
workflows
data
decisions
scenarios
requirements
recommendations
Table 13 is an example of a decision-support table for determining if a client is due for measles vaccination in countries with ongoing transmission in which the risk 
of measles mortality remains high. Table 14 is an example of a contraindications table for measles, illustrating potential contraindications for measles vaccination. 
Table 13. Example decision-support table for measles vaccination in countries with ongoing transmission in which the risk of measles mortality remains high
Decision ID
IMMZ.D2.DT.Measles.Ongoing transmission
Business rule
Determine if the client is due for a measles vaccination according to the national immunization schedule
Trigger
IMMZ.D2 Determine required vaccination(s) if any
Inputs
Output
Guidance displayed to health 
worker
Annotations
Reference(s)
Countries with ongoing transmission in which the risk of measles mortality remains high (countries that provide first dose of measles-containing vaccine (MCV) at 9 months 
and second dose of MCV at 15 months)
Number of MCV 
primary series doses 
administered
Count of vaccines 
administered (where 
“Vaccine type” = 
“Measles-containing 
vaccines” and “Type 
of dose” = “Primary 
series”)
Client’s age
Today’s date − 
“Date of birth”
Time passed since a live 
vaccine was administered
Today’s date − latest “Date and 
time of vaccination” (where 
“Live vaccine” = TRUE)
–
Client’s age 
is less than 9 
months
Today’s date − 
“Date of birth” < 9 
months
–
Client is not due for 
first dose of measles-
containing vaccine 
(MCV1)
“Immunization 
recommendation status” 
= “Not due”
Should not vaccinate client as 
client’s age is less than 9 months. 
Check for any vaccines due and 
inform the caregiver of when to 
come back for MCV1.
In countries with ongoing 
transmission in which the risk of 
measles mortality remains high, 
MCV1 should be given at 9 months 
of age.
As a general rule, live vaccines 
should be given either 
simultaneously or at intervals of 
4 weeks. An exception to this rule 
is oral polio vaccine (OPV), which 
can be given at any time before or 
after measles vaccination without 
interference in the response to 
either vaccine.
WHO recommendations 
for routine 
immunization 
– summary 
tables (March 
2023) (28)
No measles primary 
series doses were 
administered
Count of vaccines 
administered (where 
“Vaccine type” = 
“Measles-containing 
vaccines” and “Type 
of dose” = “Primary 
series”) = 0
Client’s age 
is more than 
or equal to 9 
months
Today’s date − 
“Date of birth” ≥ 9 
months
No live vaccine was 
administered in the last 4 
weeks
Today’s date − latest “Date and 
time of vaccination” (where 
“Live vaccine” = TRUE) ≥ 4 
weeks
Client is due for MCV1
“Immunization 
recommendation status” 
= “Due”
Should vaccinate client with 
MCV1 as no measles doses were 
administered, client is within 
appropriate age range and no live 
vaccine administered in the past 4 
weeks. 
Check for contraindications.
Live vaccine was administered 
in the last 4 weeks
Today’s date − latest “Date and 
time of vaccination” (where 
“Live vaccine” = TRUE) < 4 
weeks
Client is not due for 
MCV1
“Immunization 
recommendation status” 
= “Not due”
Should not vaccinate client 
with MCV1 as live vaccine was 
administered in the past 4 weeks. 
Check for any vaccines due and 
inform the caregiver of when to 
come back for MCV1.
