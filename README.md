# sales-engineering-skills

Six Agent Skills for sales engineers, presales engineers and solutions consultants working complex B2B software deals. Each skill is a working procedure an agent runs with you on a live deal. It asks for the inputs it needs, walks through the steps, produces a filled template or table, and applies checks that separate a confirmed answer from an assumption.

The skills use the SKILL.md format read by Claude Code, Claude.ai and Codex: one folder per skill, with YAML frontmatter (`name`, `description`) followed by instructions. The description tells the agent when to pick the skill up.

## Skills

| Skill | What it does | Based on |
|---|---|---|
| [proof-of-value-plan](skills/proof-of-value-plan/SKILL.md) | Plans a Proof of Value from agreed business outcomes to success criteria, the go or no-go, the pilot agreement check and the readout. | [What is a Proof of Value](https://topmoller.com/articles/what-is-a-proof-of-value/), [Proof of concept vs pilot](https://topmoller.com/articles/proof-of-concept-vs-pilot-agreement/) |
| [meddicc-qualification](skills/meddicc-qualification/SKILL.md) | Qualifies an opportunity with MEDDICC as evidence claims: questions per element, Metrics chains, decision criteria, paper process. | [MEDDICC questions](https://topmoller.com/articles/meddicc-questions-and-what-counts-as-an-answer/), [Metrics](https://topmoller.com/articles/metrics-in-meddicc-product-numbers-and-business-numbers/), [Decision criteria](https://topmoller.com/articles/meddicc-decision-criteria-examples-written-by-buyers/), [Paper process](https://topmoller.com/articles/meddpicc-paper-process/) |
| [business-value-assessment-interviews](skills/business-value-assessment-interviews/SKILL.md) | Plans stakeholder interviews for a Business Value Assessment and turns them into a business case, roadmap and proof criteria. | [Stakeholder interviews in a BVA](https://topmoller.com/articles/business-value-assessment-run-as-interviews/) |
| [mutual-action-plan](skills/mutual-action-plan/SKILL.md) | Builds and reviews a mutual action plan with named owners, owner-confirmed dates and graded evidence per step. | [Mutual action plan](https://topmoller.com/articles/mutual-action-plan-what-it-holds-and-proves/) |
| [pre-call-plan](skills/pre-call-plan/SKILL.md) | Prepares a first enterprise meeting with the account executive in three rows: technical, business value and qualification. | [Pre-call planning](https://topmoller.com/articles/pre-call-planning-first-enterprise-software-meeting/) |
| [stage-exit-criteria](skills/stage-exit-criteria/SKILL.md) | Writes or audits stage gates so each requires a recorded customer act tied to a MEDDICC element. | [Stage exit criteria](https://topmoller.com/articles/sales-stage-exit-criteria-examples/) |

## Install

Claude Code: copy a skill folder into `~/.claude/skills/` to use it everywhere, or into `.claude/skills/` inside a project to use it there.

```sh
cp -r skills/mutual-action-plan ~/.claude/skills/
```

Claude.ai: zip a skill folder and upload it in Settings > Capabilities > Skills.

```sh
cd skills && zip -r mutual-action-plan.zip mutual-action-plan
```

Codex and other agents that read SKILL.md: place the folder under that agent's skills directory.

## About

Written by Jacob Top Møller, who trains and advises sales engineers. More at https://topmoller.com/articles/ .

## License

MIT. See [LICENSE](LICENSE).
