---
name: Add OctoAcme Project Management Docs README with Process Summary and Links
description: Request to create a new README for OctoAcme Project Management Docs that consolidates all process documentation with a summary and links.
title: "[Process Doc Update]: Create README for OctoAcme Project Management Docs - Process Summary and Links"
labels: ["documentation", "process improvement"]
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
      value: "Create a new README.md file in the docs/ folder that serves as the central entry point for all OctoAcme project management processes. The README should include:\n\n- A brief overview and purpose of OctoAcme's project management approach\n- A summary of the core project management phases (Initiation, Planning, Execution, Release, Close & Retrospective)\n- Key principles guiding OctoAcme's project delivery\n- A complete set of links to all process documentation files stored in docs/\n- Quick reference guide to which document to consult for different phases and scenarios"
    validations:
      required: true

  - type: textarea
    id: rationale
    attributes:
      label: "Why is this update needed?"
      description: "Explain the reason for this addition. Is it to address a gap, improve clarity, incorporate a best practice, etc.?"
      value: "Currently, OctoAcme process documentation is scattered across multiple files in the docs/ folder with no central entry point. New team members and stakeholders need a single source of truth that:\n\n- Provides a quick overview of how OctoAcme manages projects\n- Clearly directs users to the appropriate documentation for their needs\n- Reduces friction in onboarding by centralizing scattered process knowledge\n- Improves discoverability of existing process documents\n- Aligns with the purpose of this Copilot Space: to centralize scattered project management knowledge and make it searchable and accessible"
    validations:
      required: true

  - type: textarea
    id: example_content
    attributes:
      label: "Suggested Content (optional)"
      description: "Paste the proposed new text, checklist, diagram, or example content you'd like to add. (Optional)"
      value: "# OctoAcme Project Management Documentation\n\n## Welcome to OctoAcme's Project Management Hub\n\nThis directory contains comprehensive guidance for managing projects at OctoAcme—from initial concept through delivery and continuous improvement. Whether you're a Project Manager, Product Manager, Developer, or Stakeholder, you'll find the processes and templates you need to deliver customer value with clarity, consistency, and confidence.\n\n## Our Approach\n\nOctoAcme follows a structured yet flexible project lifecycle centered on these core principles:\n\n- **Customer-first**: Prioritize customer value and usability in all decisions\n- **Iterative delivery**: Ship small, testable increments rather than large monolithic releases\n- **Clear ownership**: Every project has defined leadership with clear responsibilities\n- **Data-informed**: Measure impact and iterate based on evidence\n- **Psychological safety**: Foster feedback, learning, and continuous improvement\n\n## Project Lifecycle Phases\n\n### 1. **Initiation** — Validate & Align\nDefine the business need, confirm success metrics, align stakeholders, and make a go/no-go decision.\n- **Document**: [OctoAcme — Project Initiation Guide](./octoacme-project-initiation.md)\n\n### 2. **Planning** — Create an Actionable Plan\nTurn an approved initiative into a detailed backlog, estimate scope, identify dependencies, and establish a release timeline.\n- **Document**: [OctoAcme — Project Planning](./octoacme-project-planning.md)\n\n### 3. **Execution & Tracking** — Deliver with Visibility\nManage day-to-day work, conduct standups, track progress against milestones, and escalate blockers.\n- **Document**: [OctoAcme — Execution & Tracking](./octoacme-execution-and-tracking.md)\n\n### 4. **Release & Deployment** — Get to Production\nStandardize the process for releasing features to production with reduced risk and improved observability.\n- **Document**: [OctoAcme — Release & Deployment Guide](./octoacme-release-and-deployment.md)\n\n### 5. **Close & Retrospective** — Learn & Improve\nCapture learnings, celebrate successes, and convert insights into actionable improvements.\n- **Document**: [OctoAcme — Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)\n\n## Cross-Cutting Practices\n\n### Risk Management & Communication\nIdentify, assess, and mitigate risks throughout the project lifecycle. Maintain transparent communication with all stakeholders.\n- **Document**: [OctoAcme — Risk Management & Communication](./octoacme-risks-and-communication.md)\n\n### Project Management Overview\nA concise introduction to OctoAcme's approach, key roles, artifacts, and communication cadence.\n- **Document**: [OctoAcme Project Management Overview](./octoacme-project-management-overview.md)\n\n### Roles & Personas\nDefinitions of typical project roles (Project Manager, Product Manager, Developer, QA) and their responsibilities.\n- **Document**: [OctoAcme Personas](./octoacme-roles-and-personas.md)\n\n## Quick Start: Where to Begin?\n\n**Are you...?**\n- **Starting a new project?** → Begin with [Project Initiation](./octoacme-project-initiation.md)\n- **Planning an approved project?** → Move to [Project Planning](./octoacme-project-planning.md)\n- **In the middle of delivery?** → Check [Execution & Tracking](./octoacme-execution-and-tracking.md)\n- **Preparing for release?** → Review [Release & Deployment Guide](./octoacme-release-and-deployment.md)\n- **Wrapping up a project?** → Schedule a [Retrospective](./octoacme-retrospective-and-continuous-improvement.md)\n- **Managing risks or stakeholders?** → Reference [Risk Management & Communication](./octoacme-risks-and-communication.md)\n- **New to OctoAcme processes?** → Start with [Project Management Overview](./octoacme-project-management-overview.md)\n\n## Key Artifacts You'll Create\n\n- **Project Charter / One-pager** — Problem, Goal, Success Metrics, Stakeholders\n- **Prioritized Backlog** — With acceptance criteria and estimates\n- **Release Plan** — Timeline, milestones, and deployment checklist\n- **Risk Register** — ID, Description, Impact, Mitigation, Status\n- **Status Updates** — Progress, next steps, risks, decisions needed\n- **Retrospective Notes** — Learnings, action items, improvements\n\n## Core Roles\n\n- **Project Manager (PM)**: Coordinates delivery, schedules, risks, communications\n- **Product Manager (PdM)**: Defines outcomes, prioritizes backlog, measures success\n- **Developers**: Implement features, collaborate on design and testability\n- **QA/Testing**: Validates quality and acceptance criteria\n- **Stakeholders**: Provide inputs and approvals\n\nSee [Roles & Personas](./octoacme-roles-and-personas.md) for detailed responsibilities.\n\n## Communication Cadence\n\n- **Daily standups** (15 min): Progress, blockers, dependencies\n- **Weekly PM + PdM sync**: Alignment and risk review\n- **Twice-weekly delivery team standups** (or as agreed)\n- **Monthly stakeholder updates**: High-level status and milestones\n- **Sprint/milestone demos & reviews**: Show progress and gather feedback\n- **Ad-hoc escalations**: Trigger blocker resolution\n\n## Questions or Feedback?\n\nIf you identify gaps in these processes, have suggestions for improvement, or need clarification, please create an issue using the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template.\n\n---\n\n**Last Updated**: [Date]\n**Maintained By**: [Team/Role]"

  - type: checkboxes
    id: acceptance_criteria
    attributes:
      label: "Acceptance Criteria"
      description: "Check all that apply:"
      options:
        - label: "Content aligns with existing process docs"
          required: true
        - label: "Update improves clarity or closes a documented gap"
          required: true
        - label: "Proposed content has been reviewed with stakeholders (if needed)"

