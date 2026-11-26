# E2E Audit Logs : Implement Audit Logging for E2E and E2E Folder-Level Actions - #58326

**Type:** Prod Enhancement
**Status:** New
**Assigned To:** Unassigned
**Area Path:** Avo EEC
**Iteration:** Avo EEC

## Description
Currently, the application does not capture audit logs for End-to-End (E2E) artefacts or E2E folder-level actions. As a result, there is no visibility into who performed actions within the E2E module, when those actions occurred, or the role of the user.This enhancement introduces audit logging for both E2E artefact-level and E2E folder-level actions to provide traceability, accountability, and consistency with the audit logging capabilities available across other modules.The implementation should capture relevant audit events and record the associated user details, enabling administrators to review user activity and filter audit logs by date range.

---
[View in Azure DevOps](https://dev.azure.com/AvoAutomation/Avo%20EEC/_workitems/edit/58326)

## Analysis
Audit logging is now available for End-to-End (E2E) test actions, recording who created, renamed, added, or deleted test cases within E2E flows and folders, along with the username, timestamp, and role. Users can view these entries in the Audit Logs interface and filter them by date range, matching audit log behaviour already available in other modules.

**Remarks:** Eligible for documentation - adds visible audit log entries and filtering for E2E actions in the Audit Logs interface.


## Planning
- **Assigned to:** Unassigned
- **Requester:** Trial\PoC

## Tasks
Objective Improve traceability for testcase changes within E2E flows and allow users to view E2E flow and folder information directly from the design interface. 
Implementation Details E2E testcase identity Generate a UUID when an E2E testcase is first added. 
 
Preserve existing UUIDs when persisted E2E flows are loaded. 
 
Include testcase name and path in the E2E flow save request. 
 
 E2E flow update auditing Compare the previous testcase list with the updated testcase list. 
 
Identify added and deleted test cases using UUIDs, with testcase IDs as a fallback. 
 
Resolve testcase and folder metadata from MongoDB. 
 
Build descriptive audit messages containing the testcase name and path. 
 
Persist separate add and delete audit records using the E2E flow audit-log model. 
 
 Active E2E node handling Resolve the active node from either an E2E flow or an E2E folder. 
 
Use the resolved node for rendering, selection, and save operations. 
 
Support opening and editing E2E flows accessed through an E2E folder. 
 
 Information panel Added an information icon to E2E flow and folder views. 
 
Integrated the shared GlobalInfoPanel using the E2E screen type. 
 
Synchronized the information panel state with the design store. 
 
Preserved the active audit-log panel selection. 
 
 Test Coverage Added backend tests for added and deleted testcase audit records. 
 
Added frontend tests for UUID generation and UUID preservation. 
 
Added tests for active E2E node propagation. 
 
Added component tests for E2E flow and folder table rendering.

## Acceptance Criteria
Audit logging is implemented for E2E artefact-level actions. 
Audit logging is implemented for E2E folder-level actions. 
Each audit log entry records the username, timestamp, and role of the user who performed the action. 
Audit log entries are available through the Audit Logs interface. 
Users can filter E2E audit log entries using a date range. 
Audit log entries are generated only for supported E2E actions defined in the implementation scope. 
Audit logging behavior is consistent with the existing audit logging implementation across other application modules.

## Discussion
- Finalized.
- Clarification: audit log entries are recorded for creating, renaming, adding and deleting test cases in an E2E flow, and for E2E folder actions. Each entry shows the username, the time and the user's role.
- Re-Tested the functionality in the https://fis2-beta.avoassure.ai/ environment of build no 26.6.4-rc.3The audit logging enhancement for the E2E module has been successfully implemented and verified. 
Audit logs are now captured for both E2E artefact-level actions and E2E folder-level actions, providing improved traceability and accountability of user activities within the module. The audit records include the relevant user details, action performed, timestamp, and user role, enabling administrators to clearly identify who performed an action and when it occurred. 
The implementation also suppo

## Attachments
_None._

## Development links
_None._

## Related work items
_None._

<!-- content-fingerprint: 9588aa5c279967f4.19ddcf65.23c99b4a -->
