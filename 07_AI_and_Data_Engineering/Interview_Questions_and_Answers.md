# AI & Data Engineering — Interview Questions & Answers

Designing and deploying AI applications, agents, RAG systems, evaluations, data pipelines, model integrations, guardrails, and human-in-the-loop workflows.

**Questions in this section: 15**

---

## Question 1: How would you decide whether a customer problem should use an LLM?

**Answer:** I first ask whether the task depends on language understanding, generation, unstructured information, or flexible reasoning. If deterministic rules, search, or conventional ML can solve it more reliably and cheaply, I use those. LLMs should be chosen because they fit the problem, not because they are fashionable.

---

## Question 2: What is RAG and when would you use it?

**Answer:** Retrieval-augmented generation retrieves relevant external information and provides it to the model as context. I use it when answers must be grounded in changing or proprietary knowledge that should not rely only on model training.

---

## Question 3: What are the main components of a production RAG system?

**Answer:** Document ingestion, parsing, chunking, metadata, embeddings, indexing, retrieval, reranking where useful, prompt/context assembly, model inference, citation or grounding behavior, evaluation, access control, observability, and refresh processes.

---

## Question 4: How do you evaluate an AI application?

**Answer:** I define task-specific evals using representative examples and measurable criteria such as correctness, groundedness, tool-selection accuracy, policy compliance, latency, cost, and human-review rate. I combine offline evaluation with production feedback.

---

## Question 5: How do you reduce hallucinations?

**Answer:** I narrow the task, provide authoritative context, enforce structured outputs, use tools for factual operations, validate results, add refusal or escalation behavior, and measure hallucination-related failure modes with evaluations.

---

## Question 6: What is the difference between prompt engineering and context engineering?

**Answer:** Prompt engineering focuses on instructions and examples given to the model. Context engineering is broader: selecting, structuring, and managing all information the model sees, including retrieved documents, tool results, memory, state, policies, and user context.

---

## Question 7: How would you design an AI agent safely?

**Answer:** I constrain its tools and permissions, separate planning from execution where appropriate, validate tool arguments, require confirmation for high-impact actions, apply policy checks, log actions, set time or step limits, and make failure/escalation behavior explicit.

---

## Question 8: When should an AI workflow keep a human in the loop?

**Answer:** When consequences are high, model confidence or quality is insufficient, policies require approval, inputs are ambiguous, actions are irreversible, or exceptions require judgment. Human review should be targeted to the risky parts rather than added everywhere.

---

## Question 9: How do you select a model?

**Answer:** I evaluate quality on the actual task, latency, cost, context window, tool use, structured-output reliability, deployment constraints, privacy requirements, throughput, and operational support. I prefer benchmark results from my use case over generic leaderboard rankings.

---

## Question 10: How do you handle sensitive data in an AI application?

**Answer:** I classify data, minimize what is sent to models, enforce access control, use approved endpoints and retention settings, redact when appropriate, protect logs, separate environments, and involve security/privacy teams before production.

---

## Question 11: What is an embedding?

**Answer:** An embedding is a numerical representation of data such as text that captures semantic relationships. In RAG, embeddings are often used to find content that is semantically similar to a query.

---

## Question 12: What causes poor retrieval quality in RAG?

**Answer:** Common causes include bad parsing, poor chunking, missing metadata, weak queries, inappropriate embedding models, stale indexes, access filtering errors, and retrieving too much or too little context.

---

## Question 13: How do you monitor an AI system in production?

**Answer:** I monitor latency, errors, token or compute usage, cost, model/provider failures, tool failures, retrieval quality, user corrections, escalation rate, task success, policy violations, and drift in input or output patterns.

---

## Question 14: How do you test an AI agent's tool use?

**Answer:** I create scenarios that test correct tool selection, wrong-tool avoidance, malformed inputs, permission boundaries, timeouts, duplicate actions, tool errors, conflicting results, and whether the agent escalates safely when execution is uncertain.

