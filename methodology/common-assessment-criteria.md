# Common AI tool assessment criteria

## Purpose

This document operationalises the seven dimensions in the assessment framework so that ChatGPT, Zapier Agents, Adobe Firefly, and Runway can be assessed consistently.

The criteria provide a common evaluation structure, not a universal technical benchmark. Each assessment must identify its specific use case, tool/model version, plan, date, test conditions, evidence, and limitations.

## Assessment unit and context

Before assessing a tool, define one realistic organisational use case:

- **User and task:** who would use the tool and for what work.
- **Intended output or action:** what the tool is expected to produce or do.
- **Affected stakeholders:** who may rely on or be affected by the result.
- **Information involved:** public, synthetic, internal, personal, confidential, or otherwise restricted.
- **Impact of error:** what could happen if the output or action is wrong.
- **Human role:** who reviews, approves, corrects, or stops the output/action.
- **Out-of-scope uses:** tasks the tool must not perform in this scenario.

Use synthetic or public information only during this project. Do not enter personal, confidential, client, employee, or proprietary data.

## Common criteria

For every applicable criterion, record: finding, evidence label, source or test-case ID, date, confidence, limitation, and implication for the defined use case.

### 1. Purpose and capabilities

| Criterion | What to examine | Evidence |
|---|---|---|
| Intended-purpose fit | Whether documented capabilities support the defined task | Provider documentation and use-case analysis |
| Capability boundaries | Stated limitations, unsupported tasks, and known constraints | Provider documentation and controlled observations |
| Input and output handling | Supported input types, output formats, file handling, and context limits where documented | Product documentation and interface observations |
| Autonomy and integrations | Whether the tool only generates content or can retrieve information, connect to services, or take actions | Product settings, permissions, and workflow observations |

### 2. Reliability and performance

| Criterion | What to examine | Evidence |
|---|---|---|
| Task completion | Whether the output meets the stated task requirements | Test-case results |
| Accuracy or content validity | Whether factual claims, details, or generated elements are correct against a defined reference where one exists | Reference checks and test records |
| Instruction adherence | Whether the output follows explicit constraints and requested format | Prompt-to-output comparison |
| Consistency | Whether similar repeated inputs produce materially consistent results | Repeat tests, with variation documented |
| Uncertainty and failure behaviour | Whether the tool communicates uncertainty, missing information, errors, or limitations rather than presenting unsupported certainty | Test observations and provider documentation |

For creative outputs, assess relevance, prompt adherence, coherence, and visible defects rather than treating subjective preference as factual accuracy.

### 3. Safety and misuse

| Criterion | What to examine | Evidence |
|---|---|---|
| Harmful-output safeguards | Whether the tool identifies and handles clearly unsafe or inappropriate requests | Provider safety documentation and policy-compliant tests |
| Misuse potential | Plausible misuse in the defined organisational context, including deception or misleading content | Scenario analysis and independent sources |
| Bias and representation | Whether outputs show problematic stereotypes, exclusions, or uneven treatment in the limited scenarios examined | Carefully scoped test observations |
| Content integrity | Whether outputs could be mistaken for verified facts, authentic media, or human-created material | Interface features, labels, metadata, and use-case analysis |

Do not attempt to bypass safeguards or generate prohibited content. A small set of tests cannot establish that a tool is safe.

### 4. Privacy and data handling

| Criterion | What to examine | Evidence |
|---|---|---|
| Data collection and use | What the provider says it collects and how submitted content may be used | Current privacy and product documentation |
| Retention and deletion | Published retention, deletion, and account-control information | Provider documentation and available settings |
| Access and sharing | Visibility of prompts, files, outputs, activity, and connected services | Product settings and documentation |
| Data minimisation | Whether the use case can avoid sensitive information or use synthetic, anonymised, or public inputs | Project test design and proposed controls |

Do not infer enterprise-grade privacy protections from a consumer free plan.

### 5. Transparency and accountability

| Criterion | What to examine | Evidence |
|---|---|---|
| AI disclosure | Whether users can recognise AI-generated or AI-assisted outputs | Interface, output labels, and provider documentation |
| Traceability | Whether relevant prompts, versions, outputs, and actions can be recorded | Available history, logs, metadata, and documentation |
| Explanation of limitations | Whether the provider explains relevant limitations, model behaviour, and plan restrictions | Provider documentation |
| Responsibility | Whether an organisational owner, reviewer, and escalation route can be identified for the use case | Proposed governance arrangement |

### 6. Human oversight and control

