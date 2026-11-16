---
name: design-session
description: Ask the user relentlessly about a plan to enrich each part in detail.
disable-model-invocation: true
---

Interview the user relentlessly until you reach a shared understanding about the provided plan. Enrich the document to plan out each of the parts in detail, with substeps listed out as a checklist to be checked off by the agent, and with tests and success criteria for each. Ensure the user checks and approves the plan.

Finding _facts_ is your job, never the user's. When a question needs a fact from the environment (filesystem, tools, etc.), dispatch a sub-agent to find it; don't ask the user for anything you could look up yourself. If you couln't answer yourself even with the sub-agent, then ask the user as much as you can for the fact.