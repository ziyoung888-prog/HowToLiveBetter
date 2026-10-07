# Professional Interaction Skills — SWD/XWD Boundary Regression v2

## Purpose
Stress-test the three draft skills on cases where textbook advice can become harmful if applied mechanically.

Skills:
- workplace-transition
- workplace-communication
- negotiation

The emphasis in this round is boundary judgment:
- when not to negotiate
- when schedule pressure cannot override engineering risk
- when “keep dialogue safe” becomes too soft
- when interests are genuinely conflicting
- when a junior engineer should decide vs escalate

## Evidence handling
- Confirmed: explicitly recovered from prior SWD/XWD conversation/project context.
- Partial: real case exists, but not all original dialogue is available.
- Simulated branch: a controlled counterfactual built from a real case to test decision boundaries.
No missing dialogue is invented as factual history.

---

## Case 9 — Leader gives a clear execution instruction
**Status:** Confirmed / partial transcript  
**Context:** 2026-09-21 SWD研发流程会议要求：研发在制作前完成生产规格；生产打样/批量需跟线到ATE、老化；前1–2套ATE由研发主责并提供BOM/图纸，后续由NPI复制；冲突找曾经理沟通；缺物料延迟由项目定责；研发不到现场则定责。会议纪要口径是“请大家执行”。

### Boundary question
Should the user continue “negotiating interests” after a clear management/process decision?

### Correct routing
Primary: workplace-transition  
Secondary: workplace-communication  
Negotiation: **off by default**

### Expected judgment
If:
- the instruction is within normal authority,
- no safety/compliance/technical impossibility is identified,
- ownership and requirement are sufficiently clear,

then the default is execution, not reopening the decision.

Appropriate action:
1. clarify only operational ambiguity
2. convert instruction into checklist and personal action items
3. identify dependencies
4. execute
5. raise exceptions only with evidence

### Failure mode to avoid
Using “focus on interests” as a pretext to re-litigate a settled management decision.

### Exception
Escalate or reopen only if:
- instruction conflicts with safety / regulation / formal standard
- technically impossible under known constraints
- creates an unowned critical risk
- two authoritative instructions conflict

### Verdict
**PASS only if negotiation skill is explicitly suppressed after authority/decision finality is established.**

### New rule
“Decision finality gate”: before activating negotiation, determine whether the issue is still open for negotiation.

---

## Case 10 — Schedule pressure vs technical risk
**Status:** Confirmed context + simulated branch  
**Context:** V-Li10, 6C-85Ah and 10C-42U had explicit near-term milestones. The user owned V-Li10 wiring-diagram changes while BOM control and design optimization depended on resource coordination. Manufacturing training material also emphasizes BOM freeze timing and preventing downstream line stoppage.

### Boundary question
If a project milestone is urgent but a connector/terminal/interface remains unconfirmed, should the user “be cooperative” and release anyway?

### Correct routing
Primary: workplace-transition  
Secondary: workplace-communication  
Negotiation: only for schedule/resource tradeoffs, **not for technical acceptance**

### Expected judgment
Split the problem:
- fixed technical requirement / safety condition
- schedule preference
- reversibility of release
- downstream impact

Recommended behavior:
1. identify whether the unknown affects safety, correctness, manufacturability, or only cosmetic/detail completeness
2. if critical: do not silently release as final
3. offer bounded alternatives:
   - release as draft/preliminary
   - mark TBD explicitly
   - freeze unaffected sections
   - create a deviation/temporary-control path if process permits
4. state milestone impact factually
5. ask decision owner to choose among valid options

### Failure mode to avoid
Converting schedule pressure into undocumented technical debt.

### Verdict
**PASS, but communication must not “soften” a critical technical unknown into ambiguous wording.**

### New rule
“Risk class before schedule”: classify the unresolved issue before discussing delivery timing.

---

## Case 11 — Apparent responsibility shifting
**Status:** Confirmed / partial  
**Context:** In SWD manufacturing/process discussion, missing-material delay is assigned by project, and absence of R&D at required production follow-up can be attributed to R&D. In external-test work, test, supplier, project and engineering each own different inputs.

### Boundary question
If another function says “这个应该是你们研发给的” or pushes a problem back, should the user prioritize relationship safety?

### Correct routing
Primary: workplace-communication  
Secondary: workplace-transition  
Negotiation: sometimes

### Expected judgment
Do not jump to accusation (“甩锅”), but do not absorb undefined responsibility either.

Use:
1. identify task/output
2. identify required input
3. identify process or prior agreement
4. map owner
5. state current gap
6. propose closure

Example structure:
“这个测试条件里的应用工况由研发侧提供，我这边可以补齐；具体采样方式和设备配置需要测试侧确认。我们先按这个分工把缺口列一下，避免来回转。”

If ownership is disputed:
- cite process, meeting minutes, task assignment, or document owner
- escalate ownership ambiguity to the decision owner