| Criterion | What to examine | Evidence |
|---|---|---|
| Review before use | Whether a person can review outputs before they are relied on, published, or acted upon | Workflow and interface observations |
| Correction and override | Whether users can edit, reject, or replace outputs | Product observations |
| Permission boundaries | Whether access and connected permissions can be limited to what the task needs | Settings and provider documentation |
| Stop and recovery | Whether a user can stop an operation, revoke access, or recover from an incorrect action | Product documentation and safe observations |
| Escalation | Whether uncertain or high-impact cases can be referred to an accountable human | Proposed workflow |

For tools that do not take external actions, mark action approval, permission boundaries, and stop/recovery as not applicable only when justified. Human review of generated content remains relevant.

### 7. Organisational suitability and safeguards

| Criterion | What to examine | Evidence |
|---|---|---|
| Use-case suitability | Whether benefits plausibly justify the risks for the defined task | Combined findings |
| Stakeholder impact | Who could benefit, be harmed, or be disadvantaged | Use-case and impact analysis |
| Operational readiness | Training, support, accessibility, availability, and continuity needs | Provider information and organisational analysis |
| Governance controls | Acceptable-use rules, approval, documentation, monitoring, and incident handling needed | Risk register and proposed controls |
| Adoption decision | Whether use should proceed, proceed with conditions, require more evidence, or not proceed | Assessment synthesis |

## Category-specific extensions

The common criteria apply to all four tools. Add the following category-specific checks where relevant; do not force a criterion onto a tool that does not have the capability.

### Conversational chatbot — ChatGPT

- Factual response quality and unsupported claims.
- Source and citation accuracy when sources are requested.
- Handling of ambiguous, incomplete, or conflicting instructions.
- Appropriate expression of uncertainty.
- Risk of users treating generated advice as authoritative.

### AI agent — Zapier Agents

- Correct interpretation of the requested workflow.
- Correct selection and sequencing of tools/actions.
- Permission scope for connected applications.
- Human approval before consequential or externally visible actions.
- Duplicate, unintended, or irreversible action risk.
- Error handling, logging, and ability to stop or recover a workflow.

Do not connect real work accounts or allow external actions during project tests. Use a controlled test setup and synthetic data.

### Image generation — Adobe Firefly

- Prompt adherence and visual coherence.
- Representation and stereotype risks in selected scenarios.
- Artefacts or misleading visual details.
- Availability and meaning of content credentials or provenance information, where applicable.
- Provider statements about training data, copyright, and commercial use; distinguish provider claims from independent legal conclusions.

### Video generation — Runway

- Prompt adherence across the generated sequence.
- Temporal consistency of people, objects, and scenes.
- Motion coherence and visible artefacts.
- Realism and potential for misleading synthetic footage.
- Watermarks, labels, metadata, or provenance features where available.
- Credit consumption and practical reproducibility under the free plan.

## Rating and evidence rules

Use the existing framework's qualitative statuses for each dimension:

- **Adequate for the defined use**
- **Adequate with conditions**
- **Needs further evidence**
- **Not suitable for the defined use**
- **Not assessed**

Record evidence confidence separately as High, Medium, or Low, following the assessment framework.

For each criterion, use one evidence label:

- **Provider statement**
- **Independent source**
- **Project observation**
- **Inference**
- **Unknown / not verified**

Use **Not applicable** only when the criterion genuinely does not apply to the tool or defined use case. Give a short reason. Do not use it as a substitute for missing evidence.

Do not combine evidence confidence and risk severity into one score. A high-confidence finding can describe a high risk; a low-confidence finding can still require further investigation.

## Minimum record for each test

Record:

1. Test-case ID and date.
2. Tool, model/version if visible, and account plan.
3. Defined use case and intended outcome.
4. Exact input or prompt, excluding sensitive data.
5. Expected result or reference, where one exists.
6. Actual output or action observed.
7. Pass, partial, fail, or not applicable, with a reason.
8. Relevant common and category-specific criteria.
9. Evidence label, source, confidence, and limitations.
10. Potential risk and proposed safeguard.

## Interpretation and limitations

- This is a small, qualitative portfolio assessment, not a statistically representative benchmark.
- Free-plan observations may not generalise to paid, business, or enterprise configurations.
- Provider documentation describes provider claims and controls; it does not independently prove their effectiveness.
- A feature being present does not establish that it is enabled, effective, or appropriate for every use.
- Record the product and model version and assessment date because products and plans change.
- Do not make legal-compliance, certification, or security-audit claims.
