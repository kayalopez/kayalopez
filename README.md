# Kaya Lopez

I build small software tools for AI workflows, automation, and launch safety.

Current public project: AI Agent Launch Pack

- [Supabase Launch Risk Report](https://ai-launch-risk-check-public.vercel.app/supabase-launch-risk-report.html) - a $25, fixed-scope 24-hour report for one redacted Supabase grants/RLS/RPC packet.
- [Supabase API grants checker](https://ai-launch-risk-check-public.vercel.app/supabase-api-grants-readiness.html) - separate Data API `42501` grant failures from RLS policy problems before the May 30 / October 30 rollout.
- [Supabase grant migration builder](https://ai-launch-risk-check-public.vercel.app/supabase-grant-migration-builder.html) - generate a redacted explicit-grants migration skeleton and role-matrix test packet.
- [AI Agent Launch Pack](https://ai-launch-risk-check-public.vercel.app/) - a $25 launch-safety kit for one tool-using AI workflow, MCP server, browser automation flow, or customer-visible agent action.
- [AI Agent Launch Tools v0.1.23](https://github.com/kayalopez/ai-agent-launch-tools/releases/tag/v0.1.23) - dependency-free public scanner and CLIs for AI-agent, MCP, and Supabase launch hygiene.

Run the Supabase grants cutover check on redacted SQL or error notes:

```bash
npx --package github:kayalopez/ai-agent-launch-tools#v0.1.23 supabase-grants-cutover --file supabase_grants.redacted.sql --fail-on high
```

The public tools are designed to run without secrets, customer records, private screenshots, payment data, connection strings, or service-role keys.
