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
The ticket adds audit logging for End-to-End (E2E) artefact-level and folder-level actions. Each entry records the username, timestamp and role of the user. The entries appear in the Audit Logs interface, where users can filter them by date range. Comments say QA verified this in two builds against the acceptance criteria. I could not check the existing documentation. The fetch tool refused every docs.avoautomation.com URL I tried as not shown in the conversation, so I don't know which page covers Audit Logs. The ticket lists no links.

**Remarks:** Eligible for documentation - update the existing Audit Logs page (exact URL not verified) to cover E2E artefact and folder actions, the recorded fields (username, timestamp, role) and the date-range filter; if no such page exists, create a new page titled 'Audit Logs'.
