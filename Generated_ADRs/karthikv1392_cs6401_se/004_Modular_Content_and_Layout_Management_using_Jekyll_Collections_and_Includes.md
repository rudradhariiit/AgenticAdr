# ADR-004: Modular Content and Layout Management using Jekyll Collections and Includes

**Date**: 2025-10-01
**Status**: Proposed

## Context
The course website contains diverse content types (e.g., lectures, projects, staff profiles, announcements) that require consistent presentation, reusability of components, and an organized structure to ensure scalability, maintainability, and ease of navigation.

## Decision
To leverage Jekyll's built-in collections (e.g., `_announcements`, `_lectures`, `_projects`, `_staffers`, `_modules`, `_schedules`) for categorical organization of content, and to utilize `_includes` for reusable snippets of HTML, Liquid, or Markdown across different pages and layouts.

## Consequences
Enhances the overall content organization, making it easier to manage and extend different content categories. Promotes code reusability and improves maintainability for page layouts and UI components, leading to a consistent look and feel across the site. This approach requires an understanding of Jekyll's internal structure and templating logic, potentially adding complexity during initial setup.