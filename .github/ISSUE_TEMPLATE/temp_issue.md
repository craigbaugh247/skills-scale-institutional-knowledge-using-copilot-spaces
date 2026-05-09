---
name: Add Content to Project Management Process Docs
description: Request to add new content or updates to an existing program management process document.
title: "[Process Doc Update]: Create README for OctoAcme Project Management Docs with links and process summary"
labels: ["documentation", "process improvement"]
assignees: []
body:
  - type: dropdown
    id: process_doc
    attributes:
      label: "Which process document do you want to update? (If this is a new document, select '')"
      description: "Select the program management process document you want to add content to. If this is a new process doc, choose ''."
      options:
        - octoacme-project-management-overview.md
        - octoacme-project-initiation.md
        - octoacme-project-planning.md
        - octoacme-execution-and-tracking.md
        - octoacme-risks-and-communication.md
        - octoacme-release-and-deployment.md
        - octoacme-retrospective-and-continuous-improvement.md
        - octoacme-roles-and-personas.md
        - ""
    validations:
      required: true

  - type: textarea
    id: content_summary
    attributes:
      label: "Summary of New Content"
      description: "Briefly describe the new content or update you want to add."
      placeholder: "E.g., Add clarification to risk escalation paths, new checklist for releases, additional role responsibilities, etc."
      value: |
        Create a new README.md file for the docs/ folder that serves as a comprehensive index and entry point for all OctoAcme Project Management Process documents. The README should include:

        1. **Introduction**: Brief overview of OctoAcme's project management approach and philosophy
        2. **Process Summary**: Concise summary of the project management lifecycle (Initiation → Planning → Execution → Release → Close & Retrospective)
        3. **Core Principles**: Quick reference to customer-first, iterative delivery, clear ownership, data-informed decisions, and psychological safety
        4. **Table of Contents with Links**: Organized links to all process documentation:
           - Project Management Overview
           - Project Initiation Guide
           - Project Planning
           - Execution & Tracking
           - Risk Management & Communication
           - Release & Deployment Guide
           - Retrospective & Continuous Improvement
           - Roles and Personas
        5. **Quick Start Section**: Guidance on which document to reference for different scenarios
        6. **Contact/Support**: Information on who to reach out to for questions about these processes

  - type: textarea
    id: rationale
    attributes:
      label: "Why is this update needed?"
      description: "Explain the reason for this addition. Is it to address a gap, improve clarity, incorporate a best practice, etc.?"
      value: |
        A README for the docs/ folder is essential to:

        - **Improve Discoverability**: New team members need a clear entry point to understand OctoAcme's project management processes
        - **Reduce Navigation Friction**: Instead of searching for individual docs, users can reference a centralized index
        - **Establish Context**: A summary of processes and principles helps team members quickly understand how OctoAcme operates
        - **Accelerate Onboarding**: New employees can get up to speed faster with a guided introduction to project management practices
        - **Support Copilot Spaces**: The README acts as a companion guide to individual process documents
        - **Document Maintenance**: Centralizing the process narrative makes it easier to keep documentation aligned and up-to-date

  - type: textarea
    id: example_content
    attributes:
      label: "Suggested Content (optional)"
      description: "Paste the proposed new text, checklist, diagram, or example content you'd like to add. (Optional)"
      value: |
        # OctoAcme Project Management Process Docs

        ## Welcome to OctoAcme's Project Management Framework

        This folder contains the complete set of process documents that guide how OctoAcme runs projects. Whether you're kicking off a new initiative, planning a sprint, managing risks, or preparing a release, you'll find clear guidance and templates here.

        ## OctoAcme's Approach

        OctoAcme follows an iterative, customer-first approach to project management grounded in these principles:

        - **Customer-First**: We prioritize customer value and usability in every decision
        - **Iterative Delivery**: We deliver small, testable increments rather than big-bang releases
        - **Clear Ownership**: Every project has a named Project Manager and Product Lead
        - **Data-Informed Decisions**: We measure impact and iterate based on evidence
        - **Psychological Safety**: We encourage feedback, learning, and continuous improvement

        ## Project Lifecycle

        Every OctoAcme project follows this five-phase lifecycle:

        1. **Initiation**: Define the problem, identify stakeholders, and confirm business need
        2. **Planning**: Break work into shippable increments, estimate scope, and identify risks
        3. **Execution**: Build, test, review, and iterate toward milestones
        4. **Release**: Deploy, verify, and announce to stakeholders
        5. **Close & Retrospective**: Capture learnings and drive continuous improvement

        ## Process Documentation

        ### Getting Started

        - **[Project Management Overview](./octoacme-project-management-overview.md)** — Start here for a high-level introduction
        - **[Roles and Personas](./octoacme-roles-and-personas.md)** — Understand key roles and responsibilities

        ### By Phase

        - **[Project Initiation Guide](./octoacme-project-initiation.md)** — Validate business need, align stakeholders
        - **[Project Planning](./octoacme-project-planning.md)** — Turn an approved initiative into an actionable backlog and timeline
        - **[Execution & Tracking](./octoacme-execution-and-tracking.md)** — Manage day-to-day delivery, standups, quality
        - **[Release & Deployment Guide](./octoacme-release-and-deployment.md)** — Standardize how features move to production
        - **[Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)** — Capture learnings

        ### Cross-Cutting Concerns

        - **[Risk Management & Communication](./octoacme-risks-and-communication.md)** — Identify, track, and escalate risks

  - type: checkboxes
    id: acceptance_criteria
    attributes:
      label: "Acceptance Criteria"
      description: "Check all that apply:"
      options:
        - label: "Content aligns with existing process docs"
          checked: true
        - label: "Update improves clarity or closes a documented gap"
          checked: true
        - label: "Proposed content has been reviewed with stakeholders (if needed)"
