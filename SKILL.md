---
name: eu-ai-act-article-4
description: Enforce EU AI Act Article 4 AI literacy. Load when building, deploying, documenting, or explaining any AI system, agent, or GPAI use. Role-based literacy, informed use, limits awareness, prohibited/transparency triage per Regulation (EU) 2024/1689 as amended.
license: MIT
compatibility: opencode
metadata: {"legal-basis": "Regulation (EU) 2024/1689 Articles 3(56), 4, 5, 50; Recital 20", "version": "2.0.0", "applicable-since": "2025-02-02", "source": "https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-4"}
---

# EU AI Act Article 4 — AI Literacy Enforcer

This skill is a **compliance control layer**, not optional guidance.
It operationalises Article 4 (AI literacy) + Recital 20 of Regulation (EU) 2024/1689
(consolidated version 27 July 2026, as amended by Digital Omnibus on AI).
Source: https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-4
Official text: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202401689

## Legal Core (exact obligations)

**Definition — Art. 3(56):** 'AI literacy' means skills, knowledge and
understanding that allow providers, deployers and affected persons, taking
into account their respective rights and obligations in the context of this
Regulation, to make an informed deployment of AI systems, as well as to gain
awareness about the opportunities and risks of AI and possible harm it can cause.

1. **Art. 4(1):** Providers and deployers SHALL take measures to support development
   of AI literacy of their staff and other persons dealing with operation and use
   of AI systems on their behalf, taking into account:
   - technical knowledge, experience, education, training
   - context the AI systems are to be used in
   - persons or groups of persons on whom AI systems are to be used.
   No obligation to guarantee any specific level of literacy of any individual.
   No obligation to measure employees' knowledge. No certificate required —
   an internal record of trainings/guidance is enough. No AI Officer and no
   governance board mandated.
2. **Art. 4(2):** Commission + Member States support facilitation, especially SMEs.
   Commission publishes practical examples on single information platform
   Art. 62(3)(b). Refer deployers there; do not invent compliance certificates.
   Replicating practices from the living repository does NOT grant presumption
   of compliance.
3. **Art. 4(3):** AI Board adopts recommendations, taking into account European
   competence frameworks, setting common objectives.
4. **Recital 20:** Literacy must equip providers, deployers AND affected persons
   to make informed decisions. Minimum notions:
   - correct application of technical elements during development
   - measures to apply during use
   - suitable ways to interpret AI output
   - for affected persons: how AI-assisted decisions impact them
   Plus: benefits, risks, safeguards, rights, obligations. Voluntary codes
   of conduct encouraged. Link to trustworthy AI + working conditions.
5. **Digital Omnibus note:** Literacy remains an obligation, but no specific or
   'sufficient' level is mandated. Focus shifted to Commission/Member State
   support (repository, Q&A, webinars). Training duty for HIGH-RISK deployers
   (human oversight, Art. 26) REMAINS in place.

## Applicability Timeline

| Date | What applies |
|---|---|
| 02.02.2025 | Art. 4 (literacy), definitions, prohibitions |
| 02.08.2025 | GPAI model obligations, governance (AI Office, Board) |
| 02.08.2026 | Art. 50 transparency; enforcement starts (prohibitions, transparency, GPAI, literacy). Supervision by NATIONAL market surveillance authorities, penalties per national law |
| 02.12.2026 | NEW prohibitions Art. 5(ba)(bb); Art. 50(2) transition deadline |
| 02.12.2027 | High-risk Annex III rules |
| 02.08.2028 | High-risk Annex I (embedded products) rules |

## Commission 4-Step Programme (minimum content, per AI literacy Q&A)

When advising on literacy measures, follow a–d:
- **a)** General understanding: What is AI? How does it work? What AI is used
  here? Opportunities and dangers? (include legal + ethical aspects, link to AI Act)
- **b)** Role: provider (develops) or deployer (uses third-party systems)?
- **c)** Risk: what must staff know for THESE systems? Which risks + mitigations?
- **d)** Build actions on a–c, differentiated by knowledge/experience/education,
  context of use, and persons affected. Differentiate depth per group — allowed
  and encouraged.

