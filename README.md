# Kaya Lopez

I build small software tools for AI workflows, automation, and launch safety.

Current public project: AI Agent Launch Pack

- [AI Agent Launch Pack](https://ai-launch-risk-check-public.vercel.app/) - a $25 launch-safety kit for one tool-using AI workflow, MCP server, browser automation flow, or customer-visible agent action.
- [Buy the digital pack](https://ai-launch-risk-check-public.vercel.app/checkout-after-scope.html#digital-pack) - use this when you are shipping one agent workflow this week and need templates, local tools, and launch evidence today.
- [Free 5-minute risk score](https://ai-launch-risk-check-public.vercel.app/risk-score.html) - check one AI workflow before launch without uploading code, secrets, screenshots, or customer data.
- [MCP trust verification generator](https://ai-launch-risk-check-public.vercel.app/mcp-trust-verification-generator.html) - build server identity, manifest, mutating-tool, approval, and redacted-evidence checks.
- [AI Agent Launch Tools v0.1.4](https://github.com/kayalopez/ai-agent-launch-tools/releases/tag/v0.1.4) - dependency-free public scanner and CLI for AI-agent launch hygiene.

Run the MCP trust check CLI:

```bash
npx --package github:kayalopez/ai-agent-launch-tools#v0.1.4 mcp-trust-check --server "candidate MCP server" --json
```

The public tools are designed to run without secrets, customer records, private screenshots, or payment data.
