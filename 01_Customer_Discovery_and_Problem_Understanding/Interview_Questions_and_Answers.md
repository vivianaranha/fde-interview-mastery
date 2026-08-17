# Customer Discovery & Problem Understanding — Interview Questions & Answers

Understanding the customer's business problem, users, workflows, pain points, data, constraints, and desired outcomes before deciding what to build.

**Questions in this section: 15**

---

## Question 1: What is the purpose of customer discovery in an FDE engagement?

**Answer:** Customer discovery prevents the team from solving the wrong problem. An FDE uses discovery to understand the business objective, current workflow, users, pain points, data sources, operational constraints, and what success looks like. The output should be a shared problem definition rather than a premature technical solution.

---

## Question 2: What questions would you ask in your first customer meeting?

**Answer:** I would ask what business outcome they want, who experiences the problem, how the process works today, where delays or errors occur, what systems and data are involved, what constraints exist, how often the problem occurs, what has already been tried, who owns the workflow, and how they would measure success.

---

## Question 3: How do you distinguish a stated request from the underlying problem?

**Answer:** I treat the initial request as a hypothesis. I ask why the request matters, what happens today, what failure looks like, and what outcome the customer actually wants. For example, 'build an AI chatbot' may really mean 'reduce support resolution time without increasing headcount.'

---

## Question 4: How would you map an existing customer workflow?

**Answer:** I would identify the actors, trigger, steps, systems touched, decision points, handoffs, failure paths, manual work, timing, and outputs. I would then validate the workflow with actual users rather than relying only on executive descriptions.

---

## Question 5: What is a good way to handle conflicting stakeholder descriptions of the same problem?

**Answer:** I would document the conflicting assumptions, gather examples or data from the real workflow, and run a working session to establish a shared current-state view. The goal is not to pick a side but to make the disagreement observable and resolve it with evidence.

---

## Question 6: How do you identify whether a problem is worth solving?

**Answer:** I look at frequency, severity, business impact, number of affected users, cost of the current process, strategic importance, feasibility, and whether a measurable improvement is possible. A technically interesting problem is not automatically a valuable deployment opportunity.

---

## Question 7: How would you discover hidden constraints?

**Answer:** I explicitly ask about security, privacy, compliance, data residency, network boundaries, identity, procurement, change windows, latency, support ownership, budget, and integration restrictions. I also talk to platform and security teams early because business stakeholders may not know every constraint.

---

## Question 8: What discovery artifacts would you create?

**Answer:** Typical artifacts include a problem statement, current-state workflow, stakeholder map, use-case list, constraints and assumptions log, data inventory, risk list, success metrics, and an initial scope statement. These artifacts make later architecture and prioritization decisions traceable.

---

## Question 9: How do you know when discovery is complete enough to move forward?

**Answer:** Discovery is complete enough when the team can explain the problem, users, workflow, desired outcome, major constraints, available data, ownership, and measurable success criteria with reasonable confidence. Discovery does not need to eliminate all uncertainty; it needs to reduce the uncertainty that would make the next step reckless.

---

## Question 10: How would you handle a customer who insists on a specific technology before the problem is understood?

**Answer:** I would acknowledge the preference, then connect the technology to the desired outcome. I would test whether the technology actually fits the workflow, data, constraints, and economics. If it does, great. If not, I would explain the trade-off with evidence and propose a better option.

---

## Question 11: Give an example of a weak problem statement and improve it.

**Answer:** Weak: 'We need an AI agent for support.' Better: 'Support agents spend an average of 4.2 minutes manually triaging each ticket, causing routing delays and inconsistent assignment. We want to reduce triage time by at least 50% while maintaining at least 90% routing accuracy.'

---

## Question 12: How do you discover the real users of a system?

**Answer:** I ask who performs the work, who consumes the output, who approves exceptions, who supports the system, and who is affected when it fails. Enterprise solutions often have primary users, downstream users, administrators, and governance stakeholders.

---

## Question 13: What do you do when the customer has no baseline metrics?

**Answer:** I establish a lightweight baseline before promising improvement. That might mean sampling cases, reviewing logs, timing manual workflows, interviewing users, or instrumenting the current process. Without a baseline, claims of improvement are mostly subjective.

---

## Question 14: How would you validate that your discovery findings are correct?

