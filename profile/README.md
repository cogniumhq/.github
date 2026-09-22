# Cognium Labs

**Trust infrastructure for software built with AI agents.**
Agents do the work. Cognium proves what they did.

[![cognium.net](https://img.shields.io/badge/Cognium_Labs_Inc-cognium.net-0a0a0b?labelColor=6ee7b7&color=111111)](https://cognium.net)

---

## Open source

Three projects, each usable on its own.

### [cognium-dev](https://github.com/cogniumhq/cognium-dev) — SAST for agent-written code

[![npm](https://img.shields.io/npm/v/cognium-dev.svg?label=cognium-dev)](https://www.npmjs.com/package/cognium-dev)
[![npm](https://img.shields.io/npm/v/circle-ir.svg?label=circle-ir)](https://www.npmjs.com/package/circle-ir)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/cogniumhq/cognium-dev/blob/main/LICENSE)

Static analysis that finds real vulnerabilities through cross-file taint
analysis — across JavaScript, TypeScript, Python, Java, Go, C#, Rust and Bash.

```bash
npm install -g cognium-dev
cognium-dev scan ./src
```

Results are auditable: [sast-benchmarks](https://github.com/cogniumhq/sast-benchmarks)
publishes scored runs against OWASP Benchmark, CWE-Bench-Java and Juliet — one
dataset revision, one scorer, raw artifacts included.

### [skillsregistry](https://github.com/cogniumhq/skillsregistry) — find MCP servers and agent skills

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/cogniumhq/skillsregistry/blob/main/LICENSE)

Discover MCP servers and agent skills by what they do, with explicit trust and
scan-coverage signals. Connect a client to the hosted, read-only catalog — no
API key, no signup:

```bash
claude mcp add --transport http --scope user skillsregistry https://api.skillsregistry.net/mcp
```

The repository holds the Apache-2.0 TypeScript SDK and a self-hostable local
node. **Unscanned means unscanned, not safe** — trust signals are context for
review, not a guarantee.

### [specifica](https://github.com/cogniumhq/specifica) — an open spec format for Git

[![npm](https://img.shields.io/npm/v/@specifica/format.svg?label=@specifica/format)](https://www.npmjs.com/package/@specifica/format)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/cogniumhq/specifica/blob/main/LICENSE)

A `.specifica/` directory convention for writing software specs as markdown in
any Git repo. Three files per feature — `spec.md` (what), `design.md` (how),
`tasks.md` (work). Tool-agnostic, and deliberately useful without any tool.

```bash
npm install @specifica/format
```

An open standard anyone can adopt; [specifica.app](https://specifica.app) is
one editor that implements it.

---

## Also here

| Repo | What it is |
|---|---|
| [sast-benchmarks](https://github.com/cogniumhq/sast-benchmarks) | Auditable SAST scoring vs CodeQL, Semgrep and others |
| [cognium-ai-action](https://github.com/cogniumhq/cognium-ai-action) | GitHub Action for Cognium security scanning |
| [cognium-buildkite-plugin](https://github.com/cogniumhq/cognium-buildkite-plugin) | Buildkite plugin for Cognium Dev |
| [conformis](https://github.com/cogniumhq/conformis) | Conformance issues and findings |

## Contributing

Each repository has its own `CONTRIBUTING.md`. External contributions are
welcome and no CLA form is required — open an issue before starting
non-trivial work.

Found a vulnerability? **Do not open a public issue.** Report it privately to
[security@cognium.net](mailto:security@cognium.net); see the security policy in
the affected repository.

## Links

- [cognium.net](https://cognium.net) — company
- [cognium.dev](https://cognium.dev) — Cognium SAST
- [skillsregistry.net](https://skillsregistry.net) — catalog and product docs
- [specifica.org](https://specifica.org) — the open spec format
- [hello@cognium.net](mailto:hello@cognium.net)

---

*[Cognium Labs Inc](https://cognium.net) · 2026*
