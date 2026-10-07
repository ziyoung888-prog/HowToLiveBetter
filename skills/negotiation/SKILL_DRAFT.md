# Negotiation Skill

## Purpose
Use this skill for workplace negotiation and coordination where parties have partly shared and partly conflicting interests. It is distilled primarily from Fisher, Ury, and Patton’s *Getting to Yes* and adapted for engineering, supplier, project, resource, and career contexts.

## Core principle
Avoid positional bargaining where possible. Negotiate on the merits.

The four core elements are:
1. Separate the people from the problem.
2. Focus on interests, not positions.
3. Invent options for mutual gain.
4. Insist on objective criteria.

## Trigger conditions
Invoke when:
- Negotiating supplier test scope, data, samples, cost, lead time, warranty, or responsibility.
- Negotiating internal resources, schedule, test slots, ownership, or deliverables.
- Discussing salary, role scope, training commitments, or relocation.
- Two functions are stuck on incompatible stated positions.
- The other side has more power.
- The other side refuses to engage constructively.
- Pressure, threats, deadlines, or dubious tactics are being used.

## Decision flow

### 1. Diagnose positions and interests
For each side, write:
- Position: what they say they want.
- Interests: why they want it.
- Constraints: what they cannot easily change.
- Risks: what they are trying to avoid.
- Decision process: who actually approves.

Do not treat a stated position as the underlying need.

### 2. Separate people from problem
Treat relationship and substance as two distinct workstreams.

Ask:
- Is the disagreement caused by perception?
- Emotion?
- Communication?
- Actual substantive conflict?

Deal with people problems directly rather than paying for them through substantive concessions.

### 3. Build your BATNA
Before negotiating, identify your Best Alternative To a Negotiated Agreement.

Define:
- What will I do if no agreement is reached?
- What alternatives can I improve before negotiating?
- What is the cost of no agreement?
- What is the other side’s likely BATNA?

Do not negotiate from a vague “bottom line” alone. A stronger BATNA increases practical leverage.

### 4. Generate options before choosing
Do not force the discussion into one binary solution too early.

Generate:
- scope alternatives
- sequence alternatives
- conditional agreements
- pilot/test-first options
- phased delivery
- data-sharing options
- ownership splits
- timing trades
- low-cost/high-value exchanges

Look for differences that can be dovetailed: different priorities, forecasts, risk tolerance, timing needs, capabilities, or preferences.

### 5. Use objective criteria
Where interests conflict, move the discussion to independent standards such as:
- contract terms
- specifications
- standards
- test methods
- market benchmarks
- comparable quotes
- expert judgment
- historical data
- engineering calculations
- documented process requirements

Be open to reason, but do not yield merely to pressure.

### 6. Make the other side’s “yes” workable
A proposal must be executable from the other side’s perspective.

Ask:
- Who inside their organization must approve?
- What criticism will they receive if they accept?
- What evidence do they need?
- What can I offer that is low-cost to me but valuable to them?

Turn ideas into a “yesable proposition”: specific enough that a simple yes could lead to operational execution.

### 7. Handle stronger counterparts
If the other side has more power:
- improve BATNA
- lower dependence
- build alternatives
- use objective standards
- avoid commitments made under pressure without review
- distinguish legitimate consequence from threat

Power is not only authority; alternatives, information, legitimacy, timing, relationships, and process control also matter.

### 8. If they won’t play
Use negotiation jujitsu:
- do not attack their position
- look behind it for interests
- do not defend your idea reflexively; invite criticism
- turn personal attack into an attack on the problem
- ask questions instead of making counterattacks
- use silence deliberately after a substantive question

If necessary, involve a neutral third party or use a one-text process: circulate a draft, collect criticism, revise repeatedly, and converge on one working text.

### 9. Handle pressure and questionable tactics
When facing pressure:
- identify the tactic explicitly if useful
- return discussion to process and criteria
- verify authority, deadlines, and claims
- separate warnings from threats
- pause if needed rather than making a reactive concession

Default principle: yield to reason and principle, not pressure.

## Engineering workplace adaptations