**Answer:** I play the findings back to stakeholders using a concise problem statement, workflow, assumptions, constraints, and success metrics. I ask for explicit corrections and validate important claims against data, logs, tickets, or observed user behavior.

---

## Question 15: What is a common discovery mistake FDEs make?

**Answer:** A common mistake is jumping into solution mode too early. This creates impressive prototypes that do not address the customer's real bottleneck. Strong FDEs delay implementation just long enough to establish the problem, value, constraints, and decision criteria.

---

# Day-to-Day FDE Interview Scenarios

The following questions focus on the practical, daily work of a Forward Deployed Engineer: ambiguous customer situations, delivery pressure, debugging, cross-team collaboration, production risk, communication, prioritization, and measurable outcomes.

---

## Question 16: Walk me through how you would handle preparing for a first customer discovery call in your day-to-day FDE work when the customer has shared only a one-line problem statement.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the customer product owner, and produce a discovery agenda and question set. I would explicitly watch for jumping to a solution before understanding the workflow. Before moving on, I would confirm clarity on users, workflow, pain, baseline, and success. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 17: What would you do first if you were responsible for preparing for a first customer discovery call and discovered that the customer has shared only a one-line problem statement?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the customer product owner early, capture the result in a discovery agenda and question set, and prioritize resolving the uncertainty that could cause jumping to a solution before understanding the workflow. I would consider the task complete when we have clarity on users, workflow, pain, baseline, and success.

---

## Question 18: During preparing for a first customer discovery call, what are the most important questions you would ask because the customer has shared only a one-line problem statement?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the customer product owner needs from us. The questions should help us create a discovery agenda and question set and avoid jumping to a solution before understanding the workflow, not simply collect information for its own sake.

---

## Question 19: How would you prioritize preparing for a first customer discovery call against other work if the customer has shared only a one-line problem statement?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create jumping to a solution before understanding the workflow or block a major dependency, it moves up the queue. I would make that reasoning visible to the customer product owner, time-box lower-value exploration, and define a concrete next checkpoint around clarity on users, workflow, pain, baseline, and success.

---

## Question 20: What trade-offs would you consider while doing preparing for a first customer discovery call when the customer has shared only a one-line problem statement?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a discovery agenda and question set, make jumping to a solution before understanding the workflow explicit, and align with the customer product owner on what we are intentionally deferring.

---

## Question 21: How would you communicate progress or a blocker related to preparing for a first customer discovery call to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of jumping to a solution before understanding the workflow, show what we are doing with the customer product owner, and point to the next measurable checkpoint: clarity on users, workflow, pain, baseline, and success.

---

## Question 22: How would you collaborate with the customer product owner during preparing for a first customer discovery call?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a discovery agenda and question set as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in clarity on users, workflow, pain, baseline, and success instead of an unresolved discussion.

---

## Question 23: How would you know whether your work on preparing for a first customer discovery call was successful?

**Answer:** I would define success before completing the task. The primary signal would be clarity on users, workflow, pain, baseline, and success. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a discovery agenda and question set exists but the team is still exposed to jumping to a solution before understanding the workflow, I would not consider the work finished.

---

## Question 24: Tell me about a time you handled something similar to preparing for a first customer discovery call. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the customer product owner, what trade-off you made, and how you avoided or reduced jumping to a solution before understanding the workflow. Finish with a measurable result such as clarity on users, workflow, pain, baseline, and success, plus what you learned and would reuse in the next deployment.

---

## Question 25: Walk me through how you would handle interviewing frontline users in your day-to-day FDE work when executives describe the process differently from the people doing the work.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the frontline operations lead, and produce a validated current-state workflow. I would explicitly watch for designing from management assumptions instead of real user behavior. Before moving on, I would confirm agreement on actual steps, exceptions, and pain points. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 26: What would you do first if you were responsible for interviewing frontline users and discovered that executives describe the process differently from the people doing the work?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the frontline operations lead early, capture the result in a validated current-state workflow, and prioritize resolving the uncertainty that could cause designing from management assumptions instead of real user behavior. I would consider the task complete when we have agreement on actual steps, exceptions, and pain points.

---

## Question 27: During interviewing frontline users, what are the most important questions you would ask because executives describe the process differently from the people doing the work?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the frontline operations lead needs from us. The questions should help us create a validated current-state workflow and avoid designing from management assumptions instead of real user behavior, not simply collect information for its own sake.

---

