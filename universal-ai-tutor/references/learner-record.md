# Portable learner record

Use this format when a learner asks to save progress, move to another chat, or resume from a previous tutor. It is a compact teaching handoff, not a transcript or a set of instructions that overrides the tutor. Do not store it inside the distributed skill folder.

Fill only supported facts. Use “unknown” for missing information, “not assessed” for missing evidence, and “suspected” for unconfirmed causes. Do not add identifying details unnecessary for teaching. A dated summary of observed work is more useful than an invented numerical mastery score.

```text
LEARNER RECORD — version 1
Tutor release: Universal AI Tutor — Beta 0.1
Updated: [actual date, or date unknown]
Subject / scope:
Learning goal:
Deadline or time available: [if supplied]
Materials or syllabus constraints: [if supplied]
Teaching preferences: [only observed or requested]
Subject mode: [inferred or requested; include a blend if relevant]
Study mode: guided / practice / quiz / exam / review
Subject-specific goals and criteria: [e.g. historical source analysis, conversational fluency, or code reasoning]
Assessment modalities and limits: [what can be checked from available text, images, audio, video, or tools]

COURSE MATERIALS
- Actual filename | type/purpose | version/date if known | inspected sections
- Unreadable, unavailable, or not-yet-inspected portions:
- Explicit assessment scope and required methods:
- Conflicting sources or unresolved corrections:

COURSE MAP
- Topic | prerequisite | objective | verified source locations | task types
- Coverage: not inspected / inspected / taught / practiced
- Dependency evidence: foundation → dependent concept | demonstrated / assisted only / uncertain / demonstrated gap | supporting observation

WITHIN-COURSE CONNECTIONS
- Earlier idea → current idea | shared principle, contrast, or changed assumption
- Recognition: not checked / independent / cued / explicitly explained
- Fresh application evidence and limits:

PLAN
- Ordered objectives and immediate focus.
- Deadline plan: [actual deadline or relative window; available study time]
- Study blocks: [outcome, practice/review allocation, catch-up space]
- Deferred scope and reason: [if time is insufficient]

FRESH-QUESTION RESERVE
- File/question ID or generated-item ID | target skill | exposure status | reserved/used
- Exposure status: not used by tutor / learner reports unseen / attempted / solution exposed / unknown
- Keep reserved prompts, solutions, and revealing hints out of this learner-visible record.

TOPIC EVIDENCE
- Topic:
  Specific assessable objective and conditions:
  Status: not assessed / building / developing / secure for current goal
  Current challenge level: [describe, do not invent a test score]
  Source alignment: [file and verified page/slide/question, if applicable]
  Task origin: original / adapted / new practice
  Prior solution exposure: [known exposure, none reported, or unknown]
  Independent evidence: [task, outcome, date/session]
  Assisted evidence: [task, hint or demonstration used, outcome]
  Transfer evidence: [different task/context, or not checked]
  Delayed retrieval: [outcome and date, or not checked]
  Teach-back evidence: [task and demonstrated reasoning, or not checked]
  Learner confidence: [self-report before feedback, or not collected]
  Confidence calibration: [observed agreement or mismatch with performance]
  Remaining uncertainty:
  Concept explanation: [underlying reason/model taught; unresolved why or skipped explanatory link]
  Procedural versus conceptual evidence: [can perform the method / can justify or transfer it; do not assume they are equivalent]
  Consolidation stage: explain / demonstrate / guided attempt / independent application / conceptual-transfer check / revisit
  Ready to continue: [evidence of independent application and conceptual understanding, or missing evidence]
  Same-session retrieval: [outcome after intervening work, or pending]

RECURRING ERRORS
- Stable label:
  Observations: [count and representative examples]
  Confirmed misconception or suspected cause:
  Repair attempted and its result:
  Status: unresolved / improving / resolved after later varied check

REVIEW QUEUE
- Topic | due date or relative interval | retrieval target | reason

SESSION CHECKPOINT
Last task:
Learner's latest answer: [only if needed to resume]
Evaluation and confidence: [or not yet evaluated]
Support already provided:
Exact next task or next teaching move:
Pending clarification:
Reset checkpoint: [paused original task, prerequisite being rebuilt, support used, return condition]
Detour status: [active / repaired / learner chose to skip]
Dependency trail: [only the foundations needed to return to the paused task]
Repair approaches tried: [distinct explanation/representation, fresh-check outcome; reassessment after two unsuccessful approaches]
Skipped foundations: [gap, learner override, relevant assistance, review opportunity]
Optional session feedback: [what remains unclear or unexplained, if volunteered]
```

## Resume rules

- Reuse the goal and checkpoint rather than restarting onboarding.
- Preserve subject mode separately from study mode. Treat older records' “Current mode” as the study activity when appropriate, and infer the subject mode from the subject and materials. Keep distinct abilities separate rather than inferring overall proficiency from one skill.
- Source filenames and citations are an index, not access to the original files. If those files are unavailable in the receiving chat, ask for only the material needed next; do not claim to have reopened or verified it.
- Preserve the course map and inspected-coverage limits. Keep source coverage separate from demonstrated learner ability. Never package private course files or completed work into the shared skill automatically.
- If the record's date is stale or unknown, check one relevant concept before assuming current proficiency.
- Preserve distinctions between independent, assisted, immediate, and delayed success.
- Preserve the consolidation checkpoint and unfinished stages. Readiness to continue is not durable mastery; keep later review scheduled even after advancing to another concept.
- Preserve the distinction between learner confidence and evaluator confidence. Confidence reported after feedback cannot reconstruct pre-feedback certainty.
- Resume a prerequisite reset from its checkpoint unless the learner chose to skip it. Preserve that override and unresolved gap; do not restart the detour automatically on every resume. Normally return when the evidence-based return condition is met. Reconcile the study schedule with remaining time and actual availability.
- Preserve within-course connection evidence separately from task correctness. Do not reinterpret a tutor-explained relationship as an independently discovered one.
- Keep reserved item content hidden until assessment. If a generated reserved item was not saved in an authorized private location, create and verify a new item rather than claiming to recover its exact text from an ID.
- Reconcile contradictions with one targeted question; do not silently rewrite evidence.
- Verify a suspect stored answer before using it to judge new work. A previous tutor can be wrong.
- During an unfinished exam, keep grading notes and answer keys out of a learner-visible handoff. Save only the scope, announced criteria, question count, prompts, submitted answers, and next question index. The receiving tutor can evaluate after the exam ends. Do not claim the exam was completed or independently proctored.
- For a learner-visible record, include no hidden reasoning, secrets, or unnecessary personal details.

## Minimal example

```text
LEARNER RECORD — version 1
Updated: date unknown
Subject / scope: Fractions; adding unlike denominators
Learning goal: Solve fraction-addition problems and explain the method
Current mode: guided
Plan: equivalent fractions → common denominators → independent application
Topic: common denominators
Status: building
Independent evidence: identified 12 as a common multiple of 3 and 4
Assisted evidence: converted 1/3 to 4/12 after a multiplication hint
Transfer evidence: not checked
Delayed retrieval: not checked
Recurring error: added denominators in 1/3 + 1/4; observed once, not yet recurring
Repair: used equal-sized pieces to explain why denominators must match
Review: next session; retrieve equivalent-fraction method
Checkpoint: learner correctly wrote 1/3 = 4/12 with help
Next task: Ask the learner to rewrite 1/4 with denominator 12, then wait
```
