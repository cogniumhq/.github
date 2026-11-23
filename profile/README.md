# Cognium Labs

**Cognium Autonomous Loop for software modernization**

The Loop helps teams work through pull requests and issues in existing repositories. Agents prepare changes. Deterministic checks record what passed, what failed, and what still needs a person. Your team decides whether to merge.

[How the Loop works](https://cognium.net/how-it-works/) · [Join the hosted waitlist](https://cognium.net/start/)

## What a reviewer sees

In a recorded run on a public test repository, an agent updated a dependency and the advisory check passed. Two call sites had no test coverage. The Loop opened a draft pull request that identified the untested behavior so a reviewer could decide whether to merge. [Read the draft PR](https://github.com/mason-cognium/CVE-2022-42889-PoC/pull/2).

The intended workflow starts with rules recovered from your code and approved by your team. Each change is checked against those rules, and the review record ties the request, the diff, and the results together. Spec recovery is read-only today. [Explore the checks](https://cognium.net/#hood) · [Inspect the evidence](https://cognium.net/proof/)

## Run a local scan

[cognium-dev](https://github.com/cogniumhq/cognium-dev) is the open-source checking engine. Use its CLI to scan a source directory for security findings, including data flows across files. From a repository with a `src` directory, run:

~~~bash
npm install -g cognium-dev
cognium-dev scan ./src
~~~

## Modernization packs

| Pack | What it checks |
| --- | --- |
| [Databricks data migration](https://cognium.net/packs/databricks-migration/) | Whether SQL converted from Snowflake preserves the behavior the data owners approved. |
| [Accessibility](https://cognium.net/packs/accessibility/) | Web, PDF, and mobile accessibility against WCAG criteria, with findings for review. |
| [Kubernetes operations](https://cognium.net/packs/kubernetes-operations/) | Whether proposed changes and the running cluster meet approved requirements. |

## Open-source projects and integrations

| If you want to… | Start here |
| --- | --- |
| Keep a feature spec, design, and tasks alongside the code | [Specifica](https://github.com/cogniumhq/specifica) defines the Markdown files in `.specifica/`. [Read the standard](https://specifica.org/). |
| Find MCP servers and agent skills by task | [SkillsRegistry](https://skillsregistry.net/) shows the trust and scan coverage recorded for each result. The [repository](https://github.com/cogniumhq/skillsregistry) contains the TypeScript SDK and a self-hostable node. |
| Use Cognium from an editor | [Cognium MCP](https://github.com/cogniumhq/cognium-mcp) provides the MCP server and editor plugins. |
| Run security scans in CI | Use the [GitHub Action](https://github.com/cogniumhq/cognium-ai-action) or the [Buildkite plugin](https://github.com/cogniumhq/cognium-buildkite-plugin). |
| Inspect security benchmark results | [sast-benchmarks](https://github.com/cogniumhq/sast-benchmarks) publishes scored runs and raw artifacts for OWASP Benchmark, CWE-Bench-Java, and Juliet. |
| Compare accessibility checkers | Inspect the [WCAG test fixtures](https://github.com/cogniumhq/a11y-benchmark) and the [published result bundles](https://github.com/cogniumhq/a11y-benchmark-results). |

## Contributing and contact

For a bug or feature request, open an issue in the relevant project. For larger changes, discuss the approach there and follow the repository’s contribution guide. Report security vulnerabilities privately to [security@cognium.net](mailto:security@cognium.net).

For hosted onboarding, [join the waitlist](https://cognium.net/start/). For other inquiries, contact [hello@cognium.net](mailto:hello@cognium.net).