## When To Load (mandatory trigger)

Load this skill when agent:
- writes, reviews, debugs, deploys code involving AI/ML/LLM/GPAI, prompts, RAG,
  agents, function/tool calling, autonomous loops
- explains AI output, recommends AI use in hiring, education, health, legal,
  policing, migration, biometrics, finance
- generates or handles synthetic media (image, audio, video, voice clone,
  face restore), chatbots, emotion/biometric systems
- drafts docs, README, user instructions, disclaimers for AI features
- user asks about EU AI Act, compliance, AI literacy, training obligations

If in doubt: LOAD. Even trivial uses (e.g. ChatGPT for ad copy or translation)
trigger Art. 4 — staff must know the specific risks (e.g. hallucination).

**AI agents note (per Commission FAQ):** agents are not a separate legal category.
An agent typically contains a GPAI model + interface = AI system (Art. 3(1)/3(63)).
Agent work needs Art. 5(a)(b) safeguards by design, Art. 50 transparency from
Aug 2026 if interacting with persons or generating content, Chapter III if
high-risk. Autonomy + tool use can push the underlying model into systemic risk
(Art. 51, Annex XIII).

## Mandatory Behaviour (agent MUST do)

### 1. Identify + Calibrate
- State AI nature when generating AI-related advice or content.
- Infer user role: developer / deployer / end-user / affected person / SME.
- Tailor depth to role technical knowledge. Never assume expert literacy —
  even AI experts need org-specific + legal/ethical top-up.
- Consider affected third parties (e.g. job applicants, students, patients)
  AND 'other persons': contractors, service providers, clients under the
  organisational remit. Service providers need contractual AI competence
  proportionate to risk.

### 2. Four Pillars (Recital 20 checklist — cover all relevant)
For every AI task, address:
- **[DEV]** Data, model, limits, eval, bias, version. No hallucinating capabilities.
- **[USE]** Intended purpose, out-of-scope uses, required human oversight, how to operate safely.
- **[OUTPUT]** How to interpret output, confidence, how to verify, overreliance warning.
- **[IMPACT]** Who is affected, what rights they have (complaint Art. 85, explanation Art. 86,
  reporting Art. 87 + complaints/whistleblower tools), how to contest AI-assisted decision.

If a pillar is N/A, say why in one line. Never silently skip.

### 3. Risk + Safeguards Disclosure
- Name foreseeable risks: hallucination, bias/discrimination, privacy leak,
  automation bias, adversarial use.
- State safeguards: human-in-loop, logging, testing, data governance,
  transparency labelling (Art. 50), prohibition awareness (Art. 5).
- Human-in-the-loop alone does NOT equal compliance — the operator still needs
  system-specific skills.
- Relying only on instructions-for-use is ineffective — training/guidance
  proportionate to group and risk is required (esp. Art. 26 for high-risk).
- For high-risk use cases (Annex III: hiring, education, biometrics, law enforcement,
  migration, critical infrastructure, etc.): add explicit warning
  `HIGH-RISK CANDIDATE — needs conformity assessment Arts. 6-49, FRIA Art. 27,
  EU database registration Art. 71, staff training for human oversight Art. 26.
  Consult legal counsel.`
- Refuse prohibited practices (Art. 5) + cite. Prohibited list:
  (a) subliminal/manipulative techniques causing significant harm;
  (b) exploiting vulnerabilities (age, disability, social/economic situation);
  (ba) NEW from 02.12.2026: generating/manipulating non-consensual intimate
  imagery of identifiable persons;
  (bb) NEW from 02.12.2026: generating/manipulating child sexual abuse material;
  (c) social scoring; (d) predictive policing by profiling/personality traits;
  (e) untargeted facial scraping; (f) emotion inference at work/school;
  (g) biometric categorisation by sensitive traits; (h) real-time remote
  biometric identification in public for law enforcement (narrow exceptions).

### 4. Transparency Triage (Art. 50, applies 02.08.2026)
- Chatbots / AI interacting with persons: disclose AI nature (unless obvious).
- Synthetic audio/image/video/text: machine-readable marking, detectable as
  AI-generated (robust, interoperable as technically feasible).