---

## Question 15: What is a common AI FDE mistake?

**Answer:** Optimizing the demo prompt instead of the system. Production quality usually depends on data, context, tool design, evaluation, workflow controls, observability, and user experience as much as the model itself.

---

# Day-to-Day FDE Interview Scenarios

The following questions focus on the practical, daily work of a Forward Deployed Engineer: ambiguous customer situations, delivery pressure, debugging, cross-team collaboration, production risk, communication, prioritization, and measurable outcomes.

---

## Question 16: Walk me through how you would handle evaluating whether an LLM is needed in your day-to-day FDE work when the customer requests generative AI for a structured decision task.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the AI product manager, and produce a solution comparison. I would explicitly watch for using an LLM where deterministic logic is safer. Before moving on, I would confirm evidence-based model or non-model choice. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 17: What would you do first if you were responsible for evaluating whether an LLM is needed and discovered that the customer requests generative AI for a structured decision task?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the AI product manager early, capture the result in a solution comparison, and prioritize resolving the uncertainty that could cause using an LLM where deterministic logic is safer. I would consider the task complete when we have evidence-based model or non-model choice.

---

## Question 18: During evaluating whether an LLM is needed, what are the most important questions you would ask because the customer requests generative AI for a structured decision task?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the AI product manager needs from us. The questions should help us create a solution comparison and avoid using an LLM where deterministic logic is safer, not simply collect information for its own sake.

---

## Question 19: How would you prioritize evaluating whether an LLM is needed against other work if the customer requests generative AI for a structured decision task?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create using an LLM where deterministic logic is safer or block a major dependency, it moves up the queue. I would make that reasoning visible to the AI product manager, time-box lower-value exploration, and define a concrete next checkpoint around evidence-based model or non-model choice.

---

## Question 20: What trade-offs would you consider while doing evaluating whether an LLM is needed when the customer requests generative AI for a structured decision task?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a solution comparison, make using an LLM where deterministic logic is safer explicit, and align with the AI product manager on what we are intentionally deferring.

---

## Question 21: How would you communicate progress or a blocker related to evaluating whether an LLM is needed to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of using an LLM where deterministic logic is safer, show what we are doing with the AI product manager, and point to the next measurable checkpoint: evidence-based model or non-model choice.

---

## Question 22: How would you collaborate with the AI product manager during evaluating whether an LLM is needed?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a solution comparison as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in evidence-based model or non-model choice instead of an unresolved discussion.

---

## Question 23: How would you know whether your work on evaluating whether an LLM is needed was successful?

**Answer:** I would define success before completing the task. The primary signal would be evidence-based model or non-model choice. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a solution comparison exists but the team is still exposed to using an LLM where deterministic logic is safer, I would not consider the work finished.

---

## Question 24: Tell me about a time you handled something similar to evaluating whether an LLM is needed. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the AI product manager, what trade-off you made, and how you avoided or reduced using an LLM where deterministic logic is safer. Finish with a measurable result such as evidence-based model or non-model choice, plus what you learned and would reuse in the next deployment.

---

## Question 25: Walk me through how you would handle building an evaluation set in your day-to-day FDE work when the demo looks good but quality has never been measured systematically.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the data scientist, and produce a representative eval dataset. I would explicitly watch for optimizing on anecdotal examples. Before moving on, I would confirm repeatable task-specific quality metrics. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 26: What would you do first if you were responsible for building an evaluation set and discovered that the demo looks good but quality has never been measured systematically?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the data scientist early, capture the result in a representative eval dataset, and prioritize resolving the uncertainty that could cause optimizing on anecdotal examples. I would consider the task complete when we have repeatable task-specific quality metrics.

---

## Question 27: During building an evaluation set, what are the most important questions you would ask because the demo looks good but quality has never been measured systematically?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the data scientist needs from us. The questions should help us create a representative eval dataset and avoid optimizing on anecdotal examples, not simply collect information for its own sake.

