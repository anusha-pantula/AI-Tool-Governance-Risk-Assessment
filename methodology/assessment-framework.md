# AI tool assessment framework

## How to apply the framework

Assess each selected tool against the seven dimensions below. For every finding, record the use case, evidence source, observation date, confidence, and limitations.

Use two linked perspectives:

1. **Provider/tool perspective:** what the product is designed to do, what the provider documents, and what controls are available.
2. **Organisational/use-case perspective:** how the organisation intends to use it, what could go wrong, who may be affected, and what safeguards are needed.

Do not treat a feature being available as proof that it is effective or enabled in every plan or configuration.

## Dimension 1: Purpose and capabilities

Questions:
- What tasks is the tool designed to support?
- What are its documented capabilities and limitations?
- What level of autonomy does it have?
- Does it retrieve information, generate content, take actions, or interact with other systems?
- Is the intended organisational use within the tool's stated purpose?
- What tasks should remain outside the tool's remit?

Evidence to collect:
- Official product and technical documentation
- Feature and plan limitations
- Documented supported integrations and action permissions
- Project observations from defined test cases

## Dimension 2: Reliability and performance

Questions:
- Does the tool produce accurate and relevant outputs for the tested task?
- Does it fabricate information, citations, or details?
- Are outputs consistent across repeated or slightly varied inputs?
- Does it communicate uncertainty or limitations?
- Does it fail safely when information is missing or instructions conflict?
- What level of human verification is needed?

Evidence to collect:
- Repeatable test prompts and inputs
- Output records and evaluation notes
- Provider documentation about limitations
- Independent evaluations where available

Do not describe a small qualitative test set as a statistically representative performance benchmark.

## Dimension 3: Safety and misuse

Questions:
- What harmful or inappropriate outputs could arise in the intended use?
- Can the tool be misused to create deceptive, misleading, or harmful content?
- What safeguards are documented?
- How does the tool respond to ambiguous or risky requests?
- Could generated content affect individuals or groups unfairly?
- What misuse scenarios are relevant to the organisation?

Evidence to collect:
- Provider safety documentation
- Publicly documented limitations or incidents
- Controlled, policy-compliant tests
- Use-case-specific misuse scenarios

Do not attempt to bypass safeguards or generate prohibited content as part of testing.

## Dimension 4: Privacy and data handling

Questions:
- What information might users enter or upload?
- Does the provider explain collection, retention, deletion, and use of submitted data?
- Are there settings or contractual options relevant to data use?
- Are access controls and administrative controls documented?
- Could prompts, files, outputs, or logs expose confidential information?
- Can the use case operate with synthetic, anonymised, or minimised data?

Evidence to collect:
- Current provider privacy and data-processing documentation
- Product settings and plan-specific documentation
- Data-flow descriptions where available
- Project data-minimisation decisions

Do not submit personal, confidential, client, employee, or proprietary information to public tools for this project.

## Dimension 5: Transparency and accountability

Questions:
- Can users identify when AI has contributed to an output?
- Does the provider explain relevant system limitations?
- Can outputs be traced to a user, task, or system action where appropriate?
- Are sources, versions, or activity logs available?
- Is there a clear organisational owner for the use?
- Is there a process to report errors or concerns?

Evidence to collect:
- Provider documentation
- Product interface observations
- Available logging and audit features
- Proposed organisational ownership and escalation arrangements

## Dimension 6: Human oversight and control

Questions:
- Can a human review outputs before they are used or shared?
- Can users correct, reject, or override outputs?
- For agents, can actions be previewed, approved, paused, or stopped?
- Are permissions limited to what the task requires?
- Are escalation paths defined for uncertain or high-impact cases?
- Is human review meaningful, or is it merely a final sign-off?

Evidence to collect:
- Documented human-control features
- Practical observations of review and override options
- Workflow diagrams or action sequences
- Proposed approval and escalation controls

## Dimension 7: Organisational suitability and safeguards

Questions:
- Is the tool suitable for the intended task and users?
- What is the impact if the tool is wrong, unavailable, or misused?
- Are affected stakeholders identified?
- Are training, acceptable-use rules, and support arrangements needed?
- Are procurement, vendor review, or integration checks necessary?
- What monitoring is needed after adoption?
- Under what conditions should use be restricted or stopped?

Evidence to collect:
- Defined organisational use case
- Risk register
- Provider and independent documentation
- Proposed controls, owners, and monitoring triggers

## Rating approach

For each dimension, use a qualitative status:

- **Adequate for the defined use:** evidence supports use with routine controls.
- **Adequate with conditions:** use may be appropriate if specified safeguards are implemented.
- **Needs further evidence:** available evidence is insufficient to reach a defensible conclusion.
- **Not suitable for the defined use:** material concerns remain that cannot be adequately mitigated in the proposed context.
- **Not assessed:** the dimension has not yet been examined.

These are project assessment judgements, not certifications or universal ratings of a provider.

## Evidence confidence

Record confidence separately from the status:

- **High:** current, directly relevant evidence from authoritative documentation or repeatable observations.
- **Medium:** relevant evidence exists but is incomplete, indirect, or limited in scope.
- **Low:** evidence is sparse, unclear, outdated, or based mainly on inference.

## Required assessment record

For each dimension, capture:
- Assessment question
- Finding
- Evidence label
- Source or test-case ID
- Date checked
- Confidence
- Limitation or unknown
- Implication for the defined use case
- Recommended safeguard
