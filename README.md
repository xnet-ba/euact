# eu-ai-act-article-4 — OpenCode Skill

Enforces **EU AI Act Article 4 (AI literacy)** + Recital 20 of Regulation (EU) 2024/1689
(as amended by the Digital Omnibus on AI). Turns any OpenCode agent into a literacy-aware
assistant: it calibrates to the user's role, explains capabilities and limits, discloses
risks and safeguards, triages prohibited / transparency / high-risk cases, and never
pretends to certify compliance.

**Applies since 2 Feb 2025** to ALL providers and deployers of AI systems — including
trivial uses like ChatGPT for ad copy (staff must know the specific risks, e.g. hallucination).

## What it enforces

- **Role calibration** — developer / deployer / end-user / affected person / SME, plus
  contractors, service providers and clients under the organisational remit
- **Recital 20 four pillars** — DEV (correct technical application), USE (safe-operation
  measures), OUTPUT (how to interpret + verify), IMPACT (rights of affected persons)
- **Commission 4-step programme** (Art. 4 Q&A): general AI understanding → provider/deployer
  role → system risk → differentiated measures incl. legal/ethical aspects
- **Prohibited practices triage (Art. 5)** — incl. NEW 2026 bans: non-consensual intimate
  deepfakes (ba), CSAM generation (bb); refuses + cites
- **Transparency triage (Art. 50)** — chatbot disclosure, machine-readable marking of
  synthetic media, emotion/biometric notices, deepfake disclosure
- **High-risk deployer module (Art. 26)** — instructions, competent oversight, input data,
  monitoring + suspend, 6-month logs, worker notification, FRIA (Art. 27), registration
- **Incident literacy (Art. 73)** — recognise + report serious incidents through the
  provider → MSA chain
- **AI agents covered** — agents are AI systems/GPAI: design safeguards (Art. 5),
  transparency from Aug 2026 (Art. 50), Chapter III if high-risk
- **Myth-busting** — no certificates, no AI Officer, no knowledge measurement,
  instructions-for-use alone are NOT enough, human-in-the-loop alone ≠ compliance
- **AI Literacy Notice** template + training-log template on every AI build/explanation

## Install

Project-local (recommended):

```
.opencode/skills/eu-ai-act-article-4/SKILL.md
```

Global:

```
~/.config/opencode/skills/eu-ai-act-article-4/SKILL.md
```

Claude-compatible mirrors (`.claude/skills/`, `.agents/skills/`) work too. The agent loads
it on demand via the native `skill` tool — no configuration needed.

## Example output

```markdown
**AI Literacy Notice (EU AI Act Art. 4):**
- System: [model/system, version]
- Purpose: [intended use] / Not for: [misuses]
- Limits: [known weaknesses, eval gaps]
- Verify: [how to check output]
- Oversight: [human checkpoint required]
- Affected: [who impacted, rights + contest path]
- Risk tier: [minimal / transparency Art.50 / high-risk candidate / prohibited Art.5]
```

## Key dates

| Date | Milestone |
|---|---|
| 02.02.2025 | Art. 4, prohibitions apply |
| 02.08.2025 | GPAI obligations, governance |
| 02.08.2026 | Art. 50 transparency; enforcement starts (AI Office / EDPS / national MSAs) |
| 02.12.2026 | New prohibitions Art. 5(ba)(bb); Art. 50(2) transition ends |
| 02.12.2027 | High-risk Annex III rules |
| 02.08.2028 | High-risk Annex I (embedded products) rules |

## Legal sources

- Article 4: https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-4
- AI Literacy Q&A: https://digital-strategy.ec.europa.eu/en/faqs/ai-literacy-questions-answers
- Living repository (learning only, no presumption of compliance): https://digital-strategy.ec.europa.eu/en/library/living-repository-foster-learning-and-exchange-ai-literacy
- Transparency Guidelines (Art. 50): https://ai-act-service-desk.ec.europa.eu/en/resources
- Compliance Checker (beta): https://ai-act-service-desk.ec.europa.eu/en/eu-ai-act-compliance-checker
- Official Regulation: https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng
- Digital Omnibus: https://eur-lex.europa.eu/eli/reg/2026/1744/oj

## Versions

- **v3.0.0** — Art. 26 module, incident literacy, enforcement split, Art. 4a, SME/sandboxes, staleness rule
- **v2.0.0** — Art. 3(56) definition, 4-step programme, Art. 5(ba)(bb), Art. 50 triage, agents, timeline
- **v1.0.0** — Initial literacy enforcer

## License

MIT. Summaries are not legally binding. Verify with legal counsel.
