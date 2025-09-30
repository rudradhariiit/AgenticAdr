# ADR-005: GitHub Pages as Deployment Platform

**Date**: 2025-10-01
**Status**: Proposed

## Context
The requirement for a reliable, zero-cost, and tightly integrated version-controlled hosting solution for the static course website.

## Decision
Configure the Jekyll site for deployment on GitHub Pages, indicated by the `github-pages` Ruby gem dependency and typical repository structure.

## Consequences
Provides free, reliable hosting tightly integrated with the Git repository, simplifying the deployment pipeline (often automated on push); leverages GitHub's robust infrastructure for high availability and scalability; reduces operational overhead and hosting costs for course administrators; ties site updates directly to version control commits.
