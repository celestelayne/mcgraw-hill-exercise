# McGraw Hill Exercise

## Overview
This project is an instructor-facing content management application for creating, reviewing, publishing, and assigning educational assessments.

## Users and Roles
This project supports two primary roles:
1. Content Editor: manages educational content and its publication lifecycle.
2. Instructor: selects published assessments, assigns them to courses, and monitors completion.

## Core Content Model
Titles, Chapters, Quizzes, Questions,
Versions, Courses, and Assignments.

## Core Workflows

| Workflow | User Goal |
| :--- | :--- |
| WF-001 — Browse and Inspect | Find and understand existing educational content |
| WF-002 — Edit a Quiz | Modify draft quiz content and save changes |
| WF-003 — Publish Content | Review and publish an approved quiz version |
| WF-004 — Assign and Track | Assign published quizzes to courses and monitor completion |
| WF-005 — Handle Failures | Recover from failed operations and conflicting changes |

## Product Rules
1. What can an editor change in a quiz? Quiz metadata and multiple choice questions
2. Who approves publications? An authorized Content Editor can submit and publish
3. How much student activity should instructors track? Seeded completion records and summary metrics.

## Technology Stack

| Area | Technology |
| :--- | :--- |
| Application | Next.js App Router, TypeScript |
| Styling | CSS Modules |
| API | GraphQL Yoga |
| GraphQL client | Apollo Client |
| Database | SQLite + Prisma |
| Validation | Zod |
| Unit/component testing | Vitest + React Testing Library |
| E2E testing | Playwright |
| Development workflow | AGENTS.md, ADRs, OpenSpec, coding agents |

## Non-Goals
Features deliberately excluded: student-facing application, payments, notifications, real-time collaboration, rich-text authoring, media uploads, advanced grading, and a production-grade analytics dashboard.

## Development Approach
AI-native, spec-driven, domain-oriented,
vertical-slice implementation.