## Question 28: How would you prioritize interviewing frontline users against other work if executives describe the process differently from the people doing the work?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create designing from management assumptions instead of real user behavior or block a major dependency, it moves up the queue. I would make that reasoning visible to the frontline operations lead, time-box lower-value exploration, and define a concrete next checkpoint around agreement on actual steps, exceptions, and pain points.

---

## Question 29: What trade-offs would you consider while doing interviewing frontline users when executives describe the process differently from the people doing the work?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a validated current-state workflow, make designing from management assumptions instead of real user behavior explicit, and align with the frontline operations lead on what we are intentionally deferring.

---

## Question 30: How would you communicate progress or a blocker related to interviewing frontline users to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of designing from management assumptions instead of real user behavior, show what we are doing with the frontline operations lead, and point to the next measurable checkpoint: agreement on actual steps, exceptions, and pain points.

---

## Question 31: How would you collaborate with the frontline operations lead during interviewing frontline users?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a validated current-state workflow as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in agreement on actual steps, exceptions, and pain points instead of an unresolved discussion.

---

## Question 32: How would you know whether your work on interviewing frontline users was successful?

**Answer:** I would define success before completing the task. The primary signal would be agreement on actual steps, exceptions, and pain points. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a validated current-state workflow exists but the team is still exposed to designing from management assumptions instead of real user behavior, I would not consider the work finished.

---

## Question 33: Tell me about a time you handled something similar to interviewing frontline users. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the frontline operations lead, what trade-off you made, and how you avoided or reduced designing from management assumptions instead of real user behavior. Finish with a measurable result such as agreement on actual steps, exceptions, and pain points, plus what you learned and would reuse in the next deployment.

---

## Question 34: Walk me through how you would handle mapping a manual business process in your day-to-day FDE work when the workflow spans spreadsheets, email, and two enterprise systems.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the business analyst, and produce a current-state process map. I would explicitly watch for missing hidden handoffs and exception paths. Before moving on, I would confirm documented actors, steps, systems, timing, and failure points. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 35: What would you do first if you were responsible for mapping a manual business process and discovered that the workflow spans spreadsheets, email, and two enterprise systems?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the business analyst early, capture the result in a current-state process map, and prioritize resolving the uncertainty that could cause missing hidden handoffs and exception paths. I would consider the task complete when we have documented actors, steps, systems, timing, and failure points.

---

## Question 36: During mapping a manual business process, what are the most important questions you would ask because the workflow spans spreadsheets, email, and two enterprise systems?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the business analyst needs from us. The questions should help us create a current-state process map and avoid missing hidden handoffs and exception paths, not simply collect information for its own sake.

---

## Question 37: How would you prioritize mapping a manual business process against other work if the workflow spans spreadsheets, email, and two enterprise systems?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create missing hidden handoffs and exception paths or block a major dependency, it moves up the queue. I would make that reasoning visible to the business analyst, time-box lower-value exploration, and define a concrete next checkpoint around documented actors, steps, systems, timing, and failure points.

---

## Question 38: What trade-offs would you consider while doing mapping a manual business process when the workflow spans spreadsheets, email, and two enterprise systems?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a current-state process map, make missing hidden handoffs and exception paths explicit, and align with the business analyst on what we are intentionally deferring.

---

## Question 39: How would you communicate progress or a blocker related to mapping a manual business process to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of missing hidden handoffs and exception paths, show what we are doing with the business analyst, and point to the next measurable checkpoint: documented actors, steps, systems, timing, and failure points.

---

## Question 40: How would you collaborate with the business analyst during mapping a manual business process?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a current-state process map as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in documented actors, steps, systems, timing, and failure points instead of an unresolved discussion.

---

## Question 41: How would you know whether your work on mapping a manual business process was successful?

**Answer:** I would define success before completing the task. The primary signal would be documented actors, steps, systems, timing, and failure points. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a current-state process map exists but the team is still exposed to missing hidden handoffs and exception paths, I would not consider the work finished.

---

## Question 42: Tell me about a time you handled something similar to mapping a manual business process. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the business analyst, what trade-off you made, and how you avoided or reduced missing hidden handoffs and exception paths. Finish with a measurable result such as documented actors, steps, systems, timing, and failure points, plus what you learned and would reuse in the next deployment.

---

