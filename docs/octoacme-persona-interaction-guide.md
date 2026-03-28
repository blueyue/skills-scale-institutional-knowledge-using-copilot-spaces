# OctoAcme Persona Interaction Guide

This guide is a quick reference for understanding cross-functional dependencies and communication patterns between all personas in the OctoAcme project management framework.

---

## Persona Overview

| Persona | Primary Focus | Key Artifact |
|---|---|---|
| Developer | Build and test software components | Code, tests, PR descriptions |
| Product Manager | Define what to build and why | Roadmap, acceptance criteria, feature specs |
| Project Manager | Coordinate delivery and manage risks | Project plan, risk register, status reports |
| UX/UI Designer | Design usable and accessible interfaces | Wireframes, prototypes, design specs |
| Business Analyst | Translate business needs into requirements | Requirements docs, user stories, traceability matrix |
| Solutions Architect | Design technical solutions and set standards | Architecture decision records (ADRs), design docs |
| Support Lead | Manage post-release operations | Runbooks, incident reports, handoff docs |

---

## Cross-Functional Interaction Matrix

The table below shows the primary interactions between each pair of personas. Cells describe the nature of the collaboration.

|  | Developer | Product Manager | Project Manager | UX/UI Designer | Business Analyst | Solutions Architect | Support Lead |
|---|---|---|---|---|---|---|---|
| **Developer** | — | Clarifies acceptance criteria; demos features | Reports progress; flags blockers | Implements designs; raises feasibility concerns | Clarifies requirements; reviews specs | Follows architectural guidance; raises technical questions | Hands off release notes and runbooks |
| **Product Manager** | Reviews delivered features; adjusts priorities | — | Aligns on timeline and scope | Reviews designs for business alignment | Reviews and approves requirements | Evaluates technical trade-offs | Reviews post-release feedback |
| **Project Manager** | Tracks velocity; removes blockers | Aligns on scope and milestone status | — | Includes design tasks in plan; tracks design milestones | Incorporates BA activities into plan | Tracks architecture decisions as milestones | Coordinates release readiness and handoff |
| **UX/UI Designer** | Provides specs and assets; reviews implemented UI | Aligns designs with product goals | Reports design status; flags design risks | — | Incorporates UX insights into requirements | Reviews designs for technical feasibility | Shares accessibility requirements for operations |
| **Business Analyst** | Clarifies requirements and acceptance criteria | Refines business goals into user stories | Supports backlog grooming; tracks requirements status | Contributes UX context to requirements | — | Validates requirements against technical constraints | Provides operational requirements and support scenarios |
| **Solutions Architect** | Guides implementation; reviews technical designs | Aligns architecture with product vision | Reports technical risks and decisions | Reviews designs for technical feasibility | Validates technical feasibility of requirements | — | Ensures operational requirements are built into architecture |
| **Support Lead** | Escalates incidents for resolution; receives handoff | Reports recurring user issues and operational feedback | Communicates post-release status and readiness | Reviews accessibility post-release | Provides support scenarios as input to requirements | Escalates complex technical incidents | — |

---

## Collaboration Patterns by Project Phase

### Initiation
- **Product Manager** defines the problem statement and vision
- **Business Analyst** gathers initial stakeholder requirements
- **Solutions Architect** assesses technical feasibility
- **Project Manager** establishes governance and communication plan

### Planning
- **Product Manager** and **Business Analyst** create and prioritize the backlog
- **UX/UI Designer** produces initial wireframes and design concepts
- **Solutions Architect** produces the architectural blueprint
- **Project Manager** builds the project plan, assigns milestones, and identifies risks
- **Support Lead** defines operational requirements and handoff criteria

### Execution
- **Developers** implement features guided by design specs and requirements
- **UX/UI Designer** reviews implementation for design fidelity
- **Business Analyst** validates features against documented requirements
- **Solutions Architect** reviews technical decisions and architecture compliance
- **Project Manager** tracks progress and resolves blockers
- **Product Manager** validates acceptance criteria at sprint demos
- **Support Lead** prepares runbooks and monitors pre-release environments

### Release
- **Project Manager** and **Support Lead** conduct release readiness review
- **Developers** and **Solutions Architect** finalize handoff documentation
- **Product Manager** confirms feature completeness
- **Support Lead** takes ownership of post-release monitoring

### Post-Release
- **Support Lead** manages incident response and stakeholder communication
- **Developers** address critical bugs escalated by Support Lead
- **Product Manager** and **Business Analyst** incorporate operational feedback into the backlog
- **Project Manager** facilitates the retrospective

---

## Escalation Paths

| Situation | First Contact | Escalation Path |
|---|---|---|
| Blocker in development | Developer → Project Manager | Project Manager → Product Manager → Sponsor |
| Requirements ambiguity | Developer or Designer → Business Analyst | Business Analyst → Product Manager → Stakeholders |
| Technical design conflict | Developer → Solutions Architect | Solutions Architect → Project Manager → Sponsor |
| Post-release incident | Support Lead | Support Lead → Developers → Solutions Architect → Project Manager |
| Scope change request | Stakeholder → Product Manager | Product Manager → Project Manager → Sponsor |

---

## Communication Channels Quick Reference

| Channel | Typical Participants | Frequency | Purpose |
|---|---|---|---|
| Daily standup | Developers, Project Manager, UX/UI Designer, Business Analyst | Daily | Progress, blockers, dependencies |
| Sprint demo | All personas | End of each sprint | Showcase delivered work; validate acceptance |
| Weekly delivery sync | Project Manager, Product Manager, Solutions Architect, Support Lead | Weekly | Status, risks, upcoming milestones |
| Requirements workshop | Business Analyst, Product Manager, UX/UI Designer, Solutions Architect | As needed | Gather and refine requirements |
| Architecture review | Solutions Architect, Developers, Project Manager | As needed | Review and approve technical designs |
| Release readiness review | Project Manager, Support Lead, Product Manager, Developers | Pre-release | Confirm readiness for production deployment |
| Retrospective | All personas | End of each sprint or milestone | Continuous improvement |
