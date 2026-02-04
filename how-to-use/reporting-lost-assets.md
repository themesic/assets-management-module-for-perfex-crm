---
description: How to report lost assets in the Asset Management module
---

# 🔍 Reporting Lost Assets

When an asset is lost, stolen, or cannot be located, use the **Report Lost** feature to document the loss, update inventory, and maintain compliance records.

---

## 1. 🚨 When to Report Lost

- Asset cannot be found after search
- Asset was stolen
- Asset was misplaced and considered unrecoverable
- Asset disappeared (e.g., during move, natural disaster)

**Important:** Reporting lost **reduces** the total quantity of the asset. The item is removed from available inventory.

---

## 2. 📍 Access the Feature

**From Asset List:**
1. Go to **Assets** → **Assets**
2. Click on the asset
3. Use the **Report Lost** or **Lost** action

**From Asset Detail:**
- Open the asset and find the **Report Lost** button in the actions menu

---

## 3. 📝 Fill in Lost Report Details

### Required Information

| Field | Description |
|-------|-------------|
| **Lost Code** | Auto-generated (e.g., LST-00000001) — editable if needed |
| **Quantity** | Number of units lost |
| **Lost Time** | Date and time the loss was discovered or reported |

### Optional Information

| Field | Description |
|-------|-------------|
| **Description** | Circumstances, location last seen, police report number, etc. |

### Reference

- **Remaining Quantity** — Shows current available vs. total before this action

---

## 4. ✅ Save the Report

Click **Save**. The system will:

- ✅ Generate a unique lost report code
- ✅ **Reduce total quantity** of the asset
- ✅ Update `total_lost` counter
- ✅ Record the event in inventory history
- ✅ Log the action in the audit log
- ✅ Trigger webhook `asset.lost` (if configured)

---

## 5. ⚠️ Validation Rules

- **Quantity** cannot exceed available quantity (total - allocated)
- **Quantity** must be a positive integer
- **Lost Time** is required

---

## 6. 📊 Impact on Inventory

| Before | Action | After |
|--------|--------|------|
| Total: 10, Available: 6 | Report 2 lost | Total: 8, Available: 4, Lost: 2 |

Lost items are permanently removed from the asset's quantity. They cannot be "un-lost" — you would need to use **Additional Asset** to add new units if the asset is later found or replaced.

---

## 💡 Best Practices

- 📋 **Document thoroughly** — Include police report numbers, witness names
- 🔒 **Review security** — Use loss patterns to improve procedures
- 📊 **Track trends** — Run reports to identify high-loss categories
- 🛡️ **Insurance** — Keep records for insurance claims