## Question 43: Walk me through how you would handle discovering baseline metrics in your day-to-day FDE work when the customer says the process is slow but has no measured baseline.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the operations manager, and produce a lightweight baseline measurement plan. I would explicitly watch for claiming improvement without evidence. Before moving on, I would confirm cycle time, error rate, volume, or manual effort. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 44: What would you do first if you were responsible for discovering baseline metrics and discovered that the customer says the process is slow but has no measured baseline?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the operations manager early, capture the result in a lightweight baseline measurement plan, and prioritize resolving the uncertainty that could cause claiming improvement without evidence. I would consider the task complete when we have cycle time, error rate, volume, or manual effort.

---

## Question 45: During discovering baseline metrics, what are the most important questions you would ask because the customer says the process is slow but has no measured baseline?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the operations manager needs from us. The questions should help us create a lightweight baseline measurement plan and avoid claiming improvement without evidence, not simply collect information for its own sake.

---

## Question 46: How would you prioritize discovering baseline metrics against other work if the customer says the process is slow but has no measured baseline?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create claiming improvement without evidence or block a major dependency, it moves up the queue. I would make that reasoning visible to the operations manager, time-box lower-value exploration, and define a concrete next checkpoint around cycle time, error rate, volume, or manual effort.

---

## Question 47: What trade-offs would you consider while doing discovering baseline metrics when the customer says the process is slow but has no measured baseline?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a lightweight baseline measurement plan, make claiming improvement without evidence explicit, and align with the operations manager on what we are intentionally deferring.

---

## Question 48: How would you communicate progress or a blocker related to discovering baseline metrics to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of claiming improvement without evidence, show what we are doing with the operations manager, and point to the next measurable checkpoint: cycle time, error rate, volume, or manual effort.

---

## Question 49: How would you collaborate with the operations manager during discovering baseline metrics?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a lightweight baseline measurement plan as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in cycle time, error rate, volume, or manual effort instead of an unresolved discussion.

---

## Question 50: How would you know whether your work on discovering baseline metrics was successful?

**Answer:** I would define success before completing the task. The primary signal would be cycle time, error rate, volume, or manual effort. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a lightweight baseline measurement plan exists but the team is still exposed to claiming improvement without evidence, I would not consider the work finished.

---

## Question 51: Tell me about a time you handled something similar to discovering baseline metrics. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the operations manager, what trade-off you made, and how you avoided or reduced claiming improvement without evidence. Finish with a measurable result such as cycle time, error rate, volume, or manual effort, plus what you learned and would reuse in the next deployment.

---

## Question 52: Walk me through how you would handle identifying the real decision maker in your day-to-day FDE work when several stakeholders attend meetings but nobody appears to own the outcome.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the engagement lead, and produce a stakeholder and decision map. I would explicitly watch for building without an accountable sponsor or owner. Before moving on, I would confirm clear decision rights and escalation paths. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 53: What would you do first if you were responsible for identifying the real decision maker and discovered that several stakeholders attend meetings but nobody appears to own the outcome?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the engagement lead early, capture the result in a stakeholder and decision map, and prioritize resolving the uncertainty that could cause building without an accountable sponsor or owner. I would consider the task complete when we have clear decision rights and escalation paths.

---

## Question 54: During identifying the real decision maker, what are the most important questions you would ask because several stakeholders attend meetings but nobody appears to own the outcome?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the engagement lead needs from us. The questions should help us create a stakeholder and decision map and avoid building without an accountable sponsor or owner, not simply collect information for its own sake.

---

## Question 55: How would you prioritize identifying the real decision maker against other work if several stakeholders attend meetings but nobody appears to own the outcome?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create building without an accountable sponsor or owner or block a major dependency, it moves up the queue. I would make that reasoning visible to the engagement lead, time-box lower-value exploration, and define a concrete next checkpoint around clear decision rights and escalation paths.

---

## Question 56: What trade-offs would you consider while doing identifying the real decision maker when several stakeholders attend meetings but nobody appears to own the outcome?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a stakeholder and decision map, make building without an accountable sponsor or owner explicit, and align with the engagement lead on what we are intentionally deferring.

---

## Question 57: How would you communicate progress or a blocker related to identifying the real decision maker to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of building without an accountable sponsor or owner, show what we are doing with the engagement lead, and point to the next measurable checkpoint: clear decision rights and escalation paths.

---

## Question 58: How would you collaborate with the engagement lead during identifying the real decision maker?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a stakeholder and decision map as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in clear decision rights and escalation paths instead of an unresolved discussion.

---

