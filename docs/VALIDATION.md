# Cursor validation

## Evidence before this candidate

The earlier local package completed Uptime OAuth sign-in and a learning lookup in Cursor. Its interactive `show_hack_cards` response failed with “Unsupported UI resource type”. Version 1.0.1 replaces interactive Hack-card calls with Markdown recommendations.

## Version 1.0.3 preparation — 21 October 2026

The Cursor candidate uses the exact Academy skill and both references from
approved source commit `4894d9ec35ea2ec95e26b4e805b239188e385a7c`. The shared
skill includes native-host cover/link delivery and connection guidance.
The native Cursor MCP declaration still points to the production endpoint;
it contains no registered owner app binding or embedded credentials.

Static checks passed: JSON parsing, manifest paths, relative skill references,
byte-for-byte source parity, unchanged native MCP declaration, an obvious
credential-pattern scan and `git diff --check`.

### Exact-candidate CLI check

The candidate was loaded with Cursor Agent `v2026.10.19-6bbf2c4`,
`--plugin-dir /Users/jamestrue/.codex/worktrees/academy-cursor-current` and
`--model composer-2.5`, from an existing authenticated isolated test workspace.
The prompt was: “Uptime Academy: What can I learn from Atomic Habits?”
Cursor visibly read this candidate's `skills/academy/SKILL.md`.

It called the existing test server's `learning_brief` with
`reference_title: "Atomic Habits"`, followed by `show_hack_cards` for the selected
Hack. Each call was approved using **Run (once)**. No force, automatic MCP
approval or persistent tool allowlist was used.

The final reply identified Uptime's Atomic Habits teaching, explained the
cue/craving/response/reward loop and four laws, and gave concrete examples.
It included Markdown referring to this cover:
`https://images-na.ssl-images-amazon.com/images/P/0735211299.01._SCLZZZZZZZ_.jpg`
and this exact Hack link:
`https://to.uptime.app/OqcSfUPhm7b?$deeplink_path=hack/1300b5d1-c0e2-53bb-8e23-a3c47ecb4893`.
It ended with an application question about which habit to build next.
The answer also reused existing authenticated learner context about reading
for two minutes after brushing teeth; that detail was not supplied in this prompt.

**Proved:** exact candidate skill loading and an authenticated tool-backed
named-Hack answer containing cover Markdown, a direct link and an application
question. **Limits:** the existing separately configured MCP connection supplied
the tools; this does not prove the plugin's own fresh MCP sign-in. Terminal
output does not prove image rendering. The Hack destination was not opened.
The extra card call occurred despite the skill's native-host preference for
using already returned metadata; this run does not establish why it was needed.
Fresh-recipient installation, native desktop/mobile rendering and marketplace
approval remain unproved. An initial run from the candidate repository lacked
the authenticated test namespace and was stopped; it is not passing evidence.

## Version 1.0.2 connection correction — 21 October 2026

Version 1.0.2 adds connection-before-coaching guidance, three setup steps and
learner-facing privacy wording without internal worker or queue names. Packaged
instructions remain readable; user/workspace files remain outside the learning
workflow. The hosted endpoint and Markdown recommendation approach are unchanged.
No fresh-recipient or model retest was run for this correction. The live evidence
below applies to version 1.0.1, not a completed test of version 1.0.2.

## Static candidate checks

JSON, referenced package paths, the intended file inventory and absence of obvious credential strings passed local checks. These checks do not establish marketplace acceptance or cover every live behaviour.

## Live candidate check — 21 October 2026

Version 1.0.1 loaded in a fresh Cursor chat, “Atomic Habits learning”, using GPT-5.6 Sol Medium in No Repo / This Mac mode. Cursor showed one skill, ten MCP tools and one resource. The existing Uptime OAuth connection remained connected; a fresh sign-in flow was not repeated.

Test prompt:

> Uptime Academy, what can I learn from Atomic Habits? Show its genuine cover and direct Hack link. Use your installed academy skill. This is a test: do not save memory or inspect workspace files beyond that plugin skill and its reference. Keep it short.

The response completed in 15 seconds. Cursor reported two files explored, one search and one tool call. It displayed a short habits summary, a visually rendered genuine cover and this clickable [Atomic Habits Hack link](https://to.uptime.app/D1zON54sF6b?$deeplink_path=hack/1300b5d1-c0e2-53bb-8e23-a3c47ecb4893). No “Unsupported UI resource type” error appeared.

**Passed:** fresh candidate named-Hack lookup and cover/link display. The link's destination was not clicked or tested in this run. The prompt requested no memory save and restricted file inspection; this observation is not a general privacy or workspace-isolation certification.

## Optional regression plan

The following broader behaviours have not been tested in this candidate run:

1. Repeat authentication from a disconnected state and confirm a library lookup succeeds.
2. Ask for GitHub help with no role or goal; confirm one useful clarification, then tailored retrieval and help. Never exceed three clarification turns.
3. Test a non-AI topic, a Spanish request and a third-person situation without transferring account-owner facts.
4. Inspect, save and clear only explicitly shared non-sensitive learner facts; confirm the actual tool result before claiming success.
5. Check Academy call arguments for workspace files or editor context and confirm no website/coding task is executed.
6. Test missing-cover text fallback and click a returned Hack link to verify its actual destination and membership behaviour.

On 21 October 2026, the client-only repository was made public with the approved MIT licence scope, and Cursor acknowledged receipt of the marketplace application: “Thanks for applying” and “We've received your submission.” Marketplace review, approval and listing remain pending.