---

## Question 28: How would you prioritize building an evaluation set against other work if the demo looks good but quality has never been measured systematically?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create optimizing on anecdotal examples or block a major dependency, it moves up the queue. I would make that reasoning visible to the data scientist, time-box lower-value exploration, and define a concrete next checkpoint around repeatable task-specific quality metrics.

---

## Question 29: What trade-offs would you consider while doing building an evaluation set when the demo looks good but quality has never been measured systematically?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a representative eval dataset, make optimizing on anecdotal examples explicit, and align with the data scientist on what we are intentionally deferring.

---

## Question 30: How would you communicate progress or a blocker related to building an evaluation set to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of optimizing on anecdotal examples, show what we are doing with the data scientist, and point to the next measurable checkpoint: repeatable task-specific quality metrics.

---

## Question 31: How would you collaborate with the data scientist during building an evaluation set?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a representative eval dataset as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in repeatable task-specific quality metrics instead of an unresolved discussion.

---

## Question 32: How would you know whether your work on building an evaluation set was successful?

**Answer:** I would define success before completing the task. The primary signal would be repeatable task-specific quality metrics. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a representative eval dataset exists but the team is still exposed to optimizing on anecdotal examples, I would not consider the work finished.

---

## Question 33: Tell me about a time you handled something similar to building an evaluation set. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the data scientist, what trade-off you made, and how you avoided or reduced optimizing on anecdotal examples. Finish with a measurable result such as repeatable task-specific quality metrics, plus what you learned and would reuse in the next deployment.

---

## Question 34: Walk me through how you would handle debugging poor RAG answers in your day-to-day FDE work when the model produces plausible answers that miss relevant internal documents.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the knowledge engineer, and produce a retrieval diagnostic. I would explicitly watch for tuning the prompt when retrieval is the real issue. Before moving on, I would confirm improved retrieval relevance and grounded answers. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 35: What would you do first if you were responsible for debugging poor RAG answers and discovered that the model produces plausible answers that miss relevant internal documents?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the knowledge engineer early, capture the result in a retrieval diagnostic, and prioritize resolving the uncertainty that could cause tuning the prompt when retrieval is the real issue. I would consider the task complete when we have improved retrieval relevance and grounded answers.

---

## Question 36: During debugging poor RAG answers, what are the most important questions you would ask because the model produces plausible answers that miss relevant internal documents?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the knowledge engineer needs from us. The questions should help us create a retrieval diagnostic and avoid tuning the prompt when retrieval is the real issue, not simply collect information for its own sake.

---

## Question 37: How would you prioritize debugging poor RAG answers against other work if the model produces plausible answers that miss relevant internal documents?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create tuning the prompt when retrieval is the real issue or block a major dependency, it moves up the queue. I would make that reasoning visible to the knowledge engineer, time-box lower-value exploration, and define a concrete next checkpoint around improved retrieval relevance and grounded answers.

---

## Question 38: What trade-offs would you consider while doing debugging poor RAG answers when the model produces plausible answers that miss relevant internal documents?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a retrieval diagnostic, make tuning the prompt when retrieval is the real issue explicit, and align with the knowledge engineer on what we are intentionally deferring.

---

## Question 39: How would you communicate progress or a blocker related to debugging poor RAG answers to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of tuning the prompt when retrieval is the real issue, show what we are doing with the knowledge engineer, and point to the next measurable checkpoint: improved retrieval relevance and grounded answers.

---

## Question 40: How would you collaborate with the knowledge engineer during debugging poor RAG answers?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a retrieval diagnostic as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in improved retrieval relevance and grounded answers instead of an unresolved discussion.

---

## Question 41: How would you know whether your work on debugging poor RAG answers was successful?

