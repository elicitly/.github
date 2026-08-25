# Security Policy

## Reporting a vulnerability

**Please do not report security vulnerabilities in public GitHub issues.**

Instead, use GitHub's private vulnerability reporting: open the
[**Security** tab of the `elicitly` repository](https://github.com/elicitly/elicitly/security)
and click **Report a vulnerability**. This opens a private advisory that only
maintainers can see.

If you can't use GitHub, email
[security@elicitly.ai](mailto:security@elicitly.ai).

We will acknowledge your report within 5 business days. Please give us a
reasonable window to ship a fix before disclosing publicly — we'll coordinate
disclosure with you once one is available.

## Supported versions

Security fixes are applied to the latest release of
[`elicitly`](https://www.npmjs.com/package/elicitly) and
[`@elicitly/tools`](https://www.npmjs.com/package/@elicitly/tools) on npm.
Older releases are not patched — please update to the latest version.

## Scope

**In scope**

- The `elicitly` local (stdio) MCP server and the `@elicitly/tools` toolkit,
  as published on npm.
- The hosted Pro service at `elicitly.ai` — reports are welcome, but do not
  test against it without permission (no automated scanning, no denial of
  service, no access to data that isn't yours).

**Out of scope**

- How an MCP host renders elicitation prompts (e.g. misleading prompt text,
  or a host that auto-accepts elicitations). Elicitation content is presented
  by the host application; issues with that presentation belong upstream.
- Vulnerabilities in dependencies with no demonstrated impact on Elicitly —
  report those to the dependency's maintainers.
