# In Time PRO - Bug Tracker

This repository is dedicated to tracking bugs, usability issues, defects, edge cases, and application problems reported by users and identified by teams for **In Time PRO**.

It serves as a central place to document issues in a structured and consistent way so they can be reproduced, prioritized, investigated, and resolved efficiently. The repository is intended for issue logging and collaboration around application quality; it is not the main application source code repository.

## Purpose

The goal of this repository is to make bug reporting clear, actionable, and traceable.

This repository helps teams:
- Record bugs reported by users, testers, support teams, and stakeholders.
- Capture complete reproduction steps for faster debugging.
- Maintain visibility into known issues affecting the application.
- Standardize issue descriptions so reports are easier to review.
- Track severity, impact, status, and resolution progress over time.
- Preserve historical context for recurring or previously fixed issues.

## What belongs here

Use this repository to document:
- Functional bugs.
- UI and UX issues.
- Performance problems.
- Validation and form errors.
- Workflow failures.
- API or integration-related issues.
- Environment-specific defects.
- Regression issues.
- Inconsistent behavior across roles, devices, or browsers.
- Gaps discovered during QA, UAT, or production usage.

## What does not belong here

Please avoid using this repository for:
- Feature requests that are not defects.
- General product discussions.
- Architecture proposals.
- Source code changes for the main application.
- Personal notes without actionable issue details.
- Duplicate reports without adding new evidence.

If an item is a product enhancement rather than a defect, it should be routed to the appropriate planning or product backlog process instead of being logged here as a bug.

## Recommended issue format

For each bug report, include as much detail as possible using the structure below.

### 1. Title

Write a short, specific summary of the issue.

Good examples:
- `Login button remains disabled after entering valid OTP`
- `Timesheet save fails for approver role on Safari`
- `Expense form total amount resets after attachment upload`

### 2. Summary

Provide a concise description of the problem, including what is happening and why it matters.

### 3. Environment

Capture the context in which the issue occurs, such as:
- Environment: Production / UAT / Staging / Development
- Platform: Web / Desktop
- Browser and version
- Operating system
- User role
- Build version or release number

### 4. Preconditions

Mention any setup required before the issue can be reproduced.

Examples:
- User must be logged in as manager.
- Employee profile must already contain an assigned project.
- Existing timesheet entry must be in submitted status.

### 5. Steps to reproduce

List exact steps in sequence so another person can reproduce the problem reliably.

Example:
1. Sign in as an approver.
2. Open the Timesheet module.
3. Select a submitted timesheet.
4. Click **Approve**.
5. Enter comments and submit.

### 6. Expected result

Describe what should happen if the application is working correctly.

### 7. Actual result

Describe what actually happens, including visible errors, broken behavior, or incorrect system response.

### 8. Impact

Explain who is affected and how the issue impacts business flow, user experience, or data accuracy.

### 9. Severity / Priority

Use a consistent classification where possible:
- Critical: System unusable, data loss, blocker, or production outage.
- High: Major workflow broken, no acceptable workaround.
- Medium: Important issue with limited workaround.
- Low: Minor issue, cosmetic defect, or low-impact inconsistency.

### 10. Evidence

Attach or reference supporting material when available:
- Screenshots
- Screen recordings
- Error messages
- Console logs
- API responses
- Network traces
- Related issue links

### 11. Additional notes

Add observations such as frequency, suspected conditions, workaround, or related modules.

## Sample bug template

```md
## Title
[Short bug title]

## Summary
[Brief description of the issue]

## Environment
- Environment:
- Module:
- Role:
- Browser/Version:
- OS:
- Build/Release:

## Preconditions
- [Any required setup]

## Steps to Reproduce
1. 
2. 
3. 

## Expected Result
[What should happen]

## Actual Result
[What actually happens]

## Impact
[Business/user impact]

## Severity
[Critical / High / Medium / Low]

## Evidence
- Screenshot:
- Recording:
- Logs:

## Additional Notes
[Any extra context]
```

## Writing guidelines

To keep reports useful and easy to act on:
- Use clear and specific titles.
- Write reproducible steps, not vague descriptions.
- Separate expected behavior from actual behavior.
- Mention role, module, and environment whenever relevant.
- Include attachments or logs for difficult-to-reproduce bugs.
- Report one issue per entry unless multiple issues are clearly the same defect.
- Check existing issues before creating a new one to reduce duplicates.
- Update existing reports when new findings become available.

## Triage workflow

A typical issue lifecycle in this repository may follow this flow:
1. Bug is reported by user, QA, support, or internal team.
2. Report is reviewed for completeness.
3. Issue is reproduced and validated.
4. Severity and priority are assigned.
5. Defect is linked to the appropriate release or fix plan.
6. Status is updated as work progresses.
7. Fix is verified in the target environment.
8. Issue is closed with relevant resolution notes.

## Suggested labels

To improve organization, use labels consistently. Example categories:
- `bug`
- `ui`
- `ux`
- `backend`
- `frontend`
- `api`
- `performance`
- `validation`
- `regression`
- `production`
- `uat`
- `needs-repro`
- `needs-info`
- `blocked`
- `high-priority`
- `critical`
- `resolved`

## Repository usage expectations

Contributors should ensure that every issue added here is actionable and testable. A useful report should enable another team member to 
