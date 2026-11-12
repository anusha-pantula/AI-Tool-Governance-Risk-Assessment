# AI Tool Governance & Risk Assessment Framework

An evidence-based, repeatable framework for assessing AI tools in general organisational settings.

## Project dashboard

**[Open the interactive project dashboard](https://anusha-pantula.github.io/AI-Tool-Governance-Risk-Assessment/)**

The dashboard is the visual entry point to the project. It summarises the selected tools, assessment dimensions, evidence approach and current testing status. It is updated as documented assessments are completed.

The first practical observations are documented in [ChatGPT initial practical results](assessments/chatbot-chatgpt/initial-practical-results.md). The [provider evidence register](research/provider-evidence-register.md) records provider statements and source links.

## Project purpose

AI tools can create value, but their suitability depends on what they are used for, what information they process, who relies on their outputs, and what oversight is in place. This project develops a practical way to examine those factors before and during organisational adoption.

## Selected tools

1. **Chatbot:** ChatGPT
2. **AI agent:** Zapier Agents
3. **Image generation:** Adobe Firefly
4. **Video generation:** Runway

The project owner has confirmed free access to all four selected tools. Exact feature availability, model/version, and usage quotas will be recorded before practical testing.

See [tool selection and access checks](research/tool-selection-and-access-checks.md).

## Assessment approach

Each selected tool will be examined across seven dimensions:

1. Purpose and capabilities
2. Reliability and performance
3. Safety and misuse
4. Privacy and data handling
5. Transparency and accountability
6. Human oversight and control
7. Organisational suitability and safeguards

The common criteria are operationalised in [Common AI tool assessment criteria](methodology/common-assessment-criteria.md). The work combines provider documentation, independent sources, practical observations using non-sensitive inputs, a qualitative risk register, and adoption recommendations.

## Evidence discipline

Findings will distinguish between provider statements, independent sources, project observations, inferences, and unknown or unverified information. Provider claims will not be presented as independently verified results. Limited project tests will not be described as comprehensive benchmarks, security audits, or proof of safety.

## Boundaries

This is an educational and research portfolio project. It is not a legal opinion, formal certification, regulatory compliance assessment, penetration test, or security audit. It will not use confidential or personal data, bypass safeguards, or test systems without authorisation.

## Current status

**Dashboard prototype created.** Project design and initial tool selection are complete. Provider documentation has been reviewed and recorded. Four ChatGPT test cases have been executed and documented; the remaining ChatGPT privacy-control check and practical tests for Zapier Agents, Adobe Firefly and Runway are still pending. No overall tool ranking or adoption recommendation has been assigned.

## Repository structure

- `index.html`: dashboard entry point
- `assets/`: dashboard styling and interactions
- `methodology/`: scope, assessment framework, criteria, methods and [practical test execution guide](methodology/practical-test-execution-guide.md)
- `templates/`: reusable assessment and tracking templates
- `assessments/`: tool-specific assessment notes and practical results
- `research/provider-evidence-register.md`: sourced provider documentation and governance implications
- `templates/test-case-catalogue.csv`: 20 planned test cases and recorded execution status
- `templates/initial-risk-register.csv`: preliminary evidence-linked risk register
- `research/`: tool selection, access checks and sources
- `findings/`: cross-tool comparison and recommendations
