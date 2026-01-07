# secuity-workflows
Centralized security workflows: CodeQL analysis, Octoscan, and permissions auditing for all repositories

## What's Included
- **CodeQL Analysis** - Automated code security scanning for github actions
- **Zizmor** - GitHub Actions workflow vulnerability detection
- **Octoscan** - GitHub Actions workflow vulnerability detection
- **Permissions Advisor** - Workflow permissions optimization and least-privilege enforcement

## Coming soon
- **How to use it**
- **Summary of Github best practises**
- **CodeQL auery help for Github Actions** https://codeql.github.com/codeql-query-help/actions/
- **How to resolve issues**
- **How to configure CodeQL to scanning repo's code**

## infos
- **Exclustions reasons**: 
    - unpinned-tag => because if you add commit sha instead of version, we got api errors because 

## How to publish
Releases are managed by *Semantic release.*

Each commit **must** follow the [Conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) specification.
To release a new version, you have to go on the [Release version](https://github.com/huggingface/security-workflows/blob/main/.github/workflows/manual-create-release.yml), and click on the `Run workflow` button.
A new release and tag will be created according the last commits. 

To add a new major version, execute [New major version](https://github.com/huggingface/security-workflows/blob/main/.github/workflows/update-major-version-tag.yml)

- **fix:** a commit of the type fix patches a bug in your codebase 
- **feat:**  a commit of the type feat introduces a new feature to the codebase
- **BREAKING CHANGE:** a commit that has a footer BREAKING CHANGE:, or appends a ! after the type/scope, introduces a breaking API change 
- types other than fix: and feat: are allowed, for example @commitlint/config-conventional (based on the Angular convention) recommends build:, chore:, ci:, docs:, style:, refactor:, perf:, test:, and others.
