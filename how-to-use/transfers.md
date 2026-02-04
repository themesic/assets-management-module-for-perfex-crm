---
description: How to transfer assets between locations and departments
---

# 🚚 Transfers

The **Transfers** feature lets you move assets from one location or department to another. Track the full transfer lifecycle from initiation to completion.

---

## 1. 📍 Access Transfers

**Navigation:** **Assets** → **Transfers** from the sidebar.

---

## 2. ➕ Initiate a Transfer

### Steps

1. Click **New Transfer** or **Initiate Transfer**
2. Select **Asset**
3. Select **From Location** (current — optional, can be auto-filled)
4. Select **To Location** (required) — where the asset is moving
5. Optionally: **From Department** and **To Department**
6. Enter **Quantity** (default: 1)
7. Set **Transfer Date**
8. Add **Reason** (optional) — e.g., "Office relocation", "Department reassignment"
9. Add **Notes** (optional)
10. Click **Save**

### Initial Status

- Transfer is created with status **Pending**
- Asset location is **not** updated yet — that happens when the transfer is completed

---

## 3. ✅ Complete a Transfer

When the asset has physically arrived at the new location:

1. Go to **Assets** → **Transfers**
2. Find the transfer with status **Pending** or **In Transit**
3. Click **Complete Transfer** or **Mark as Received**
4. The system records who received it and when

### What Happens on Completion

- ✅ Asset's **location** is updated to the new location
- ✅ Asset's **department** is updated (if specified)
- ✅ Transfer status changes to **Completed**
- ✅ Audit log and webhook `asset.transferred` are triggered

---

## 4. 📋 Transfer Statuses

| Status | Description |
|--------|-------------|
| **Pending** | Transfer initiated, not yet completed |
| **In Transit** | Asset is being moved (optional workflow) |
| **Completed** | Asset received at new location |
| **Cancelled** | Transfer cancelled |

---

## 5. 📊 Viewing Transfers

In **Assets** → **Transfers** you can see:

| Column | Description |
|--------|-------------|
| Asset | Asset name and code |
| From Location | Origin |
| To Location | Destination |
| Transfer Date | When transfer was initiated |
| Transferred By | Who initiated |
| Received By | Who confirmed receipt (when completed) |
| Status | Pending, In Transit, Completed, Cancelled |

---

## 💡 Best Practices

- ✅ **Complete transfers promptly** when assets arrive
- ✅ **Document reason** for audits and reporting
- ✅ **Use departments** for multi-department organizations
- ✅ **Run transfer reports** to track asset movement over time