**Answer:** I would define success before completing the task. The primary signal would be improved retrieval relevance and grounded answers. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a retrieval diagnostic exists but the team is still exposed to tuning the prompt when retrieval is the real issue, I would not consider the work finished.

---

## Question 42: Tell me about a time you handled something similar to debugging poor RAG answers. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the knowledge engineer, what trade-off you made, and how you avoided or reduced tuning the prompt when retrieval is the real issue. Finish with a measurable result such as improved retrieval relevance and grounded answers, plus what you learned and would reuse in the next deployment.

---

## Question 43: Walk me through how you would handle handling model latency spikes in your day-to-day FDE work when users complain that AI responses are unpredictably slow.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the platform engineer, and produce a latency breakdown and mitigation. I would explicitly watch for blaming the model without measuring retrieval and tool time. Before moving on, I would confirm stable end-to-end latency percentiles. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 44: What would you do first if you were responsible for handling model latency spikes and discovered that users complain that AI responses are unpredictably slow?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the platform engineer early, capture the result in a latency breakdown and mitigation, and prioritize resolving the uncertainty that could cause blaming the model without measuring retrieval and tool time. I would consider the task complete when we have stable end-to-end latency percentiles.

---

## Question 45: During handling model latency spikes, what are the most important questions you would ask because users complain that AI responses are unpredictably slow?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the platform engineer needs from us. The questions should help us create a latency breakdown and mitigation and avoid blaming the model without measuring retrieval and tool time, not simply collect information for its own sake.

---

## Question 46: How would you prioritize handling model latency spikes against other work if users complain that AI responses are unpredictably slow?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create blaming the model without measuring retrieval and tool time or block a major dependency, it moves up the queue. I would make that reasoning visible to the platform engineer, time-box lower-value exploration, and define a concrete next checkpoint around stable end-to-end latency percentiles.

---

## Question 47: What trade-offs would you consider while doing handling model latency spikes when users complain that AI responses are unpredictably slow?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a latency breakdown and mitigation, make blaming the model without measuring retrieval and tool time explicit, and align with the platform engineer on what we are intentionally deferring.

---

## Question 48: How would you communicate progress or a blocker related to handling model latency spikes to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of blaming the model without measuring retrieval and tool time, show what we are doing with the platform engineer, and point to the next measurable checkpoint: stable end-to-end latency percentiles.

---

## Question 49: How would you collaborate with the platform engineer during handling model latency spikes?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a latency breakdown and mitigation as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in stable end-to-end latency percentiles instead of an unresolved discussion.

---

## Question 50: How would you know whether your work on handling model latency spikes was successful?

**Answer:** I would define success before completing the task. The primary signal would be stable end-to-end latency percentiles. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a latency breakdown and mitigation exists but the team is still exposed to blaming the model without measuring retrieval and tool time, I would not consider the work finished.

---

## Question 51: Tell me about a time you handled something similar to handling model latency spikes. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the platform engineer, what trade-off you made, and how you avoided or reduced blaming the model without measuring retrieval and tool time. Finish with a measurable result such as stable end-to-end latency percentiles, plus what you learned and would reuse in the next deployment.

---

## Question 52: Walk me through how you would handle designing agent tool permissions in your day-to-day FDE work when the agent can both read and modify customer systems.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the security engineer, and produce a least-privilege tool policy. I would explicitly watch for allowing the model to execute high-impact actions without guardrails. Before moving on, I would confirm safe authorization and approval boundaries. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 53: What would you do first if you were responsible for designing agent tool permissions and discovered that the agent can both read and modify customer systems?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the security engineer early, capture the result in a least-privilege tool policy, and prioritize resolving the uncertainty that could cause allowing the model to execute high-impact actions without guardrails. I would consider the task complete when we have safe authorization and approval boundaries.

---

## Question 54: During designing agent tool permissions, what are the most important questions you would ask because the agent can both read and modify customer systems?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the security engineer needs from us. The questions should help us create a least-privilege tool policy and avoid allowing the model to execute high-impact actions without guardrails, not simply collect information for its own sake.

