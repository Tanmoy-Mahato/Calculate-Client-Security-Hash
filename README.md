# Calculate Client Security Hash – Workflow Overview

## Overview

This UiPath automation processes WI5 work items from ACME System 1 and generates a Security Hash for each client using their details.

The bot retrieves client information, generates a SHA1 hash, and updates the work item status to Completed with the generated hash.

---

## Process Flow

| Step | Description |
|------|-------------|
| 1.1 | Open the ACME System 1 Web Application |
| 1.2 | Log in to System 1 using email and password |
| 1.3 | Access the Dashboard |
| 1.4 | Open the Work Items listing |
| 1.5 | Process each WI5 activity |
| 1.5.A | Open Work Item Details and retrieve Client Details |
| 1.5.B | Open SHA1 Generator and provide input:<br>`ClientID-ClientName-ClientCountry` |
| 1.5.C | Retrieve generated Client Security Hash |
| 1.5.D | Open Update Work Item page |
| 1.5.E | Set status to **Completed** and add Security Hash in comments |
| 1.6 | Continue with the next WI5 activity |

---

