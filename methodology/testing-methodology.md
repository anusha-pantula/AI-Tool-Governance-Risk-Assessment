# Practical testing methodology

## Purpose

This document defines a small, repeatable, low-risk testing approach for the four selected tools. The baseline is **five carefully designed test cases per tool**, for **20 planned test cases in total**. Additional tests will be added only when the initial evidence is insufficient to answer an important assessment question.

Testing is intended to generate documented project observations, not to certify products or establish comprehensive safety.

## Selected tools

1. Chatbot: ChatGPT
2. AI agent: Zapier Agents
3. Image generation: Adobe Firefly
4. Video generation: Runway

Record the product name, plan or access tier, feature, model/version if visible, date checked, and any feature restrictions before testing.

## Baseline test design

Each tool receives five tests. The tests are designed to cover multiple relevant assessment dimensions without forcing every dimension into every test.

| Test slot | Main purpose | Common dimensions typically informed |
|---|---|---|
| 1. Core task performance | Test the tool on a realistic, clearly specified organisational task | Purpose and capabilities; reliability and performance |
| 2. Ambiguity and limitations | Examine missing information, ambiguous instructions, or a task outside the stated capability | Reliability and performance; transparency and accountability |
| 3. Safety and misuse | Examine a plausible, policy-compliant risk scenario relevant to the tool | Safety and misuse; organisational suitability |
| 4. Human control and accountability | Examine review, correction, approval, traceability, or action boundaries | Human oversight and control; transparency and accountability |
| 5. Privacy and organisational fit | Examine data-minimisation choices, information handling, and suitability for a defined workplace context | Privacy and data handling; organisational suitability and safeguards |

The five slots are a planning structure, not five identical prompts across all products. Use category-specific scenarios and evaluation criteria. Record a dimension as not assessed if the test set does not provide evidence for it; do not infer coverage merely because a test was run.

### Category-specific focus

**ChatGPT**
1. A realistic workplace information-synthesis task with a checkable reference.
2. An ambiguous request with an important missing detail.
3. A safe scenario involving a potentially harmful or misleading request; evaluate refusal or redirection without attempting to bypass safeguards.
4. Review and correction of an output containing a deliberately planted, harmless error.
5. A privacy-aware task using synthetic information; examine whether the response encourages data minimisation and appropriate human review.

**Zapier Agents**
1. A simple multi-step task in a controlled test environment using synthetic data.
2. An ambiguous instruction; assess whether the agent seeks clarification before proceeding.
3. A simulated failed step or unavailable tool; assess error handling and reporting.
4. A workflow with a consequential step; assess whether permissions and human approval can prevent unintended execution.
5. A restricted-scope workflow; assess whether the agent stays within authorised actions and reports what it did and did not complete.

If a safe sandbox or safe approval control is unavailable, do not connect real accounts or allow external actions. Use a documented simulation and mark hands-on action behaviour as not tested.

**Adobe Firefly**
1. A clear, neutral workplace visual brief.
2. A prompt with a deliberate ambiguity or conflicting visual constraint.
3. A representation and stereotype scenario framed neutrally and respectfully.
4. Revision of an initial image, examining user control and visible artefacts.
5. A synthetic-media/provenance scenario; inspect available labels or content credentials and record provider claims separately from project observations.

**Runway**
1. A short, neutral workplace scene brief.
2. A scene with multiple specified visual elements; examine prompt adherence.
3. A sequence requiring consistent objects or scene details over time.
4. A revision or regeneration task; examine user control, visible artefacts, and repeatability.
5. A synthetic-media scenario; examine how realism, labelling, watermarking, or provenance could affect organisational use.

The exact prompts, settings, expected outcomes, and scoring notes must be written into the test register before running each test.

## Test design principles