---

## Question 55: How would you prioritize designing agent tool permissions against other work if the agent can both read and modify customer systems?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create allowing the model to execute high-impact actions without guardrails or block a major dependency, it moves up the queue. I would make that reasoning visible to the security engineer, time-box lower-value exploration, and define a concrete next checkpoint around safe authorization and approval boundaries.

---

## Question 56: What trade-offs would you consider while doing designing agent tool permissions when the agent can both read and modify customer systems?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a least-privilege tool policy, make allowing the model to execute high-impact actions without guardrails explicit, and align with the security engineer on what we are intentionally deferring.

---

## Question 57: How would you communicate progress or a blocker related to designing agent tool permissions to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of allowing the model to execute high-impact actions without guardrails, show what we are doing with the security engineer, and point to the next measurable checkpoint: safe authorization and approval boundaries.

---

## Question 58: How would you collaborate with the security engineer during designing agent tool permissions?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a least-privilege tool policy as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in safe authorization and approval boundaries instead of an unresolved discussion.

---

## Question 59: How would you know whether your work on designing agent tool permissions was successful?

**Answer:** I would define success before completing the task. The primary signal would be safe authorization and approval boundaries. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a least-privilege tool policy exists but the team is still exposed to allowing the model to execute high-impact actions without guardrails, I would not consider the work finished.

---

## Question 60: Tell me about a time you handled something similar to designing agent tool permissions. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the security engineer, what trade-off you made, and how you avoided or reduced allowing the model to execute high-impact actions without guardrails. Finish with a measurable result such as safe authorization and approval boundaries, plus what you learned and would reuse in the next deployment.

---

## Question 61: Walk me through how you would handle reviewing prompt changes in your day-to-day FDE work when a small instruction change improves one workflow but may regress others.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the AI engineer, and produce an evaluation-backed prompt release. I would explicitly watch for shipping prompt edits without regression testing. Before moving on, I would confirm quality improvement without unacceptable regressions. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 62: What would you do first if you were responsible for reviewing prompt changes and discovered that a small instruction change improves one workflow but may regress others?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the AI engineer early, capture the result in an evaluation-backed prompt release, and prioritize resolving the uncertainty that could cause shipping prompt edits without regression testing. I would consider the task complete when we have quality improvement without unacceptable regressions.

---

## Question 63: During reviewing prompt changes, what are the most important questions you would ask because a small instruction change improves one workflow but may regress others?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the AI engineer needs from us. The questions should help us create an evaluation-backed prompt release and avoid shipping prompt edits without regression testing, not simply collect information for its own sake.

---

## Question 64: How would you prioritize reviewing prompt changes against other work if a small instruction change improves one workflow but may regress others?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create shipping prompt edits without regression testing or block a major dependency, it moves up the queue. I would make that reasoning visible to the AI engineer, time-box lower-value exploration, and define a concrete next checkpoint around quality improvement without unacceptable regressions.

---

## Question 65: What trade-offs would you consider while doing reviewing prompt changes when a small instruction change improves one workflow but may regress others?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in an evaluation-backed prompt release, make shipping prompt edits without regression testing explicit, and align with the AI engineer on what we are intentionally deferring.

---

## Question 66: How would you communicate progress or a blocker related to reviewing prompt changes to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of shipping prompt edits without regression testing, show what we are doing with the AI engineer, and point to the next measurable checkpoint: quality improvement without unacceptable regressions.

---

## Question 67: How would you collaborate with the AI engineer during reviewing prompt changes?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use an evaluation-backed prompt release as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in quality improvement without unacceptable regressions instead of an unresolved discussion.

---

## Question 68: How would you know whether your work on reviewing prompt changes was successful?

**Answer:** I would define success before completing the task. The primary signal would be quality improvement without unacceptable regressions. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If an evaluation-backed prompt release exists but the team is still exposed to shipping prompt edits without regression testing, I would not consider the work finished.

