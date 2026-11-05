<div align="center">

# AI Model Engineering Studio

**A coordinated workflow for machine learning, neural networks, LLMs, training, evaluation, and inference.**

`1 Master Skill` · `5 Internal Modules` · `Claude Code` · `OpenCode`

</div>

---

## About

Design reproducible model experiments and training/inference pipelines with data governance, measurable evaluation, and realistic compute constraints.

This repository exposes one discoverable skill: `ai-model-engineering-studio`. Specialist playbooks live inside that skill's `references/` directory and are loaded by the master workflow as needed. You do not select each module separately.

## Quick start

### Project-local use

Copy this repository's `.claude/skills/ai-model-engineering-studio/` folder into the target project's `.claude/skills/` directory. Then invoke the master skill from your compatible coding agent.

### Claude Code

```text
/ai-model-engineering-studio
```

### OpenCode

```text
@ai-model-engineering-studio
```

Agent discovery behavior can vary by installed version and configuration. Confirm the skill appears in the agent's available skill list before relying on it.

## Internal specialist modules

| Module | Role |
|---|---|
| `llm-engineer` | Internal specialist reference |
| `neural-network-engineer` | Internal specialist reference |
| `machine-learning-engineer` | Internal specialist reference |
| `model-training-engineer` | Internal specialist reference |
| `computer-vision-engineer` | Internal specialist reference |

## Repository layout

```text
ai-model-engineering-studio/
├── .claude/skills/ai-model-engineering-studio/
│   ├── SKILL.md
│   ├── references/
│   ├── scripts/
│   ├── templates/
│   └── assets/
├── scripts/
├── README.md
├── README_BN.md
└── AGENTS.md
```

## Validation

Run: `python scripts/validate_pack.py`

The validator checks the master skill, expected reference files, frontmatter, basic link integrity, and accidental secrets. It does not prove provider/API availability or guarantee production behavior.

## Safety and service requirements

This repository contains agent instructions, reference playbooks, templates, and helper scripts. It is not itself a model, API subscription, cloud runtime, media-generation engine, or deployment service. Actual capabilities depend on tools, credentials, permissions, provider terms, quotas, dependencies, and hardware configured in your environment. Never commit secrets.

## Contribution and updates

Keep the master skill as the sole discoverable entry point. Add new specialist knowledge as internal references unless there is a deliberate decision to expose a new independent skill. Update the manifest and validation checks whenever modules change.
