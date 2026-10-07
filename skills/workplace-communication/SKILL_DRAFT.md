# Workplace Communication Skill

## Purpose
Use this skill for high-stakes workplace conversations where opinions differ, emotions rise, or outcomes matter. It is distilled primarily from *Crucial Conversations* and adapted for an early-career engineering individual contributor.

## Trigger conditions
Invoke when:
- A manager, mentor, supplier, testing engineer, project manager, quality engineer, or peer disagrees with you.
- You need to raise a risk, challenge an assumption, give bad news, or correct misinformation.
- Someone becomes defensive, silent, sarcastic, aggressive, or evasive.
- You need to ask for missing information without sounding accusatory.
- A conversation has stalled or become emotionally charged.
- You need to turn a discussion into a clear action and ownership plan.

## Core model
A crucial conversation is characterized by high stakes, differing opinions, and strong emotions. The goal is not to “win” the exchange but to restore and maintain dialogue so relevant meaning can enter the shared pool.

## Decision flow

### 1. Start with Heart
Before speaking, answer:
- What do I really want for myself?
- What do I really want for the other person?
- What do I really want for the relationship?
- How would I behave if I genuinely wanted those outcomes?

Avoid the false choice between “say nothing” and “fight.”

### 2. Learn to Look
Monitor two channels at once:
- Content: what is being discussed.
- Conditions: whether the conversation is still safe enough for dialogue.

Watch for:
- Silence: masking, avoiding, withdrawing, withholding.
- Violence: controlling, labeling, attacking, forcing.
- Your own physical, emotional, and behavioral stress signals.

If dialogue is breaking down, stop solving the substantive problem temporarily and restore safety.

### 3. Make It Safe
Safety mainly depends on:
- Mutual Purpose: both parties believe the other cares about a shared or compatible outcome.
- Mutual Respect: both parties believe the other respects them as a person or professional.

Use:
- Apology when you clearly created harm.
- Contrasting when your intent has been misunderstood:
  - “I don’t mean X. I do mean Y.”
- CRIB when mutual purpose is missing:
  - Commit to seek Mutual Purpose.
  - Recognize the purpose behind the strategy.
  - Invent a Mutual Purpose.
  - Brainstorm new strategies.

Do not buy safety by making unnecessary technical or substantive concessions.

### 4. Master My Stories
Separate:
- observable facts
- your interpretation/story
- resulting emotion
- resulting action

Ask:
- What facts would a neutral observer record?
- What story am I adding?
- What evidence would contradict my story?
- What role have I played in creating the problem?

Do not treat motive assumptions as facts.

### 5. STATE My Path
When presenting a concern:
- Share your facts.
- Tell your story.
- Ask for others’ paths.
- Talk tentatively.
- Encourage testing.

Engineering adaptation:
- Begin with data, requirement, test result, timestamp, interface, or documented statement.
- Then explain the inference.
- Explicitly invite correction.

Example structure:
“目前我确认到的是 A、B、C。基于这些信息，我担心会导致 D。我的理解可能不完整，你这边看到的情况是什么？”

### 6. Explore Others’ Paths
If the other person moves to silence or violence, become curious instead of reactive.

Use AMPP:
- Ask to Get Things Rolling.
- Mirror to Confirm Feelings.
- Paraphrase to Acknowledge the Story.
- Prime When You’re Getting Nowhere.

Goal: reconstruct the other person’s facts, story, feelings, and intended action.

Understanding is not agreement.

### 7. Move to Action
Dialogue is incomplete until a decision process is explicit.

Clarify:
- Who does what?
- By when?
- What does “done” mean?
- Who owns the decision?
- Who needs to be informed?
- When will progress be checked?

Distinguish four decision modes where useful:
- Command
- Consult
- Vote
- Consensus

Do not imply consensus when only consultation occurred.

## Engineering workplace patterns

### Raising a technical risk
Preferred sequence:
1. Facts
2. Impact
3. Uncertainty
4. Recommendation
5. Ask for decision/confirmation

### Correcting a senior colleague
Do not lead with “you are wrong.”
Use:
- shared objective
- observed facts
- tentative interpretation
- request for correction

### Following up on no response
Separate non-response from motive.
Do not infer “they don’t care” or “they are blocking me” without evidence.
State the dependency and consequence:
“这个参数如果今天不能确认，会影响明天测试单冻结。麻烦今天 17:00 前帮忙确认一下；如果当前还没有结论，我先按待定项标识。”

### Cross-functional disagreement
Translate positions into interests:
- Testing may care about measurability and reproducibility.
- Project may care about schedule.
- Supplier may care about scope and liability.
- Engineering may care about technical sufficiency and risk.
Search for a process that protects the legitimate interests of all parties.

## Output format when invoked
1. Situation diagnosis
2. Confirmed facts vs interpretations
3. Safety status: normal / silence / violence
4. What each stakeholder likely needs to resolve
5. Recommended conversation strategy
6. Suggested wording
7. Required decision / owner / deadline
8. Escalation threshold
9. What not to say

## Guardrails
- Do not use “safety” as an excuse to avoid necessary disagreement.
- Do not confuse understanding with agreement.
- Do not manufacture mutual purpose where interests truly conflict.
- Do not soften technical risk until it becomes ambiguous.
- Do not assume silence means consent.
- Do not infer malicious intent without evidence.
- For safety, compliance, quality, or technical acceptance issues, documented requirements override conversational convenience.


## Regression additions from SWD/XWD cases

### Evidence-maturity wording
Prefer:
- “已确认”
- “目前初步方案”
- “待确认”
- “我再和X核一下”
- “评审时确认”

Avoid weakening credibility with unnecessary self-devaluation such as:
- “我不太懂”
- “我就是随便想的”
- “可能是吧”

State uncertainty precisely, not emotionally.

### No-response follow-up ladder
When someone does not reply:
1. Separate silence from motive.
2. Check whether a real dependency/deadline exists.
3. Send a concise follow-up with a concrete ask.
4. If a milestone is at risk, state the impact and requested response time.
5. If still blocked, switch channel or involve the responsible coordinator.
6. Escalate factually, never as a complaint about attitude.

### Technical information relay protocol
When relaying a mentor’s / owner’s technical answer:
- preserve the original scope
- preserve qualifiers and uncertainty
- do not add causal explanation that was not confirmed
- attribute the source when useful
- if decision-critical, ask the original owner to confirm
- distinguish “张工确认的是…” from “我的理解是…”

### Decision-ready message format
For enterprise chat, prefer:
1. context (one sentence)
2. confirmed facts
3. issue / dependency
4. proposed action
5. explicit ask / owner / timing

Do not bury the ask in a long background paragraph.

### Progress update format
Use:
- status
- blocker
- next action
- ETA / downstream impact

Treat “催进度” as dependency management unless evidence shows otherwise.


## Boundary rules from SWD/XWD regression v2

### Respect does not mean accepting undefined responsibility
If another function pushes work back:
1. define the output
2. define the missing input
3. identify the process/document owner
4. state the gap neutrally
5. propose closure
6. escalate ownership ambiguity if needed

Do not use “maintain safety” to absorb work with unclear ownership.

### Clarity over comfort for technical risk
For safety, compliance, quality, or critical technical uncertainty:
- state the risk explicitly
- do not dilute it with vague language
- separate respect for the person from firmness on the requirement

### Progress pressure response
When a milestone is urgent:
- state what is complete
- state what remains unknown
- classify whether the unknown is critical/major/minor
- offer valid release options
- ask the decision owner to choose if a tradeoff remains

Never imply “final” when the work is actually provisional.