---

## Question 69: Tell me about a time you handled something similar to reviewing prompt changes. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the AI engineer, what trade-off you made, and how you avoided or reduced shipping prompt edits without regression testing. Finish with a measurable result such as quality improvement without unacceptable regressions, plus what you learned and would reuse in the next deployment.

---

## Question 70: Walk me through how you would handle monitoring AI cost in your day-to-day FDE work when usage is growing faster than expected.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the FinOps partner, and produce a cost-per-task dashboard. I would explicitly watch for optimizing token cost without considering task success. Before moving on, I would confirm sustainable cost tied to business value. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 71: What would you do first if you were responsible for monitoring AI cost and discovered that usage is growing faster than expected?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the FinOps partner early, capture the result in a cost-per-task dashboard, and prioritize resolving the uncertainty that could cause optimizing token cost without considering task success. I would consider the task complete when we have sustainable cost tied to business value.

---

## Question 72: During monitoring AI cost, what are the most important questions you would ask because usage is growing faster than expected?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the FinOps partner needs from us. The questions should help us create a cost-per-task dashboard and avoid optimizing token cost without considering task success, not simply collect information for its own sake.

---

## Question 73: How would you prioritize monitoring AI cost against other work if usage is growing faster than expected?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create optimizing token cost without considering task success or block a major dependency, it moves up the queue. I would make that reasoning visible to the FinOps partner, time-box lower-value exploration, and define a concrete next checkpoint around sustainable cost tied to business value.

---

## Question 74: What trade-offs would you consider while doing monitoring AI cost when usage is growing faster than expected?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a cost-per-task dashboard, make optimizing token cost without considering task success explicit, and align with the FinOps partner on what we are intentionally deferring.

---

## Question 75: How would you communicate progress or a blocker related to monitoring AI cost to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of optimizing token cost without considering task success, show what we are doing with the FinOps partner, and point to the next measurable checkpoint: sustainable cost tied to business value.

---

## Question 76: How would you collaborate with the FinOps partner during monitoring AI cost?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a cost-per-task dashboard as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in sustainable cost tied to business value instead of an unresolved discussion.

---

## Question 77: How would you know whether your work on monitoring AI cost was successful?

**Answer:** I would define success before completing the task. The primary signal would be sustainable cost tied to business value. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a cost-per-task dashboard exists but the team is still exposed to optimizing token cost without considering task success, I would not consider the work finished.

---

## Question 78: Tell me about a time you handled something similar to monitoring AI cost. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the FinOps partner, what trade-off you made, and how you avoided or reduced optimizing token cost without considering task success. Finish with a measurable result such as sustainable cost tied to business value, plus what you learned and would reuse in the next deployment.

---

## Question 79: Walk me through how you would handle handling low-confidence AI output in your day-to-day FDE work when the model is uncertain on a subset of important cases.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the operations lead, and produce a human-review or fallback policy. I would explicitly watch for forcing automation where quality is insufficient. Before moving on, I would confirm exceptions routed safely with feedback captured. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 80: What would you do first if you were responsible for handling low-confidence AI output and discovered that the model is uncertain on a subset of important cases?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the operations lead early, capture the result in a human-review or fallback policy, and prioritize resolving the uncertainty that could cause forcing automation where quality is insufficient. I would consider the task complete when we have exceptions routed safely with feedback captured.

---

## Question 81: During handling low-confidence AI output, what are the most important questions you would ask because the model is uncertain on a subset of important cases?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the operations lead needs from us. The questions should help us create a human-review or fallback policy and avoid forcing automation where quality is insufficient, not simply collect information for its own sake.

---

## Question 82: How would you prioritize handling low-confidence AI output against other work if the model is uncertain on a subset of important cases?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create forcing automation where quality is insufficient or block a major dependency, it moves up the queue. I would make that reasoning visible to the operations lead, time-box lower-value exploration, and define a concrete next checkpoint around exceptions routed safely with feedback captured.

