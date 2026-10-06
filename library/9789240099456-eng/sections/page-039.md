---
doc_id: 9789240099456-eng
doc_title: "9789240099456-eng"
section_id: page-039
section_title: "Page 39"
pages: 39-39
pdf_page: 39
source_pdf: 9789240099456-eng.pdf
source_sha256: 6b0f603e2a792bb4
text_source: embedded
granularity: page
---
29
Generic business processes and workflows
personas
indicators
workflows
data
decisions
scenarios
requirements
recommendations
Symbol
Symbol name
Description
Lane 2
Lane 3
Pool
Lane 1
Swim lane 
Each individual or type of user is assigned to a swim lane, a designated area for noting the activities performed or expected by that specific 
actor. For example, a family planning health worker may have one swim lane; the supervisor would be in another swim lane; the clients would 
be classified in another swim lane. If the activities can be performed by either actor, then those activities can be depicted overlapping the two 
relevant swim lanes.
Start event or 
trigger event
The workflow diagram should contain both a start and an end event, defining the beginning and completion of the task, respectively.
End event
There can be multiple end events depicted across multiple swim lanes in a business process diagram. However, for diagram clarity, there should 
only be one end event per swim lane.
Activity, process, 
step or task
Each activity should start with a verb, (e.g. “Register client”, “Calculate risk”). Between the start and end of a task, there should be a series of 
activities noting the successive actions performed by the actor in that swim lane. There can also be subprocesses within each activity. 
Activity with 
subprocess
This denotes an activity that has a much longer subprocess to be detailed in another diagram. If the diagram starts to become too complex and 
unhelpful, the subprocess symbol should be used to reference this subprocess depicted in another diagram (an activity with subprocess in a grey 
box is not covered in this DAK).
Activity with 
business rule
This denotes a decision-making activity that requires the business rule, or decision-support logic, to be detailed in a “decision-support table”. 
This means that the logic described in the decision-support table will come into play during this activity as outlined in the business process. This 
is usually reserved for complex decisions.
Sequence flow
This denotes the flow direction from one process to the next. The end event should not have any output arrows. All symbols (except start event) may 
have an unlimited number of input arrows. All symbols (except end event and gateway) should have one and only one output arrow, leading to a new 
symbol, looping back to a previously used symbol or to the end event symbol. Connecting arrows should not intersect (cross) each other. 
 Gateway 
This symbol is used to depict a fork, or decision point, in the workflow, which may be a simple binary (e.g. yes/no) filter with two corresponding 
output arrows or a different set of outputs. There should only be two different outputs that originate from the decision point. If more than two 
outputs or sequence flow arrows are needed, you most likely are trying to depict “decision-support logic” or a “business rule”. This should be 
depicted as an “Activity with business rule” (above) instead.
Throw – Link
The “Throw – Link” serves as the start an off-page connector. It is the end of the process when there is no more room for the workflow page. It 
is the end of a process on the current page or the end of a subprocess that is part of a larger process. There will need to be a “Catch – Link” that 
follows the “Throw – Link”. 
Catch – Link
The “Catch – Link” serves as the end an off-page connector. It is the start of the new process on a different page from the “Throw – Link” or the 
start of a subprocess that is part of a larger process. There needs to be a “Throw – Link” that is aligned to the “Catch – Link”. 
Loop activity
This “Loop Activity” symbolizes an activity or task that is repeated until it no longer needs to be repeated. For example, vaccine administration 
can happen as many times as the number of vaccines that need to be given.