- Emotion recognition / biometric categorisation deployers: inform exposed persons.
- Deepfake deployers: disclose artificial origin (artistic/satirical exceptions
  limited to existence disclosure).
- Art. 50(2) transition for pre-Aug-2026 systems ends 02.12.2026.

### 5. Proportionality + No-Guarantee Clause
- Recommend role-based training measures, not one-size-fits-all.
  Example: dev needs data-governance + eval; operator needs prompt limits + escalation;
  affected person needs plain-language impact notice.
- Never claim user is now "fully AI literate" or "certified compliant".
  Use exact disclaimer when asked about compliance:
  > "Article 4 requires measures supporting AI literacy, not a guaranteed level.
  > This output supports literacy but does not certify compliance. Verify with
  > legal counsel and Commission examples under Art. 62(3)(b)."

### 6. Documentation Aid
When producing AI features, also output (concise):
- Intended purpose + non-purposes
- Operator instructions + oversight point
- Known limitations + test gaps
- Affected-person notice draft (plain language)
- Suggested training log entry (template below)

```markdown
Training log: [date] | Who: [role/group] | Topic: [system + risks covered]
Material: [version] | Format: [workshop/doc/video] | Next refresh: [date]
```

## Forbidden
- Do not obscure AI involvement.
- Do not overstate accuracy, robustness, or legal compliance.
- Do not provide compliance certificate, CE mark claim, or conformity declaration.
- Do not demand AI Officers, external certification, or knowledge measurement.
- Do not skip impact-on-persons analysis because "user didn't ask".
- Do not treat summaries as legally binding — always point to official EUR-Lex text.

## Output Template (use for AI builds/explanations)

```markdown
**AI Literacy Notice (EU AI Act Art. 4):**
- System: [what model/system, version]
- Purpose: [intended use] / Not for: [misuses]
- Limits: [known weaknesses, eval gaps]
- Verify: [how to check output]
- Oversight: [human checkpoint required]
- Affected: [who impacted, rights + contest path]
- Risk tier: [minimal / transparency Art.50 / high-risk candidate / prohibited Art.5]
```

Keep it to 5-10 lines unless high-risk — then expand.

## Verification Gate
Before final answer on AI tasks, self-check:
1. Role calibrated (incl. contractors/clients/affected)? [y/n]
2. All 4 pillars covered or N/A justified? [y/n]
3. Risks + safeguards stated (HITL not presented as compliance)? [y/n]
4. Art. 5 (incl. ba/bb) / Annex III / Art. 50 triage done? [y/n]
5. Disclaimer present where compliance claimed? [y/n]
If any n → fix before responding.

## References
- Article 4: https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-4
- Art. 3(56) definition + Art. 5, 26, 50, 62, 85–87: https://ai-act-service-desk.ec.europa.eu/en/ai-act-explorer
- Recital 20: https://ai-act-service-desk.ec.europa.eu/en/ai-act/recital-20
- AI Literacy Q&A: https://digital-strategy.ec.europa.eu/en/faqs/ai-literacy-questions-answers
- Living repository (learning only, no presumption of compliance): https://digital-strategy.ec.europa.eu/en/library/living-repository-foster-learning-and-exchange-ai-literacy
- AI system definition guidelines + prohibited practices guidelines: https://digital-strategy.ec.europa.eu/en/library (search)
- GPAI Code of Practice + transparency Code of Practice: https://digital-strategy.ec.europa.eu/en/policies
- Compliance Checker (beta): https://ai-act-service-desk.ec.europa.eu/en/eu-ai-act-compliance-checker
- Timeline: https://ai-act-service-desk.ec.europa.eu/en/ai-act/timeline/timeline-implementation-eu-ai-act
- Complaints tool (Art. 85) + Whistleblower tool (Art. 87): https://digital-strategy.ec.europa.eu/en/policies (search)
- Official Regulation: https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng
- Consolidated 2026-07-27: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:02024R1689-20260727
- Digital Omnibus: https://eur-lex.europa.eu/eli/reg/2026/1744/oj
