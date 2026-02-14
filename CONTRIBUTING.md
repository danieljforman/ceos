# Contributing to CEOS

Thank you for your interest in improving CEOS! This project serves two communities, and we welcome contributions from both.

## Two Types of Contributors

### EOS Practitioners

You know EOS inside and out. You run L10s, set Rocks, and live the process. You may not be a git expert, and that's fine.

**How you can help:**

- Suggest improvements to how skills implement EOS processes
- Report when a skill doesn't match how EOS actually works in practice
- Propose new EOS workflows or tool integrations
- Improve templates based on real-world usage
- Review documentation for EOS accuracy

### Developers

You know Claude Code and AI tooling. You may not know EOS terminology, and that's fine.

**How you can help:**

- Improve skill implementations (better prompts, smarter workflows)
- Fix bugs in setup.sh or skill logic
- Add new features to the data format
- Improve documentation for technical accuracy
- Build adapters for other AI agents

## Getting Started

1. **Fork** this repository
2. **Clone** your fork: `git clone https://github.com/YOUR-USERNAME/ceos.git`
3. **Create a branch**: `git checkout -b my-improvement`
4. **Make your changes**
5. **Push** and open a Pull Request

## Contribution Paths

### New EOS Workflows

Have an idea for a new skill or workflow?

1. Open an **Issue** first — describe the EOS process and how it should work
2. We'll discuss the design collaboratively
3. Once agreed, submit a PR with the implementation

### Skill Improvements

Want to make an existing skill better?

1. Fork the repo
2. Modify the skill in `skills/ceos-*/SKILL.md`
3. Submit a PR with **before/after** examples showing the improvement

### Template Improvements

Templates are the starting point for new companies.

- PRs to `templates/` are **additive only** — never remove or rename existing templates
- New templates are welcome
- Improvements to existing templates should maintain backward compatibility

### Data Format Extensions

The data format (YAML frontmatter keys, status values) is a contract that tools depend on.

- **Non-breaking additions** (new optional fields): Submit a PR with documentation
- **Breaking changes** (renaming fields, changing status values): Open an RFC-style Issue first. Breaking changes require a major version bump.

### Bug Fixes

Found a bug?

1. Fork the repo
2. Fix the issue
3. Submit a PR with reproduction steps

## Protected Files

Some files require extra care:

| File/Area | Rule |
|-----------|------|
| Data format spec (frontmatter keys, status values) | RFC + major version for breaking changes |
| Skill names and triggers | Issue discussion first |
| `setup.sh` interface | Backward-compatible changes only |
| Templates | Additive only — never remove or rename |

## Pull Request Process

1. **One concern per PR** — don't mix unrelated changes
2. **Describe the change** — what it does and why
3. **Test your changes** — run `./setup.sh` to verify skills still install correctly
4. **Update docs** if your change affects how things work

All PRs are reviewed by the maintainer before merging.

## Versioning

CEOS follows [Semantic Versioning](https://semver.org/):

- **Major** (1.0 → 2.0): Data format breaking changes
- **Minor** (1.0 → 1.1): New skills, new features
- **Patch** (1.0.0 → 1.0.1): Bug fixes, documentation

## Code of Conduct

Be kind, be constructive, be helpful. We're building tools for teams that want to run better businesses. Let's model that behavior here.

## Questions?

Open an Issue. There are no dumb questions — especially about EOS terminology or Claude Code concepts. The whole point of this project is bridging those two worlds.
