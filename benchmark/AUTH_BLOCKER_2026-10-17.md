# SNATCHER one-shot benchmark — execution status (2026-10-17)

**State: NOT EXECUTED.** This note is an authentication/network audit, not a port result.

## Working
- Ghidra 12.1.4, REA 6.4.0, Node 24.18.0 and Codex CLI 0.163.0 installed in a local Linux workspace.
- REA MCP integration previously validated (170/170 tools).
- Original SNATCHER ISO staged privately, never in this public repository.
- One-shot instruction saved at [ONESHOT_PROMPT.md](./ONESHOT_PROMPT.md).

## Exact blockers
1. The local sandbox cannot resolve external hosts (api.openai.com, auth.openai.com, github.com), so Codex CLI cannot connect to a model even after a potential login.
2. Codex CLI has no independent model authentication. The ChatGPT/GitHub connector is separate from CLI model credentials.
3. A network-capable GitHub Actions probe with models:read did not demonstrate GitHub Models inference. The request to https://models.github.ai/inference/chat/completions returned HTTP 200, content-type text/plain, body "OK" followed by CRLF, **not model output**. Diagnostic retry confirmed it.
4. The game ISO has not been sent to an authenticated remote agent. Do not upload it to this public repository.

## Evidence
- [First model-access probe](https://github.com/nickdjanuary-bit/Nonlocality/actions/runs/39081016432)
- [Model-access diagnostic retry](https://github.com/nickdjanuary-bit/Nonlocality/actions/runs/39081072243)
- [Codex installation build](https://github.com/nickdjanuary-bit/Nonlocality/actions/runs/39079713464)

## Decision
Stop unauthenticated network probes. A valid one-shot benchmark requires **one authenticated network-capable agent with private access to the original game image**. No agent inference, port generation, or gameplay validation has occurred yet.
