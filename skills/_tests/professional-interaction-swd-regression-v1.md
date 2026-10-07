# Professional Interaction Skills — SWD/XWD Regression Test v1

## Purpose
Use real past SWD/XWD work cases to test three draft skills:
- workplace-transition
- workplace-communication
- negotiation

The goal is not to prove the books are right. The goal is to test whether the skills produce useful, low-risk actions in actual engineering work.

## Evidence rule
Each case is marked as:
- Confirmed: explicitly recovered from past conversation/project context.
- Partial: enough context to test the skill, but not a complete verbatim transcript.
- Not reconstructed: do not invent missing dialogue.

---

## Case 1 — External test request rejected as “not detailed enough”
**Status:** Confirmed  
**Context:** 肖工负责外发测试。早期需求只写到类似“512 VDC / 430 A，温升测试”，肖工反馈需求不够详细，不能直接外发。后续需要补充样品、安装、接线、环境、施加条件、测点、采样、结束条件、判据、报告要求等。

### Routing
Primary: workplace-transition  
Secondary: workplace-communication  
Negotiation: not primary yet

### What the skills should diagnose
This is not mainly a “communication attitude” problem. It is an engineering deliverable-definition problem.

The user had a goal (“做温升测试”) but had not converted it into an executable test specification.

### Expected recommendation
Before messaging testing:
1. define DUT/sample
2. define setup and installation
3. define input conditions
4. define measurement points
5. define sampling / waveform / logging
6. define duration and stop condition
7. define pass/fail criteria
8. define report output
9. mark unknowns as TBD with owner

### Result
**PASS with modification required.**

The existing skills correctly emphasize acceptance criteria, facts, ownership and action, but they underweight “technical completeness before communication.”

### Rule learned
For engineering coordination, never diagnose a rejected request as merely “表达不清楚” until checking whether the underlying engineering input is actually complete.

---

## Case 2 — Supplier manager asks “您这边比较看重的是？”
**Status:** Confirmed  
**Context:** In the 良信&能源科技 technical group, 李文博经理 asked “您这边比较看重的是？”. The response focus was 600H product capability plus actual application conditions: 512V/430A temperature rise and breaking life, repeated surge-current life, 4kA/6kA short-circuit breaking count and final failure mode.

### Routing
Primary: negotiation  
Secondary: workplace-communication

### What the skills should diagnose
The supplier is asking for priority, not a full technical specification yet.

A weak answer would dump every possible test item.
A better answer separates:
- product intrinsic evidence
- application-specific evidence
- high-priority unknowns

### Expected recommendation
Reply in three layers:
1. what matters most
2. why it matters in the system
3. what existing evidence can be shared before requesting new tests

### Result
**PASS.**

The negotiation skill’s “interests, objective criteria, make yes workable” fits well.

### Rule learned
When a supplier asks “what do you care about?”, answer with prioritized decision needs, not a raw checklist.

---

## Case 3 — Supplier group has no reply after the technical response
**Status:** Confirmed  
**Context:** After the above reply, the group had no response by the next day.

### Routing
Primary: workplace-communication  
Secondary: negotiation

### What the skills should diagnose
“No reply” is not evidence of refusal, disrespect, or bad faith.

The real question is whether there is a dependency and deadline.

### Expected recommendation
Use a follow-up ladder:
1. no deadline / low urgency -> wait reasonable time
2. dependency exists -> follow up with concrete ask
3. milestone at risk -> state impact and requested response time
4. still no response -> switch channel or ask the owner/manager for coordination
5. escalate only with factual dependency, not emotion

Example pattern:
“李经理，补充确认一下，上面几项主要是为了收敛6C实际工况下的验证缺口。麻烦帮忙看下现有报告能覆盖哪些，哪些需要补测；如果方便，今天/明天给个初步结论即可，我们这边好继续整理测试需求。”

### Result
**PASS with modification required.**

The current skill says to separate non-response from motive, which is correct. It needs a clearer escalation ladder.

### Rule learned
Silence is a workflow state, not a personality judgment.

---

## Case 4 — Reporting the fuse test plan to the manager
**Status:** Confirmed  
**Context:** Only two fuse samples were available. Initial thinking: both samples first do temperature-rise and surge-life testing, then one sample does minimum breaking and one does maximum breaking. User wanted to state clearly that this was a personal preliminary plan and would be checked with 李亮 / reviewed later.

### Routing
Primary: workplace-communication  
Secondary: workplace-transition

### What the skills should diagnose
A junior engineer should not present an unreviewed draft as an approved test plan.

But excessive self-deprecation (“我不懂”“只是我瞎想”) weakens credibility.

### Expected recommendation
Use:
- current known facts
- preliminary proposal
- uncertainty / open item
- who will verify
- next checkpoint

Good pattern:
“目前只有2只样品。我的初步安排是两只先做温升和冲击寿命，再分别做最小/最大分断。这个顺序目前还是初步方案，我准备再和李亮核一下，后续评审时把具体参数和顺序一起确认。”

### Result
**PASS.**

### Rule learned
Junior status should be expressed through evidence maturity, not through self-devaluation.

Use “初步方案 / 待确认 / 已确认” instead of “我觉得 / 我不太懂 / 可能是吧”.

---

