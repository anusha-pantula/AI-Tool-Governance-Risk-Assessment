# Provider evidence register

**Research snapshot:** 12 November 2026  
**Scope:** Public provider documentation reviewed for the four selected products. This is desk research, not independent verification of provider claims.  
**Evidence status:** Provider statement unless explicitly marked otherwise.

## ChatGPT — OpenAI

| Topic | Documented information | Governance relevance | Source |
|---|---|---|---|
| Consumer data controls | Personal ChatGPT users can manage whether eligible conversations are used to improve models through Settings → Data Controls → “Improve the model for everyone”. Availability may depend on account and workspace settings. | An organisation should verify the actual account/workspace configuration and not assume consumer defaults match managed-workspace defaults. | [OpenAI Data Controls FAQ](https://help.openai.com/en/articles/7730893-data-controls-in-chatgpt) |
| Temporary Chat | Temporary Chats do not appear in chat history and are not used to improve models while temporary; OpenAI may retain a copy for up to 30 days for safety purposes. | Temporary Chat is not equivalent to zero retention. Retention and access requirements still need review. | [Temporary Chat](https://help.openai.com/en/articles/8914046-temporary-chat-in-chatgpt) |
| Business data | OpenAI states that ChatGPT Business, Enterprise, Edu and API inputs/outputs are not used to train models by default, subject to applicable terms and settings. | Product tier and contract matter. Do not generalise personal-account settings to business workspaces. | [How your data is used to improve model performance](https://help.openai.com/en/articles/5722486-how-your-data-is-used-to-improve-model-performance) |

**Not established by this desk review:** the user's precise account data-control setting, retention configuration, or the suitability of ChatGPT for any particular organisational data classification.

## Zapier Agents — Zapier

| Topic | Documented information | Governance relevance | Source |
|---|---|---|---|
| Agent capabilities | Agents can perform tasks independently or in response to user interaction, use app actions and answer questions using connected knowledge sources. | Agent autonomy and connected permissions expand the potential impact of errors compared with a read-only chatbot. | [Build an agent in Zapier Agents](https://help.zapier.com/hc/en-us/articles/24393442652557-Build-an-agent-in-Zapier-Agents) |
| Configuration and publishing | Provider instructions describe configuring triggers, actions and knowledge sources, testing an agent, and publishing it to activate it. | Separate test and production states; publishing should be a deliberate approval step. | [Build an agent in Zapier Agents](https://help.zapier.com/hc/en-us/articles/24393442652557-Build-an-agent-in-Zapier-Agents) |
| Knowledge sources | Agents can use supported files and connected apps as knowledge sources; the documentation describes sync behaviour and search actions. | Stale or incorrect source content can lead to incorrect answers or actions. Source ownership and refresh cadence should be governed. | [Add your own data to an agent](https://help.zapier.com/hc/en-us/articles/24569690575117-Add-your-own-data-to-an-agent) |
| Account transition | Zapier's documentation states that it is moving Agents to AI by Zapier. | Product continuity, feature availability and migration status should be verified before relying on this product for a long-term workflow. | [Zapier Agents help article](https://help.zapier.com/hc/en-us/articles/24393442652557-Build-an-agent-in-Zapier-Agents) |

**Not established by this desk review:** the user's exact free-tier activity allowance, enabled actions, connected-app permissions, approval controls, or migration availability in their account. These require direct account inspection.

## Adobe Firefly — Adobe

| Topic | Documented information | Governance relevance | Source |
|---|---|---|---|
| Training-data description | Adobe says its initial commercial Firefly model was trained on Adobe Stock images, openly licensed content and public-domain content where copyright has expired. | Provider-described training sources are relevant to intellectual-property risk, but are not a guarantee that every output is non-infringing or legally safe in every jurisdiction. | [Adobe Firefly FAQ](https://helpx.adobe.com/firefly/web/get-started/learn-the-basics/adobe-firefly-faq.html) |
| Customer content | Adobe says it does not train Firefly on Creative Cloud subscribers' personal content. | This is a provider statement; the relevant product, account type and applicable terms must be checked. | [Adobe Firefly FAQ](https://helpx.adobe.com/firefly/web/get-started/learn-the-basics/adobe-firefly-faq.html) |
| Content provenance | Adobe describes Content Credentials as metadata that can communicate information such as creation date, tools used and edits; certain Firefly exports automatically include credentials indicating AI use. | Provenance metadata can support disclosure, but users should check whether a particular export actually retains it. | [Adobe Firefly FAQ](https://helpx.adobe.com/firefly/web/get-started/learn-the-basics/adobe-firefly-faq.html) |
| Legal caution | Adobe notes that generative-AI laws are evolving and recommends seeking local legal advice for copyright questions. | Avoid presenting the product's “commercially safe” positioning as a legal conclusion for all outputs and jurisdictions. | [Adobe Firefly FAQ](https://helpx.adobe.com/firefly/web/get-started/learn-the-basics/adobe-firefly-faq.html) |

**Not established by this desk review:** the user's current model selection, available features, remaining generative credits, exact export metadata, or rights applicable to a particular generated asset.

## Runway — Runway

| Topic | Documented information | Governance relevance | Source |
|---|---|---|---|
| Free-plan credits | Runway's help article states that the Free plan includes a one-time deposit of 125 credits that does not expire. Rates vary by tool/model. | A fixed credit allowance constrains the number of repeatability tests; record the balance and displayed cost before generation. | [How do credits work?](https://help.runwayml.com/hc/en-us/articles/15124877443219-How-do-credits-work) |
| Current Gen-4.5 access | Runway's Gen-4.5 guide lists Standard and higher as the plan requirement, at 12 credits per second, with 2–10 second durations. | Do not assume the user's free account can access Gen-4.5. Record the model actually available in the account. | [Creating with Gen-4.5](https://help.runwayml.com/hc/en-us/articles/46974685288467-Creating-with-Gen-4-5) |
| Older Gen-4 model | Runway documents Gen-4 as image-to-video with 5- or 10-second durations; its Turbo version uses fewer credits than Gen-4. | Model version and input requirements materially affect cost and what is being tested. | [Creating with Gen-4 Video](https://help.runwayml.com/hc/en-us/articles/37327109429011-Creating-with-Gen-4-Video) |
| Content moderation | Runway says its moderation system scans inputs and generated outputs against its Usage Policy and cannot be disabled for an account, project or topic. | Moderation is a control, but users should understand its scope, false positives and appeal/operational implications. | [Why is my input getting content moderated?](https://help.runwayml.com/hc/en-us/articles/21745792516371-Why-is-my-input-getting-content-moderated) |

**Not established by this desk review:** the user's exact available model, credit balance, cost for their selected settings, watermark/export conditions, or data retention and model-training terms. Check the signed-in account and current terms before testing.

## Research limitations

- These are provider-authored sources and are not independent audits.
- Product interfaces, model availability, plan limits and policies can change. Re-check them on the date of each practical test.
- The project does not infer that provider statements are independently verified.
- No legal conclusion is made about copyright, privacy, data protection or regulatory compliance.

## Governance reference points

- [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) — voluntary framework for incorporating trustworthiness considerations into AI design, development, use and evaluation. NIST notes that AI RMF 1.0 is being revised.
- [OECD AI Principles](https://www.oecd.org/en/topics/sub-issues/ai-principles.html) — updated in 2024; includes transparency, robustness, security, safety and accountability.
