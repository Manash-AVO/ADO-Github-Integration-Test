# Viewing E2E Flow Details and Audit Logs

The E2E Flow details help you understand the key information related to E2E Flow. You can view details such as the E2E Flow name, description, status, creation date, time, and the user who created it. 

The E2E Flow audit logs track the history of changes made to E2E Flow folder or E2E Flow. Each audit log entry records the username, timestamp, and role of the user who performed the action, so you can see who did what and when. Use this article to understand how to view E2E Flow details and audit logs.

## Viewing E2E Flow Details

To view E2E Flow Details, perform the following actions:

1. On the **Home** page, from **Projects** list, select required project.
2. Select **Design Studio**.
3. Select **Test Case**.
4. On the **Test Case** page, expand the **E2E Flows** and select the E2E Flow for which you want to see the details.
5. Select the **Information Panel** (**i**) icon. The **Details** tab opens.
6. On the **Details** tab, you can view the following information:

* **E2E Flow Name**: The E2E Flow name.
* **Description**: The E2E Flow description.
* **Status**: The E2E Flow [status](https://docs.avoautomation.com/avo-assure/create-and-execute-tests-with-design-studio/test-artifacts-in-avo-assure.md#understanding-different-statuses-of-test-artifacts) (New, In Progress, Under Review, Approved or Rejected).
* **Created On**: The E2E Flow creation date and time.
* **Created By**: The username of the person who created the E2E Flow.

## Viewing E2E Flow Audit Logs

To view E2E Flow Audit Logs, perform the following actions:

1. On the **Home** page, from **Projects** list, select required project.
2. Select **Design Studio**.
3. Select **Test Case**.
4. On the **Test Case** page, expand the **E2E Flow** and select the E2E Flow for which you want to see the details.
5. Select the **Information Panel** (**i**) icon. The **Details** tab opens.
6. Select the **Audit Logs** tab.
7. Select **Date Range** to view the actions performed between the specified dates.
8. Expand the month to view the actions performed in the E2E flow. Each entry shows the username, the action performed, the timestamp, and the role of the user who performed the action.

### E2E Flow Audit Log Inclusions

The following actions are captured in the E2E Flow audit logs:

* Performing Folder Level Actions
* Creating E2E Flow Folder
* Renaming E2E Flow Folder
* Creating E2E Flow
* Renaming E2E Flow
* Adding Test Case to E2E Flow
* Deleting Test Case from E2E Flow

> **Note:** Audit log entries are generated only for the supported E2E artefact-level and folder-level actions listed above, and are consistent with the audit logging available across other modules.

### E2E Flow Audit Log Exclusions

The following actions are currently not captured in the E2E Flow audit logs:

* Reordering E2E Flow
