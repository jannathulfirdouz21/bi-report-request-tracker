
# BI Report Request Tracker

An end-to-end Microsoft Power Platform project that streamlines how report requests and data quality issues are submitted, approved, and tracked, replacing ad hoc email/chat based tracking with a structured workflow and live dashboard.

## Problem

BI and reporting teams often receive report requests and data quality issues informally through email or chat. This makes it hard to see what is open, what is high priority, and how long items take to resolve.

## Solution

This project connects three Power Platform tools into one workflow:

1. **Power Apps** (intake form): a simple canvas app where users submit a request (New Report, Change Request, or Data Issue), select a priority, and provide a description.
2. **Power Automate** (approval workflow): when a new request is submitted, it automatically routes to an approver, updates the request status based on the outcome, and emails the requestor with the result.
3. **Power BI** (reporting dashboard): visualizes request volume by type, status, and priority, tracks open requests, and calculates average resolution time.

All three tools share a single SharePoint list as the data source, so the app, workflow, and dashboard always stay in sync.

## Architecture

```
Power Apps (intake form)
        |
        v
SharePoint List (Report Requests)
        |
        v
Power Automate (approval + status update + email)
        |
        v
Power BI (dashboard)
```

## Screenshots

*(Add your screenshots here, e.g.)*

![Power App form](./01-power-app-form.png)
![Power Automate flow](./02-automate-flow.png)
![Power BI dashboard](./03-powerbi-dashboard.png)

## Skills Demonstrated

- Low-code app development (Power Apps canvas app, SharePoint data source)
- Workflow automation and conditional logic (Power Automate approvals, branching, notifications)
- Data modeling and visualization (Power BI, DAX calculated columns)
- End-to-end integration across the Microsoft Power Platform

## Author

Jannathul Firdouz
