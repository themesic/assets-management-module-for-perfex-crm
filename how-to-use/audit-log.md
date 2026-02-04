---
description: How to use the Audit Log to track all asset-related activities
---

# 📋 Audit Log

The **Audit Log** records every significant action on assets: creation, updates, allocations, revocations, checkouts, transfers, and more. Use it for compliance, security reviews, and troubleshooting.

---

## 1. 📍 Access Audit Log

**Navigation:** **Assets** → **Audit Log** from the sidebar.

---

## 2. 📊 What Is Logged

| Action | Description |
|--------|-------------|
| `created` | New asset created |
| `updated` | Asset details changed |
| `deleted` | Asset deleted |
| `allocated` | Asset allocated to staff |
| `revoked` | Allocation revoked |
| `checked_out` | Asset checked out |
| `checked_in` | Asset checked in |
| `maintenance_scheduled` | Maintenance scheduled |
| `maintenance_completed` | Maintenance completed |
| `transferred` | Asset transferred |
| `transfer_initiated` | Transfer started |
| `reserved` | Asset reserved |
| `lost` | Asset reported lost |
| `broken` | Asset reported broken |
| `liquidated` | Asset liquidated |
| `warranty` | Asset sent for warranty |

---

## 3. 📋 Log Entry Details

Each log entry typically includes:

| Field | Description |
|-------|-------------|
| **Date/Time** | When the action occurred |
| **Asset** | Asset code and name (or "deleted" if asset was removed) |
| **Action** | Type of action |
| **Description** | Human-readable summary |
| **Performed By** | Staff member who performed the action |
| **IP Address** | Client IP (for security) |
| **Old Values** | Previous data (for updates) |
| **New Values** | New data after the action |

---

## 4. 🔍 Filtering

- **By Asset** — View all actions for a specific asset
- **By Date Range** — Focus on a time period
- **By Action** — e.g., only allocations or only transfers
- **By User** — See what a specific user did

---

## 5. 📤 Export Audit Log

1. Go to **Assets** → **Reports**
2. Select **Audit Report**
3. Optionally filter by asset
4. Choose format (PDF, Excel, CSV)
5. Generate and download

---

## 💡 Use Cases

- **Compliance** — Prove who did what and when
- **Security** — Detect unauthorized changes
- **Troubleshooting** — Trace why an asset's data changed
- **Training** — Review user activity patterns
