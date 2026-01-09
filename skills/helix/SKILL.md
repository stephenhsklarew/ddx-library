---
name: helix-workflow
description: HELIX is a test-driven development workflow for AI-assisted collaboration. Use when building features, implementing user stories, or when the user mentions HELIX, TDD, or needs structured development guidance.
---

# HELIX Workflow Skill

You are guiding development using the HELIX methodology - a test-driven development workflow with AI-assisted collaboration for building high-quality software iteratively.

## The HELIX Phases

```
FRAME → DESIGN → TEST → BUILD → DEPLOY → ITERATE
```

1. **Frame** - Define the problem and establish context
2. **Design** - Architect the solution approach
3. **Test** - Write failing tests that define behavior (Red phase)
4. **Build** - Implement code to make tests pass (Green phase)
5. **Deploy** - Release to production with monitoring
6. **Iterate** - Learn and improve for the next cycle

## Core Principles

### Test-First Development (TDD)
- Tests ARE the specification - they define exactly what the system should do
- **Red**: Write a failing test that defines desired behavior
- **Green**: Write minimal code to make the test pass
- **Refactor**: Improve code while keeping tests green

### Human-AI Collaboration
**Human responsibilities**: Problem definition, strategic decisions, code review, UX/business logic
**AI responsibilities**: Pattern recognition, code generation, test case generation, documentation

### Security Integration
Security is built into every phase, not bolted on:
- Frame: Security requirements and threat modeling
- Design: Security architecture and controls
- Test: Security test suites
- Build: Secure coding practices
- Deploy: Security monitoring
- Iterate: Security metrics tracking

## Input Gates

Each phase has gates that validate previous outputs:
- **Design** cannot start until Frame outputs are validated
- **Test** cannot start until Design is reviewed
- **Build** cannot start until Tests are written and failing
- **Deploy** cannot start until all Tests pass
- **Iterate** begins once deployed and operational

## How to Guide Users

### Starting a New Feature
1. Ask what they're building (Frame)
2. Help define requirements and acceptance criteria
3. Guide through design decisions
4. Write tests BEFORE implementation
5. Implement to make tests pass
6. Review and refactor

### Key Questions Per Phase

**Frame**: What problem are we solving? Who are the users? What are the acceptance criteria?

**Design**: What's the architecture? What are the components? What are the interfaces?

**Test**: What tests prove this works? What edge cases exist? What could fail?

**Build**: What's the minimal code to pass tests? Can we refactor?

**Deploy**: Is it ready for users? What monitoring is needed?

**Iterate**: What did we learn? What should improve?

## Artifacts Reference

### Frame Phase Artifacts
- PRD (Product Requirements Document)
- User Stories
- Security Requirements
- Threat Model

### Design Phase Artifacts
- Technical Design
- Architecture Decision Records (ADRs)
- API Contracts
- Data Design

### Test Phase Artifacts
- Test Plan
- Test Suites
- Security Tests

### Build Phase Artifacts
- Implementation Plan
- Secure Coding Guidelines

### Deploy Phase Artifacts
- Deployment Checklist
- Monitoring Setup
- Runbooks

### Iterate Phase Artifacts
- Metrics Dashboard
- Lessons Learned
- Improvement Backlog

## When to Use HELIX

**Good fit**:
- New products or features requiring high quality
- Mission-critical systems where bugs are expensive
- Teams practicing or adopting TDD
- AI-assisted development needing structure
- Security-sensitive applications

**Not ideal for**:
- Quick prototypes or POCs
- Simple scripts with minimal complexity
- Emergency fixes needing immediate deployment

Always enforce the test-first approach: specifications drive implementation, quality is built in from the start.
