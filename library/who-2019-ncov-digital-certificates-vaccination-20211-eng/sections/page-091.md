---
doc_id: who-2019-ncov-digital-certificates-vaccination-20211-eng
doc_title: "WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng"
section_id: page-091
section_title: "Page 91"
pages: 91-91
pdf_page: 91
source_pdf: WHO-2019-nCoV-Digital-certificates-vaccination-2021.1-eng.pdf
source_sha256: f57b14cb2acb728d
text_source: embedded
granularity: page
---
Page
74
DDCC:VS - Technical Specifications and Implementation Guidance, 27 August 2021
Requirement ID
Category
Non-functional requirement
DDCC.NFXNREQ.014
Disaster recovery, 
business continuity, 
resilience
The system SHOULD provide near-instantaneous switch-over if any one component of 
the physical architecture fails critically (data centre destroyed, server destroyed, etc.)
DDCC.NFXNREQ.015
Disaster recovery, 
business continuity, 
resilience
All components of the solution SHOULD be underpinned by robust monitoring 
tools that track usage across space and time, so that system load and source can be 
queried.
DDCC.NFXNREQ.016
Disaster recovery, 
business continuity, 
resilience
Data concerning system usage SHOULD be available to system administrators via a 
dashboard to show current load, and recent load (last week, last month), and be able 
to perform custom queries by place and time. It SHOULD be possible to export this 
data.
DDCC.NFXNREQ.017
Disaster recovery, 
business continuity, 
resilience
It SHALL be possible to automatically log any periods of outage of the system and to 
supplement and update this record manually.
DDCC.NFXNREQ.018
Disaster recovery, 
business continuity, 
resilience
It SHALL be possible to trigger system alerts based on uptime and performance.
DDCC.NFXNREQ.019
Disaster recovery, 
business continuity, 
resilience
It SHOULD be possible to use system alerts to perform actions such as dispatch of a 
warning email/SMS to a system administrator or to execute a script that (for example) 
spins up a new virtual machine for load balancing.
DDCC.NFXNREQ.020
Performance/
response time
The solution SHALL follow best practices to deliver a responsive interface in which 
typical requests can be served (end-to-end interaction) in a maximum time specified 
in a number of seconds to be determined based on typical bandwidths. Degradation 
to a greater maximum time in number of seconds for limited-bandwidth scenarios is 
acceptable.
DDCC.NFXNREQ.021
Performance/
response time
The solution SHOULD be designed so that degradation of performance due to 
increased load (surge of users) is minimized.
DDCC.NFXNREQ.022
Performance/
response time
Where appropriate, long-running processes such as complex queries MAY be available 
for asynchronous execution, to allow a user to continue to interact with the system 
while the job executes and to receive a notification when the work is complete.
DDCC.NFXNREQ.023
Performance/
response time
The system MAY implement detection of a frozen (“hung”) interface to give the user 
the option to cancel a current request.
DDCC.NFXNREQ.024
Performance/
response time
The system SHOULD collect metrics on performance and response time to allow a 
system administrator to monitor system behaviour, identify bottlenecks or issues, 
and pro-actively address any risk of unacceptable degradation of speed.
DDCC.NFXNREQ.025
Performance/
response time
As with system availability, the solution SHALL provide dashboards of performance 
metrics, allow querying of the performance log and export of performance data for 
reports.
DDCC.NFXNREQ.026
Performance/
response time
As with system availability, the solution SHALL have the ability to set thresholds on 
performance and use the breach of those thresholds to raise alerts that can trigger 
email notifications or automated system actions (bring an extra server into a load-
balanced set, for example).
DDCC.NFXNREQ.027
Security and privacy
Tools to request an account, log in, log out, set and change passwords, and receive 
password reminders SHALL be provided.
DDCC.NFXNREQ.028
Security and privacy
All interactions between a client and a server component of the solution SHALL be 
securely encrypted to prevent “man in the middle” interference with data in transit.
DDCC.NFXNREQ.029
Security and privacy
Any cloud components of the solution SHALL store their cloud data-at-rest in an 
encrypted format.
DDCC.NFXNREQ.030
Security and privacy
The solution SHALL have a security model that is robust and flexible and controls both 
access to data and the operations that can be executed against data.
