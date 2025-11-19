# Power-Apps---Petty-Cash-Management-System
Power Apps - Petty Cash Management System

![1](https://github.com/user-attachments/assets/9fcb90ee-3779-4d36-a781-65dd07299c4f)
![5](https://github.com/user-attachments/assets/35214298-5795-43ae-a827-a36b212b3be0)
![4](https://github.com/user-attachments/assets/07f80895-c9eb-4e23-be72-2622efcf16d3)
![3](https://github.com/user-attachments/assets/3dea2391-50a6-4d4f-9b4b-20c67bdc9b69)
![2](https://github.com/user-attachments/assets/e8d30da1-f2b1-46ab-b889-9dc3f67dbec1)


Overview

The Petty Cash Management System is a Power Apps solution built on top of SharePoint and Power Automate to digitalize how organizations submit, approve and track petty cash expenses. The system eliminates manual paperwork by providing an automated workflow for requests, approvals, cash issuance, receipt upload and reconciliation, ensuring transparency and proper financial control.

Key Features
1. Petty Cash Request Form

Users submit requests through the system.

Captures purpose, required amount, category and attachments (bills/receipts).

Stores data in a SharePoint list.

2. Automated Approval Workflow (Power Automate)

Multi-level approvals based on department or amount.

Approvers receive email/Teams notifications.

Approvers can approve/reject directly from email/Teams or the app.

Auto-reminders for pending approvals.

3. Cash Issuance & Tracking

Finance/Admin sees a dashboard inside the app with all approved requests.

Cash issuance is recorded against each request.

System tracks pending issuance, issued and reconciled statuses.

4. Receipt Upload & Reconciliation

After spending, users upload receipts using attachment control.

Admin verifies receipts and marks the request as reconciled.

Supports adjustments if the actual amount differs from the requested amount.

5. Petty Cash Balance Dashboard (Inside Power Apps)

Displays:

Opening balance

Total issued

Total reconciled

Remaining balance

Updated using SharePoint lists and calculated columns.

6. Role-Based Access

Users only see their own requests.

Approvers see only items requiring their approval.

Finance/Admin sees all transactions and cash balance.

Implemented through SharePoint groups + conditional visibility in Power Apps.

6.Challenges & How You Overcame Them

1.Handling Attachments for Receipts

Issue: Receipts must be previewed easily without large delays.
Solution:

Used Power Apps Attachments control with direct link preview.

Stored attachments properly in SharePoint to reduce load times.

2. Duplicate Requests

Issue: Some users tried submitting the same expense multiple times.
Solution:

Added validation rules in Power Apps:

Check previous requests by amount and category.

Show warnings for possible duplicates.

