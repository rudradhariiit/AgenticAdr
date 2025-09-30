# ADR-002: Structured Content Management with Jekyll Collections

**Date**: 2025-10-01
**Status**: Proposed

## Context
The requirement to organize and manage diverse, distinct types of course content (e.g., announcements, modules, staff profiles, schedules) in a consistent, structured, and scalable manner within a static site environment.

## Decision
Utilize Jekyll's custom collections (e.g., `_announcements/`, `_modules/`, `_staffers/`) to define and manage different content types, applying specific layouts and metadata for each.

## Consequences
Establishes a clear, scalable information architecture; enforces content consistency through dedicated layouts and front matter; simplifies content authoring and retrieval; improves overall site maintainability as course content grows and evolves.
