# Operations Log Schema

Use these fields when structuring rough notes.

Required when known:
- date
- initiative
- note
- note_type
- owner
- due_date
- status
- impact
- next_step
- decision_needed
- escalation_needed
- source

Allowed note_type values:
- status_update
- action
- decision
- risk
- issue
- dependency
- escalation
- meeting_logistics
- project_plan_update
- follow_up
- open_question
- value_follow_up

If a field is missing, do not invent it. Flag it as missing and add a clarification question.

Use `value_follow_up` when a governance note carries a benefit, outcome, adoption, finance-validation, or measurement action. Include the measurement contract fields when known: expected outcome, benefit type, metric, baseline, target, actual if available, measurement period, source, measure owner, review cadence, validation need, confidence, realization risk, finance-sensitive flag, and downstream route. Keep missing fields visible.

For value follow-up records, also capture:

- follow-up gap: missing baseline, missing actual, finance validation, stale source, owner gap, proxy-only metric, or high realization risk
- next evidence source
- review cadence
- decision needed
- escalation path

Do not close value follow-up because delivery launched or status is green. Close
only when the accountable human owner confirms the evidence, decision, or
validation outcome.
