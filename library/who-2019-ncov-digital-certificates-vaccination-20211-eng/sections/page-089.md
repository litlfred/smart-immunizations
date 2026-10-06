---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-089
section_title: "Page 89"
pages: 89-89
pdf_page: 89
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
72
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Annex 5
Non-functional requirements
This section contains a suggested set of generic non-functional requirements (see Table A5.1). Along 
with the functional requirements in sections 3.3 and 4.3, these non-functional requirements can be 
adapted when specifying a digital solution for the scenarios in this paper. Non-functional requirements 
explain the conditions under which any digital solution must remain effective and are organized into 
the following categories.
	
→ACCESSIBILITY: The provision of flexibility to accommodate each user’s needs and preferences, along 
with appropriate measures to ensure access to persons with disabilities on an equal basis with 
others; for example, the solution should still be accessible to those with visual impairment.
	
→AVAILABILITY (SERVICE LEVEL AGREEMENTS; SLAS): The definition of when the system will be 
available to the user community, how such metrics will be measured, and the functionality in the 
tool for managing planned downtime.
	
→CAPACITY – CURRENT AND FORECAST: The number of concurrent users that can interact with the 
system without an unacceptable degradation in performance, speed or responsiveness. User 
populations are never static, and so the ability to handle current typical and peak volumes of usage 
and predicted future states, and the strategy for handling a traffic surge, must be considered.
	
→UPTIME SLAs – DISASTER RECOVERY, BUSINESS CONTINUITY, RESILIENCE: The requirements for the 
system in terms of how it recovers from critical, unexpected failure and the support for business 
continuity. This includes time to recovery, how recovery is established, and at what levels resilience 
and redundancy are built into the system to minimize any data loss.
	
→PERFORMANCE/RESPONSE TIME: The speed with which the system is expected to respond under 
normal and exceptional loads, with a definition of what those terms mean.
	
→PLATFORM COMPATIBILITY: The different operating systems, machines and configuration on which 
the solution is expected to run.
	
→SECURITY AND PRIVACY: The levels of security that the solution must provide in terms of user 
authentication and data protection.
	
→REGULATION AND COMPLIANCE: Any regulatory/legal constraints with which the system must 
comply, such as data protection policies, WHO cloud policies, and information management and 
retention rules of the jurisdiction(s) in which the solution will run.
	
→RELIABILITY: A measure of the reliability of the tool, for example the acceptable mean time between 
failures of the solution (both hardware and software components). 
	
→SCALABILITY (HORIZONTAL, VERTICAL): The ability to, and strategy for, handling an increasing load 
on the solution (in terms of increased number of users it can support, higher volumes of data it 
can handle, quicker performance and response, etc.). A solution can be scaled either horizontally 
(adding more elements to the solution, such as extra load-balanced servers) or vertically (adding 
extra capacity in existing elements, such as upgrading an existing server).
	
→SUPPORTABILITY: The requirements for engineers to detect, diagnose, resolve and monitor any 
issues and faults that arise while the solution is being used. This covers the features/functions that 
will be built into the system to facilitate technical support work.
