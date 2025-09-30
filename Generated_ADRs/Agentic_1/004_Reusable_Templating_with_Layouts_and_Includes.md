# ADR-004: Reusable Templating with Layouts and Includes

**Date**: 2025-10-01
**Status**: Proposed

## Context
The necessity to create a consistent look and feel across various page types while maximizing code reusability for common UI elements and structural components within the static site.

## Decision
Design a comprehensive templating system leveraging Jekyll `_layouts/` for defining reusable page structures (e.g., `minimal.html`, `staffer.html`) and `_includes/` for modular HTML snippets (e.g., `head.html`, `minutes.liquid`).

## Consequences
Ensures a consistent user experience and brand identity across the site; significantly reduces HTML code duplication and development effort; facilitates the implementation of complex UI features like dynamic navigation, breadcrumbs, and tables of contents; enhances overall development efficiency.
