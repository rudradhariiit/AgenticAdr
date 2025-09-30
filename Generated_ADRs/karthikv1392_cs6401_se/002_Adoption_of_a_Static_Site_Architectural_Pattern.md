# ADR-002: Adoption of a Static Site Architectural Pattern

**Date**: 2025-10-01
**Status**: Proposed

## Context
The primary goal was to deliver course content (lectures, projects, announcements) to students with maximum speed, reliability, and security, while minimizing operational complexity and cost for a university course website.

## Decision
To implement a purely static site architecture for the course website, where all content is pre-rendered into HTML, CSS, and JavaScript files and served directly to users without server-side processing per request.

## Consequences
Ensures extremely fast page load times, high availability, and reduced infrastructure costs. Significantly enhances security by eliminating common dynamic server-side vulnerabilities. The trade-off is the inherent lack of dynamic server-side features (e.g., user accounts, databases, real-time updates) without integrating external services or complex client-side logic.