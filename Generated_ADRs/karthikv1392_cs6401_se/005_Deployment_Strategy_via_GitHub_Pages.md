# ADR-005: Deployment Strategy via GitHub Pages

**Date**: 2025-10-01
**Status**: Proposed

## Context
A cost-effective, reliable, and easily manageable hosting solution was required for the course website, ideally one that integrated seamlessly with the existing Git-based development workflow and simplified the deployment process for academic staff.

## Decision
The Jekyll-generated static website is intended for deployment and hosting on GitHub Pages, as strongly indicated by the presence of the `github-pages` gem in the project's dependencies.

## Consequences
Provides free and highly reliable hosting directly integrated with the Git repository, automating the build and deployment process upon every push to the main branch. Leverages GitHub's robust infrastructure for performance and scalability. However, it imposes restrictions on the use of custom Jekyll plugins and might have limitations for very large sites or specific server-side processing requirements.