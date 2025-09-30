# ADR-001: Selection of Jekyll as the Static Site Generator

**Date**: 2025-10-01
**Status**: Proposed

## Context
The project required a tool to generate a comprehensive, easily maintainable, and high-performance website for a university Software Engineering course, enabling instructors to manage course materials efficiently without extensive web development expertise.

## Decision
The core technology chosen for building the course website was Jekyll, a Ruby-based static site generator. This decision established the foundational development framework and workflow.

## Consequences
Enables the adoption of a static site architecture, leading to high performance, enhanced security, and low hosting costs. Facilitates content creation in Markdown and provides robust templating capabilities (Liquid) and modularity (collections, includes). However, it introduces a dependency on the Ruby ecosystem and inherently limits dynamic server-side functionalities.