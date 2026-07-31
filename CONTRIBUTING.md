# Contributing to Octacity

Thank you for your interest in contributing to Octacity.

This document provides the default contribution guidelines used across the organization. Individual repositories may define additional or different requirements, so always read the repository's README, contribution guidelines, issue templates, and pull request template before beginning work.

Repository-specific rules take precedence over this document.

## Who Can Contribute

Contributions are welcome from both:

- Octacity members
- Public contributors outside the organization

Membership is not required to contribute to repositories that accept public contributions.

Each repository should state whether it is currently open to outside contributions.

## Before Starting

Open an issue before beginning any contribution.

The issue should explain:

- What you want to change
- Why the change is useful
- The general approach you intend to take
- Any alternatives or uncertainties you are considering

This gives the maintaining team an opportunity to provide context, confirm that the work is appropriate, and prevent duplicated or conflicting effort.

For small changes such as obvious typo fixes, a repository may define a lighter process.

## Claiming an Issue

When you intend to work on an existing issue, you are encouraged to leave a comment such as:

> I would like to work on this.

Waiting for confirmation is strongly recommended. Another contributor may already be working on the same problem, or the maintaining team may have additional context that has not yet been documented.

Claiming an issue is not universally mandatory unless the repository states otherwise. However, contributors who begin work without communicating accept the risk that:

- The same work may already be in progress
- The proposed approach may conflict with the project's direction
- The contribution may no longer be needed
- Significant changes may be requested during review
- The pull request may be declined despite the effort involved

Communication before implementation helps avoid wasted work for everyone.

## Architectural and Significant Changes

Architectural changes must be discussed before implementation.

Open an issue and wait for approval before making changes that significantly affect:

- Project architecture
- Public APIs
- Data formats or storage
- Security boundaries
- Dependencies
- Build or deployment systems
- Repository structure
- Major user-facing behavior
- Compatibility or migration requirements

Do not submit large unsolicited rewrites.

The maintaining team may request a proposal, design document, proof of concept, or smaller implementation plan before approving the work.

## Development Guidelines

Follow the instructions provided by the repository.

These may include requirements for:

- Building and running the project
- Testing
- Formatting and linting
- Documentation
- Supported platforms
- Dependency changes
- Security-sensitive work
- Generated files
- Backward compatibility

Keep changes focused. Avoid unrelated refactoring, formatting changes, or dependency updates unless they are necessary for the contribution.

## Commit Messages

Octacity uses Conventional Commits.

Use the following structure:

```text
type(optional scope): description
```

Common types include:

```text
feat: add a new feature
fix: correct a bug
docs: update documentation
refactor: restructure code without changing behavior
test: add or update tests
build: change the build system or dependencies
ci: update continuous integration
chore: perform maintenance work
```

Examples:

```text
feat(auth): add session expiration
fix(parser): handle empty input safely
docs: clarify local setup instructions
refactor(storage): separate cache management
```

Write commit messages that clearly describe the change. Individual repositories may define additional conventions.

## Pull Requests

Pull request requirements are defined by each repository's pull request template.

In general, a pull request should:

- Address an approved or discussed issue
- Stay focused on one clear purpose
- Explain what changed and why
- Link the relevant issue
- Follow the repository's technical requirements
- Include appropriate tests or verification
- Update documentation when behavior changes
- Clearly identify incomplete work or known limitations
- Respond constructively to review feedback

Submitting a pull request does not guarantee that it will be merged.

Reviewers may request changes, suggest another approach, divide the work into smaller contributions, or decline the pull request when it does not fit the project.

## Review and Decision-Making

Each repository has a maintaining team responsible for its direction and continued development.

The team leader decides how contributions are reviewed. They may:

- Review the contribution directly
- Delegate the review to a member of their team
- Assign a repository maintainer
- Request review from a qualified member of another Octacity team

Review authority may vary between repositories.

The maintaining team has the final decision on whether a contribution is accepted, revised, postponed, or declined.

Reviews should focus on:

- Correctness
- Maintainability
- Security
- Scope
- Project direction
- Documentation
- Testing
- Compatibility
- Long-term maintenance cost

## AI-Assisted Contributions

AI-assisted development is allowed.

Octacity evaluates contributions by their quality, honesty, maintainability, and compliance with project rules—not by whether an AI tool was used.

The contributor remains fully responsible for all submitted work.

This means you must:

- Understand the code, text, design, or other work you submit
- Be able to explain the approach and important decisions
- Verify that the contribution works as claimed
- Review generated output for errors, security issues, and unsuitable changes
- Follow the repository's contribution and licensing requirements
- Respond personally and meaningfully during review
- Correct problems found in the submitted work

Do not submit large amounts of unreviewed generated content.

Reviewers may be less tolerant of repeated rule violations, careless output, or misleading claims when a contributor is using automated tools but makes no effort to understand or verify the result.

Octacity expects to communicate with the contributor, not with an autonomous agent. Bots and agents must not independently conduct discussions, argue with reviewers, or represent themselves as the accountable author of a contribution.

## Respectful Collaboration

Follow the Octacity [Code of Conduct](CODE_OF_CONDUCT.md) in all project interactions.

Technical disagreement is welcome, but discussion must remain constructive and focused on the work.

Be honest about:

- Your experience
- What you understand
- What you tested
- Where you used external assistance
- Known problems or uncertainty
- Whether work is complete

Asking questions is encouraged. Concealing uncertainty is not.

## Security Issues

Do not report suspected security vulnerabilities through a public issue unless the repository explicitly instructs you to do so.

Follow the process described in the Octacity [Security Policy](SECURITY.md) or the repository's own security documentation.

## Licensing

By submitting a contribution, you agree that it may be distributed under the license used by the repository.

Do not submit work that you do not have the right to contribute.

When adapting code, documentation, designs, or other material from elsewhere, disclose the source and ensure that its license is compatible with the project.

## Questions

Use the communication channel defined by the repository when you need clarification.

When no project-specific channel is provided, open an issue describing your question and the relevant context.