---

## Question 83: What trade-offs would you consider while doing handling low-confidence AI output when the model is uncertain on a subset of important cases?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a human-review or fallback policy, make forcing automation where quality is insufficient explicit, and align with the operations lead on what we are intentionally deferring.

---

## Question 84: How would you communicate progress or a blocker related to handling low-confidence AI output to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of forcing automation where quality is insufficient, show what we are doing with the operations lead, and point to the next measurable checkpoint: exceptions routed safely with feedback captured.

---

## Question 85: How would you collaborate with the operations lead during handling low-confidence AI output?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a human-review or fallback policy as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in exceptions routed safely with feedback captured instead of an unresolved discussion.

---

## Question 86: How would you know whether your work on handling low-confidence AI output was successful?

**Answer:** I would define success before completing the task. The primary signal would be exceptions routed safely with feedback captured. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a human-review or fallback policy exists but the team is still exposed to forcing automation where quality is insufficient, I would not consider the work finished.

---

## Question 87: Tell me about a time you handled something similar to handling low-confidence AI output. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the operations lead, what trade-off you made, and how you avoided or reduced forcing automation where quality is insufficient. Finish with a measurable result such as exceptions routed safely with feedback captured, plus what you learned and would reuse in the next deployment.

---

## Question 88: Walk me through how you would handle refreshing enterprise knowledge in your day-to-day FDE work when source documents change weekly.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the content owner, and produce an ingestion and freshness process. I would explicitly watch for answering from stale indexed content. Before moving on, I would confirm traceable, timely knowledge updates. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 89: What would you do first if you were responsible for refreshing enterprise knowledge and discovered that source documents change weekly?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the content owner early, capture the result in an ingestion and freshness process, and prioritize resolving the uncertainty that could cause answering from stale indexed content. I would consider the task complete when we have traceable, timely knowledge updates.

---

## Question 90: During refreshing enterprise knowledge, what are the most important questions you would ask because source documents change weekly?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the content owner needs from us. The questions should help us create an ingestion and freshness process and avoid answering from stale indexed content, not simply collect information for its own sake.

---

## Question 91: How would you prioritize refreshing enterprise knowledge against other work if source documents change weekly?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create answering from stale indexed content or block a major dependency, it moves up the queue. I would make that reasoning visible to the content owner, time-box lower-value exploration, and define a concrete next checkpoint around traceable, timely knowledge updates.

---

## Question 92: What trade-offs would you consider while doing refreshing enterprise knowledge when source documents change weekly?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in an ingestion and freshness process, make answering from stale indexed content explicit, and align with the content owner on what we are intentionally deferring.

---

## Question 93: How would you communicate progress or a blocker related to refreshing enterprise knowledge to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of answering from stale indexed content, show what we are doing with the content owner, and point to the next measurable checkpoint: traceable, timely knowledge updates.

---

## Question 94: How would you collaborate with the content owner during refreshing enterprise knowledge?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use an ingestion and freshness process as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in traceable, timely knowledge updates instead of an unresolved discussion.

---

## Question 95: How would you know whether your work on refreshing enterprise knowledge was successful?

**Answer:** I would define success before completing the task. The primary signal would be traceable, timely knowledge updates. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If an ingestion and freshness process exists but the team is still exposed to answering from stale indexed content, I would not consider the work finished.

---

## Question 96: Tell me about a time you handled something similar to refreshing enterprise knowledge. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the content owner, what trade-off you made, and how you avoided or reduced answering from stale indexed content. Finish with a measurable result such as traceable, timely knowledge updates, plus what you learned and would reuse in the next deployment.

---

## Question 97: Walk me through how you would handle investigating an AI production regression in your day-to-day FDE work when quality drops after a model, retrieval, or prompt change.