- Use synthetic or public inputs only.
- Define the task, expected behaviour, and evaluation criteria before running a test.
- Keep settings consistent when comparing repeated or similar tests where practical.
- Record the exact input, relevant settings, output, date, and observations.
- Record failures, partial results, and ambiguous outcomes, not just successful examples.
- Do not cherry-pick outputs.
- Do not bypass safety controls, access controls, or provider restrictions.
- Do not connect agents to real organisational systems or grant unnecessary permissions.
- Avoid unnecessary regenerations. For image and video tools, one planned generation per test is the default; a second generation is justified only when the test specifically examines repeatability or a first attempt fails for a documented technical reason.
- Record credit/activity consumption so the project stays within the free allowance.

## Evaluation dimensions for each test

Choose task-specific criteria before testing. Possible criteria include:

- **Task fulfilment:** did the output address the requested task?
- **Accuracy or fidelity:** was it factually correct or visually faithful to the brief?
- **Consistency:** did comparable inputs produce materially comparable results?
- **Uncertainty handling:** did the tool acknowledge missing information or limitations?
- **Control:** could the user review, correct, reject, approve, or stop the output/action?
- **Risk signal:** did the test reveal a relevant safety, privacy, transparency, or misuse concern?

Use descriptive notes rather than false precision. Where a qualitative outcome is useful, use: Meets expectation, Partly meets, Does not meet, Not applicable, or Not tested. Explain each judgement.

## Conditional additional testing

Start with the baseline five tests per tool. Add a test only when at least one of the following applies:

1. A material assessment dimension remains **not assessed** or has insufficient evidence.
2. An important finding is ambiguous and a targeted test could resolve the ambiguity.
3. A potentially significant risk is identified and needs a safe, bounded follow-up.
4. A test failed for a technical reason unrelated to the tool's intended behaviour and a repeat is necessary.
5. A category-specific capability central to the defined use case was not exercised by the baseline tests.

For every additional test, document:
- The evidence gap or finding that triggered it.
- The question the new test is intended to answer.
- Why existing evidence is insufficient.
- The expected evidence and stopping condition.

Do not add tests merely to increase the sample size or produce more impressive-looking results. If an issue cannot be safely or meaningfully tested with available access, document the limitation rather than forcing a test.

## Free allowance and resource controls

Before testing, record the visible free-plan allowance for each tool. Keep a simple usage log.

- ChatGPT: note applicable message/model limits and any tool limits.
- Zapier Agents: record available activities and avoid unnecessary agent runs or live integrations.
- Adobe Firefly: record available generations and use one planned generation per image test unless a justified repeat is approved.
- Runway: record available credits and the credit cost of the selected video model before generating. Prioritise the five planned tests and do not spend credits on exploratory prompts.

If the free allowance is insufficient for the five planned tests, pause and revise the plan with the project owner. Do not purchase credits or subscriptions without explicit approval.

## Test record fields

For every test, record:
- Test ID and test slot
- Tool and category
- Date and access tier
- Feature or model/version, if known
- Test objective and evidence gap addressed
- Use-case scenario
- Exact input or prompt
- Relevant settings
- Expected behaviour and evaluation criteria
- Observed output or action
- Task fulfilment and category-specific observations
- Relevant assessment dimensions
- Evidence label and source
- Risk or concern identified
- Limitations
- Credit/activity usage where applicable
- Retest or additional test needed, with reason

## Reporting results

Separate:
- What the provider claims
- What the project directly observed
- What independent sources report
- What the project infers
- What remains unknown

A test result applies only to the tested configuration, date, prompt, and access tier. Product features and model behaviour may change. Record this limitation in every assessment.

The approach is a small qualitative portfolio assessment, not a statistically representative benchmark, comprehensive security audit, or proof of safety. This is consistent with risk-based evaluation: methods and metrics should be appropriate to the intended context, documented, and proportionate to the risks being examined. See the [NIST AI RMF Measure function](https://airc.nist.gov/airmf-resources/airmf/5-sec-core/) and [NIST AI RMF Playbook: Measure](https://airc.nist.gov/airmf-resources/playbook/measure/).

## Safety and ethics

Do not use real personal data, confidential business information, employee records, customer data, or proprietary material. Do not impersonate real people, create deceptive media of identifiable individuals, attempt to defeat safeguards, or test integrations without explicit authorisation.
