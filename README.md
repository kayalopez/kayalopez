# Kaya Lopez

I build small software tools for AI workflows, automation, and launch safety.

Current public project: AI Agent Launch Pack

- [Supabase Launch Risk Report](https://ai-launch-risk-check-public.vercel.app/supabase-launch-risk-report.html) - a $25, fixed-scope 24-hour report for one redacted Supabase grants/RLS/RPC packet.
- [Supabase API grants checker](https://ai-launch-risk-check-public.vercel.app/supabase-api-grants-readiness.html) - separate Data API `42501` grant failures, `supabase db reset` replay gaps, and RLS policy problems before the May 30 / October 30 rollout.
- [Supabase db pull REVOKE replay checker](https://ai-launch-risk-check-public.vercel.app/supabase-db-pull-revoke-replay.html) - review generated `REVOKE` blocks and local reset replay before broad-granting around `42501`.
- [Supabase Data API grants deadline checklist](https://github.com/kayalopez/ai-agent-launch-tools/blob/main/checklists/supabase-data-api-grants-deadline-checklist.md) - review generated migrations, Lovable/v0-style Supabase apps, local replay behavior, and new tables before missing grants or broad fixes create launch risk.
- [Supabase grant migration builder](https://ai-launch-risk-check-public.vercel.app/supabase-grant-migration-builder.html) - generate a redacted explicit-grants migration skeleton and role-matrix test packet.
- [Supabase anonymous RLS matrix](https://ai-launch-risk-check-public.vercel.app/supabase-anonymous-rls-audit.html) - review redacted policies for anonymous sign-in drift where temporary users still use the `authenticated` role.
- [AI Agent Launch Pack](https://ai-launch-risk-check-public.vercel.app/) - a $25 launch-safety kit for one tool-using AI workflow, MCP server, browser automation flow, or customer-visible agent action.
- [AI Agent Launch Tools v0.1.28](https://github.com/kayalopez/ai-agent-launch-tools/releases/tag/v0.1.28) - dependency-free public scanner and CLIs for AI-agent, MCP, and Supabase launch hygiene.

Run the Supabase grants cutover check on redacted SQL, generated migration notes, or `42501` errors:

```bash
npx --package github:kayalopez/ai-agent-launch-tools#v0.1.28 supabase-grants-cutover --file supabase_grants.redacted.sql --fail-on high
```

The public tools are designed to run without secrets, customer records, private screenshots, payment data, connection strings, or service-role keys.
