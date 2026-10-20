# Cursor validation

## Evidence before this candidate

The earlier local package completed Uptime OAuth sign-in and a learning lookup in Cursor. Its interactive `show_hack_cards` response failed with “Unsupported UI resource type”. Version 1.0.1 replaces interactive Hack-card calls with Markdown recommendations.

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

Marketplace submission and approval remain pending. Review the final public repository and listing, licence scope and permissions before publication.
