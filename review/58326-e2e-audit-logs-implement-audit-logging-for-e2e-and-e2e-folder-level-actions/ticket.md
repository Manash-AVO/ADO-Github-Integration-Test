# E2E Audit Logs : Implement Audit Logging for E2E and E2E Folder-Level Actions - #58326

**Type:** Prod Enhancement
**Status:** In Progress
**Assigned To:** Unassigned
**Area Path:** Avo EEC
**Iteration:** Avo EEC

## Description
Currently, the application does not capture audit logs for End-to-End (E2E) artefacts or E2E folder-level actions. As a result, there is no visibility into who performed actions within the E2E module, when those actions occurred, or the role of the user.This enhancement introduces audit logging for both E2E artefact-level and E2E folder-level actions to provide traceability, accountability, and consistency with the audit logging capabilities available across other modules.The implementation should capture relevant audit events and record the associated user details, enabling administrators to review user activity and filter audit logs by date range.

---
[View in Azure DevOps](https://dev.azure.com/AvoAutomation/Avo%20EEC/_workitems/edit/58326)

## Analysis
Audit logging is now implemented for End-to-End (E2E) artefact and folder-level actions, recording the username, role, and timestamp for each action. These entries appear in the Audit Logs interface, where administrators can filter E2E activity by date range, matching audit log behavior used in other modules.

**Remarks:** Eligible for documentation - adds visible audit log entries and filtering for E2E actions in the Audit Logs interface.
