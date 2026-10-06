---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-097
section_title: "Page 97"
pages: 97-97
pdf_page: 97
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
annexes
87
Annex
Data type
The data types (2) are:
	» Boolean (i.e. true/false, yes/no) 
	» String (i.e. a sequence of Unicode characters – e.g. name) 
	» Date (e.g. date of birth) – used when only the date is recorded 
	» Time (e.g. time of delivery) – used when only the time is recorded 
	» DateTime (e.g. appointment) – used when the date and time are recorded 
	» ID (e.g. unique identifier assigned to the health service user) 
	» Quantity – a number that is associated with a unit of measure outlined in the standard for Unified Code for Units of Measure; quantities include any number that is associated 
with a unit, such as “number of past pregnancies”, where “past pregnancies” is the unit of measure (3) (if the data type is a quantity, there should be an associated subtype listed 
in the quantity subtype column) 
	» Signature (e.g. supervisor’s approval) – an electronic representation of a signature that is either cryptographic or a graphical image that represents a signature or a signature 
process 
	» Attachment (e.g. image) – additional data content defined in other formats 
	» Coding (e.g. symptoms, reason for coming to the facility, danger signs) – multiple-choice data elements for which the input options are codes 
	» Codes (e.g. pregnant, HIV positive, combined pill) – data elements that are input options to multiple-choice data elements, which are none of the above data types.  
Input options
Input options are used for multiple-choice fields only. Write the list of responses from which the health worker may select. Each of these options should be labelled with a Data 
type as indicated above. For other fields, leave this column blank.
Calculation
If a calculation is needed to define the data element, write the formula here. Leave this column blank if no calculation is needed. Write the formula using standard mathematical 
symbols and the data element label included in the formula (e.g. for the body mass index calculation, “weight in kilograms/(height in meters)2”). 
Quantity 
subtype
Quantity data types can include any number that is associated with a unit of measure. However, there are many subtypes of Quantity that should be listed here:
	» Integer quantity – a whole number (e.g. number of past pregnancies, pulse, systolic blood pressure, diastolic blood pressure)
	» Decimal quantity – rational numbers that have a decimal representation (e.g. exact weight in kilograms, exact height in centimetres, location coordinates, percentages, 
temperature) 
	» Duration – duration of time associated with time units (e.g. number of minutes, number of hours, number of days).
Required
Note whether this field is:
	» Required (R)
	» Optional (O)
	» Conditional on answers from other data fields (C).
Reason for 
requiring data
If this field is required (R), state the reason here:
	» Accountability for national-level reporting
	» Service delivery or clinical decision-making 
	» Client ID.
The digital system should not only replace paper registers, but also streamline processes; thus, it is important to understand why a certain data field is actually required and seek 
opportunities to optimize data flows. Given the high volume of data collection required of health service providers, it might be better to remove a data entry field if it serves no real 
purpose for the clinician, public health reporting or any other identified purpose.