## Question 59: How would you know whether your work on identifying the real decision maker was successful?

**Answer:** I would define success before completing the task. The primary signal would be clear decision rights and escalation paths. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a stakeholder and decision map exists but the team is still exposed to building without an accountable sponsor or owner, I would not consider the work finished.

---

## Question 60: Tell me about a time you handled something similar to identifying the real decision maker. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the engagement lead, what trade-off you made, and how you avoided or reduced building without an accountable sponsor or owner. Finish with a measurable result such as clear decision rights and escalation paths, plus what you learned and would reuse in the next deployment.

---

## Question 61: Walk me through how you would handle handling conflicting stakeholder goals in your day-to-day FDE work when operations wants speed while security wants tighter controls.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the security lead, and produce a documented trade-off and decision record. I would explicitly watch for optimizing for one team and creating risk for another. Before moving on, I would confirm an agreed priority and guardrail set. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 62: What would you do first if you were responsible for handling conflicting stakeholder goals and discovered that operations wants speed while security wants tighter controls?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the security lead early, capture the result in a documented trade-off and decision record, and prioritize resolving the uncertainty that could cause optimizing for one team and creating risk for another. I would consider the task complete when we have an agreed priority and guardrail set.

---

## Question 63: During handling conflicting stakeholder goals, what are the most important questions you would ask because operations wants speed while security wants tighter controls?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the security lead needs from us. The questions should help us create a documented trade-off and decision record and avoid optimizing for one team and creating risk for another, not simply collect information for its own sake.

---

## Question 64: How would you prioritize handling conflicting stakeholder goals against other work if operations wants speed while security wants tighter controls?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create optimizing for one team and creating risk for another or block a major dependency, it moves up the queue. I would make that reasoning visible to the security lead, time-box lower-value exploration, and define a concrete next checkpoint around an agreed priority and guardrail set.

---

## Question 65: What trade-offs would you consider while doing handling conflicting stakeholder goals when operations wants speed while security wants tighter controls?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a documented trade-off and decision record, make optimizing for one team and creating risk for another explicit, and align with the security lead on what we are intentionally deferring.

---

## Question 66: How would you communicate progress or a blocker related to handling conflicting stakeholder goals to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of optimizing for one team and creating risk for another, show what we are doing with the security lead, and point to the next measurable checkpoint: an agreed priority and guardrail set.

---

## Question 67: How would you collaborate with the security lead during handling conflicting stakeholder goals?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a documented trade-off and decision record as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in an agreed priority and guardrail set instead of an unresolved discussion.

---

## Question 68: How would you know whether your work on handling conflicting stakeholder goals was successful?

**Answer:** I would define success before completing the task. The primary signal would be an agreed priority and guardrail set. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a documented trade-off and decision record exists but the team is still exposed to optimizing for one team and creating risk for another, I would not consider the work finished.

---

## Question 69: Tell me about a time you handled something similar to handling conflicting stakeholder goals. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the security lead, what trade-off you made, and how you avoided or reduced optimizing for one team and creating risk for another. Finish with a measurable result such as an agreed priority and guardrail set, plus what you learned and would reuse in the next deployment.

---

## Question 70: Walk me through how you would handle observing a live workflow in your day-to-day FDE work when what users say they do differs from what actually happens.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the end user, and produce observation notes and revised workflow. I would explicitly watch for missing workarounds and informal steps. Before moving on, I would confirm validated real-world behavior. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 71: What would you do first if you were responsible for observing a live workflow and discovered that what users say they do differs from what actually happens?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the end user early, capture the result in observation notes and revised workflow, and prioritize resolving the uncertainty that could cause missing workarounds and informal steps. I would consider the task complete when we have validated real-world behavior.

---

## Question 72: During observing a live workflow, what are the most important questions you would ask because what users say they do differs from what actually happens?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the end user needs from us. The questions should help us create observation notes and revised workflow and avoid missing workarounds and informal steps, not simply collect information for its own sake.

---

## Question 73: How would you prioritize observing a live workflow against other work if what users say they do differs from what actually happens?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create missing workarounds and informal steps or block a major dependency, it moves up the queue. I would make that reasoning visible to the end user, time-box lower-value exploration, and define a concrete next checkpoint around validated real-world behavior.

---

## Question 74: What trade-offs would you consider while doing observing a live workflow when what users say they do differs from what actually happens?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in observation notes and revised workflow, make missing workarounds and informal steps explicit, and align with the end user on what we are intentionally deferring.

