---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-090
section_title: "Page 90"
pages: 90-90
pdf_page: 90
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Page
73
	
→USABILITY BY TARGET USER COMMUNITY: The extent to which a product can be used by specified 
users to achieve specified goals with effectiveness, efficiency and satisfaction in a specified context 
of use. This includes optimization of the interface for clarity and efficiency, and ensuring that the 
solution is appropriate to the needs and the experience level and expectations of the target users.
	
→DATA RETENTION/ARCHIVING: Requirements relating to how information will be archived from its 
normal location and then retained, including the frequency, the approval process and any process 
for restoring information from the archive.
Table A5.1 
Non-functional requirements for the DDCC:VS 
Requirement ID
Category
Non-functional requirement
DDCC.NFXNREQ.001
Accessibility
Any solution SHALL provide optimization for delivery to users with low bandwidth, as 
in a low digital maturity setting users will often have limited (or intermittent) Internet 
connectivity.
DDCC.NFXNREQ.002
Accessibility
Any solution SHOULD provide offline availability that permits a user to continue to 
work with data while offline, such as by creating a set of requests to be sent when 
next online.
DDCC.NFXNREQ.003
Accessibility
Any solution SHALL provide a mechanism for the resynchronization/dispatch of data 
created offline when the solution is reconnected.
DDCC.NFXNREQ.004
Accessibility
Any solution SHOULD follow best practice to deliver interfaces that are clear, intuitive 
and consistent (standardized colour schemes, icons, placement of visual elements – 
titles, buttons, filters, navigation, etc.)
DDCC.NFXNREQ.005
Accessibility
Any solution SHOULD follow best practice to deliver interfaces that are accessible by 
the widest range of users, including considerations for different cultures (e.g. left-to-
right and right-to-left scripts), visual impairment (e.g. colour blindness) and physical 
disability (e.g. the need to interact using one hand).
DDCC.NFXNREQ.006
Accessibility
Any solution SHOULD automatically optimize its interface (layout of elements, 
organization of information, etc.) to adapt to the device on which it is being used, 
so that it is accessible on personal computers (desktops, laptops), tablets and 
smartphones using principles of adaptive design.
DDCC.NFXNREQ.007
Availability
Any solution developed SHOULD NOT be able to accept more than 10 minutes of 
outage during normal usage and cannot accept more than 1 minute of data loss of 
queries and responses.
DDCC.NFXNREQ.008
Availability
It MAY be possible to provide an indication of the availability status of any solution so 
that users can check the system’s “health”. The same functionality MAY also notify of 
any planned downtime, retired functionality, release notes, etc.
DDCC.NFXNREQ.009
Capacity – current and 
forecast
The system SHALL be able to support the potentially large number of concurrent users 
performing read and write operations during normal operation. This metric will vary 
significantly between different country contexts and will depend on the design, but 
should be used as the anticipated capacity standard.
DDCC.NFXNREQ.010
Capacity, current and 
forecast
During periods of peak usage, system traffic MAY surge the number of concurrent 
users performing read and write operations.
DDCC.NFXNREQ.011
Capacity, current and 
forecast
Forecast growth of the user base is anticipated to be high. As a safety contingency, 
the system SHOULD support, or have scaling plans to support, growth of 25% per year.
DDCC.NFXNREQ.012
Disaster recovery, 
business continuity, 
resilience
All data and derived analysis SHALL be stored within an appropriate data architecture 
to ensure redundancy and rapid disaster recovery, to eliminate the risk of data loss.
DDCC.NFXNREQ.013
Disaster recovery, 
business continuity, 
resilience
The system SHOULD provide near-instantaneous switch-over if any one component 
of the system architecture fails critically (database server, web server, system 
monitoring job, service bus, etc.).