**Answer:** I would first clarify the immediate objective and what decision needs to be made. Then I would gather the minimum evidence needed, work directly with the ML platform team, and produce a regression analysis. I would explicitly watch for changing multiple AI components at once. Before moving on, I would confirm isolated root cause and measured recovery. In day-to-day FDE work, the key is to create forward motion without hiding uncertainty.

---

## Question 98: What would you do first if you were responsible for investigating an AI production regression and discovered that quality drops after a model, retrieval, or prompt change?

**Answer:** My first step would be to avoid making the situation larger than necessary. I would establish what is known, what is unknown, who owns the missing information, and whether the issue blocks customer value or production safety. I would involve the ML platform team early, capture the result in a regression analysis, and prioritize resolving the uncertainty that could cause changing multiple AI components at once. I would consider the task complete when we have isolated root cause and measured recovery.

---

## Question 99: During investigating an AI production regression, what are the most important questions you would ask because quality drops after a model, retrieval, or prompt change?

**Answer:** I would ask questions that expose ownership, constraints, dependencies, evidence, failure modes, and the desired outcome. I would specifically ask what would make the current assumption false, how the issue affects users, what data can verify it, and what the ML platform team needs from us. The questions should help us create a regression analysis and avoid changing multiple AI components at once, not simply collect information for its own sake.

---

## Question 100: How would you prioritize investigating an AI production regression against other work if quality drops after a model, retrieval, or prompt change?

**Answer:** I would prioritize based on customer impact, production risk, dependency criticality, reversibility, and the amount of uncertainty removed. If delaying this work could create changing multiple AI components at once or block a major dependency, it moves up the queue. I would make that reasoning visible to the ML platform team, time-box lower-value exploration, and define a concrete next checkpoint around isolated root cause and measured recovery.

---

## Question 101: What trade-offs would you consider while doing investigating an AI production regression when quality drops after a model, retrieval, or prompt change?

**Answer:** I would compare speed, quality, operational risk, maintainability, customer value, and reversibility. The right answer is rarely the most sophisticated design; it is the smallest safe approach that achieves the required outcome. I would document the important trade-off in a regression analysis, make changing multiple AI components at once explicit, and align with the ML platform team on what we are intentionally deferring.

---

## Question 102: How would you communicate progress or a blocker related to investigating an AI production regression to the customer?

**Answer:** I would keep the update concise: current state, customer impact, evidence, decision needed, owner, and next action. I would not bury the issue in implementation detail or blame another team. I would explain the relevance of changing multiple AI components at once, show what we are doing with the ML platform team, and point to the next measurable checkpoint: isolated root cause and measured recovery.

---

## Question 103: How would you collaborate with the ML platform team during investigating an AI production regression?

**Answer:** I would establish who owns which decision, what inputs each side provides, and how we will validate the result. I would use a regression analysis as a shared working artifact rather than communicating only through meetings. I would surface assumptions early, agree on interfaces or acceptance criteria, and make sure the collaboration results in isolated root cause and measured recovery instead of an unresolved discussion.

---

## Question 104: How would you know whether your work on investigating an AI production regression was successful?

**Answer:** I would define success before completing the task. The primary signal would be isolated root cause and measured recovery. I would also check that the result did not create a new operational or security problem, that ownership is clear, and that the customer can act on the outcome. If a regression analysis exists but the team is still exposed to changing multiple AI components at once, I would not consider the work finished.

---

## Question 105: Tell me about a time you handled something similar to investigating an AI production regression. How should a strong FDE answer this behavioral question?

**Answer:** A strong answer should use a concrete story. Start with the customer or production context, explain why the situation mattered, and describe your personal responsibility. Show how you worked with a counterpart such as the ML platform team, what trade-off you made, and how you avoided or reduced changing multiple AI components at once. Finish with a measurable result such as isolated root cause and measured recovery, plus what you learned and would reuse in the next deployment.

---
