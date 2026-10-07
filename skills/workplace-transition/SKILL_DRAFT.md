# workplace-transition Skill Draft

## Positioning
A practical transition skill for early-career engineers entering or adapting to a new technical role. Based primarily on Michael Watkins, *The First 90 Days*, but adapted away from executive/manager assumptions toward individual-contributor engineering work.

## When to invoke
- New job / new team / new manager / new project
- Unclear expectations from manager
- Need to ramp up quickly in unfamiliar product/domain
- Need to establish credibility without overpromising
- Need to coordinate across testing, project, supplier, quality, structure, manufacturing, etc.
- Need to diagnose whether to observe, learn, act, escalate, or deliver an early win

## Core decision flow
1. Clarify transition type
   - New company / new team / new manager / new technical domain / new project
   - Internal promotion vs lateral move
2. Define success conditions
   - What outputs will matter in 30/60/90 days?
   - Who evaluates success?
   - What failure modes matter most?
3. Accelerate learning
   - Product/system architecture
   - Process and standards
   - Stakeholders and informal network
   - Historical failures / recurring issues
   - Decision rights and escalation paths
4. Align with manager
   - Expectations
   - Priorities
   - Working style
   - Communication cadence
   - Resource constraints
5. Select early wins
   - Visible enough to build credibility
   - Valuable to team
   - Low-to-moderate execution risk
   - Does not create hidden technical debt
6. Build stakeholder map
   - Who owns what?
   - Who can block progress?
   - Who has information?
   - Who needs advance notice?
7. Maintain balance
   - Avoid trying to prove yourself by accepting every task
   - Protect learning time
   - Track open loops and risks
   - Escalate ambiguity before it becomes failure

## High-value principles adapted for an engineering IC

### 1. Transition starts with role reset
Do not assume behaviors that worked at university, in internships, or in a previous team will automatically transfer. Identify what the new role rewards: technical correctness, execution speed, risk control, communication, ownership, or cross-functional coordination.

### 2. Learning is a deliverable
Learning should produce artifacts, not just understanding:
- system block diagram
- interface map
- test checklist
- decision log
- issue list
- stakeholder map
- standard/specification index

### 3. Manager alignment must remove ambiguity
For important work, establish:
- objective
- scope
- deadline
- decision owner
- expected output format
- acceptance criteria
- update cadence

### 4. Early wins should create trust, not theater
Good early wins are useful, visible, and low-regret. Avoid flashy changes before understanding the system.

### 5. Relationships are part of engineering execution
Treat testing, supplier, project, quality, manufacturing, and other functions as stakeholders. Understand incentives, information needs, and response latency.

### 6. Escalate unresolved ambiguity
Ambiguity around objectives, acceptance criteria, ownership, or constraints is a project risk. Surface it early and neutrally.

## Output format when invoked
Provide:
1. Current transition diagnosis
2. Confirmed facts vs assumptions
3. Main risks
4. 30/60/90-day priorities or next-step plan
5. Manager alignment actions
6. Stakeholder actions
7. One or two early-win candidates
8. What not to do
9. Suggested wording for key communication if relevant

## Chapter relevance from The First 90 Days

### High priority now
- Chapter 2: Accelerate Your Learning
- Chapter 4: Secure Early Wins
- Chapter 5: Negotiate Success
- Chapter 8: Create Coalitions
- Chapter 9: Keep Your Balance

### Medium priority
- Chapter 1: Promote Yourself — reinterpret as role/identity transition, not self-promotion
- Chapter 3: Match Strategy to Situation — useful for diagnosing project/team context
- Chapter 6: Achieve Alignment — use selectively for understanding organization/process interfaces

### Lower priority for current stage
- Chapter 7: Build Your Team
- Chapter 10: Expedite Everyone
These become more relevant after taking formal leadership responsibility.

## Guardrails
- Do not apply executive-management advice mechanically to an individual contributor.
- Do not recommend organizational change before sufficient learning.
- Do not confuse visibility with value.
- Do not treat all manager preferences as correct; distinguish preference from technical/safety requirements.
- For technical, legal, financial, or compliance decisions, use authoritative sources separately; this skill only structures transition behavior.


## Regression additions from SWD/XWD cases

### Engineering completeness gate
Before treating a problem as a communication problem, check whether the underlying engineering deliverable is executable.

For test requests, drawings, BOM changes, supplier questions, and design reviews, verify:
- design/test input is defined
- conditions and boundaries are explicit
- acceptance criteria exist
- unknowns are marked TBD
- each TBD has an owner

If the content is incomplete, fix the engineering input before polishing wording.

### Evidence maturity labels
Use explicit maturity states:
- Confirmed
- Preliminary proposal
- TBD
- Awaiting owner confirmation

Do not present preliminary thinking as an approved design decision.

### Four-owner model
For cross-functional work, identify:
- Input owner — supplies application/design conditions
- Evidence owner — supplies data/reports/technical proof
- Execution owner — performs the task/test/change
- Decision owner — accepts the result or chooses the path

One person may hold multiple roles, but do not leave them implicit.

### Review-to-system rule
After a review, convert recurring comments into a checklist or template. Correcting only the current document is insufficient learning.

### Dependency-oriented status
Progress updates should include:
1. current status
2. blocker / open item
3. next action
4. ETA or milestone impact
