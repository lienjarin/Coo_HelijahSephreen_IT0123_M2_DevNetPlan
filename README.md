# IT0123 DevNet Resource Validation Plan

## Student and Project

- Name: Helijah Sephreen Tria Coo
- Section: TS31
- Repository name: `Coo_HelijahSephreen_IT0123_M2_DevNetPlan`

## Purpose

Explain in 2-3 sentences why selecting the correct DevNet resource matters before beginning a network-automation task.

Choosing the right DevNet resource before starting a network-automation task saves time keeps credentials safe and avoids setup work. Picking the environment such as reserving a sandbox for a task that only needed a shared one slows things down and uses up limited reservation slots that others might need. Checking the DevNet resource against Cisco documentation makes sure the plan is accurate, can be defended and repeated instead of relying on an unverified AI suggestion.

## Validated Resource Decisions

Summarize your four selections from `student_plan.json`. For each use case, state the selected resource, the most important requirement, and the official Cisco evidence used.

UC1
- Quick read-only API exploration: Selected Always-On Sandbox.
- The decisive requirement was immediate, shared, non-admin access with no time to wait for provisioning.
- https://developer.cisco.com/docs/sandbox/
  
UC2
- Private configuration testing: Selected Reservation Sandbox.
- The decisive requirement was private, administrative access with acceptable setup time and VPN use.
- https://developer.cisco.com/docs/sandbox/
  
UC3
- Guided API concept practice: Selected Learning Lab.
- The decisive requirement was structured, step-by-step instructional content for a beginner rather than a live device environment.
- https://developer.cisco.com/learning/
  
UC4
- Reusable automation example: Selected Cisco Code Exchange.
- The decisive requirement was browsing existing community and Cisco-maintained repositories before building a new solution.
- https://developer.cisco.com/codeexchange/

## AI Evaluation

Identify at least one AI recommendation that you accepted, rejected, or modified. Explain the evidence behind your decision.

The AI's recommendations were all accepted. Each one needed confirmation of the exact access model (shared or private, VPN or no VPN, admin or non-admin) instead of just trusting the resource name by itself. The AI-generated claims were fact-checked via the official Cisco Sandbox documentation before they were verified. For instance, the AIs assertion that Always‑On Sandboxes have restricted access was verified on the official Sandbox documentation page. That page states that Always‑On Sandboxes are shared among all users so administrative access is restricted.

## Validation Evidence

- Validator result: Validation Complete: 9/9 checks passed.
- Command used: python validate_plan.py
- Official Cisco pages reviewed:
  https://developer.cisco.com/docs/sandbox/
  https://developer.cisco.com/learning/
  https://developer.cisco.com/codeexchange/

## Git Evidence

- Initial commit message: Initial commit: add starter files and README
- Validation commit message:
  PASS: JSON file loaded
  PASS: student and AI disclosure completed
  PASS: all four scenario IDs present
  PASS: resource classifications match scenario requirements
  PASS: official Cisco evidence URLs supplied
  PASS: AI verification statuses are valid
  PASS: rationales are sufficiently detailed
  PASS: AI recommendations are summarized in the student's own words
  PASS: no credential-like fields detected
  VALIDATION COMPLETE: 9/9 checks passed.
- Output of `git log --oneline`:
  

## AI-Use Disclosure

State the AI tool used, the type of assistance received, what was independently checked, and what you revised.

Claude AI was used for this activity as tasked. It was asked to recommend one DevNet resource type (learning-lab, always-on-sandbox, reservation-sandbox, or code-exchange), state the deciding requirement, and flag an access/isolation/privilege claim to verify. Moreover, every claim, about the access model, sharing, administrative privileges, VPN requirement and setup time was verified using the Cisco DevNet Sandbox, Learning Labs and Code Exchange documentation pages before being accepted. No claims required changing. 