---

## Question 75: How would you communicate progress or a blocker related to observing a live workflow to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of missing workarounds and informal steps, show what we are doing with the end user, and point to the next measurable checkpoint: validated real-world behavior.

---

## Question 76: How would you collaborate with the end user during observing a live workflow?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use observation notes and revised workflow as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in validated real-world behavior instead of an unresolved discussion.

---

## Question 77: How would you know whether your work on observing a live workflow was successful?

**Answer:** I would define success before completing the task. The primary signal would be validated real-world behavior. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If observation notes and revised workflow exists but the team is still exposed to missing workarounds and informal steps, I would not consider the work finished.

---

## Question 78: Tell me about a time you handled something similar to observing a live workflow. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the end user, what trade-off you made, and how you avoided or reduced missing workarounds and informal steps. Finish with a measurable result such as validated real-world behavior, plus what you learned and would reuse in the next deployment.

---

## Question 79: Walk me through how you would handle testing whether AI is actually needed in your day-to-day FDE work when the customer asks for an agent but the task may be deterministic.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the solution architect, and produce a solution-options comparison. I would explicitly watch for forcing AI into a problem better solved with rules or search. Before moving on, I would confirm evidence that the chosen approach fits the task. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 80: What would you do first if you were responsible for testing whether AI is actually needed and discovered that the customer asks for an agent but the task may be deterministic?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the solution architect early, capture the result in a solution-options comparison, and prioritize resolving the uncertainty that could cause forcing AI into a problem better solved with rules or search. I would consider the task complete when we have evidence that the chosen approach fits the task.

---

## Question 81: During testing whether AI is actually needed, what are the most important questions you would ask because the customer asks for an agent but the task may be deterministic?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the solution architect needs from us. The questions should help us create a solution-options comparison and avoid forcing AI into a problem better solved with rules or search, not simply collect information for its own sake.

---

## Question 82: How would you prioritize testing whether AI is actually needed against other work if the customer asks for an agent but the task may be deterministic?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create forcing AI into a problem better solved with rules or search or block a major dependency, it moves up the queue. I would make that reasoning visible to the solution architect, time-box lower-value exploration, and define a concrete next checkpoint around evidence that the chosen approach fits the task.

---

## Question 83: What trade-offs would you consider while doing testing whether AI is actually needed when the customer asks for an agent but the task may be deterministic?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a solution-options comparison, make forcing AI into a problem better solved with rules or search explicit, and align with the solution architect on what we are intentionally deferring.

---

## Question 84: How would you communicate progress or a blocker related to testing whether AI is actually needed to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of forcing AI into a problem better solved with rules or search, show what we are doing with the solution architect, and point to the next measurable checkpoint: evidence that the chosen approach fits the task.

---

## Question 85: How would you collaborate with the solution architect during testing whether AI is actually needed?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a solution-options comparison as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in evidence that the chosen approach fits the task instead of an unresolved discussion.

---

## Question 86: How would you know whether your work on testing whether AI is actually needed was successful?

**Answer:** I would define success before completing the task. The primary signal would be evidence that the chosen approach fits the task. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a solution-options comparison exists but the team is still exposed to forcing AI into a problem better solved with rules or search, I would not consider the work finished.

---

## Question 87: Tell me about a time you handled something similar to testing whether AI is actually needed. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the solution architect, what trade-off you made, and how you avoided or reduced forcing AI into a problem better solved with rules or search. Finish with a measurable result such as evidence that the chosen approach fits the task, plus what you learned and would reuse in the next deployment.

---

## Question 88: Walk me through how you would handle discovering data availability in your day-to-day FDE work when the proposed use case depends on historical data the team has never inspected.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the data owner, and produce a data inventory and access plan. I would explicitly watch for designing around data that is unavailable or poor quality. Before moving on, I would confirm confirmed source, owner, quality, access, and freshness. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 89: What would you do first if you were responsible for discovering data availability and discovered that the proposed use case depends on historical data the team has never inspected?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the data owner early, capture the result in a data inventory and access plan, and prioritize resolving the uncertainty that could cause designing around data that is unavailable or poor quality. I would consider the task complete when we have confirmed source, owner, quality, access, and freshness.

---

