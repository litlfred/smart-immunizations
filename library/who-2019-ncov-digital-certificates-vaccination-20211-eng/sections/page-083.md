---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-083
section_title: "Page 83"
pages: 83-83
pdf_page: 83
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
66
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Key principles for usage validation of maps include:
a.	 Use a “gold standard” (i.e. a statement in the original source data – e.g. a diagnosis as written in 
the medical record) as the reference point. 
b.	 Compare the original source data with the end results of the following two processes.
	»
Coding of original source data with a source terminology – map code(s) of source terminology to 
code(s) of target terminology; and
	»
Coding of original source data with target terminology.
c.	 Use a statistically significant sample size that is representative of the target terminology and its 
prototypical use case settings.
d.	 When performing usage validation of automated maps, always include human (i.e. manual) 
validation.
8.	
Upon publication and release, include information about release mechanisms, release cycle, 
versioning, source/target and licence agreement requirements, and provide a feedback mechanism 
for users. Dissemination of maps should also include documentation as stated above, describing 
the purpose, scope, limitations and methodology used to create the maps.
9.	
Establish an ongoing maintenance mechanism, release cycle, types and drivers of changes, and 
versioning of maps. The maintenance phase should include an outline of the overall life-cycle 
plan for the map, conflict resolution mechanism, continuous improvement process, and decision 
process around when an update is required. Whenever maps are updated, the cycle of QA and 
validation must be repeated.
10.	 When map specialists are conducting mapping manually, it is recommended to provide the 
necessary tools and documentation to drive consistency. Such items include: the tooling 
environment (workflow details and resources related to both source and target schemes); source 
and target browsers, if available; technical specifications (use case, scope, definitions); editorial 
mapping principles or rules to ensure consistency of the maps, particularly where human 
judgement is required; and implementation guidance. Additionally, it is best practice to provide an 
environment that supports dual independent authoring of maps, as this is thought to reduce bias 
among human map specialists. Development of a consensus management process to aid in the 
resolution of discrepancies and complex issues is also beneficial. 
11.	 In computational mapping, it is advisable to include resources to ensure consistency when 
building a map using a computational approach, including a description of the tooling 
environment, when human intervention would occur, documentation (e.g. the rules used in 
computerized algorithms), and implementation guidance. It is also advisable to always compute 
the accuracy and error rate of maps. It is important to manually verify and validate the computer-
generated mapping lists. Such manual checking is necessary in the QA process, as maps that are 
generated automatically often contain errors. Such manually verified maps can also assist in the 
training of the machine-learning model when maps for different sections of terminologies are 
being generated sequentially.
12.	 The level of equivalence between source and target entities – such as equivalent, broader, 
narrower – should be specified.
