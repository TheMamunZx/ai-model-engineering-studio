---
name: ai-model-engineering-studio
description: "Coordinate end-to-end ai model engineering studio workflows from one master skill, loading specialist playbooks as needed."
---

# AI Model Engineering Studio

## Mission
Design reproducible model experiments and training/inference pipelines with data governance, measurable evaluation, and realistic compute constraints.

## Use this skill when
The user asks to create, extend, analyze, or deliver a ai model engineering studio project and expects one coordinated workflow rather than manually selecting individual specialist skills.

## Invocation contract
This is the only selectable skill in this repository. The specialist modules below are internal reference playbooks, not separate skills to invoke. Start from the user's brief, load only relevant references, and coordinate the complete workflow.

## Required inputs
Infer what is clear from the user's brief and repository. Identify only essential missing information. Typical inputs include goal, target users/platform, scope, references, constraints, existing stack, output format, budget, deadline, and acceptance criteria. Ask one concise clarification only when a missing fact blocks safe or correct execution; otherwise state reasonable assumptions and proceed.

## Operating protocol
1. Inspect the current repository, project instructions, files, configuration, and existing conventions before editing.
2. Translate the request into deliverables, explicit assumptions, non-goals, acceptance criteria, and risks.
3. Build a short phased plan. Prefer a working vertical slice over broad scaffolding that does not run.
4. Read the relevant internal references from the map below. Do not load unrelated modules or duplicate work.
5. Discover the actual tools, dependencies, APIs, providers, and runtime capabilities available in the current environment. Never invent tool names, provider availability, model IDs, endpoints, test results, or completed outputs.
6. Implement the requested outcome in the existing project. Preserve working behavior and avoid unnecessary rewrites.
7. Validate with the strongest available automated and manual checks. Fix issues found, then re-run the relevant checks.
8. Report exact files changed, commands/tests executed and results, deliverables created, unresolved issues, and what remains unverified.

## Internal specialist reference map
- `llm-engineer` — read `references/llm-engineer.md` when this capability is needed.
- `neural-network-engineer` — read `references/neural-network-engineer.md` when this capability is needed.
- `machine-learning-engineer` — read `references/machine-learning-engineer.md` when this capability is needed.
- `model-training-engineer` — read `references/model-training-engineer.md` when this capability is needed.
- `computer-vision-engineer` — read `references/computer-vision-engineer.md` when this capability is needed.

## Coordinated workflow
1. Define task, baseline, target metrics, dataset provenance, and compute budget.
2. Inspect data quality, licensing, privacy, splits, leakage risks, and preprocessing.
3. Select model families and baselines justified by evidence and constraints.
4. Create reproducible training and evaluation configurations with fixed seeds where applicable.
5. Track experiments, checkpoints, environment, hardware, and resource use.
6. Evaluate robustness, bias, calibration, latency, memory, and failure cases.
7. Optimize inference only against measured bottlenecks.
8. Document model cards, limitations, data lineage, reproducibility, and deployment requirements.

## Expected deliverables
- experiment plan and baseline
- data and training pipeline
- evaluation results with reproducibility details
- inference profile and optimization report
- model card and deployment notes

## Quality gates
- Requirements map to implemented behavior or clearly documented non-goals.
- The project builds/runs with available dependencies, or blockers are stated with evidence.
- Tests cover critical user flows or critical subsystem invariants.
- Security, privacy, accessibility, performance, and failure states are considered where relevant.
- Documentation matches the delivered implementation.
- No capability is described as complete unless the corresponding artifact exists and has been checked.


## Security, privacy, and rights
- Protect secrets and personal data. Never place API keys, access tokens, passwords, signing keys, or private credentials in source files, prompts, examples, or logs.
- Use only dependencies, media, datasets, and assets with verified rights and compatible licenses.
- Do not claim external APIs, models, services, or tools are configured unless verified in the current environment.

## Approval gates
Ask before paid API/service usage, production deployment, public publication, destructive changes, external account actions, large cloud jobs, or changes that can incur charges. Do not ask for approval for ordinary reversible local edits within the user's requested scope.

## Stop conditions
Stop and explain the blocker when required permissions, credentials, source material, tools, dependencies, or target hardware are unavailable. Continue with independent work where possible, but do not simulate unavailable external generation or claim a final build succeeded.

## Final response format
Summarize: outcome; key implementation; files/artifacts; validation results; required user actions; known limitations. Be explicit about partial completion.
