# E2E Audit Logs

This feature enables audit logging for End-to-End (E2E) artefact-level and E2E folder-level actions. Audit log entries capture the username, timestamp, and role of the user who performed the action, providing traceability and accountability for activity within the E2E module, consistent with audit logging available across other modules.

> **Note:** Audit log entries are generated only for supported E2E actions defined in the implementation scope.

> **Reviewer TODO:** list the specific E2E artefact-level and E2E folder-level actions that are supported for audit logging.

## Overview

Audit logs for the E2E module record relevant user activity at both the artefact level and the folder level. Each log entry includes the username, timestamp, and role of the user who performed the action. These entries are available through the Audit Logs interface, where users can filter entries by date range.

## Steps

1. Navigate to the Audit Logs interface.

> **Reviewer TODO:** add screenshot of the Audit Logs interface showing E2E entries.

2. Locate the audit log entries corresponding to E2E artefact-level or E2E folder-level actions.
3. Review the recorded details for each entry: username, timestamp, and role of the user who performed the action.
4. To narrow down results, apply a date range filter to view audit log entries within a specific time period.

> **Reviewer TODO:** add screenshot of the date range filter control in the Audit Logs interface.

## Notes

- Audit log entries for E2E actions follow the same logging behavior used across other application modules.
- Only actions defined within the supported E2E audit logging scope generate audit log entries.

> **Reviewer TODO:** confirm whether there are any additional prerequisites (e.g., user permissions) required to view E2E audit log entries.