### Failure mode to avoid
“为了关系好”把所有任务都接下，形成长期责任漂移。

### Verdict
**PASS after adding a boundary rule: respect does not equal accepting unowned work.**

### New rule
“Relationship safety cannot override role clarity.”

---

## Case 12 — Supplier interests genuinely conflict with ours
**Status:** Confirmed technical context + simulated branch  
**Context:** For contactor/fuse validation, the company wants evidence under actual and worst-case conditions; the supplier may prefer narrower scope, existing standard reports, fewer destructive tests, lower cost and lower liability. The system side may care about 512V/430A temperature rise, surge life, 4kA/6kA breaking, and failure mode.

### Boundary question
Does “win-win” always exist?

### Correct routing
Primary: negotiation  
Secondary: workplace-communication

### Expected judgment
No. Some interests are structurally conflicting:
- we want stronger evidence
- supplier wants lower test burden / liability
- destructive testing consumes samples and budget

The goal is not forced harmony. The goal is a defensible agreement or a clean no-agreement decision.

Recommended sequence:
1. identify minimum evidence required for engineering decision
2. ask which evidence already exists
3. define non-negotiable technical minimum
4. negotiate only the flexible dimensions:
   - sequence
   - sample allocation
   - evidence reuse
   - scope split
   - timing
   - cost-sharing / who performs
5. if minimum evidence cannot be obtained, improve BATNA:
   - alternate supplier
   - independent test
   - redesign / derating
   - reject component for this use case

### Failure mode to avoid
Using “mutual gain” to rationalize accepting insufficient evidence.

### Verdict
**PASS if BATNA and minimum technical evidence are treated as real exit conditions.**

### New rule
“Win-win is optional; decision quality is mandatory.”

---

## Case 13 — Junior engineer: decide independently or escalate?
**Status:** Confirmed recurring context  
**Context:** User is an early-career system electrical engineer with mentor/manager support. Real tasks included test-plan drafting, BOM/drawing changes, supplier technical questions, component validation, and interpreting requirements.

### Boundary question
When should the user stop asking and make the call?

### Correct routing
Primary: workplace-transition  
Secondary: workplace-communication

### Decision test
Make the decision independently when most of the following are true:
- decision is within assigned scope
- reversible
- low safety/compliance impact
- low cost of correction
- acceptance criteria are known
- precedent/process exists
- downstream impact is contained

Escalate when any of the following is true:
- safety / compliance / certification implication
- irreversible or destructive test with limited samples
- external commitment to supplier/customer
- unclear authority or conflicting instructions
- large schedule/cost consequence
- requirement or acceptance criteria unclear
- decision crosses functions and no owner is established

For medium-risk cases:
- prepare a recommendation first, then ask for confirmation
- do not escalate a blank question

Preferred pattern:
“我目前判断A方案更合适，依据是1/2/3；风险是X。若没有其他约束，我准备按A执行。这里涉及Y，所以想请你确认一下。”

### Failure mode to avoid
Two extremes:
- student mode: everything asks the mentor
- overcompensation: making high-impact decisions to prove independence

### Verdict
**PASS with a new autonomy/escalation matrix.**

### New rule
“Escalate decisions, not thinking.”

---

# Boundary findings

## 1. Negotiation has an activation condition
Do not activate negotiation merely because another person is involved.
First check:
- Is the decision still open?
- Is there a legitimate trade space?
- Is the issue actually ownership, technical completeness, or authority?

## 2. Dialogue safety is not the highest value
For safety, compliance, quality, or technical correctness:
- clarity > comfort
- evidence > face-saving
- explicit ownership > vague harmony

Respect remains mandatory; substantive concession does not.

## 3. Urgency changes process, not physics
An urgent milestone may justify:
- faster review
- parallel work
- temporary status
- phased release
- explicit deviation path

It does not justify hiding an unresolved critical technical risk.

## 4. “甩锅” should be translated into an ownership question
Avoid motive language unless there is evidence.
Ask:
- what output?
- what input?
- whose process responsibility?
- who decides?

## 5. Independence should be risk-scaled
Junior engineers should decide more low-risk, reversible, in-scope matters.
High-impact uncertainty should be escalated with a prepared recommendation.

# Required skill changes
1. Add decision-finality gate before negotiation.
2. Add technical-risk class before schedule discussion.
3. Add role-clarity boundary to communication.
4. Add “minimum evidence / no-deal” rule to negotiation.
5. Add autonomy-escalation matrix to transition skill.

# Regression verdict v2
- workplace-transition: **PASS after autonomy + authority boundary additions**
- workplace-communication: **PASS after role-clarity + risk-clarity additions**
- negotiation: **PASS after activation gate + minimum-evidence/no-deal additions**

## Stable-release decision
Still **do not promote to v1.0 stable**.

Reason:
The skills have now passed retrospective/simulated regression, but at least three prospective live cases should be tracked from recommendation -> user action -> actual outcome.
