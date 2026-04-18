---
layout: default
title: GuardRail for Jira
---

# GuardRail for Jira

Zero-code compliance enforcement with audit trails for Jira Cloud.

## Documentation

- [Getting Started](#getting-started)
- [Privacy Policy](privacy-policy)
- [End User License Agreement](eula)
- [Support & SLA](sla)

---

## Getting Started

### 1. Install from Atlassian Marketplace

Search for "GuardRail" in the Atlassian Marketplace, or install directly from your Jira instance under **Apps > Find new apps**.

### 2. Open GuardRail

After installation, find **GuardRail** under **Apps** in your Jira top navigation bar.

### 3. Install a Template Pack

On first launch, the onboarding wizard helps you pick a pre-built rule set:

- **Scrum Best Practices** — Story points, descriptions, assignees, subtask completion
- **Code Quality Gates** — Linked reviews, acceptance criteria, subtask resolution
- **Security Review** — Linked review requirements for security-sensitive issues
- **Release Readiness** — Fix version, subtask completion, documentation checks

All template rules start in **Dry Run** mode — they evaluate without blocking anyone.

### 4. Monitor the Audit Log

Switch to the **Audit Log** tab to see how your rules perform. Check the compliance score, review violations, and export data as CSV.

### 5. Enable Enforcement

When you're confident a rule works correctly:
1. Go to the **Rules** tab
2. Click the **mode badge** on a rule to switch from "Dry Run" to "Active"
3. For hard blocking, go to the **Setup** tab and click **Enable Blocking** on your project

---

## Features

### Visual Rule Builder
Create compliance rules with dropdown-based configuration. No scripting required. Select fields, statuses, and conditions from your actual Jira data with autocomplete.

### Graduated Enforcement
Roll out compliance safely in three stages:
1. **Dry Run** — Evaluate silently, review results in the dashboard
2. **Warn** — Log violations, notify assignees via comments and Jira notifications
3. **Block** — Deny non-compliant transitions with actionable error messages

### Automatic Monitoring
Every issue transition is automatically evaluated — no workflow setup needed for monitoring. Results appear in the audit log and on each issue's compliance panel.

### Compliance Dashboard
Real-time compliance score, top violations, result breakdown, and CSV export for SOC2/ISO auditors.

### Override Workflow
When blocking rules are too strict for a specific case, team members can request an override with a justification. Administrators review and approve or reject from the Overrides tab.

### Notifications
Configurable per rule: add a comment on the issue and/or send a Jira notification to the assignee and reporter when a rule fires.

### Template Packs
Pre-built rule sets for common workflows. Install in one click, customize later.

---

## FAQ

**Q: Does GuardRail work on team-managed (next-gen) projects?**
A: Monitoring and audit logging work on all project types. Transition blocking (hard enforcement) requires company-managed projects, which is a Jira platform limitation shared by all workflow plugins.

**Q: Will GuardRail slow down my Jira?**
A: No. Rule evaluation typically takes 1-3 seconds. The automatic monitoring runs asynchronously after transitions complete, so it never blocks the Jira UI.

**Q: Can I export audit data for compliance audits?**
A: Yes. The Audit Log tab has a CSV export button that downloads all filtered evaluations with timestamps, issue keys, rule names, and results.

**Q: What happens if I delete a rule?**
A: The rule stops evaluating immediately. Historical audit log entries for that rule are preserved for your configured retention period (default: 90 days).

**Q: How do notifications work?**
A: Each rule has configurable notification settings. When a rule fires on an active (non-dry-run) evaluation, GuardRail can add a comment on the issue and/or send a Jira notification to the assignee and reporter. You can customize the message with placeholders.

---

## Support

- **Email**: pavel.jira@gmail.com
- **Issues**: [GitHub Issues](https://github.com/PavelJ/guardrail-docs-/issues)

---

## Legal

- [Privacy Policy](privacy-policy)
- [End User License Agreement](eula)
- [Support & SLA](sla)
