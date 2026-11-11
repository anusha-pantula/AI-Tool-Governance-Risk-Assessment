# Practical testing methodology

## Purpose

This document defines a small, repeatable, low-risk testing approach for comparing representative tools. Testing is intended to generate project observations, not to certify products or establish comprehensive safety.

## Tool selection criteria

Select one representative tool in each category:

1. Conversational AI chatbot
2. AI agent or agentic workflow tool
3. AI image-generation tool
4. AI video-generation tool

Before selection, check:
- Whether a free or otherwise accessible test environment is available
- Whether the relevant features can actually be tested
- Whether official documentation is sufficiently clear
- Whether the tool can be used without submitting sensitive data
- Whether the chosen tool is reasonably representative of its category

Record the product name, provider, plan or access tier, model/version if visible, date checked, and any feature restrictions. Tool candidates are not final selections until this check is completed.

## Test design principles

- Use synthetic or non-sensitive inputs only.
- Define the task and expected evaluation criteria before running a test.
- Keep prompts and settings consistent when comparing tools where practical.
- Record the exact input, relevant settings, output, date, and observations.
- Repeat a test only when repetition answers a defined question.
- Do not cherry-pick outputs.
- Record failures and ambiguous outcomes, not just successful examples.
- Do not bypass safety controls, access controls, or provider restrictions.
- Do not connect an agent to real organisational systems or grant unnecessary permissions.

## Suggested test themes

The themes below are starting points. Adapt them to the capabilities of the selected product and document any change.

### Chatbots

- Factual response to a clearly scoped question
- Handling of missing information
- Citation or source quality, if citations are offered
- Consistency across paraphrased prompts
- Expression of uncertainty
- Response to conflicting instructions
- Privacy-aware handling of a synthetic scenario
- Suitability of output for a defined workplace task

### AI agents

- Understanding a multi-step task
- Planning and sequencing actions
- Correct use of permitted tools or integrations in a sandbox
- Handling an unavailable tool or failed step
- Asking for clarification when instructions are ambiguous
- Requesting approval before consequential actions
- Respecting a restricted scope or permission boundary
- Reporting completed, failed, and unverified actions accurately

If a safe sandbox is unavailable, assess documented capabilities and use a simulated workflow rather than connecting to live systems.

### Image-generation tools

- Following a neutral, clearly specified brief
- Consistency with requested visual elements
- Handling of ambiguous instructions
- Representation errors or unwanted artefacts
- Ability to revise an output
- Transparency about generated content, where available
- Potential for misleading or deceptive use
- Suitability for a defined workplace communication task

### Video-generation tools

- Following a short, neutral scene description
- Consistency with requested sequence and visual details
- Temporal continuity across frames or shots
- Handling of ambiguous instructions
- Visible artefacts or unexpected content
- Revision and control options
- Transparency about generated content, where available
- Potential for misleading or deceptive use

## Evaluation dimensions for each test

Use task-specific criteria, selected before testing. Possible criteria include:

- **Task fulfilment:** did the output address the requested task?
- **Accuracy or fidelity:** was it factually correct or visually faithful to the brief?
- **Consistency:** did comparable inputs produce materially comparable results?
- **Uncertainty handling:** did the tool acknowledge missing information or limitations?
- **Control:** could the user review, correct, reject, or stop the output/action?
- **Risk signal:** did the test reveal a relevant safety, privacy, transparency, or misuse concern?

Use descriptive notes rather than false precision. A simple qualitative scale may be used where useful: Meets expectation, Partly meets, Does not meet, Not applicable, Not tested.

## Test record fields

For every test, record:
- Test ID
- Tool and category
- Date and access tier
- Feature or model/version, if known
- Test objective
- Use-case scenario
- Exact input or prompt
- Relevant settings
- Expected behaviour
- Observed output or action
- Evaluation against criteria
- Evidence label
- Risk or concern identified
- Limitations
- Retest needed (yes/no)

## Reporting results

Separate:
- What the provider claims
- What the project directly observed
- What independent sources report
- What the project infers
- What remains unknown

A test result applies only to the tested configuration, date, prompt, and access tier. Product features and model behaviour may change. Record this limitation in every assessment.

## Safety and ethics

Do not use real personal data, confidential business information, employee records, customer data, or proprietary material. Do not impersonate real people, create deceptive media of identifiable individuals, attempt to defeat safeguards, or test integrations without explicit authorisation.
