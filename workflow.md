# IT Service Ticket Lifecycle & Workflow Analysis

## Overview
This document defines the end-to-end lifecycle, status transitions, and SLA (Service Level Agreement) parameters for IT support and service desk requests.

## 1. Ticket States
* **New (Open):** The ticket has been submitted by the end-user and awaits triage.
* **Assigned:** The ticket is assigned to a designated support technician or tier.
* **In Progress:** Troubleshooting and active resolution work are underway.
* **Pending Vendor / User:** Execution is paused awaiting third-party input or user clarification.
* **Resolved:** A solution has been deployed or provided, awaiting user verification.
* **Closed:** The user has confirmed resolution or the auto-close SLA timer has expired.

## 2. SLA Matrix
| Priority | Response Time | Resolution Target |
| :--- | :--- | :--- |
| **Critical (P1)** | 15 Minutes | 2 Hours |
| **High (P2)** | 1 Hour | 8 Hours |
| **Medium (P3)** | 4 Hours | 24 Hours |
| **Low (P4)** | 8 Hours | 72 Hours |

## 3. Escalation Rules
- If a P1 ticket remains in `Assigned` status for more than 30 minutes without moving to `In Progress`, an automated alert is triggered to the IT Operations Manager.
