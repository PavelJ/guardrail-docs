# GuardRail for Jira — Privacy Policy

**Last updated:** April 6, 2026

## Introduction

This Privacy Policy describes how GuardRail for Jira ("GuardRail", "we", "our", "the App") collects, uses, and protects information when you use our Atlassian Forge application.

GuardRail is developed and maintained by Pavel Jira ("Developer"). This policy applies to all users of the GuardRail for Jira application installed via the Atlassian Marketplace.

## Information We Collect

### Data Processed Within Your Jira Instance

GuardRail operates entirely within the Atlassian Forge platform. The following data is accessed and processed:

- **Issue data**: Issue keys, field values (e.g., story points, descriptions, statuses, labels, assignees), linked issues, subtask statuses. This data is read during rule evaluation to determine compliance.
- **Workflow data**: Transition names, status names, and workflow configurations. Used for rule matching and enforcement setup.
- **User identifiers**: Atlassian account IDs of users who trigger issue transitions. Stored in audit logs to record who performed an action.
- **Project metadata**: Project keys, names, issue types, priorities. Used for rule scoping and autocomplete in the user interface.

### Data Stored by GuardRail

All data stored by GuardRail resides in Atlassian Forge Entity Storage, which is:
- Encrypted at rest by Atlassian
- Scoped to your Jira Cloud instance (not shared across instances)
- Subject to Atlassian's data residency and security policies

The following data is stored:

- **Compliance rules**: Rule configurations you create (names, conditions, severity, scope)
- **Evaluation logs**: Records of rule evaluations including issue key, rule name, result (pass/fail), user ID, timestamp, and condition details. Retained for 90 days (configurable) and then automatically deleted.
- **Daily aggregates**: Summarized compliance scores per project per day. Retained indefinitely.
- **App configuration**: Your settings (notification preferences, retention period, enabled features)

### Data We Do NOT Collect

- We do **not** collect personal information beyond Atlassian account IDs
- We do **not** transmit data outside of your Atlassian Forge environment
- We do **not** use analytics, tracking pixels, or third-party data collection services
- We do **not** sell, rent, or share your data with third parties
- We do **not** store passwords, API tokens, or authentication credentials

## How We Use Information

Information processed by GuardRail is used solely to:

1. Evaluate compliance rules against Jira issue data during transitions
2. Log evaluation results for audit trail purposes
3. Display compliance status on issues and in the dashboard
4. Generate compliance reports and exports
5. Provide autocomplete suggestions in the rule builder interface

## Data Retention

- **Evaluation logs**: Retained for the number of days configured in your app settings (default: 90 days). Older logs are automatically deleted by a daily cleanup process.
- **Compliance rules**: Retained until you delete them.
- **Daily aggregates**: Retained indefinitely for historical trend analysis.
- **All stored data** is automatically removed if you uninstall the GuardRail app from your Jira instance.

## Data Security

GuardRail leverages Atlassian Forge's built-in security:

- All data is stored in Atlassian's infrastructure (encrypted at rest)
- The app runs in Atlassian's sandboxed Forge environment
- API calls to Jira use Atlassian's authenticated request mechanism
- No external network calls are made (all processing happens within Forge)
- Input validation is applied to all user-submitted data using schema-based validation

## Your Rights

As the Jira instance administrator, you have full control over your data:

- **Access**: View all stored rules, evaluations, and configurations through the app UI
- **Export**: Download audit logs as CSV files
- **Delete**: Delete individual rules or uninstall the app to remove all stored data
- **Modify**: Edit rules, change retention settings, and configure the app at any time

## Third-Party Services

GuardRail does **not** integrate with or transmit data to any third-party services. All processing occurs within the Atlassian Forge platform.

Future versions may offer optional integrations with Bitbucket, GitHub, and Jenkins for PR/CI status checks. These integrations will only be activated by explicit admin configuration and will only receive webhook data that you configure the external service to send.

## Changes to This Policy

We may update this Privacy Policy to reflect changes in the app's functionality. Changes will be noted with an updated "Last updated" date. Continued use of the app after changes constitutes acceptance of the updated policy.

## Contact

For questions about this Privacy Policy or GuardRail's data practices:

- **Developer**: Pavel Jira
- **Email**: pavel.jira@gmail.com

## Atlassian Marketplace

GuardRail is distributed through the Atlassian Marketplace and is subject to the [Atlassian Marketplace Terms of Use](https://www.atlassian.com/licensing/marketplace/termsofuse) and [Atlassian's Privacy Policy](https://www.atlassian.com/legal/privacy-policy).
