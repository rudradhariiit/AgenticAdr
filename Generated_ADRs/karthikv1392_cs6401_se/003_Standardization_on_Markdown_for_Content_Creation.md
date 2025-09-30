# ADR-003: Standardization on Markdown for Content Creation

**Date**: 2025-10-01
**Status**: Proposed

## Context
Instructors and course staff needed a simple, accessible, and version-control-friendly format to author and update all educational materials, administrative information, and project outlines efficiently, without requiring specialized web development skills.

## Decision
All textual course content, including lecture notes, tutorials, project descriptions, and announcements, is written and maintained using Markdown (`.md`) files.

## Consequences
Simplifies content creation and updates for non-technical users, making it highly readable and manageable within a version control system (like Git). Promotes a clear separation between content and presentation logic. While versatile, it might require embedding custom HTML/CSS or Liquid for highly complex layouts or interactive elements, and external tools for certain diagramming or rich media embedding.