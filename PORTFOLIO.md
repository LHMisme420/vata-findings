# VATA Portfolio - MCP Ecosystem Security Audit (Oct 2026)

## Summary
6 critical/high vulnerabilities discovered through systematic VATA methodology audit:
- 1 protocol-level design gap (CVSS 9.1 CRITICAL)
- 5 reference server vulnerabilities (3 CRITICAL + 1 HIGH + 1 MODERATE)

## MCP Protocol Gap (CVSS 9.1 CRITICAL)
Missing originatingClientId in RequestParamsMeta prevents client identification.
GHSA: Filed to modelcontextprotocol/modelcontextprotocol

## Reference Server Vulnerabilities

1. **Memory Server Multi-Client Data Leakage** (CVSS 9.1 CRITICAL)
   - GHSA: GHSA-wpqh-c37q-9gpm
   - Clients can read/modify/delete each other's knowledge graphs

2. **Streamable HTTP: Zero Auth + CORS** (CRITICAL)
   - GHSA: GHSA-wp76-8c37-j786

3. **SSE Transport: Zero Auth + CORS** (CRITICAL)
   - GHSA: GHSA-r8j4-r6hx-mg4f

4. **Everything Server: Env Var Disclosure** (MODERATE)
   - GHSA: GHSA-r4h4-c98q-h9mc

5. **Memory Server: Path Traversal** (HIGH)
   - GHSA: GHSA-2r74-p2mr-9xj7

## Status
All findings filed to GitHub (Jun-Oct 2026). No maintainer response. Public disclosure Oct 12 2026.

**Discoverer:** Leroy (VATA)
**Methodology:** Receipts Over Promises 🧾