## Question 90: During discovering data availability, what are the most important questions you would ask because the proposed use case depends on historical data the team has never inspected?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the data owner needs from us. The questions should help us create a data inventory and access plan and avoid designing around data that is unavailable or poor quality, not simply collect information for its own sake.

---

## Question 91: How would you prioritize discovering data availability against other work if the proposed use case depends on historical data the team has never inspected?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create designing around data that is unavailable or poor quality or block a major dependency, it moves up the queue. I would make that reasoning visible to the data owner, time-box lower-value exploration, and define a concrete next checkpoint around confirmed source, owner, quality, access, and freshness.

---

## Question 92: What trade-offs would you consider while doing discovering data availability when the proposed use case depends on historical data the team has never inspected?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a data inventory and access plan, make designing around data that is unavailable or poor quality explicit, and align with the data owner on what we are intentionally deferring.

---

## Question 93: How would you communicate progress or a blocker related to discovering data availability to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of designing around data that is unavailable or poor quality, show what we are doing with the data owner, and point to the next measurable checkpoint: confirmed source, owner, quality, access, and freshness.

---

## Question 94: How would you collaborate with the data owner during discovering data availability?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a data inventory and access plan as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in confirmed source, owner, quality, access, and freshness instead of an unresolved discussion.

---

## Question 95: How would you know whether your work on discovering data availability was successful?

**Answer:** I would define success before completing the task. The primary signal would be confirmed source, owner, quality, access, and freshness. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a data inventory and access plan exists but the team is still exposed to designing around data that is unavailable or poor quality, I would not consider the work finished.

---

## Question 96: Tell me about a time you handled something similar to discovering data availability. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the data owner, what trade-off you made, and how you avoided or reduced designing around data that is unavailable or poor quality. Finish with a measurable result such as confirmed source, owner, quality, access, and freshness, plus what you learned and would reuse in the next deployment.

---

## Question 97: Walk me through how you would handle running a discovery playback in your day-to-day FDE work when you believe you understand the problem but need stakeholder alignment.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the customer sponsor, and produce a concise problem statement and playback deck. I would explicitly watch for moving into build with unresolved assumptions. Before moving on, I would confirm explicit stakeholder confirmation or corrections. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 98: What would you do first if you were responsible for running a discovery playback and discovered that you believe you understand the problem but need stakeholder alignment?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the customer sponsor early, capture the result in a concise problem statement and playback deck, and prioritize resolving the uncertainty that could cause moving into build with unresolved assumptions. I would consider the task complete when we have explicit stakeholder confirmation or corrections.

---

## Question 99: During running a discovery playback, what are the most important questions you would ask because you believe you understand the problem but need stakeholder alignment?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the customer sponsor needs from us. The questions should help us create a concise problem statement and playback deck and avoid moving into build with unresolved assumptions, not simply collect information for its own sake.

---

## Question 100: How would you prioritize running a discovery playback against other work if you believe you understand the problem but need stakeholder alignment?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create moving into build with unresolved assumptions or block a major dependency, it moves up the queue. I would make that reasoning visible to the customer sponsor, time-box lower-value exploration, and define a concrete next checkpoint around explicit stakeholder confirmation or corrections.

---

## Question 101: What trade-offs would you consider while doing running a discovery playback when you believe you understand the problem but need stakeholder alignment?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a concise problem statement and playback deck, make moving into build with unresolved assumptions explicit, and align with the customer sponsor on what we are intentionally deferring.

---

## Question 102: How would you communicate progress or a blocker related to running a discovery playback to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of moving into build with unresolved assumptions, show what we are doing with the customer sponsor, and point to the next measurable checkpoint: explicit stakeholder confirmation or corrections.

---

## Question 103: How would you collaborate with the customer sponsor during running a discovery playback?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a concise problem statement and playback deck as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in explicit stakeholder confirmation or corrections instead of an unresolved discussion.

---

## Question 104: How would you know whether your work on running a discovery playback was successful?

**Answer:** I would define success before completing the task. The primary signal would be explicit stakeholder confirmation or corrections. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a concise problem statement and playback deck exists but the team is still exposed to moving into build with unresolved assumptions, I would not consider the work finished.

---

## Question 105: Tell me about a time you handled something similar to running a discovery playback. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the customer sponsor, what trade-off you made, and how you avoided or reduced moving into build with unresolved assumptions. Finish with a measurable result such as explicit stakeholder confirmation or corrections, plus what you learned and would reuse in the next deployment.

---
