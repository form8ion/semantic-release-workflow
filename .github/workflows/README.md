# GitHub Workflows

This directory contains both the workflow that is intended to be reusable and
the workflow(s) for maintaining this repository.

## Reusable workflow

The `release.yml` workflow is the workflow that is intended to be reusable.
See [Usage Details](../../README.md#usage) in the root [README](../../README.md).

## Workflow-Release workflow

The `workflow-release.yml` workflow releases the reusable workflow with
`semantic-release` so it is possible to depend on specific versions of the
workflow.