### Supplier test negotiation
Do not argue:
“We need all these tests.”
Instead clarify interests:
- Engineering: evidence that component works under actual and worst-case conditions.
- Supplier: bounded scope, cost, lead time, liability.
- Testing: measurable parameters, setup, acquisition, pass/fail criteria.

Then create options:
- supplier shares existing reports first
- gap analysis
- only missing conditions are retested
- test order by risk
- agreed failure criteria and sample count

### Internal resource negotiation
Position conflict:
“We need the lab this week” vs “No slots.”

Translate to interests:
- critical milestone
- duration
- equipment dependency
- sequencing flexibility
- business consequence

Then propose alternatives:
- shorter first-pass test
- night/off-peak slot
- split test sequence
- alternate equipment
- exchange priority on another task

### Salary or offer negotiation
Build:
- target
- BATNA
- evidence
- package dimensions
- non-cash tradeoffs
- walk-away conditions

Use market and role evidence rather than personal need as the primary criterion.

## Output format when invoked
1. Negotiation objective
2. Your position vs interests
3. Their likely position vs interests
4. BATNA on both sides
5. Leverage map
6. Objective criteria
7. Option set
8. Recommended opening
9. Concession strategy
10. Walk-away / escalation conditions
11. Suggested wording

## Guardrails
- Do not assume every interaction is a negotiation.
- Do not trade technical safety, compliance, or quality requirements for relationship comfort.
- Do not expose sensitive bottom-line information unnecessarily.
- Do not confuse “win-win” with always splitting the difference.
- Do not accept arbitrary deadlines without checking whether they are real constraints.
- Do not recommend bluffing where credibility or long-term reputation matters.
- Relationship value matters, but it should not silently override substantive risk.


## Regression additions from SWD/XWD cases

### Do not negotiate before the engineering input exists
A negotiation skill cannot repair an undefined technical requirement.

Before supplier/test-scope negotiation, ensure the application side has defined:
- operating condition
- abnormal / worst-case condition
- voltage/current/time or equivalent key parameters
- required evidence
- pass/fail intent
- sample constraints if known

Then negotiate scope, sequence, evidence reuse, cost, lead time, and ownership.

### Supplier evidence gap workflow
When asking a supplier for validation:
1. list the decision-critical conditions
2. ask what existing reports already cover
3. map evidence gaps
4. request only missing tests where possible
5. agree on conditions, samples, measurements, and failure criteria
6. record unresolved items and owners

This avoids asking for “all tests” without prioritization.

### Responsibility interface model
For technical negotiation distinguish:
- project/engineering: application inputs and risk scenarios
- supplier: product limits, historical reports, recommended constraints
- test function: executable method, instrumentation, acquisition
- decision owner: final acceptance / release decision

Many apparent negotiation conflicts are actually ownership-interface ambiguity.

### Priority response pattern
If the other side asks “what do you care about?”, answer:
1. top decision needs
2. why they matter
3. existing evidence you want to reuse
4. remaining gaps

Do not respond with an undifferentiated checklist.


## Boundary rules from SWD/XWD regression v2

### Negotiation activation gate
Before using negotiation tactics, determine:
- Is the decision still open?
- Is there genuine trade space?
- Is this actually a technical-definition, ownership, or authority issue?

If there is no legitimate trade space, do not manufacture one.

### Minimum technical evidence / no-deal condition
Before negotiating flexible terms, define the minimum evidence required to make the engineering decision.

Flexible dimensions may include:
- sequence
- sample allocation
- reuse of existing reports
- timing
- cost
- who performs the test

Non-negotiable dimensions may include:
- required safety evidence
- applicable operating/worst-case condition
- pass/fail basis
- critical failure-mode visibility

If minimum evidence cannot be obtained, use BATNA rather than forcing agreement.

### Win-win is optional
Some interests genuinely conflict. The objective is a defensible decision, not artificial harmony.

If the counterpart cannot or will not satisfy the minimum requirement, valid outcomes include:
- independent test
- alternate supplier
- redesign / derating
- reject component for the use case
- escalate for a conscious risk decision