## Case 5 — System conditions vs supplier parameters
**Status:** Confirmed  
**Context:** In fuse testing, questions arose about whether surge parameters and short-circuit test voltage should be provided by the project side or supplier side. The mature resolution was: application/system conditions are project inputs; supplier assesses component applicability and may provide product limits / historical evidence.

### Routing
Primary: negotiation  
Secondary: workplace-transition

### What the skills should diagnose
This is an ownership/interface problem.

### Expected recommendation
Split responsibility:
- Project/engineering owns actual application and worst-case conditions.
- Supplier owns product limits, capability evidence, recommended setup constraints.
- Test side owns executable test method and measurement implementation.
- Final test plan is jointly closed.

### Result
**PASS with modification required.**

Current skills mention ownership, but need an explicit “input-owner / evidence-owner / execution-owner / decision-owner” model.

### Rule learned
In engineering collaboration, many arguments are actually interface-definition failures.

---

## Case 6 — Forwarding a technical answer from mentor to another colleague
**Status:** Partial but sufficient  
**Context:** A project colleague raised a question; the user asked mentor 张工, then needed to relay the answer and worried about transmitting incorrect information. Another recovered example: 彭磊 questioned why a low-capacity 314A cell was being requested; 张工 clarified that home-storage and network-energy product lines differ and the user should clearly state “你是网能的”.

### Routing
Primary: workplace-communication  
Secondary: workplace-transition

### What the skills should diagnose
Risk arises when the messenger converts a mentor’s statement into a stronger claim than was actually confirmed.

### Expected recommendation
Use a relay protocol:
1. distinguish direct fact from your interpretation
2. preserve qualifiers
3. attribute when appropriate
4. if decision-critical, ask the original owner to confirm
5. do not add causal explanation you were not given

Example:
“我刚和张工确认了，这个是网能产品线的需求，不是家储那边。85Ah电芯用于融捷85Ah项目样机，所以需要新增物料编码。申请字段如果还有不规范的地方我再按要求调整。”

### Result
**PASS with modification required.**

### Rule learned
When relaying technical information, fidelity is more important than sounding authoritative.

---

## Case 7 — 10C test-case review exposed design weaknesses
**Status:** Partial  
**Context:** 9/6 test-case review produced lessons around case structure, abnormal handling, and judgment criteria. The user wanted these lessons turned into guidance for independently designing future product test cases.

### Routing
Primary: workplace-transition  
Secondary: workplace-communication

### What the skills should diagnose
A review comment is not just “领导否定方案”; it is training data about the organization’s quality bar.

### Expected recommendation
For every review comment, classify:
- missing input
- missing condition
- missing procedure
- missing acquisition
- missing expected result
- missing pass/fail criterion
- missing abnormal handling
- missing traceability/configuration

Then convert recurring findings into a reusable checklist.

### Result
**PASS.**

### Rule learned
Feedback should become process assets. A corrected document without a new checklist is only local repair.

---

## Case 8 — V-Li10 / BOM / drawing schedule coordination
**Status:** Partial  
**Context:** Around 9/16, internal coordination covered 6C-85Ah specification timing, V-Li10 BOM control, 10C-42U design optimization. The user was responsible for V-Li10 wiring-diagram changes. Project pressure involved dependencies between drawing, BOM, resources and release timing.

### Routing
Primary: workplace-transition  
Secondary: workplace-communication  
Negotiation: only if resource/schedule conflict exists

### What the skills should diagnose
A project colleague asking for progress is not automatically “催你”. It may be dependency management.

### Expected recommendation
Report in four fields:
- current status
- remaining blocker
- next action
- expected completion / risk

Example:
“V-Li10接线图修改已完成A、B，目前还差C端子确认。端子今天确认的话我预计明天下午更新完图纸并提交；如果未确认，会影响BOM受控时间，我会先把该项标TBD并同步风险。”

### Result
**PASS with modification required.**

### Rule learned
Progress communication should be dependency-oriented, not emotion-oriented.

---

# Cross-case findings

## What worked
1. Facts vs interpretation is consistently useful.
2. Mutual-purpose framing reduces unnecessary conflict.
3. Interests vs positions is effective in supplier and cross-functional cases.
4. Ownership + deadline + acceptance criteria strongly improves execution.
5. The skills correctly discourage motive attribution from silence or disagreement.

## What was missing
1. **Engineering completeness gate**
   Before optimizing wording, verify whether the technical input is complete enough to execute.

2. **Evidence maturity labels**
   Use: confirmed / preliminary / TBD / awaiting owner confirmation.

3. **Four-owner model**
   - input owner
   - evidence owner
   - execution owner
   - decision owner

4. **Follow-up escalation ladder**
   Silence -> dependency reminder -> deadline/impact -> alternate channel -> factual escalation.

5. **Information relay protocol**
   Preserve source, qualifiers, uncertainty, and attribution.

6. **Review-to-checklist conversion**
   Repeated review comments must become reusable process rules.

7. **Dependency-oriented progress reporting**
   Status should show blockers and downstream impact, not just “done/not done.”

# Regression verdict

- workplace-transition: **PASS, but needs engineering-IC hardening**
- workplace-communication: **PASS, but needs follow-up/relay rules**
- negotiation: **PASS, but must not activate before engineering inputs are defined**

# Promotion status
Do **not** promote the three skills from draft to stable yet.

Recommended next validation gate:
- run 5 more real cases
- require at least 3 cases where the recommended wording/action was actually used
- capture outcome
- only then consider v1.0 stable
