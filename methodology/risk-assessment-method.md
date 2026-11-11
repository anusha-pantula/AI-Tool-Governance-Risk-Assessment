# Qualitative risk assessment method

## Purpose

This method supports consistent identification, evaluation, treatment, and monitoring of risks associated with a defined AI tool use case. It is a qualitative project method, not a formal enterprise risk standard or certification.

## 1. Define the use case

Before scoring risks, document:
- The business or organisational purpose
- Intended users
- People or groups potentially affected
- Information entered, generated, retrieved, or shared
- Systems and integrations involved
- Level of autonomy
- Human review and approval points
- Consequences if the tool is wrong, unavailable, or misused

Avoid assigning one risk score to a tool without stating the use case.

## 2. Identify risks

Consider risks across:
- Reliability and inaccurate outputs
- Bias, unfairness, or exclusion
- Privacy and confidentiality
- Security and unauthorised access
- Safety and harmful content
- Misuse, deception, and synthetic media
- Transparency and traceability
- Human oversight and automation bias
- Accountability and unclear ownership
- Operational dependency and service disruption
- Legal, regulatory, contractual, or intellectual-property concerns requiring specialist review

This list is a prompt for analysis, not a claim that every risk applies to every tool.

## 3. Estimate likelihood

Use the following qualitative scale:

| Rating | Meaning |
|---|---|
| 1 – Rare | Unlikely in the defined context; no known indication in available evidence |
| 2 – Unlikely | Could occur, but is not expected under current conditions |
| 3 – Possible | Credible scenario that may occur |
| 4 – Likely | Expected to occur in some circumstances or supported by repeated evidence |
| 5 – Almost certain | Expected frequently or already observed repeatedly in the defined context |

State the evidence and assumptions behind each likelihood rating. Lack of evidence is not proof that a risk is rare.

## 4. Estimate impact

Assess impact in the context of the use case. Consider people, operations, finances, reputation, privacy, and legal or contractual consequences.

| Rating | Meaning |
|---|---|
| 1 – Negligible | Minimal, readily reversible effect |
| 2 – Minor | Limited disruption or harm, manageable through routine action |
| 3 – Moderate | Material effect requiring planned intervention |
| 4 – Major | Serious harm, disruption, or exposure requiring urgent intervention |
| 5 – Severe | Very serious or potentially irreversible harm or consequences |

If impacts differ across stakeholders, record the most significant credible impact and explain it.

## 5. Determine inherent risk

Inherent risk is the risk before considering the specific controls being assessed.

Calculate a simple score:

**Inherent risk score = Likelihood × Impact**

| Score | Indicative level |
|---|---|
| 1–4 | Low |
| 5–9 | Moderate |
| 10–16 | High |
| 17–25 | Critical |

These bands are a project convention for prioritisation. They are not universal thresholds and should not replace judgement. A severe impact may warrant escalation even if the numerical score is lower.

## 6. Identify controls and mitigations

Record existing controls separately from proposed mitigations.

Examples:
- Approved-use policy and prohibited-use rules
- Data minimisation and restrictions on sensitive inputs
- Role-based access and least-privilege permissions
- Human review before consequential use
- Output verification against authoritative sources
- Approval gates for agent actions
- Logging and traceability
- User training and clear disclosure
- Incident reporting and escalation
- Periodic reassessment and change monitoring
- Fallback or manual process if the tool is unavailable

Do not assume a control exists merely because it is recommended by the project. Record its implementation status and evidence.

## 7. Estimate residual risk

Residual risk is the risk remaining after the stated controls are applied.

Record:
- Controls that are implemented and evidenced
- Controls that are planned but not yet implemented
- Residual likelihood and impact
- Residual score and level
- Whether the remaining risk is acceptable for the defined use
- Who has authority to accept or escalate the risk

Do not lower a score for a planned control as though it were already operating.

## 8. Assign ownership and monitoring

Use role titles rather than personal names. Possible owner roles include:
- Business/use-case owner
- IT or system owner
- Information security
- Privacy or data protection lead
- Procurement/vendor management
- HR or people function
- Legal/compliance specialist
- AI governance or risk committee

Define monitoring triggers, such as:
- A material model, feature, or provider-policy change
- A new integration or expanded permission
- A change in data type or user group
- A serious error, incident, or complaint
- A change in intended use
- Evidence that controls are not working

## 9. Evidence and uncertainty

Every risk should link to evidence or be explicitly labelled as a scenario or inference. Use the repository evidence labels:
- Provider statement
- Independent source
- Project observation
- Inference
- Unknown / not verified

Record confidence and limitations. Where evidence is insufficient, use a provisional rating and identify what information is needed.

## Important limitation

This method is intended for a transparent portfolio demonstration. Real organisational adoption decisions may require specialist privacy, security, legal, procurement, safety, and domain reviews.
